# Comparing `tmp/balcony-0.0.80.tar.gz` & `tmp/balcony-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.0.80.tar", max compression
+gzip compressed data, was "balcony-0.0.9.tar", max compression
```

## Comparing `balcony-0.0.80.tar` & `balcony-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,29 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.0.80/LICENSE
--rw-r--r--   0        0        0     1678 2023-04-07 10:53:24.563354 balcony-0.0.80/README.md
--rw-r--r--   0        0        0      807 2023-04-10 20:37:57.778565 balcony-0.0.80/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.0.80/balcony/__main__.py
--rw-r--r--   0        0        0     5519 2023-04-15 18:38:15.802110 balcony-0.0.80/balcony/aws.py
--rw-r--r--   0        0        0    11897 2023-04-09 19:54:54.475953 balcony-0.0.80/balcony/botocore_utils.py
--rw-r--r--   0        0        0    12914 2023-04-15 21:01:02.410989 balcony-0.0.80/balcony/cli.py
--rw-r--r--   0        0        0     2717 2023-04-15 19:57:42.810012 balcony-0.0.80/balcony/config.py
--rw-r--r--   0        0        0      475 2023-04-06 12:25:21.609711 balcony-0.0.80/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.0.80/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.0.80/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.0.80/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.0.80/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.0.80/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.0.80/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.0.80/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.0.80/balcony/custom_nodes/yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.0.80/balcony/custom_nodes/yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.0.80/balcony/custom_nodes/yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.0.80/balcony/custom_nodes/yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.0.80/balcony/custom_nodes/yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.0.80/balcony/errors.py
--rw-r--r--   0        0        0    44051 2023-04-15 19:28:13.682357 balcony-0.0.80/balcony/nodes.py
--rw-r--r--   0        0        0    16754 2023-04-15 20:00:13.652536 balcony-0.0.80/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.0.80/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.0.80/balcony/relations.py
--rw-r--r--   0        0        0     2533 2023-04-10 20:21:35.912135 balcony-0.0.80/balcony/test.py
--rw-r--r--   0        0        0     3783 2023-04-10 20:06:26.393503 balcony-0.0.80/balcony/utils.py
--rw-r--r--   0        0        0     2735 2023-04-15 19:57:02.419610 balcony-0.0.80/balcony/yaml_config.py
--rw-r--r--   0        0        0     1612 2023-04-15 19:59:18.959931 balcony-0.0.80/balcony/yaml_validators.py
--rw-r--r--   0        0        0      672 2023-04-15 21:01:19.574095 balcony-0.0.80/pyproject.toml
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 balcony-0.0.80/setup.py
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 balcony-0.0.80/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.0.9/LICENSE
+-rw-r--r--   0        0        0      353 2022-09-26 12:41:48.924073 balcony-0.0.9/README.md
+-rw-r--r--   0        0        0      286 2022-10-09 10:37:47.142816 balcony-0.0.9/balcony/__init__.py
+-rw-r--r--   0        0        0       53 2022-10-04 08:01:49.289224 balcony-0.0.9/balcony/__main__.py
+-rw-r--r--   0        0        0     1432 2022-10-09 09:50:45.143185 balcony-0.0.9/balcony/app.py
+-rw-r--r--   0        0        0    10347 2022-10-08 07:04:48.840377 balcony-0.0.9/balcony/botocore_utils.py
+-rw-r--r--   0        0        0     7724 2022-10-09 10:41:41.880849 balcony-0.0.9/balcony/cli.py
+-rw-r--r--   0        0        0      264 2022-09-30 20:25:42.597791 balcony-0.0.9/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0     1444 2022-09-29 13:15:21.107762 balcony-0.0.9/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     1095 2022-10-09 17:51:42.748364 balcony-0.0.9/balcony/custom_nodes/ec2.py
+-rw-r--r--   0        0        0     2530 2022-09-29 13:15:21.126367 balcony-0.0.9/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     3140 2022-10-10 07:22:17.872579 balcony-0.0.9/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0     1018 2022-09-29 19:23:48.871446 balcony-0.0.9/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1410 2022-10-01 08:48:13.809464 balcony-0.0.9/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0     2214 2022-09-30 20:31:15.045592 balcony-0.0.9/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0       26 2022-10-04 07:57:08.884233 balcony-0.0.9/balcony/exceptions.py
+-rw-r--r--   0        0        0     2011 2022-10-09 10:37:09.474616 balcony-0.0.9/balcony/factories.py
+-rw-r--r--   0        0        0     1261 2022-09-26 08:05:59.761176 balcony-0.0.9/balcony/logs.py
+-rw-r--r--   0        0        0     4012 2022-10-09 11:11:51.901472 balcony-0.0.9/balcony/main.py
+-rw-r--r--   0        0        0    33760 2022-10-09 10:52:29.206820 balcony-0.0.9/balcony/nodes.py
+-rw-r--r--   0        0        0    20844 2022-10-11 20:37:36.250496 balcony-0.0.9/balcony/reader.py
+-rw-r--r--   0        0        0     6560 2022-10-09 10:03:48.761239 balcony-0.0.9/balcony/registries.py
+-rw-r--r--   0        0        0     9472 2022-10-09 17:45:39.425216 balcony-0.0.9/balcony/relations.py
+-rw-r--r--   0        0        0      386 2022-10-13 07:07:22.872196 balcony-0.0.9/balcony/rrr.py
+-rw-r--r--   0        0        0      377 2022-10-09 17:48:27.201727 balcony-0.0.9/balcony/settings.py
+-rw-r--r--   0        0        0     3231 2022-10-08 07:24:30.953384 balcony-0.0.9/balcony/utils.py
+-rw-r--r--   0        0        0      521 2022-10-13 07:16:58.915722 balcony-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 balcony-0.0.9/setup.py
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 balcony-0.0.9/PKG-INFO
```

### Comparing `balcony-0.0.80/LICENSE` & `balcony-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.0.80/balcony/botocore_utils.py` & `balcony-0.0.9/balcony/botocore_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,39 @@
-from utils import icompare_two_camel_case_words
-from config import get_rich_console
-
+from functools import lru_cache
 from typing import List, Union
 from botocore.model import Shape, DenormalizedStructureBuilder, OperationModel
-from rich.markup import escape
-import re
+
+try:
+    from .utils import icompare_two_camel_case_words
+    from .logs import get_rich_console
+except ImportError:
+    from utils import icompare_two_camel_case_words
+    from logs import get_rich_console
+
+
+
 from collections import namedtuple
+from rich.text import Text
 from rich.tree import Tree
+from rich.layout import Layout
+ShapeAndTargetPath = namedtuple('ShapeAndTargetPath', ['shape', 'target_path'])
 
-ShapeAndTargetPath = namedtuple("ShapeAndTargetPath", ["shape", "target_path"])
-
-UNWANTED_SHAPE_NAMES = ("String", "DateTime", "Name", "Id", "Arn", "__string")
+UNWANTED_SHAPE_NAMES = ('String', 'DateTime', 'Name', 'Id', 'Arn', '__string')
 UNWANTED_SHAPE_NAMES_LOWERED = [_.lower() for _ in UNWANTED_SHAPE_NAMES]
 SHAPE_SCALAR_TYPES = DenormalizedStructureBuilder.SCALAR_TYPES
-_MAX_ALLOWED_RECURSION = 10
-SHAPE_COLLECTION_TYPES = ("structure", "list", "map")
-READ_ONLY_VERBS = ("Describe", "List", "Get")
-IDENTIFIER_NAMES = (
-    "arn",
-    "id",
-    "name",
-    "arns",
-    "ids",
-    "names",
-    "identifier",
-    "identifiers",
-    "number",
-    "url",
-)
-
-# shape_resolver can't find the reference of BLACKLISTED_SHAPE_NAMES, so they're ignored
-BLACKLISTED_SHAPE_NAMES = (
-    "ComponentChildList",
-    "FirewallManagerRuleGroups",
-    "Rules",
-    "HeaderNames",  # noqa
-    "ExcludedRules",
-    "CountryCodes",
-    "CookieNames",
-    "TextTransformations",
-    "ComponentSummaryList",  # noqa
-    "AnomalyMonitors",
-    "ConfigurationList",
-    "HandshakeResources",
-    "JsonPointerPaths",  # noqa
-    "AdministrativeActions",
-    "DataValueList",
-    "ThemeValuesList",
-    "Expression",
-    "Expressions",
-    "CostCategoryRulesList",
-    "GetCostAndUsageRequest",
-    "GetCostAndUsageWithResourcesRequest",
-    "GetAnomaliesRequest",
-    "InventoryAggregator",
-    "OpsFilter",
-    "OpsAggregator",
-    "QueryStagePlanNodes",
-    "QueryStagePlanNode",
-    "QueryStage",
-    "ElicitSubSlot",
-    "DialogAction"
-)  # noqa
-# regex expr for removing html caret tags
-HTML_CLEANER_REGEX = re.compile("<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});")
+SHAPE_COLLECTION_TYPES = ('structure', 'list','map')
+READ_ONLY_VERBS = ('Describe', 'List', 'Get')
+IDENTIFIER_NAMES = ('arn', 'id', 'name', 'arns', 'ids',
+                    'names', 'identifier', 'identifiers', 'number', 'url')
+BLACKLISTED_SHAPE_NAMES = ('ComponentChildList','FirewallManagerRuleGroups', 'Rules','HeaderNames', 'ExcludedRules', 'CountryCodes', 'CookieNames', 'TextTransformations', 'ComponentSummaryList','AnomalyMonitors','ConfigurationList','HandshakeResources','JsonPointerPaths','AdministrativeActions','DataValueList','ThemeValuesList','Expressions','CostCategoryRulesList')
 
 console = get_rich_console()
 
-
-def find_key_in_dict_keys(key: str, dict_keys: Union[list, dict]) -> str:
-    """Case insensitive search for a `key` in a `list` or `dict.keys()`.
-    Returns the existing key.
+def find_key_in_dict_keys(key:str, dict_keys: Union[list, dict]) -> str:
+    """Case insensitive search for a `key` in a `list` or `dict.keys()`. 
 
     Args:
         key (str): Search case insensively for
         dict_keys (Union[list, dict]): In a list or keys of dictionary
 
     Returns:
         str: Found key that case insensively matches the given key.
@@ -83,17 +42,16 @@
     if type(dict_keys) == dict:
         dict_keys_list = dict_keys.keys()
     for dict_key in dict_keys_list:
         if key.lower() == dict_key.lower():
             return dict_key
     return False
 
-
-def ifind_key_in_dict_keys(key: str, dict_keys: Union[list, dict]) -> str:
-    """Case insensitive search for a `key` in a `list` or `dict.keys()`.
+def ifind_key_in_dict_keys(key:str, dict_keys: Union[list, dict]) -> str:
+    """Case insensitive search for a `key` in a `list` or `dict.keys()`. 
 
     Args:
         key (str): Search case insensively for
         dict_keys (Union[list, dict]): In a list or keys of dictionary
 
     Returns:
         str: Found key that case insensively matches the given key.
@@ -102,266 +60,211 @@
     if type(dict_keys) == dict:
         dict_keys_list = dict_keys.keys()
     for dict_key in dict_keys_list:
         if icompare_two_camel_case_words(key, dict_key):
             return dict_key
     return False
 
-
 def get_max_results_value_from_shape(input_shape: Shape) -> int:
     """Finds the `MaxResults` highest value for an input shape.
 
     Args:
         input_shape (Shape): Input shape of an operation. Generally postfixed with `Request`.
 
     Returns:
         int: `MaxResults` highest value if found in the Shape definition
     """
