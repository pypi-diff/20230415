# Comparing `tmp/jsonschema_gentypes-1.7.2.tar.gz` & `tmp/jsonschema_gentypes-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-1.7.2.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-2.0.0.tar", max compression
```

## Comparing `jsonschema_gentypes-1.7.2.tar` & `jsonschema_gentypes-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,32 @@
--rw-r--r--   0        0        0     1304 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/LICENSE
--rw-r--r--   0        0        0     3554 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/README.md
--rw-r--r--   0        0        0    41603 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0     7376 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2429 2023-04-09 06:57:21.171635 jsonschema_gentypes-1.7.2/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     5125 2023-04-09 06:57:21.575640 jsonschema_gentypes-1.7.2/jsonschema_gentypes/jsonschema.py
--rw-r--r--   0        0        0        0 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     2842 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     5413 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/validate.py
--rw-r--r--   0        0        0     2500 2023-04-09 06:57:27.759710 jsonschema_gentypes-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     5051 1970-01-01 00:00:00.000000 jsonschema_gentypes-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/README.md
+-rw-r--r--   0        0        0    21740 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0    17139 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api.py
+-rw-r--r--   0        0        0    12886 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_04.py
+-rw-r--r--   0        0        0     1767 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_06.py
+-rw-r--r--   0        0        0      149 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_07.py
+-rw-r--r--   0        0        0     2999 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_2019_09.py
+-rw-r--r--   0        0        0     4296 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_2020_12.py
+-rw-r--r--   0        0        0     7328 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     2538 2023-04-15 09:41:31.924517 jsonschema_gentypes-2.0.0/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     4982 2023-04-15 09:41:34.536516 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_04.py
+-rw-r--r--   0        0        0     5251 2023-04-15 09:41:36.888514 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_06.py
+-rw-r--r--   0        0        0     5481 2023-04-15 09:41:39.152513 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_07.py
+-rw-r--r--   0        0        0     1698 2023-04-15 09:41:41.516512 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
+-rw-r--r--   0        0        0     1596 2023-04-15 09:41:48.024510 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
+-rw-r--r--   0        0        0      384 2023-04-15 09:41:54.484511 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
+-rw-r--r--   0        0        0     1260 2023-04-15 09:41:43.672510 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
+-rw-r--r--   0        0        0      296 2023-04-15 09:41:52.360511 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
+-rw-r--r--   0        0        0      973 2023-04-15 09:41:45.848510 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-04-15 09:41:50.236511 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
+-rw-r--r--   0        0        0     2569 2023-04-15 09:41:57.064512 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
+-rw-r--r--   0        0        0     1691 2023-04-15 09:42:03.348514 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
+-rw-r--r--   0        0        0      384 2023-04-15 09:42:07.720515 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
+-rw-r--r--   0        0        0      859 2023-04-15 09:41:59.116513 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
+-rw-r--r--   0        0        0      973 2023-04-15 09:42:01.164513 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-04-15 09:42:05.572515 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
+-rw-r--r--   0        0        0        0 2023-04-15 09:40:34.880489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     4133 2023-04-15 09:40:34.880489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/resolver.py
+-rw-r--r--   0        0        0     3067 2023-04-15 09:40:34.880489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     2514 2023-04-15 09:43:16.148113 jsonschema_gentypes-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.0.0/PKG-INFO
```

### Comparing `jsonschema_gentypes-1.7.2/LICENSE` & `jsonschema_gentypes-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.2/jsonschema_gentypes/cli.py` & `jsonschema_gentypes-2.0.0/jsonschema_gentypes/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 Generate the Python type files from the JSON schema files.
 """
 
 import argparse
-import json
 import logging
 import os
 import pkgutil
 import random
 import re
 import subprocess  # nosec
 import sys
 from typing import Dict, Optional, Set, Tuple, cast
 
-import requests
-import ruamel.yaml
-from jsonschema import RefResolver
+import yaml
 
-import jsonschema_gentypes
-from jsonschema_gentypes import configuration, validate
+import jsonschema_gentypes.api
+import jsonschema_gentypes.api_draft_04
+import jsonschema_gentypes.api_draft_06
+import jsonschema_gentypes.api_draft_07
+import jsonschema_gentypes.api_draft_2019_09
+import jsonschema_gentypes.api_draft_2020_12
+import jsonschema_gentypes.resolver
+from jsonschema_gentypes import configuration
 
 LOG = logging.getLogger(__name__)
 
 
 def _add_type(
     type_: jsonschema_gentypes.Type,
     imports: Dict[str, Set[str]],
@@ -91,23 +94,17 @@
                 }
             ],
         }
     else:
         schema_data = pkgutil.get_data("jsonschema_gentypes", "schema.json")
         assert schema_data
         with open(args.config, encoding="utf-8") as data_file:
-            yaml = ruamel.yaml.YAML()
-            data = yaml.load(data_file)
-        errors, data = validate.validate(args.config, data, json.loads(schema_data), True)
+            data = yaml.load(data_file, Loader=yaml.SafeLoader)
         config = cast(configuration.Configuration, data)
 
-        if errors:
-            LOG.error("The config file is invalid:\n%s", "\n".join(errors))
-            if not args.skip_config_errors:
-                sys.exit(1)
     process_config(config)
 
 
 def process_config(config: configuration.Configuration) -> None:
     """
     Run the tasks defined in the given configuration.
     """
@@ -117,32 +114,33 @@
         python_version = tuple(int(x) for x in str_python_version.split("."))
     else:
         python_version = sys.version_info[:3]
 
     for gen in config["generate"]:
         source = gen["source"]
         print(f"Processing {source}")
-        if source.startswith("http://") or source.startswith("https://"):
-            response = requests.get(source, timeout=60)
-            response.raise_for_status()
-            schema = response.json()
-        else:
-            with open(os.path.abspath(source), encoding="utf-8") as source_file:
-                schema = json.load(source_file)
 
-        resolver: RefResolver = RefResolver.from_schema(schema)
+        resolver = jsonschema_gentypes.resolver.RefResolver(source)
+        schema = resolver.schema
+
+        if "vocabularies" in gen:
+            for vocab, uri in gen["vocabularies"].items():
+                resolver.add_vocabulary(vocab, uri)
+
         schema_ref = schema.get("$schema", "default")
         schema_match = re.match(r"https?\:\/\/json\-schema\.org\/(.*)\/schema", schema_ref)
         api_version = {
-            "draft-04": jsonschema_gentypes.APIv4,
-            "draft-06": jsonschema_gentypes.APIv6,
-            "draft-07": jsonschema_gentypes.APIv7,
+            "draft-04": jsonschema_gentypes.api_draft_04.APIv4,
+            "draft-06": jsonschema_gentypes.api_draft_06.APIv6,
+            "draft-07": jsonschema_gentypes.api_draft_07.APIv7,
+            "draft/2019-09": jsonschema_gentypes.api_draft_2019_09.APIv201909,
+            "draft/2020-12": jsonschema_gentypes.api_draft_2020_12.APIv202012,
         }.get(
             schema_match.group(1) if schema_match else "default",
-            jsonschema_gentypes.APIv7,
+            jsonschema_gentypes.api_draft_2019_09.APIv201909,
         )
         api_args = gen.get("api_arguments", {})
         api = api_version(resolver, **api_args)
 
         types: Dict[str, jsonschema_gentypes.Type] = {}
         imports: Dict[str, Set[str]] = {}
```

### Comparing `jsonschema_gentypes-1.7.2/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-2.0.0/jsonschema_gentypes/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 Automatically generated file from a JSON schema.
 """
 
 