-    flat_shapes_and_target_paths = (
-        flatten_shape_to_its_non_collection_shape_and_target_paths(input_shape)
-    )
+    flat_shapes_and_target_paths = flatten_shape_to_its_non_collection_shape_and_target_paths(input_shape)
     flat_members = [_.shape for _ in flat_shapes_and_target_paths]
+    result = False
     for member_shape in flat_members:
-        shape_key_name = getattr(member_shape, "key_name", False)
-        is_key_name_maxresults = shape_key_name and (
-            shape_key_name.lower() == "maxresults"
-        )
+        shape_key_name = getattr(member_shape, 'key_name', False)
+        is_key_name_maxresults = shape_key_name and (shape_key_name.lower() == 'maxresults')
         shape_name = get_shape_name(member_shape)
-        if shape_name.lower() == "maxresults" or is_key_name_maxresults:
+        if shape_name.lower() == 'maxresults' or is_key_name_maxresults:
             member_shape
-            max_value = member_shape.metadata.get("max", False)
+            max_value = member_shape.metadata.get('max', False)
             if max_value:
                 return max_value
     return False
 
-
 def get_input_shape(operation_model: OperationModel) -> Shape:
     """Get the input shape of the operation model
 
     Args:
-        operation_model (OperationModel): botocore OperationModel
+        operation_model (OperationModel): botocore OperationModel 
 
     Returns:
         Shape: Input Shape of the OperationModel
     """
-    return getattr(operation_model, "input_shape", False)
+    return getattr(operation_model, 'input_shape', False)
+
 
 
-def get_members_shapes(shape: Shape, _recursion_count=0) -> List[Shape]:
+def get_members_shapes(shape: Shape) -> List[Shape]:
     """Get the member shapes of and input or output Shape.
 
     Args:
         shape (Shape): Shape to get members from
 
     Returns:
         List[Shape]: Member Shapes, added `key_name` and `parent_name` values to objects.
     """
-
     found_members_shapes = []
-
-    if _recursion_count >= _MAX_ALLOWED_RECURSION:
-        return found_members_shapes
-
     if not shape:
         return found_members_shapes
     if shape.name in BLACKLISTED_SHAPE_NAMES:
         return found_members_shapes
-
-    if shape.type_name == "structure":
+    if shape.type_name == 'structure':
         for shape_key, member in shape.members.items():
-            setattr(member, "key_name", shape_key)
-            setattr(member, "parent_name", shape.name)
+            setattr(member, 'key_name', shape_key)
+            setattr(member, 'parent_name', shape.name)
             found_members_shapes.append(member)
-    elif shape.type_name == "list":
+    elif shape.type_name == 'list':
         only_member = shape.member
         found_members_shapes.append(only_member)
-    elif shape.type_name == "map":
-        t = get_members_shapes(shape.value, _recursion_count+1)
+    elif shape.type_name == 'map':
+        t = get_members_shapes(shape.value)
         return t
     return found_members_shapes
 
 
-def is_shape_non_collection_type(shape_and_target_path: ShapeAndTargetPath) -> bool:
-    """Boolean function to check ShapeAndTargetPath Named Tuple
+def filter_non_collection_shape(shape_and_target_path: ShapeAndTargetPath) -> bool:
+    """Bool function to check ShapeAndTargetPath Named Tuple 
 
     Args:
-        shape_and_target_path (ShapeAndTargetPath): Named Tuple
+        shape_and_target_path (ShapeAndTargetPath): Named Tuple. 
 
     Returns:
         bool: _description_
     """
     shape = shape_and_target_path.shape
-    has_key_name = getattr(shape, "key_name", False)
+    has_key_name = getattr(shape, 'key_name', False)
     is_non_collection = shape.type_name not in SHAPE_COLLECTION_TYPES
     return has_key_name and is_non_collection
 
 
-def _flatten_shape_to_its_members_and_target_paths(
-    shape: Shape, target_str: str = ""
-) -> List[ShapeAndTargetPath]:
-    """Recursive function to get a shape's all members with targetpaths.
-    Generates target_str JMESPath selector for each member as it's located in the hierarchy.
-    Returns a flattened list of (shape, target_path) namedtuples
-
-    Args:
-        shape (Shape): botocore shape, possibly output shape of an operation
-        target_str (str, optional): Used for keeping track of the target path in recursion.
-
-    Returns:
-        List[ShapeAndTargetPath]: List of ShapeAndTargetPath NamedTuple
-    """
+def _flatten_shape_to_its_members_and_target_paths(shape, target_str='', ):
     result = []
     members = get_members_shapes(shape)
     for member in members:
-        member_key_name = getattr(member, "key_name", False)
+        member_key_name = getattr(member, 'key_name', False)
         new_target_str = target_str
         if member_key_name:
-            if target_str == "":
+            if target_str == '':
                 new_target_str = f"{member_key_name}"
             else:
                 new_target_str = f"{target_str}[*].{member_key_name}"
-        if member.type_name in (
-            "structure",
-            "list",
-        ):  # TODO:SHAPE_COLLECTION_TYPES-('map',):
-            # if the member is a collection type, recurse into it
-            inner_list = _flatten_shape_to_its_members_and_target_paths(
-                member, new_target_str
-            )
+        if member.type_name in ('structure', 'list'):# TODO:SHAPE_COLLECTION_TYPES-('map',):
+            inner_list = _flatten_shape_to_its_members_and_target_paths(member, new_target_str)
             result.extend(inner_list)
         else:
             result.append(ShapeAndTargetPath(member, new_target_str))
     return result
 
-
-def flatten_shape_to_its_non_collection_shape_and_target_paths(
-    shape: Shape,
-) -> List[ShapeAndTargetPath]:
-    """Return a flat list of shapes all member shapes w/ their JMESPath selector `target_path`
-
-    Args:
-        shape (Shape): botocore shape to list its members
-
-    Returns:
-        List[ShapeAndTargetPath]: (shape, target_path) custom namedtuple
-    """
-    # generate all possible members and their target paths
-    all_flat_members_and_target_paths = _flatten_shape_to_its_members_and_target_paths(
-        shape
-    )
-    # filter out the collection types beacuse they are not supported by JMESPath
-    non_collection_shapes_and_target_paths = list(
-        filter(is_shape_non_collection_type, all_flat_members_and_target_paths)
-    )
+def flatten_shape_to_its_non_collection_shape_and_target_paths(shape):
+    all_flat_members_and_target_paths = _flatten_shape_to_its_members_and_target_paths(shape)
+    non_collection_shapes_and_target_paths = list(filter(filter_non_collection_shape, all_flat_members_and_target_paths))
     return non_collection_shapes_and_target_paths
 
+"""
+    root = Tree("🌲 [b green]Rich Tree", highlight=True, hide_root=True)
+    node = root.add(":file_folder: Renderables", guide_style="red")
+    simple_node = node.add(":file_folder: [bold yellow]Atomic", guide_style="uu green")
+    simple_node.add(Group("📄 Syntax", syntax))
+    simple_node.add(Group("📄 Markdown", Panel(markdown, border_style="green")))
+    containers_node = node.add(
+        ":file_folder: [bold magenta]Containers", guide_style="bold magenta"
+    )
+    containers_node.expanded = True
+    panel = Panel.fit("Just a panel", border_style="red")
+    containers_node.add(Group("📄 Panels", panel))
 
-def cleanhtml(raw_html: str) -> str:
-    """Removes the HTML tags from given raw_html
+therewillbebeloodthere
+        containers_node.add(Group("📄 [b magenta]Table", table))
 
-    Args:
-        raw_html (str): HTML string to clean the tags off of
+    console = Console()
 
-    Returns:
-        str: HTML with tags removed
-    """
-    cleantext = re.sub(HTML_CLEANER_REGEX, "", raw_html)
-    return cleantext
+    console.print(root)
+"""
 
 
 def rich_str_shape(shape: Shape) -> str:
     """Transforms a Shape to rich supported string.
 
     Args:
         shape (Shape): botocore.model.Shape object.
 
     Returns:
         str: Rich string for shape.
     """
-    key_name = getattr(shape, "key_name", "")
+    key_name = getattr(shape, 'key_name', '{')
     type_name = str(shape.type_name)
-    shape_documentation = cleanhtml(shape.documentation)
-
-    shape_str = (
-        f"[blue bold]{key_name}[/] [white]({type_name})[/]: {shape_documentation}"
-    )
-    if key_name == "":
-        lead = ""
-        if type_name == "list":
-            lead = "["
-        elif type_name == "structure":
-            lead = "{"
-        shape_str = f"[red]{escape(lead)}[/] — [white](({type_name}))[/]: [gray]{shape_documentation}[/]"
-
+    if key_name == '{' and type_name == 'structure':
+        type_name = ''
+    if type_name:
+        type_name = f"({type_name})"
+    shape_str = f"[blue]{key_name} [white]{type_name}"
     return shape_str
 
 
 def generate_rich_tree_from_shape(shape: Shape) -> Tree:
     """Genereate a rich Tree containing `shape` and it's members."""
     tree = Tree(rich_str_shape(shape), guide_style="red")
-
-    def _recursive_stringify_shape(shape, node: Tree):
+    def _recursive_stringify_shape(shape, node):
 
         members = get_members_shapes(shape)
         for member in members:
-            member_str = rich_str_shape(member)
+            member_str = rich_str_shape(member) 
             if member.type_name in SHAPE_COLLECTION_TYPES:
                 new_node = node.add(member_str)
                 _recursive_stringify_shape(member, new_node)
             else:
                 node.add(member_str)
-
     _recursive_stringify_shape(shape, tree)
     return tree
-
-
+        
+    
 # @lru_cache(maxsize=500) # print(get_shape_name.cache_info())
 def get_shape_name(shape: Shape) -> str:
-    """Returns the shapes name, using custom set 'key_name' attr
-
-    Args:
-        shape (Shape): botocore Shape obj
-
-    Returns:
-        str: Name of the shape.
-    """
+    """Returns the shapes name, using custom set object values"""
     shape_name = shape.name
-    shape_key_name = getattr(shape, "key_name", False)
+    shape_key_name = getattr(shape, 'key_name', False)
     if shape_name.lower() in UNWANTED_SHAPE_NAMES_LOWERED:
         # check for name forgotten in shape.serialization if the name is a type name.
         if shape_key_name:
             return shape_key_name
-        elif shape.serialization and shape.serialization.get("name", False):
-            given_serialization_name = shape.serialization.get("name")
+        elif shape.serialization and shape.serialization.get('name', False):
+            given_serialization_name = shape.serialization.get('name')
             return given_serialization_name
-    if shape_key_name:
-        return shape_key_name
     return shape_name
-
-
-def get_required_parameter_shapes_from_operation_model(
-    operation_model: OperationModel,
-) -> List[Shape]:
-    """Finds required parameter shapes of the operation models input_shape.
-
-    Args:
-        operation_model (OperationModel): botocore OperationModel obj of the Operation
-
-    Returns:
-        List[Shape]: Required parameter shapes.
-    """
+   
+def get_required_parameter_shapes_from_operation_model(operation_model: OperationModel) -> List[Shape]:
     input_shape = get_input_shape(operation_model)
     if not input_shape:
-        return []  # there's no input shape
+        return [] # there's no input shape
     input_shape_members = get_members_shapes(input_shape)
     input_required_member_names = input_shape.required_members
     if input_required_member_names == []:
         return []
-
+    
     required_member_shapes = []
     for input_member in input_shape_members:
         input_member_name = get_shape_name(input_member)
         for required_name in input_required_member_names:
             if icompare_two_camel_case_words(required_name, input_member_name):
                 required_member_shapes.append(input_member)
-
+            
     return required_member_shapes
+
+# def get_required_parameters_for_operation(operation_model):
+#     required_parameter_shapes = get_required_parameters_for_operation(operation_model)
+#     required_parameter_names = [
+#         get_shape_name(r_param_shape)
+#         for r_param_shape in required_parameter_shapes
+#     ]
+#     return required_parameter_names
+
+def compare_shape_names(member, search_shape):
+    return get_shape_name(member) == get_shape_name(search_shape)
+
+
```

### Comparing `balcony-0.0.80/balcony/custom_nodes/lambda_functions.py` & `balcony-0.0.9/balcony/custom_nodes/lambda_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-# from ..nodes import ResourceNode
-# from ..config import get_logger
+try:
+    from ..nodes import ResourceNode
+    from ..registries import ResourceNodeRegistry
+    from ..logs import get_logger
+    from ..relations import FindRelationResultTypes
+except ImportError:
+    from nodes import ResourceNode
+    from registries import ResourceNodeRegistry
+    from logs import get_logger
+    from relations import FindRelationResultTypes
+logger = get_logger(__name__)
 
-# logger = get_logger(__name__)
-
-# class Function(ResourceNode, service_name="lambda", name="Function"):
-#     def __init__(self, *args, **kwargs):
-#         super().__init__(*args, **kwargs)
+class Lambda_Function(ResourceNode, ResourceNodeRegistry, service_name="lambda", name="Function"):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
     
-#     def define_extra_relations(self):
-#         r= super().define_extra_relations()
-#         return [{
-#             "service_name": "lambda",
-#             "resource_node_name": "Function",
-#             "operation_name": "ListFunctions",
-#             "required_shape_name": "FunctionName",
-#             "target_shape_name": "FunctionName",
-#             "target_shape_type": "string",
-#             "target_path": "Functions[*].FunctionName"
-#         }]
+    def define_extra_relations(self):
+        r= super().define_extra_relations()
+        return [{
+            "service_name": "lambda",
+            "resource_node_name": "Function",
+            "operation_name": "ListFunctions",
+            "search_shape_name": "FunctionName",
+            "target_shape_name": "FunctionName",
+            "target_shape_type": "string",
+            "target_path": "Functions[*].FunctionName"
+        }]
```

### Comparing `balcony-0.0.80/balcony/custom_nodes/s3.py` & `balcony-0.0.9/balcony/custom_nodes/s3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-from nodes import ResourceNode
-from config import get_logger
-
+try:
+    from ..nodes import ResourceNode
+    from ..registries import ResourceNodeRegistry
+    from ..logs import get_logger
+    from ..relations import FindRelationResultTypes
+except ImportError:
+    from nodes import ResourceNode
+    from registries import ResourceNodeRegistry
+    from logs import get_logger
+    from relations import FindRelationResultTypes
 logger = get_logger(__name__)
 
-class BucketLifecycleConfiguration(ResourceNode, service_name="s3", name="BucketLifecycleConfiguration"):
+class S3_BucketLifecycleConfiguration(ResourceNode, ResourceNodeRegistry, service_name="s3", name="BucketLifecycleConfiguration"):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
     def define_extra_relations(self):
         r= super().define_extra_relations()
         return [{
             "service_name": "s3",
             "resource_node_name": "Buckets",
-            "required_shape_name": "Bucket",
+            "search_shape_name": "Bucket",
             "target_shape_name": "Name",
             "target_shape_type": "string",
             "operation_name": "ListBuckets",
             "target_path": "Buckets[*].Name"
         }]
 
     # def find_best_relations_for_operation(self, operation_name, relation_map):
```

### Comparing `balcony-0.0.80/balcony/nodes.py` & `balcony-0.0.9/balcony/nodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1017 +1,605 @@
-from botocore_utils import (
-    _flatten_shape_to_its_members_and_target_paths,
-    get_shape_name,
-)
-from utils import (
-    camel_case_split,
-    compare_nouns,
-    icompare_two_token_lists,
-    compare_two_camel_case_words,
-    str_relations,
-    is_word_in_a_list_of_words
-)
-from botocore_utils import (
-    get_input_shape,
-    get_max_results_value_from_shape,
-    find_key_in_dict_keys,
-    generate_rich_tree_from_shape,
-    icompare_two_camel_case_words,
-    ifind_key_in_dict_keys,
-    READ_ONLY_VERBS,
-    IDENTIFIER_NAMES,
-    cleanhtml,
-)
-from relations import RelationMap, Relation
-from reader import ServiceReader
-from registries import ResourceNodeRegistry
-from config import get_logger, get_rich_console
-from errors import Error
-
-from typing import List, Dict, Tuple, Union
+try:
+    from .utils import camel_case_split, compare_nouns, ifind_similar_names_in_list , icompare_two_token_lists, compare_two_camel_case_words, str_relations
+    from .botocore_utils import *
+    from .relations import RelationMap, FindRelationResultTypes
+    from .reader import ServiceReader
+    from .registries import ResourceNodeRegistry
+    from .logs import get_logger, get_rich_console
+except ImportError:
+    from utils import camel_case_split, compare_nouns, ifind_similar_names_in_list , icompare_two_token_lists, compare_two_camel_case_words, str_relations
+    from botocore_utils import *
+    from relations import RelationMap, FindRelationResultTypes
+    from reader import ServiceReader
+    from registries import ResourceNodeRegistry
+    from logs import get_logger, get_rich_console
+
+from pprint import pprint
+import json
+import boto3
+from itertools import product as cartesian_product
+from enum import Enum
+import copy
+from termcolor import colored
 from botocore.utils import ArgumentGenerator
+from botocore.validate import validate_parameters
 from botocore.hooks import EventAliaser
 from botocore.model import OperationModel, ServiceModel
 from rich.text import Text
 from rich.panel import Panel
 from rich.console import Group
-from rich.padding import Padding
+from rich.layout import Layout
 import jmespath
-
+from abc import ABC, abstractmethod
+# class AbstractResourceNode(ABC):
+    
+#     @abstractmethod
+#     def get_resource_nodes(self): ...
+    
 logger = get_logger(__name__)
 
+
 _resource_node_registry = ResourceNodeRegistry()
 argument_generator = ArgumentGenerator()
 console = get_rich_console()
-PAGINATION_TOKEN_KEYS = ("nexttoken", "continuationtoken", "marker", "nextcontinuationtoken")
 
 class ResourceNode:
-    def __init__(
-        self, service_node: "ServiceNode", name: str, operation_names: List[str]
-    ) -> None:
+    def __init__(self, service_node: 'ServiceNode', name: str, operation_names: List[str]):
         self.service_node = service_node
         self.name = name
         self.operation_names = operation_names
         self._operation_models = {}
 
-    def __init_subclass__(cls, service_name=None, name=None, **kwargs) -> None:
-        """Initializes the custom subclasses of ResourceNode to ResourceNodeRegistry.
-
-        Args:
-            service_name (_type_, optional): Name of the AWS service. Defaults to None.
-            name (_type_, optional): Name of the AWS Resource Node. Defaults to None.
-        """
-        super().__init_subclass__(**kwargs)
-        if service_name and name:
-            _resource_node_registry.register_class(cls, service_name, name)
-        else:
-            logger.debug(
-                f'{cls.__name__} invalid! You must define "service_name" and "name"'
-            )
-
-    def get_operation_types_and_names(self) -> Dict[str, str]:
-        operation_names = self.get_operation_names()
-        types_to_operation_names = {}
-        for op_name in operation_names:
-            verb, *resource_node_name_tokens = camel_case_split(op_name)
-            resource_node_name = "".join(resource_node_name_tokens)
-            if verb.lower() == "describe":
-                types_to_operation_names["describe"] = op_name
-            if verb.lower() == "list":
-                types_to_operation_names["list"] = op_name
-
-            if verb.lower() == "get":
-                if self.name != resource_node_name:
-                    types_to_operation_names["gets"] = op_name
-                else:
-                    types_to_operation_names["get"] = op_name
-        return types_to_operation_names
-
-
-    def get_operation_names(self) -> List[str]:
-        """Returns the available operation names in the ResourceNode.
-
-        Returns:
-            List[str]: Operation names tied to the ResourceNode
-        """
-        return self.operation_names
 
     # NOTE: +overrideable
-    def define_extra_relations(self) -> Union[List[Dict], List[Relation]]:
-        """Extra relations defined in the custom subclasses of ResourceNode
-
-        Returns:
-            Union[List[Dict], List[Relation]]: List of relations as dicts or Relation objects
-        """
+    def define_extra_relations(self):
         return []
-
+    
     # NOTE: +overrideable
-    def get_operations_relations(
-        self, operation_name: str
-    ) -> Tuple[Union[List[Dict], bool], Union[Error, None]]:
-        """_summary_
-
-        Args:
-            operation_name (str): Name of the operation.
-
-        Returns:
-            Tuple[Union[List[Dict], bool], Union[Error, None]]: Returns value and error.
-                                                                True: No required parameters
-                                                                False: Failure
-                                                                List[Dict]: List of relations
-        """
-
+    def get_operations_relations(self, operation_name:str, relation_map: RelationMap=None):
         resource_node = self
-        relation_map = self.service_node.get_relation_map()
-        required_parameter_names = (
-            resource_node.get_required_parameter_names_from_operation_name(
-                operation_name
-            )
-        )
-        # required_parameter_names_to_relations_map = {
-        #     r_param_name: None for r_param_name in required_parameter_names
-        # }
-
+        if relation_map is None:
+            relation_map = self.service_node.get_relation_map()
+        required_parameter_names = resource_node.get_required_parameter_names_from_operation_name(operation_name)
+        required_parameter_names_to_relations_map = {
+            r_param_name:None 
+            for r_param_name in required_parameter_names
+        }
+        
         if not required_parameter_names:
             # no required parameters
-            return True, None
-
-        operation_markup = (
-            f"[bold][green]{self.service_node.name}[/].[blue]{operation_name}[/][/]"
-        )
-        req_param_markup = f"[bold magenta]{', '.join(required_parameter_names)}[/]"
+            logger.debug(f"NO REQUIRED PARAMETERS. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has no required parameters")
+            return True, FindRelationResultTypes.NoRequiredParameters
 
         if len(required_parameter_names) == 1:
-
             # only one parameter exists
-            single_relation_list = None
+            selected_relations = None
             single_parameter_name = required_parameter_names[0]
-            generated_relations_for_parameter = (
-                relation_map.get_parameters_generated_relations(
-                    single_parameter_name, operation_name
-                )
-            )
+            generated_relations_for_parameter = relation_map.get_parameters_generated_relations(single_parameter_name, operation_name)
             if not generated_relations_for_parameter:
-                logger.debug(
-                    f"Failed to generate relations. {operation_markup} has a required parameters: {req_param_markup}"
-                )
-                return False, Error(
-                    "failed to generate relations",
-                    {
-                        "required_parameter_names": required_parameter_names,
-                        "service": self.service_node.name,
-                        "resource_node": self.name,
-                        "operation_name": operation_name,
-                    },
-                )
+                logger.debug(f"NO RELATIONS GENERATED. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameter: {single_parameter_name}. {generated_relations_for_parameter=}")
+                return False, FindRelationResultTypes.NoGeneratedParameters
 