-from typing import Union, Any, TypedDict, Dict, List, Literal
-from typing_extensions import Required
+from typing import Any, Dict, List, Literal, TypedDict, Union
 
+from typing_extensions import Required
 
 AdditionalProperties = Union[Literal["Always"], Literal["Only explicit"]]
 """
 Additional properties.
 
 Describe how to deal with additional properties
 """
 ADDITIONALPROPERTIES_ALWAYS: Literal["Always"] = "Always"
 """The values for the 'Additional properties' enum"""
 ADDITIONALPROPERTIES_ONLY_EXPLICIT: Literal["Only explicit"] = "Only explicit"
 """The values for the 'Additional properties' enum"""
 
 
-
 class ApiArguments(TypedDict, total=False):
     """
     API arguments.
 
     The argument passed to the API
     """
 
@@ -37,22 +36,21 @@
     The JSON Schema generate Python types configuration
     """
 
     headers: str
     callbacks: List[List[str]]
     pre_commit: "PreCommitConfiguration"
     lineLength: int
-    """The maximum line length"""
+    """ The maximum line length """
 
     python_version: str
-    """The minimum Python version to support."""
+    """ The minimum Python version to support. """
 
     generate: Required[List["GenerateItem"]]
-    """Required property"""
-
+    """ Required property """
 
 
 class GenerateItem(TypedDict, total=False):
     """Generate item."""
 
     source: Required[str]
     """
@@ -65,34 +63,38 @@
     """
     The generated Python file name
 
     Required property
     """
 
     root_name: str
-    """The name of the root element"""
+    """ The name of the root element """
 
     api_arguments: "ApiArguments"
     name_mapping: Dict[str, str]
     """
     Name mapping.
 
     Used to map the name of an alternate name
     """
 
+    vocabularies: Dict[str, str]
+    """
+    vocabularies.
+
+    Used to add some vocabularies
+    """
 
 
 PRE_COMMIT_ARGUMENTS_DEFAULT: List[Any] = []
-"""Default value of the field path 'Pre-commit configuration arguments'"""
-
+""" Default value of the field path 'Pre-commit configuration arguments' """
 
 
 PRE_COMMIT_ENABLE_DEFAULT = False