-            single_relation_list = (
-                resource_node.find_best_relation_for_single_parameter(
-                    single_parameter_name, generated_relations_for_parameter
-                )
-            )
-            if single_relation_list:
-                logger.debug(
-                    f"[green]Success finding relations.[/] {operation_markup} has a required parameter: {req_param_markup}. Relation found: [yellow]{str_relations(single_relation_list)}[/]"
-                )
-                return single_relation_list, None
+            selected_relations = resource_node.find_best_relation_for_single_parameter(single_parameter_name, generated_relations_for_parameter)
+            # required_parameter_names_to_relations_map[single_parameter_name]=selected_relations
+            if selected_relations:
+                logger.debug(f"SINGLE PARAMETER FOUND. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameter: [bold]{single_parameter_name}[/]. Relation found: [yellow]{str_relations(selected_relations)}[/]")
+                return selected_relations, FindRelationResultTypes.RelationsFound
             else:
-                logger.debug(
-                    f"Failed to choose the best relation for operation. {operation_markup} has required parameters: {req_param_markup}"
-                )
-                return False, Error(
-                    "failed to choose the best relation",
-                    {
-                        "service": self.service_node.name,
-                        "resource_node": self.name,
-                        "operation_name": operation_name,
-                        "generated_relations_for_parameter": generated_relations_for_parameter,
-                    },
-                )
+                logger.debug(f"CAN'T DECIDE BTWN RELATIONS. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameters: {required_parameter_names}.")
+                return False, FindRelationResultTypes.CantDecideBetweenGeneratedParameters
         else:
-            # multiple required parameters does not supported
-            return False, Error(
-                "multiple parameters - must be extended with a subclass",
-                {
-                    "service": self.service_node.name,
-                    "resource_node": self.name,
-                    "operation_name": operation_name,
-                },
-            )
+            # multiple required parameters, zip and check
+            # required_parameter_names = list(required_parameter_names_to_relations_map.keys())
+            # temporary_parameters_to_relations_map = dict()
+            for r_parameter_name in required_parameter_names:
+                generated_relations_for_parameter = relation_map.get_parameters_generated_relations(r_parameter_name, operation_name)
+                if generated_relations_for_parameter:
+                    required_parameter_names_to_relations_map[r_parameter_name]=generated_relations_for_parameter
+                # return False, FindRelationResultTypes.NoGeneratedParameters
+                # selected_relations = resource_node.find_best_relation_for_single_parameter(r_parameter_name, generated_relations_for_parameter)
+                # ignore relations to self
+
+            _all_parameters_have_relations = [
+                bool(_found_relations) 
+                for _found_relations in required_parameter_names_to_relations_map.values()
+                
+            ]
+
+            if not all(_all_parameters_have_relations):
+                # all parameters doesnt have relations
+                if any(_all_parameters_have_relations):
+                    # some found but not all
+                    partial_relations_str = ", ".join([
+                        str_relations(_found_relations)
+                        for _found_relations in required_parameter_names_to_relations_map.values()
+                        if _found_relations
+                    ])
+                    logger.debug(f"NOT ALL RELATIONS FOUND. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameter: {required_parameter_names}. Partially found relations: {partial_relations_str}")
+                    return False, FindRelationResultTypes.SomeRelationsFoundButNotAll
+                else:
+                    # nothing found
+                    logger.debug(f"NO RELATIONS FOUND. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameter: {required_parameter_names}.")
+                    return False, FindRelationResultTypes.NoRelations
+            
+            def check(list_of_relations):
+                if not list_of_relations:
+                    return False
+                first_operation_name = list_of_relations[0].get('operation_name')
+                return all([l_o_r.get('operation_name')==first_operation_name for l_o_r in list_of_relations])
+       
+            possible_relation_combinations = None
+            relation_matrix = list(required_parameter_names_to_relations_map.values())
+            if relation_matrix:
+                relations_cartesian_product = cartesian_product(*relation_matrix)
+                possible_relation_combinations = list(filter(check, relations_cartesian_product))            
+            
+            if not possible_relation_combinations:
+                logger.debug(f"CAN'T DECIDE BTWN RELATIONS. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameters: {required_parameter_names}.")
+                return False, FindRelationResultTypes.CantDecideBetweenGeneratedParameters
+                # TODO: add required parameters to attributes + making them available as relations. add metadata.
+            
+            # find common target_operation relations across the permutation.
+            relation_chosen_from_possible_combinations = self.select_between_possible_relation_combinations_matrix(possible_relation_combinations)    
+            if relation_chosen_from_possible_combinations:
+                logger.debug(f"MULTIPLE PARAMETERS FOUND. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameters: {required_parameter_names}. Relations found: {str_relations(relation_chosen_from_possible_combinations)}")
+                return relation_chosen_from_possible_combinations, FindRelationResultTypes.RelationsFound
+            else:
+                logger.debug(f"CAN'T DECIDE BTWN RELATIONS. [bold][blue]{self.service_node.name}[/].[green]{operation_name}[/][/] has req parameters: {required_parameter_names}.")
+                return False, FindRelationResultTypes.CantDecideBetweenGeneratedParameters
 
     # NOTE: +overrideable
-    def generate_jmespath_selector_from_relations(
-        self, operation_name: str, relation_list: List[Dict]
-    ) -> str:
-        """
-        Tries to generate the jmespath selector string from given relations. Could be overridden with custom subclasses.
-
-        Args:
-            operation_name (str): Name of the operation
-            relation_list (List[Dict]): List of relations for the operation. Used to generate the jmespath selector.
-
-        Returns:
-            str: Jmespath selector string
-        """
-        if not len(relation_list) == 1:
-            return False
-        relation = relation_list[0]
-
-        target_path = relation.target_path
-        search_shape = relation.required_shape_name
-
-        _for_all_the_responses = ""
-        if not target_path.startswith("[*]."):
-            _for_all_the_responses = "[*]."
-        _flatten_two_times = "[][]"
+    def generate_jmespath_selector_from_relations(self, operation_name, relation_list):
+        _for_all_the_responses = '[*].'
+        _flatten_two_times = '[][]'
         if not relation_list:
             return False
-
-        if "." not in target_path:
-            return False
-
-        before_last_attr, last_attribute = target_path.rsplit(".", maxsplit=1)
-        # name switch
-        jmespath_curly_name_transform = f"{search_shape}: {last_attribute}"
-
+        # [*].Stacks[*].{StackName: StackName, age: age}[] -> [*].Stacks[*].StackName[][]
+        # [*].Stacks[*].StackName[], [*].Stacks[*].Description[]  
+        target_shape_and_min_nested_target_paths = None
+        # TODO: if type is list, do something different!!
+        if len(relation_list) == 1:
+            relation = relation_list[0]
+            selected_target_path = min(relation.get('target_path').split(','), key=lambda tp: tp.count('.'))
+            target_shape_and_min_nested_target_paths = [
+                (relation.get('target_shape_name'), selected_target_path)
+            ]
+        else:
+            # multiple relations
+            # all relations point to same operation_name
+            target_shape_and_min_nested_target_paths = [    
+                (
+                    relation.get('target_shape_name'), 
+                    min(
+                        relation.get('target_path').split(','), 
+                        key=lambda tp: tp.count('.')
+                    )
+                )
+                for relation in relation_list
+            ]
+            # all_selected_target_paths_same_depth = False
+            # if len(relations_and_min_nested_target_paths) >= 2:
+
+            # ensure target paths are same deep nested
+            first_target_shape_and_target_path, *rest_of_target_shape_and_target_path = target_shape_and_min_nested_target_paths
+            _, first_target_path = first_target_shape_and_target_path
+            first_target_path_deepness = first_target_path.count('.')
+            first_target_path_before_last_attribute = first_target_path.rsplit('.', maxsplit=1)[0]
+            all_selected_target_paths_same_depth = all([
+                r_target_path.count('.') == first_target_path_deepness \
+                    and r_target_path.rsplit('.', maxsplit=1)[0] == first_target_path_before_last_attribute
+                for _, r_target_path in rest_of_target_shape_and_target_path
+            ])
+                    
+            if not all_selected_target_paths_same_depth:
+                logger.debug(f"[red]DOES NOT START WITH same json nest: {target_shape_and_min_nested_target_paths}")
+                return False
+                
+        jmespath_nested_selector = None
+        
+        # if len(target_shape_and_min_nested_target_paths) == 1:
+        #     jmespath_nested_selector
+        # else:
+        _jmespath_selectors_list = []
+        before_last_attr = None
+        for target_shape, target_path in target_shape_and_min_nested_target_paths:
+            if '.' not in target_path:
+                target_path = f".{target_path}"
+            before_last_attr, last_attribute = target_path.rsplit('.', maxsplit=1)
+                
+            jmespath_nested_selector = f"{target_shape}: {last_attribute}"
+            _jmespath_selectors_list.append(jmespath_nested_selector)
         if not before_last_attr:
-            before_last_attr = "[*]"
-
-        # patching in the first part
-        jmespath_selector = (
-            before_last_attr + ".{" + jmespath_curly_name_transform + "}"
-        )
-        flattened_jmespath_nested_selector = (
-            f"{_for_all_the_responses}{jmespath_selector}{_flatten_two_times}"
-        )
+             before_last_attr = ''
+        jmespath_nested_selector = before_last_attr+'.{'+', '.join(_jmespath_selectors_list)+'}'
+        jmespath_nested_selector
+        flattened_jmespath_nested_selector = f"{_for_all_the_responses}{jmespath_nested_selector}{_flatten_two_times}"
         return flattened_jmespath_nested_selector
 
     # NOTE: +overrideable
-    def _generate_raw_api_parameters_from_operation_data(
-        self,
-        operation_name: str,
-        relations_of_operation: List[dict],
-        related_operations_data: Union[Dict, List],
-    ) -> List:
-        """Generates the jmespath selector and search the data with it. Output is the list of api_parameters dictionaries.
-        Only considers the required parameters(raw parameters) of the operation.
-        > Note: Pagination parameters (e.g. `NextToken`, `MaxResults`) are not included.
-
-        Args:
-            operation_name (str): Name of the operation
-            relations_of_operation (List[dict]): Relations of the operation
-            related_operations_data (Union[Dict, List]): All related operations data
-
-        Returns:
-            List: List of required _raw_ API parameters, not including pagination parameters
-        """
-        if len(relations_of_operation) != 1:
-            logger.debug(
-                f"Not supported: jmespath selector genereation for multiple relations: {operation_name}"
-            )
-            return False, Error(
-                "multiple parameters - must be extended with a subclass",
-                {
-                    "service": self.service_node.name,
-                    "resource_node": self.name,
-                    "operation_name": operation_name,
-                },
-            )
-
-        direct_relation = relations_of_operation[0]
-        direct_relation_op_markup = f"[bold][green]{direct_relation.resource_node_name}[/].[blue]{direct_relation.operation_name}[/][/]"
-
+    def _generate_raw_api_parameters_from_operation_data(self, operation_name, relations_of_operation, related_operations_data):
         resource_node = self
-        generated_jmespath_nested_selector = (
-            resource_node.generate_jmespath_selector_from_relations(
-                operation_name, relations_of_operation
-            )
-        )
+        generated_jmespath_nested_selector = resource_node.generate_jmespath_selector_from_relations(operation_name, relations_of_operation)
         if not generated_jmespath_nested_selector:
-            logger.debug(
-                f"Failed to generate JMESPATH selector for [bold][blue][{resource_node.name}[/].[green]{operation_name}[/]]"
-            )
-            return False, Error(
-                "failed to generate jmespath selector",
-                {
-                    "service": self.service_node.name,
-                    "resource_node": self.name,
-                    "operation_name": operation_name,
-                },
-            )
-        logger.debug(
-            f"Successfuly generated JMESPATH Selector: '[bold]{generated_jmespath_nested_selector}[/]' to extract from {direct_relation_op_markup}"
-        )
+            logger.debug(f"CAN'T GENERATE JMESPATH SELECTOR: {resource_node.name} {operation_name} {generated_jmespath_nested_selector}")
+            return False
+        logger.debug(f"JMESPATH SELECTOR GENERATED: [blue]{generated_jmespath_nested_selector}[/], target operation: [bold][blue][{resource_node.name}[/].[green]{operation_name}[/]]")
 
         if not related_operations_data:
-            logger.debug(
-                "Failed to find related operations data. Can't generate api parameters with the generated JMESPATH Selector"
-            )
+            logger.debug(f"NO OPERATION DATA FOUND. {related_operations_data=}")
 
-        # the first relation we will get
-        direct_related_operation = direct_relation.operation_name
-        directly_related_operation_data = related_operations_data.get(
-            direct_related_operation
-        )
-        found_api_paramaters = jmespath.search(
-            generated_jmespath_nested_selector, directly_related_operation_data
-        )
-        raw_api_parameters_list = found_api_paramaters
-        # for r_api_param in found_api_paramaters:
-        #     for r_api_p_value in r_api_param.values():
-        #         if bool(r_api_p_value):
-        #             raw_api_parameters_list.append(r_api_param)
+        raw_api_parameters_list = jmespath.search(generated_jmespath_nested_selector, related_operations_data)
+        
         if raw_api_parameters_list == []:
             # successfull jmespath search that yielded no results. operation data might be empty
-            return raw_api_parameters_list, Error(
-                "related resources not found",
-                {
-                    "service": self.service_node.name,
-                    "resource_node": self.name,
-                    "operation_name": operation_name,
-                },
-            )
+            return raw_api_parameters_list
         elif not raw_api_parameters_list:
-            logger.debug(
-                f"CANT GENERATE API PARAMETERS LIST WITH [bold][red]{generated_jmespath_nested_selector}[/] {related_operations_data=}"
-            )
-            return False, Error(
-                "failed to generate api parameters",
-                {
-                    "service": self.service_node.name,
-                    "resource_node": self.name,
-                    "operation_name": operation_name,
-                },
-            )
-
-        return raw_api_parameters_list, None
-
+            logger.debug(f"CANT GENERATE API PARAMETERS LIST WITH [bold][red]{generated_jmespath_nested_selector}[/] {related_operations_data=}")
+            return False
+        
+        return raw_api_parameters_list
+    
     # NOTE: +overrideable
-    def complement_api_parameters_list(
-        self,
-        operation_name: str,
-        related_operations_data: Union[List, Dict],
-        relations_of_operation: List[Dict],
-        raw_api_parameters_list: List,
-    ) -> List[Dict]:
-        """Uses the `raw_api_parameters_list` and appends pagination parameters(MaxResults,...) to them.
-            Also provided for easy subclass overriding.
-
-        Args:
-            operation_name (str): Name of the operation.
-            related_operations_data (Union[List, Dict]): All related operations data
-            relations_of_operation (List[Dict]): Relations of the operation
-            raw_api_parameters_list (List): Generated raw API parameters
-
-        Returns:
-            List[Dict]: Valid API parameters to call the boto operation with
-        """
-
+    def create_valid_api_parameters_list(self, operation_name, related_operations_data, relations_of_operation, raw_api_parameters_list ):
         operation_model = self.get_operation_model(operation_name)
-        required_parameter_names = (
-            self.get_required_parameter_names_from_operation_model(operation_model)
-        )
+        required_parameter_names = self.get_required_parameter_names_from_operation_name(operation_name)
 
         input_shape = get_input_shape(operation_model)
         generated = {}
-
-        # input shape may not exists, meaning no required parameters
+        
         if input_shape:
             generated = argument_generator.generate_skeleton(input_shape)
+        
+        result = {}
 
-        api_params = [{}]
-        if raw_api_parameters_list:
-            api_params = raw_api_parameters_list
-
+        for r_parameter_name in required_parameter_names:
+            r_key = find_key_in_dict_keys(r_parameter_name, generated)
+            if r_key:
+                result[r_key] = generated[r_key]
+                
         # handle MaxResults
         max_results_value = get_max_results_value_from_shape(input_shape)
-        max_results_key = find_key_in_dict_keys("maxresults", generated)
+        max_results_key = find_key_in_dict_keys('maxresults', generated)
         if max_results_key and max_results_value:
-            for api_param in api_params:
-                api_param.update({max_results_key: max_results_value})
-
+            result[max_results_key]=max_results_value
         # sometimes MaxResults can be seen as non required parameter, but in fact is
         if not required_parameter_names:
-            return api_params
-
+            return [result]
+        
+        
+        search_to_target_names = {relation.get('target_shape_name'):relation.get('search_shape_name') for relation in relations_of_operation}
+        
+        generated_api_params = []
         if raw_api_parameters_list == False:
-            # this func expect raw_api_parameters_list present, only adds to prepared parameters
-            logger.debug(
-                f"FAILED TO CREATE VALID API PARAMETERS. Required Parameters are: [bold]{required_parameter_names}[/]"
-            )
+            # TODO: add logic here
+            logger.debug(f"FAILED TO CREATE VALID API PARAMETERS. Required Parameters are: [bold]{required_parameter_names}[/]")
             return False
-
-        return api_params
-
+        for raw_api_parameter_dict in raw_api_parameters_list:
+            result_copy = copy.deepcopy(result)
+            for raw_key in raw_api_parameter_dict.keys():
+                found_parameter_key = find_key_in_dict_keys(raw_key, result_copy)
+                if not found_parameter_key:
+                    # search to target name
+                    new_key = find_key_in_dict_keys(raw_key, search_to_target_names)
+                    if new_key:
+                        found_parameter_key = find_key_in_dict_keys(search_to_target_names[new_key], result_copy)
+                result_copy[found_parameter_key] = raw_api_parameter_dict[raw_key]
+            generated_api_params.append(result_copy)
+        # Handle NextToken and DryRun
+        # dry_run_key_name = find_key_in_dict_keys('dryrun', generated)
+        # generated.pop(dry_run_key_name)
+        # next_token_key_name = find_key_in_dict_keys('nexttoken', generated)
+        # generated.pop(next_token_key_name)
+        # generated
+        # # handle multiple required parameters
+        # generated_api_params_list = []
+        # for r_parameter_name in required_parameter_names:
+        #     r_parameter_name_key = find_key_in_dict_keys(r_parameter_name, generated)
+        #     r_parameter_value = generated.get(r_parameter_name_key)
+        #     # if type
+            
+        #     # result[r_parameter_name_key] = ?
+        # generated
+        return generated_api_params
+    
     # NOTE: +overrideable
-    def generate_api_parameters_from_operation_data(
-        self,
-        operation_name: str,
-        relations_of_operation: List[Dict],
-        related_operations_data: Union[List, Dict],
-    ) -> Tuple[Union[List, bool], Union[Error, None]]:
-        """Generates API parameters for the given operation including pagination parameters.
-
-        Args:
-            operation_name (str): Name of the operation
-            relations_of_operation (List[Dict]): Relations of the operation
-            related_operations_data (Union[List, Dict]): All related operations data
-
-        Returns:
-            List: Generated API Parameters to call the Operations with
-        """
+    def generate_api_parameters_from_operation_data(self, operation_name, relations_of_operation, related_operations_data):
         resource_node = self
-        required_parameters = (
-            resource_node.get_required_parameter_names_from_operation_name(
-                operation_name
-            )
-        )
-        no_relations = relations_of_operation == []
-        no_required_parameters = required_parameters == []
+        resource_node_name = resource_node.name
+        no_required_parameters = relations_of_operation == []
 
         if no_required_parameters:
-            # Even though we know there are no required parameters,
-            # some parameters like MaxResults must be filled, if available.
-            api_parameters = resource_node.complement_api_parameters_list(
-                operation_name, related_operations_data, [], []
-            )
-            return api_parameters, None
-
-        if no_relations:
-            # todo
-            pass
-        # try to automatically generate the required parameters with relations
-        (
-            raw_api_parameters_list,
-            raw_param_error,
-        ) = self._generate_raw_api_parameters_from_operation_data(
-            operation_name, relations_of_operation, related_operations_data
-        )
-        if raw_param_error is not None:
-            # failed to generate raw api parameters list
-            return False, raw_param_error
-
-        # fill out the pagination parameters like MaxResults, ...
-        api_parameters_list = resource_node.complement_api_parameters_list(
-            operation_name,
-            related_operations_data,
-            relations_of_operation,
-            raw_api_parameters_list,
-        )
-        if not api_parameters_list:
-            return api_parameters_list, Error(
-                "failed to generate api parameters",
-                {
-                    "service": self.service_node.name,
-                    "resource_node": self.name,
-                    "operation_name": operation_name,
-                },
-            )
-
-        return api_parameters_list, None
-
-    def print_operation(self, operation_name: str) -> None:
+            # Even though we know there are no required parameters, 
+            # some parameters like MaxResults must be filled.
+            api_parameters = resource_node.create_valid_api_parameters_list(operation_name, related_operations_data, [], [])
+            return api_parameters
+
+        related_operations_data
+        raw_api_parameters_list = self._generate_raw_api_parameters_from_operation_data(operation_name, relations_of_operation, related_operations_data)
+                
+        api_parameters_list = resource_node.create_valid_api_parameters_list(operation_name, related_operations_data, relations_of_operation, raw_api_parameters_list)
+        return api_parameters_list
+    
+    def print_operation(self, operation_name):
         operation_panel = self._rich_operation_details_panel(operation_name)
         console.print(operation_panel)
 
-    def _rich_operation_details_panel(self, operation_name: str) -> Panel:
-
+    def _rich_operation_details_panel(self, operation_name):
+        
         operation_model = self.get_operation_model(operation_name)
         input_shape = get_input_shape(operation_model)
         output_shape = operation_model.output_shape
-
+        
         input_shape_tree = Text("[yellow]No Input Shape Found")
         if input_shape:
             input_shape_tree = generate_rich_tree_from_shape(input_shape)
         output_shape_tree = generate_rich_tree_from_shape(output_shape)
-
-        operation_docs = cleanhtml(operation_model.documentation)
-        panel_group = Group(
-            Padding(f"[bold underline]Documentation:[/] {operation_docs}", (1, 2)),
-            Panel(
-                input_shape_tree,
-                title=f"Input: [yellow]{input_shape.name}",
-                title_align="left",
-                padding=(1, 1),
-            ),
-            Panel(
-                output_shape_tree,
-                title=f"Output: [yellow]{output_shape.name}",
-                title_align="left",
-                padding=(1, 1),
-            ),
-        )
-
-        required_parameters = self.get_required_parameter_names_from_operation_name(
-            operation_name
-        )
-        _title = f"[bold]Operation[/]: [magenta bold]{operation_name}[/]"
+        layout = Layout()
+        layout.split_row(
+            Panel(input_shape_tree, title='[yellow]Input Shape'),# subtitle=get_shape_name(input_shape)),
+            Panel(output_shape_tree, title='[yellow]Output Shape'),# subtitle=get_shape_name(output_shape)),
+        )
+      
+        required_parameters = self.get_required_parameter_names_from_operation_name(operation_name)
+        _title = f"Operation: [green][bold]{operation_name}[/]"
         if required_parameters:
             _title = f"{_title}   [white][Required: {', '.join(required_parameters)}]"