-"""Default value of the field path 'Pre-commit configuration enable'"""
-
+""" Default value of the field path 'Pre-commit configuration enable' """
 
 
 class PreCommitConfiguration(TypedDict, total=False):
     """
     Pre-commit configuration.
 
     The pre-commit configuration
@@ -124,8 +126,7 @@
 
     hooks_skip: List[str]
     """
     Pre-commit skipped hooks.
 
     The hooks to skip, none by default
     """
-
```

### Comparing `jsonschema_gentypes-1.7.2/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-2.0.0/jsonschema_gentypes/schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999975887345679%*

 * *Differences: {"'properties'": "{'generate': {'items': {'properties': {'vocabularies': OrderedDict([('title', "*

 * *                 "'vocabularies'), ('description', 'Used to add some vocabularies'), ('type', "*

 * *                 "'object'), ('additionalProperties', OrderedDict([('type', 'string')]))])}}}}"}*

```diff
@@ -48,14 +48,22 @@
                     "root_name": {
                         "description": "The name of the root element",
                         "type": "string"
                     },
                     "source": {
                         "description": "The JSON schema file name",
                         "type": "string"
+                    },
+                    "vocabularies": {
+                        "additionalProperties": {
+                            "type": "string"
+                        },
+                        "description": "Used to add some vocabularies",
+                        "title": "vocabularies",
+                        "type": "object"
                     }
                 },
                 "required": [
                     "source",
                     "destination"
                 ],
                 "title": "Generate item",
```

### Comparing `jsonschema_gentypes-1.7.2/pyproject.toml` & `jsonschema_gentypes-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "1.7.2"
+version = "2.0.0"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
@@ -41,19 +41,20 @@
 jsonschema-gentypes = "jsonschema_gentypes.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 jsonschema = "4.17.3"
 typing-extensions = "4.5.0"
 requests = "2.28.2"
-"ruamel.yaml" = "0.17.21"
+"PyYAML" = "6.0"
 pinyin = { version = "0.4.0", optional = true }
 romkan = { version = "0.2.1", optional = true }
 romanize = { version = "1.0.2", optional = true }
 pre-commit = { version = "3.2.1", optional = true }
+referencing = "0.27.1"
 
 [tool.poetry.extras]
 generate = []
 tools = ["pre-commit"]
 extra = ['pinyin', 'romkan', 'romanize']
 
 [tool.poetry.dev-dependencies]
```

### Comparing `jsonschema_gentypes-1.7.2/PKG-INFO` & `jsonschema_gentypes-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 1.7.2
+Version: 2.0.0
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4
@@ -22,21 +22,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Typing :: Typed
 Provides-Extra: extra
 Provides-Extra: generate
 Provides-Extra: tools
+Requires-Dist: PyYAML
 Requires-Dist: jsonschema
 Requires-Dist: pinyin ; extra == "extra"
 Requires-Dist: pre-commit ; extra == "tools"
+Requires-Dist: referencing
 Requires-Dist: requests
 Requires-Dist: romanize ; extra == "extra"
 Requires-Dist: romkan ; extra == "extra"
-Requires-Dist: ruamel.yaml
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/camptocamp/jsonschema-gentypes
 Description-Content-Type: text/markdown
 
 # JSON Schema generate Python types
 
 Tools to generate Python types based on TypedDict from a JSON schema
@@ -51,22 +52,14 @@
 
 Convert a JSON schema to a Python file contains the types:
 
 ```bash
 jsonschema-gentypes --json-schema=<JSON schema> --python=<destination Python file>
 ```
 
-## Docker
-
-You can also run it with Docker:
-
-```bash
-docker run --rm --user=$(id --user) --volume=$(pwd):/src camptocamp/jsonschema-gentypes
-```
-
 ## Config file
 
 You can also write a config file named `jsonschema-gentypes.yaml` with:
 
 ```yaml
 headers: >
   # Automatically generated file from a JSON schema
@@ -102,41 +95,14 @@
 
 The default values are exported in the Python file, then you can do something like that:
 
 ```python
 value_with_default = my_object.get('field_name', my_schema.FIELD_DEFAULT)
 ```
 
-## Validation
-
-This package also provide some validations features for YAML file based on `jsonschema`.
-
-Additional features:
-
-- Obtain the line and columns number in the errors, if the file is loaded with `ruamel.yaml`.
-- Export the default provided in the JSON schema.
-
-```python
-    import ruamel.yaml
-    import pkgutil
-    import jsonschema_gentypes.validate
-
-    schema_data = pkgutil.get_data("jsonschema_gentypes", "schema.json")
-    with open(filename) as data_file:
-        yaml = ruamel.yaml.YAML()  # type: ignore
-        data = yaml.load(data_file)
-    errors, data = jsonschema_gentypes.validate.validate(filename, data, schema)
-    if errors:
-        print("\n".join(errors))
-        sys.exit(1)
-```
-
-The filling of the default value is deprecated because it can produce quite peculiar things, see also
-[the jsonschema documentation](https://python-jsonschema.readthedocs.io/en/stable/faq/#why-doesn-t-my-schema-s-default-property-set-the-default-on-my-instance).
-
 ## Limitations
 
 Requires Python 3.8
 
 See the [issues with label "limitation"](https://github.com/camptocamp/jsonschema-gentypes/issues?q=is%3Aissue+is%3Aopen+label%3Alimitation).
 
 ## Pre-commit hooks
```