-        operation_panel = Panel(
-            panel_group, title=_title, highlight=True, title_align="left"
-        )
+        operation_panel = Panel(layout, title=_title, highlight=True, title_align='left')
         return operation_panel
 
-    def find_best_relation_for_single_parameter(
-        self, parameter_name: str, generated_relations_for_parameter: List[Dict]
-    ) -> List[Dict]:
-        if len(generated_relations_for_parameter) == 1:
-            # found only one relation, no need to find the correct one
-            return generated_relations_for_parameter
 
-        # strip the required parameter name's identifiers
+    # todo: move to Reader
+    def select_between_possible_relation_combinations_matrix(self, possible_relation_combinations):
+        if len(possible_relation_combinations)==1:
+            return possible_relation_combinations[0]
+        # each combination will have the same operation name
+        # prefer using non-GET function
+        # prefer the operation that has no required parameters
+        combination_index_to_score_map = {str(i):0 for i in range(len(possible_relation_combinations))}
+        
+        for i, relation_combination in enumerate(possible_relation_combinations):
+            current_combination_point = 0
+            combinations_operation_name = relation_combination[0].get('operation_name') # promised to all have same operation
+            
+            # negative point if it has required parameters
+            combinations_required_parameters = self.get_required_parameter_names_from_operation_name(combinations_operation_name)
+            current_combination_point -= len(combinations_required_parameters)
+            
+            # negative point if its a get function, we'd like to prefer list or describe functions
+            if combinations_operation_name.lower().startswith('get'):
+                current_combination_point -= 1
+            
+            combination_index_to_score_map[str(i)] = current_combination_point
+        selected_index_str, selected_score = max(combination_index_to_score_map.items(), key=lambda index_and_score: index_and_score[1])
+        selected_combination = possible_relation_combinations[int(selected_index_str)]
+        
+        return selected_combination
+
+    # todo: move to Reader
+    def select_between_possible_relation_combinations_list(self, possible_relation_list):
+        if len(possible_relation_list)<1:
+            return False
+        if len(possible_relation_list)==1:
+            return possible_relation_list[0]
+        # each combination will have the same operation name
+        # prefer using non-GET function
+        # prefer the operation that has no required parameters
+        combination_index_to_score_map = {str(i):0 for i in range(len(possible_relation_list))}
+        
+        get_operation_count  = [p_rel.get('operation_name').startswith('Get') for p_rel in possible_relation_list].count(True)
+        for i, relation_dict in enumerate(possible_relation_list):
+            current_combination_point = 0
+            relations_operation_name = relation_dict.get('operation_name') # promised to all have same operation
+            
+            # negative point if it has required parameters
+            combinations_required_parameters = self.get_required_parameter_names_from_operation_name(relations_operation_name)
+            current_combination_point -= len(combinations_required_parameters)
+            
+            # negative point if its a get function, we'd like to prefer list or describe functions
+            if get_operation_count <= 1 and relations_operation_name.lower().startswith('get'):
+                current_combination_point -= 1
+            
+            combination_index_to_score_map[str(i)] = current_combination_point
+        selected_index_str, selected_score = max(combination_index_to_score_map.items(), key=lambda index_and_score: index_and_score[1])
+        selected_combination = possible_relation_list[int(selected_index_str)]
+        
+        return selected_combination
+    
+    # todo: move to Reader
+    def find_best_relation_for_single_parameter(self, parameter_name, relation_list):
         _parameter_name_tokens = camel_case_split(parameter_name)
         non_id_parameter_tokens = [
-            p_token
-            for p_token in _parameter_name_tokens
+            p_token for p_token in _parameter_name_tokens
             if p_token.lower() not in IDENTIFIER_NAMES
         ]
+        
+        # if not non_id_parameter_tokens:
+        #     # only contains id 
+        #     non_id_parameter_tokens  =_parameter_name_tokens
 
-        # filter the gen. relation's resource name and required parameter name
         same_resource_name_relations = []
-        for relation_obj in generated_relations_for_parameter:
-            resource_node_name = relation_obj.resource_node_name
-            resource_name_tokens = camel_case_split(resource_node_name)
+        for relation_dict in relation_list:
+            operation_name = relation_dict.get('operation_name')
+            operation_verb, *operation_name_tokens = camel_case_split(operation_name)
+            # relation_dict.update({'operation_verb': operation_verb, 'operation_name_tokens': operation_name_tokens})
+            # TODO: here
             all_tokens_match = icompare_two_token_lists(
-                non_id_parameter_tokens, resource_name_tokens
-            )
+                non_id_parameter_tokens, operation_name_tokens)
             if all_tokens_match:
-                same_resource_name_relations.append(relation_obj)
-
-        if not same_resource_name_relations:
-            return False
-
-        # if there is only one relation with the same resource name, return it
-        if len(same_resource_name_relations) == 1:
-            return same_resource_name_relations
-
-        # try to filter out the bad relations
-        possible_relation_list = same_resource_name_relations
-        relation_index_to_score_map = {
-            str(i): 0 for i in range(len(possible_relation_list))
-        }
-
-        for i, relation_obj in enumerate(possible_relation_list):
-            current_point = 0
-            relations_operation_name = relation_obj.operation_name
-            # promised to all have same operation
-            # negative point if it has required parameters
-            relations_required_parameters = (
-                self.get_required_parameter_names_from_operation_name(
-                    relations_operation_name
-                )
-            )
-            current_point -= len(relations_required_parameters)
-
-            # List verb gets +1 point
-            if relations_operation_name.lower().startswith("list"):
-                current_point += 1
-
-            relation_index_to_score_map[str(i)] += current_point
-
-        # select the best score
-        selected_index_str, selected_score = max(
-            relation_index_to_score_map.items(),
-            key=lambda index_and_score: index_and_score[1],
-        )
-        selected_relation = possible_relation_list[int(selected_index_str)]
-
+                same_resource_name_relations.append(relation_dict)
+                    
+        # what we are left with is different operations names 
+        selected_relation = self.select_between_possible_relation_combinations_list(same_resource_name_relations)
         if selected_relation:
             return [selected_relation]
-
-        return False
-
-    def get_pagination_token_output_to_parameter_name_mapping(
-        self, operation_name: str
-    ) -> Union[Dict[str, str], bool]:
-        """Some Operations paginate their output using Pagination Token Parameters defined in `PAGINATION_TOKEN_KEYS`.
-
-        Args:
-            resource_node (ResourceNode): _description_
-            operation_name (str): Name of the operation in the resource_node.
-
-        Returns:
-            Union[Dict[str, str], bool]: False or A dictionary with `parameter_name` and `output_key` keys. e.g. `{"parameter_name":"nextToken", "output_key": "NextToken"}`.
-        """
-        resource_node: ResourceNode = self
-
-        # find all parameter names that are in `PAGINATION_TOKEN_KEYS`, case insensitive
-        parameter_names = [
-            pn
-            for pn in resource_node.get_all_parameter_names_from_operation_name(
-                operation_name
-            )
-            if is_word_in_a_list_of_words(pn, PAGINATION_TOKEN_KEYS)
-        ]
-
-        #  find all output keys that are in `PAGINATION_TOKEN_KEYS`, case insensitive
-        output_keys = [
-            ok
-            for ok in resource_node.get_all_output_keys_from_operation_name(
-                operation_name
-            )
-            if is_word_in_a_list_of_words(ok, PAGINATION_TOKEN_KEYS)
-        ]
-
-        if output_keys and parameter_names:
-            return {
-                "parameter_name": parameter_names[0],
-                "output_key": output_keys[0],
-            }
         return False
-
-    def get_required_parameter_names_from_operation_model(self, operation_model):
+    
+    def get_required_parameter_names_from_operation_name(self, operation_name):
+        
+        operation_model = self.get_operation_model(operation_name)
         input_shape = get_input_shape(operation_model)
         if not input_shape:
             return []
-        required_parameter_names = getattr(input_shape, "required_members", False)
-        max_results_key = find_key_in_dict_keys("maxresults", required_parameter_names)
+        required_parameter_names = getattr(input_shape, 'required_members', False)
+        max_results_key = find_key_in_dict_keys('maxresults', required_parameter_names)
         if max_results_key:
             required_parameter_names.remove(max_results_key)
         return required_parameter_names
-
-    def get_all_parameter_names_from_operation_name(self, operation_name):
-        operation_model = self.get_operation_model(operation_name)
-        input_shape = get_input_shape(operation_model)
-        if not input_shape:
-            return []
-
-        all_parameter_names = []
-        input_shape_and_target_paths = _flatten_shape_to_its_members_and_target_paths(
-            input_shape
-        )
-        for shape_and_target_path in input_shape_and_target_paths:
-            shape_name = get_shape_name(shape_and_target_path.shape)
-            if shape_name:
-                all_parameter_names.append(shape_name)
-        return all_parameter_names
-
-    def get_all_output_keys_from_operation_name(self, operation_name):
-        operation_model = self.get_operation_model(operation_name)
-        output_shape = operation_model.output_shape
-        if not output_shape:
-            return []
-
-        all_parameter_names = []
-        input_shape_and_target_paths = _flatten_shape_to_its_members_and_target_paths(
-            output_shape
-        )
-        for shape_and_target_path in input_shape_and_target_paths:
-            shape_name = get_shape_name(shape_and_target_path.shape)
-            if shape_name:
-                all_parameter_names.append(shape_name)
-        return all_parameter_names
-
-    # TODO: memoization
-    def get_required_parameter_names_from_operation_name(
-        self, operation_name: str
-    ) -> List[str]:
-        operation_model = self.get_operation_model(operation_name)
-        return self.get_required_parameter_names_from_operation_model(operation_model)
-
-    def get_all_required_parameter_names(self) -> List[str]:
+    
+    def get_all_required_parameter_names(self):
         all_required_names = []
         for operation_name in self.operation_names:
             required_shapes = self.get_required_parameter_names_from_operation_name(
-                operation_name
-            )
+                operation_name)
             all_required_names.extend(required_shapes)
         return all_required_names
-
+    
     def get_operation_model(self, operation_name: str) -> OperationModel:
+        """client._service_model"""
         if operation_name in self._operation_models:
             return self._operation_models[operation_name]
         service_model = self.service_node.get_service_model()
         operation_model = service_model.operation_model(operation_name)
         self._operation_models[operation_name] = operation_model
         return operation_model
 
-    def json(self) -> Dict:
+    def json(self):
         return {
             "service_node_name": self.service_node.name,
             "name": self.name,
-            "operation_names": self.operation_names,
+            "operation_names": self.operation_names
         }
 
-    def __str__(self) -> str:
+    def __str__(self):
         # return f"[{self.service_node.name}.{self.name}]"
         return f"[{self.name}]"
 
-
-class YamlResourceNode(ResourceNode):
-    def __init__(
-        self,
-        service_node: "ServiceNode",
-        name: str,
-        operation_names: List[str],
-        yaml_config: Dict = None,
-    ) -> None:
-        super().__init__(service_node, name, operation_names)
-        self.yaml_config = yaml_config
-
-    def define_extra_relations(self) -> Union[List[Dict], List[Relation]]:
-        if not self.yaml_config.extra_relations:
-            return []
-        extra_relations = [
-            Relation(**extra_relation.__dict__)
-            for extra_relation in self.yaml_config.extra_relations
-        ]
-        return extra_relations
-
-    def get_pagination_token_output_to_parameter_name_mapping(
-            self, operation_name: str
-        ) -> Union[Dict[str, str], bool]:
-        operations = self.yaml_config.operations
-        for operation in operations:
-            if operation_name == operation.operation_name:
-                if operation.pagination_token_mapping:
-                    return operation.pagination_token_mapping
-
-        return super().get_pagination_token_output_to_parameter_name_mapping(operation_name)
-
-    # NOTE: +overrideable
-    def get_operations_relations(
-        self, operation_name: str
-    ) -> Tuple[Union[List[Dict], bool], Union[Error, None]]:
-        operations = self.yaml_config.operations
-        for operation in operations:
-            if operation_name == operation.operation_name:
-                # cast schema to Relation objects
-                if operation.explicit_relations:
-                    explicit_relations = [
-                        Relation(**rel_model.__dict__)
-                        for rel_model in operation.explicit_relations
-                    ]
-                    return explicit_relations, None
-        # if no explicit relations are defined, then call the ResourceNode method and return it
-        return super().get_operations_relations(operation_name)
-
-    # NOTE: +overrideable
-    def generate_jmespath_selector_from_relations(
-        self, operation_name: str, relation_list: List[Dict]
-    ) -> str:
-        operations = self.yaml_config.operations
-        for operation in operations:
-            if operation_name == operation.operation_name:
-                if operation.jmespath_selector:
-                    js_selector = operation.jmespath_selector
-                    return js_selector
-
-        return super().generate_jmespath_selector_from_relations(
-            operation_name, relation_list
-        )
-
-    # NOTE: +overrideable
-    def complement_api_parameters_list(
-        self,
-        operation_name: str,
-        related_operations_data: Union[List, Dict],
-        relations_of_operation: List[Dict],
-        raw_api_parameters_list: List,
-    ) -> List:
-
-        precomplemented_api_params = super().complement_api_parameters_list(
-            operation_name,
-            related_operations_data,
-            relations_of_operation,
-            raw_api_parameters_list,
-        )
-
-        for operation in self.yaml_config.operations:
-            if operation_name == operation.operation_name:
-                if operation.complement_api_parameters:
-                    # if the option is defined
-                    for complement_action in operation.complement_api_parameters:
-                        if complement_action.action == "add":
-                            data = complement_action.data
-                            for api_param_item in precomplemented_api_params:
-                                api_param_item.update(data)
-
-                        elif complement_action.action == "remove":
-                            for api_param_item in precomplemented_api_params:
-                                for remove_key in complement_action.keys:
-                                    api_param_item.pop(remove_key, None)
-
-        return precomplemented_api_params
-
-    def generate_api_parameters_from_operation_data(
-        self,
-        operation_name: str,
-        relations_of_operation: List[Dict],
-        related_operations_data: Union[List, Dict],
-    ) -> Tuple[Union[List, bool], Union[Error, None]]:
-        """
-        get a list for api parameters, override them
-        """
-        operations = self.yaml_config.operations
-        for operation in operations:
-            if operation_name == operation.operation_name:
-                override_parameters = operation.override_api_parameters
-                if override_parameters:
-                    return override_parameters, None
-
-        # if not defined, fall back to the default super class method
-        return super().generate_api_parameters_from_operation_data(
-            operation_name, relations_of_operation, related_operations_data
-        )
+    def __rich__(self):
+        return 'ss'
+ 
+ 
 
 
 class ServiceNode:
     def __init__(self, name, session):
         self.name = name
         self.session = session
         self.client = self.session.client(self.name)
         self.resource_nodes = None
         self._relation_map = None
         self._reader = None
         self._read_operation_name_to_tokens_map = None
 
-    def get_client(self):
-        return self.client
-
-    def get_service_reader(self) -> ServiceReader:
-        """Returns/creates the ServiceReader for the current ServiceNode
 
-        Returns:
-            ServiceReader: ServiceReader object for current ServiceNode
-        """
+    def read(self, resource_node_name):
+        reader = self.get_service_reader()
+        return reader.read_resource_node(resource_node_name)
+    
+    def get_service_reader(self):
         if not self._reader:
             self._reader = ServiceReader(self)
         return self._reader
 
-    def print_resource_node(self, resource_node_name: str) -> None:
+    def print_resource_node(self, resource_node_name):
         # TODO: check if resource node exists
         operations_panel = self._get_operation_details_panel(resource_node_name)
         if operations_panel:
             console.print(operations_panel)
-
-    def _get_operation_details_panel(self, resource_node_name: str) -> Panel:
-        resource_node = self.get_resource_node_by_name(resource_node_name)
+        
+    def _get_operation_details_panel(self, resource_node_name):
+        resource_node =  self.get_resource_node_by_name(resource_node_name)
         if not resource_node:
             return False
         panels_for_operations = [
             resource_node._rich_operation_details_panel(operation_name)
             for operation_name in resource_node.operation_names
         ]
 
-        operations_group = Group(*panels_for_operations)
-        return Panel(
-            operations_group,
-            title=f"[bold]Resource Node: [blue]{resource_node.name} ",
-            title_align="left",
+        operations_group = Group(
+            *panels_for_operations
         )
-
-    def get_resource_node_by_name(self, resource_node_name: str) -> ResourceNode:
-        """Searches the current ServiceNode for the given `resource_node_name`,
-        and returns it.
-
-        Args:
-            resource_node_name (str): Name of the ResourceNode
-
-        Returns:
-            ResourceNode: The ResourceNode object, `False` if not found.
-        """
+        return Panel(operations_group, title=f'Resource Node: [blue][bold]{resource_node.name} ', title_align='left')
+        
+    def get_resource_node_by_name(self, resource_node_name):
         if not resource_node_name:
             return False
-
+        
         for r_node in self.get_resource_nodes():
             # FIXME: laterr
             # if r_node.name == resource_node_name:
             if icompare_two_camel_case_words(r_node.name, resource_node_name):
                 return r_node
         return False
-
-    def json(self) -> Dict:
+    
+    def json(self):
         return {
             "service_name": self.name,
             # TODO:
         }
 
-    # TODO: memoization
-    def find_resource_node_by_operation_name(self, operation_name: str) -> ResourceNode:
-        """Traverses the ResourceNodes of the current ServiceNode and tries to find
-        the ResourceNode that has the `operation_name` in it.
-
-        Args:
-            operation_name (str): Name of the operation
-
-        Returns:
-            ResourceNode: ResourceNode object that has the `operation_name`, or None.
-        """
+    def find_resource_node_by_operation_name(self, operation_name):
         for r_node in self.get_resource_nodes():
             if operation_name in r_node.operation_names:
                 return r_node
         return None
 
-    def get_relation_map(self) -> RelationMap:
-        """Gets the relation map object.
-
-        Returns:
-            RelationMap: RelationMap object for the current ServiceNode
-        """
+    def get_relation_map(self):
         if self._relation_map is not None:
             return self._relation_map
         self._relation_map = RelationMap(self)
         return self._relation_map
 
-    def get_resource_nodes(self) -> List[ResourceNode]:
-        """Gets the available `ResourceNode`s of the current ServiceNode
-
-        Returns:
-            List[ResourceNode]: List of `ResourceNode`s available in the ServiceNode
-        """
+    def get_resource_nodes(self):
         if self.resource_nodes is None:
             self.resource_nodes = self._generate_resource_nodes()
         return self.resource_nodes
 
-    def create_resource_node(self, **kwargs: Dict) -> ResourceNode:
-        """Creates the ResourceNode object with the given `kwargs`.
-        Uses the `ResourceNodeRegistry` to find the custom subclasses of the
-        `ResourceNode` class, else defaults to use the ResourceNode class
-
-        Raises: # TODO: fix this, return false instead
-            Exception: _description_
-
-        Returns:
-            ResourceNode: _description_
-        """
+    def create_resource_node(self, **kwargs):
         service_name = self.name
-        resource_node_name = kwargs.get("name", False)
+        resource_node_name = kwargs.get('name', False)
         _ResourceNodeClass = ResourceNode
         if not resource_node_name:
-            logger.debug("A resource name must be provided on creation.", extra=kwargs)
-            raise Exception("ResourceNode name must be provided.")
-        _custom_cls_for_resource_node = (
-            _resource_node_registry.find_custom_class_for_resource_node(
-                service_name, resource_node_name
-            )
-        )
+            logger.debug(f"A resource name must be provided on creation.", extra=kwargs)
+            raise Exception('ResourceNode name must be provided.')
+        _custom_cls_for_resource_node = _resource_node_registry.find_custom_class_for_resource_node(service_name, resource_node_name)
         if _custom_cls_for_resource_node:
-            logger.debug(
-                f"ResourceNodeRegistry: [bold][green]{service_name}[/].[blue]{resource_node_name}[/][/] has extended with custom class."
-            )
+            # print(_custom_cls_for_resource_node, 'is used for ', service_name, resource_node_name)
+            logger.debug(f"Registry: {_custom_cls_for_resource_node} class is used for  [bold][green]{service_name}[/].[blue]{resource_node_name}")
             _ResourceNodeClass = _custom_cls_for_resource_node
-            return _ResourceNodeClass(**kwargs)
-
-        # try to find yaml config defined for this ResourceNode
-        yaml_config_found = _resource_node_registry.search_yaml_config_registry(
-            service_name, resource_node_name
-        )
-        if yaml_config_found:
-            # add the yaml_config for the YamlResourceNode subclass initialization
-            kwargs.update({"yaml_config": yaml_config_found})
-            logger.debug(f"ResourceNodeRegistry: [bold][green]{service_name}[/].[blue]{resource_node_name}[/][/] has extended with custom yaml config.")
-            yaml_resource_node_obj = YamlResourceNode(**kwargs)
-            return yaml_resource_node_obj
-
-        # return default ResourceNode class
         return _ResourceNodeClass(**kwargs)
-
-    def _generate_resource_nodes(self) -> List[ResourceNode]:
-        """Parses `botocore` client for the AWS service and generates ResourceNodes.
-        Generated `ResourceNode`s can be subclasses of `ResourceNode`.
-
-        Returns:
-            List[ResourceNode]: List of generated `ResourceNode`s
-        """
+    
+    def _generate_resource_nodes(self):
         generated_resouce_nodes = []
         op_name_to_tokens_map = self.get_read_operation_name_to_tokens_map()
         resource_name_to_operations_map = {}
         for operation_name, op_name_tokens in op_name_to_tokens_map.items():
             verb, *resource_name_list = op_name_tokens
-            resource_node_name = "".join(resource_name_list)
-
-            found_key = ifind_key_in_dict_keys(
-                resource_node_name, resource_name_to_operations_map.keys()
-            )
+            resource_node_name = ''.join(resource_name_list)
+            
+            found_key = ifind_key_in_dict_keys(resource_node_name, resource_name_to_operations_map.keys())
             if found_key:
                 # decide if we want to keep the plural or singular name
-
+                
                 sp_comparison = compare_nouns(resource_node_name, found_key)
-                if sp_comparison == "s:p":
+                if sp_comparison == 's:p':
                     # swap the found_key with resource_node_name as dict key
-                    resource_name_to_operations_map[resource_node_name] = [
-                        operation_name
-                    ] + resource_name_to_operations_map[found_key]
+                    resource_name_to_operations_map[resource_node_name] = [operation_name] + resource_name_to_operations_map[found_key]
                     resource_name_to_operations_map.pop(found_key)
                 else:
-                    resource_name_to_operations_map[found_key].append(operation_name)
+                    resource_name_to_operations_map[found_key].append(operation_name)                
             else:
-                resource_name_to_operations_map[resource_node_name] = [operation_name]
+                resource_name_to_operations_map[resource_node_name] = [
+                    operation_name]
 
         # createt the resource nodes
-        for (
-            resource_node_name,
-            operations_list,
-        ) in resource_name_to_operations_map.items():
+        for resource_node_name, operations_list in resource_name_to_operations_map.items():
             created_resource_node = self.create_resource_node(
-                service_node=self,
-                name=resource_node_name,
-                operation_names=operations_list,
+                service_node=self, 
+                name=resource_node_name, 
+                operation_names=operations_list
             )
             if created_resource_node:
                 generated_resouce_nodes.append(created_resource_node)
 
         if len(generated_resouce_nodes) <= 1:
             return generated_resouce_nodes
 
@@ -1019,91 +607,64 @@
         # concat same names
         combined_resource_nodes = []
         _used_for_combining_resource_nodes = []
 
         for i, gen_resource_node in enumerate(generated_resouce_nodes[:-1]):
             if gen_resource_node in _used_for_combining_resource_nodes:
                 continue
-            for other_resource_node in generated_resouce_nodes[i + 1 :]:
+            for other_resource_node in generated_resouce_nodes[i+1:]:
                 # FIXME: IMPORTANT
-                if compare_two_camel_case_words(
-                    gen_resource_node.name, other_resource_node.name
-                ):
+                if compare_two_camel_case_words(gen_resource_node.name, other_resource_node.name):
                     # select the shortest name, meaning singular
                     singular_named_resource_node = gen_resource_node
                     plural_named_resource_node = other_resource_node
-                    if len(singular_named_resource_node.name) > len(
-                        plural_named_resource_node.name
-                    ):
-                        singular_named_resource_node, plural_named_resource_node = (
-                            plural_named_resource_node,
-                            singular_named_resource_node,
-                        )
+                    if len(singular_named_resource_node.name) > len(plural_named_resource_node.name):
+                        singular_named_resource_node, plural_named_resource_node = plural_named_resource_node, singular_named_resource_node
                     _used_for_combining_resource_nodes.append(
-                        plural_named_resource_node
-                    )
+                        plural_named_resource_node)
                     singular_named_resource_node.operation_names.extend(
-                        plural_named_resource_node.operation_names
-                    )
+                        plural_named_resource_node.operation_names)
 
             if gen_resource_node not in _used_for_combining_resource_nodes:
                 combined_resource_nodes.append(gen_resource_node)
 
         return combined_resource_nodes
 
-    def get_read_operation_name_to_tokens_map(self) -> Dict:
-        """Generate `operation name to word tokens` map for the
-        available read operations in the ServiceNode.
-
-        Caches the output in the class attr. `_read_operation_name_to_tokens_map`.
-
-        Returns:
-            Dict: dictionary
-        """
+    def get_read_operation_name_to_tokens_map(self):
         if self._read_operation_name_to_tokens_map is not None:
             return self._read_operation_name_to_tokens_map
         read_operation_names = self.get_read_operation_names()
-        self._read_operation_name_to_tokens_map = (
-            self._generate_operation_name_to_tokens_map(read_operation_names)
-        )
+        self._read_operation_name_to_tokens_map = self._generate_operation_name_to_tokens_map(
+            read_operation_names)
         return self._read_operation_name_to_tokens_map
 
-    def _generate_operation_name_to_tokens_map(
-        self, operation_names: List[str] = None
-    ) -> Dict:
+    def _generate_operation_name_to_tokens_map(self, operation_names:List[str]=None):
         if operation_names is None:
             operation_names = self.get_operation_names()
 
         op_name_to_tokens = {
-            op_name: camel_case_split(op_name) for op_name in operation_names
+            op_name: camel_case_split(op_name)
+            for op_name in operation_names
         }
         return op_name_to_tokens
 
     def get_read_operation_names(self) -> List[str]:
-        """Gets the operation names from the boto3 client and
-        filters the operation names starting with `List`,`Get` or `Describe`.
-
-        Returns:
-            List[str]: Read Only operation names
-        """
         operation_names = self.get_operation_names()
         read_only_operation_names = [
             op_name
             for op_name in operation_names
             if any([op_name.startswith(read_verb) for read_verb in READ_ONLY_VERBS])
         ]
         return read_only_operation_names
 
     def get_service_model(self) -> ServiceModel:
-        """Returns the ServiceModel obj from boto3 client"""
         service_model = self.client._service_model
         return service_model
 
     def get_event_system(self) -> EventAliaser:
-        """Returns the boto3 clients event system"""
         event_system = self.client.meta.events
         return event_system
 
     def get_operation_names(self) -> List[str]:
         """Returns the `operation_names` defined in the boto client._service_model"""
         service_model = self.get_service_model()
         operation_names = service_model.operation_names
```

### Comparing `balcony-0.0.80/balcony/utils.py` & `balcony-0.0.9/balcony/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,96 @@
-from collections import Counter
 from re import finditer, compile
 from typing import List
 import inflect
+inflect_engine = inflect.engine()  # used for same word comparing
 import os
 import boto3
 
-# from functools import lru_cache
-
-inflect_engine = inflect.engine()  # used for singular/plural word comparing
-
-
 _camel_case_regex_compiled = compile(
-    r".+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)"
-)
-
+    r".+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)")
 
 def _create_boto_session():
-    profile_name = os.environ.get("AWS_PROFILE", False)
-    region_name = os.environ.get("AWS_REGION", False)
+    profile_name = os.environ.get('AWS_PROFILE', False)
+    region_name = os.environ.get('AWS_REGION', False)
     _kwargs_dict = {}
     if profile_name:
-        _kwargs_dict["profile_name"] = profile_name
+        _kwargs_dict['profile_name']=profile_name
     if region_name:
-        _kwargs_dict["region_name"] = region_name
+        _kwargs_dict['region_name']=region_name
     session = boto3.session.Session(**_kwargs_dict)
-    return session
-
-
-def are_two_lists_same(list_one: List, list_two: List) -> bool:
-    """Compares the contents of two lists"""
-    return Counter(list_one) == Counter(list_two)
-
+    return session 
 
-def is_word_in_a_list_of_words(word: str, list_of_words: List[str]) -> bool:
-    """Checks if a word is a is in a list_of_words, case insensitive"""
-    lower_word = word.lower()
-    for a_word in list_of_words:
-        if lower_word == a_word.lower():
-            return True
-    return False
-
-    return word.lower() in []
-
-
-def ifind_similar_names_in_list(
-    search_for: str, search_in_list: List[str]
-) -> List[str]:
-    """Case insensitive find in list"""
-    result = []
-    if not search_for or not search_in_list:
+def ifind_similar_names_in_list(search_for, search_in_list):
+    # TODO: regex support
+    result = [] 
+    if not search_for:
         return result
     lower_search_for = search_for.lower()
-
+    
     for l_name in search_in_list:
         if l_name.lower().startswith(lower_search_for):
             result.append(l_name)
     return result
-
-
-def str_relations(relations: List[dict]) -> str:
-    """Stringify list of relations"""
-    return ", ".join(
-        [f"[{r.service_name}.{r.operation_name} > {r.target_path}]" for r in relations]
-    )
-
+# >>> items = set([-1, 0, 1, 2])
+# >>> set([1, 2]).issubset(items)
+# True
+# >>> set([1, 3]).issubset(items)
+# False
+
+def str_relations(relations):
+    return ", ".join([
+        f"[{r.get('service_name')}.{r.get('operation_name')} > {r.get('target_path')}]"
+        for r in relations
+    ])
 
 def get_all_available_services(session) -> List[str]:
-    """Gets available services from boto3 session"""
     return session.get_available_services()
 
-
-def compare_nouns(word1: str, word2: str) -> bool:
-    """Singular/plural insensitive word comparison"""
+def compare_nouns(word1: str, word2: str):
     return inflect_engine.compare_nouns(word1, word2)
 
-
-def compare_two_token_lists(
-    token_list_one: List[str], token_list_two: List[str]
-) -> bool:
-    """Compares to word lists one by one in lowercase"""
+def compare_two_token_lists(token_list_one, token_list_two):
     if len(token_list_one) != len(token_list_two):
         return False
     token_by_token_match = [
-        w1.lower() == w2.lower() for w1, w2 in zip(token_list_one, token_list_two)
+        w1.lower()==w2.lower()
+        for w1, w2 in zip(token_list_one, token_list_two)
     ]
     has_token_by_token_match = all(token_by_token_match)
     return has_token_by_token_match
 
-
-def icompare_two_token_lists(
-    token_list_one: List[str], token_list_two: List[str]
-) -> bool:
-    """Singular/plural insensitive token list comparison"""
+def icompare_two_token_lists(token_list_one, token_list_two):
     if len(token_list_one) != len(token_list_two):
         return False
     token_by_token_match = [
         bool(inflect_engine.compare_nouns(w1.lower(), w2.lower()))
         for w1, w2 in zip(token_list_one, token_list_two)
     ]
     has_token_by_token_match = all(token_by_token_match)
     return has_token_by_token_match
 
-
 def camel_case_split(identifier: str) -> List[str]:
-    """Splits CamelCase string to it's tokens"""
-    matches = finditer(_camel_case_regex_compiled, identifier)
+    """Splits camel case string to it's tokens"""
+    matches = finditer(
+        _camel_case_regex_compiled, identifier
+    )
     return [m.group(0) for m in matches]
 
-
-def compare_two_camel_case_words(word1: str, word2: str) -> bool:
+def compare_two_camel_case_words(word1, word2):
     token_list_1 = [_.lower() for _ in camel_case_split(word1)]
     token_list_2 = [_.lower() for _ in camel_case_split(word2)]
     return compare_two_token_lists(token_list_1, token_list_2)
 
 
-def icompare_two_camel_case_words(word1: str, word2: str) -> bool:
+def icompare_two_camel_case_words(word1, word2):
     token_list_1 = [_.lower() for _ in camel_case_split(word1)]
     token_list_2 = [_.lower() for _ in camel_case_split(word2)]
     return icompare_two_token_lists(token_list_1, token_list_2)
+
+def compare_two_tokens(token_one, token_two):
+    return bool(inflect_engine.compare_nouns(token_one, token_two))
+
+
+def get_last_token_of_target_path(target_path, delimiter='.'):
+    split_return_key = target_path.split(delimiter)
+    *prev_return_keys, last_return_key_name = split_return_key
+    return last_return_key_name
```

### Comparing `balcony-0.0.80/pyproject.toml` & `balcony-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.0.80"
+version = "0.0.9"
 description = "AWS API for humans"
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
@@ -12,20 +12,14 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 typer = "^0.6.1"
 rich = "^12.5.1"
 boto3 = "^1.24.80"
 jmespath = "^1.0.1"
 inflect = "^6.0.0"
-mkdocstrings = {version = "^0.19.0", extras = ["python"]}
-mkdocs-material = "^8.5.7"
-mkdocs-autorefs = "^0.4.1"
-PyYAML = "^6.0"
-pydantic = "^1.10.7"
-
 
 [tool.poetry.group.dev.dependencies]
 nose3 = "^1.3.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

