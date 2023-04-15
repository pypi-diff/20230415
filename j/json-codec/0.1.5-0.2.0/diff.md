# Comparing `tmp/json_codec-0.1.5.tar.gz` & `tmp/json_codec-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_codec-0.1.5.tar", max compression
+gzip compressed data, was "json_codec-0.2.0.tar", max compression
```

## Comparing `json_codec-0.1.5.tar` & `json_codec-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3033 2022-12-10 21:43:50.025310 json_codec-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-15 02:13:43.379791 json_codec-0.1.5/json_codec/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 02:13:43.339791 json_codec-0.1.5/json_codec/codecs/__init__.py
--rw-r--r--   0        0        0      960 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/date_codec.py
--rw-r--r--   0        0        0     1111 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/datetime_codec.py
--rw-r--r--   0        0        0     2211 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/dict_codec.py
--rw-r--r--   0        0        0     1223 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/list_codec.py
--rw-r--r--   0        0        0      906 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/primitive_codec.py
--rw-r--r--   0        0        0     1151 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/set_codec.py
--rw-r--r--   0        0        0      960 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/time_codec.py
--rw-r--r--   0        0        0     1002 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/tuple_codec.py
--rw-r--r--   0        0        0     1000 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/union_codec.py
--rw-r--r--   0        0        0     9581 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/json_codec.py
--rw-r--r--   0        0        0     8691 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/test_json_codec.py
--rw-r--r--   0        0        0     2272 2023-04-15 02:13:43.439792 json_codec-0.1.5/json_codec/types.py
--rw-r--r--   0        0        0      502 2023-04-15 02:14:33.609790 json_codec-0.1.5/json_codec/utils.py
--rw-r--r--   0        0        0      484 2023-04-15 02:15:14.079786 json_codec-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 json_codec-0.1.5/setup.py
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 json_codec-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3033 2022-12-10 21:43:50.025310 json_codec-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 02:13:43.379791 json_codec-0.2.0/json_codec/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 02:13:43.339791 json_codec-0.2.0/json_codec/codecs/__init__.py
+-rw-r--r--   0        0        0      960 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/date_codec.py
+-rw-r--r--   0        0        0     1111 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/datetime_codec.py
+-rw-r--r--   0        0        0     2211 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/dict_codec.py
+-rw-r--r--   0        0        0     1223 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/list_codec.py
+-rw-r--r--   0        0        0      906 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/primitive_codec.py
+-rw-r--r--   0        0        0     1151 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/set_codec.py
+-rw-r--r--   0        0        0      960 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/time_codec.py
+-rw-r--r--   0        0        0     1002 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/tuple_codec.py
+-rw-r--r--   0        0        0     1000 2023-04-15 02:14:25.229790 json_codec-0.2.0/json_codec/codecs/union_codec.py
+-rw-r--r--   0        0        0     9743 2023-04-15 13:12:41.931987 json_codec-0.2.0/json_codec/json_codec.py
+-rw-r--r--   0        0        0     9295 2023-04-15 13:15:25.691940 json_codec-0.2.0/json_codec/test_json_codec.py
+-rw-r--r--   0        0        0     2272 2023-04-15 02:13:43.439792 json_codec-0.2.0/json_codec/types.py
+-rw-r--r--   0        0        0      502 2023-04-15 02:14:33.609790 json_codec-0.2.0/json_codec/utils.py
+-rw-r--r--   0        0        0      484 2023-04-15 13:15:45.041935 json_codec-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 json_codec-0.2.0/setup.py
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 json_codec-0.2.0/PKG-INFO
```

### Comparing `json_codec-0.1.5/README.md` & `json_codec-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/date_codec.py` & `json_codec-0.2.0/json_codec/codecs/date_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/datetime_codec.py` & `json_codec-0.2.0/json_codec/codecs/datetime_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/dict_codec.py` & `json_codec-0.2.0/json_codec/codecs/dict_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/list_codec.py` & `json_codec-0.2.0/json_codec/codecs/list_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/primitive_codec.py` & `json_codec-0.2.0/json_codec/codecs/primitive_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/set_codec.py` & `json_codec-0.2.0/json_codec/codecs/set_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/time_codec.py` & `json_codec-0.2.0/json_codec/codecs/time_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/tuple_codec.py` & `json_codec-0.2.0/json_codec/codecs/tuple_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/codecs/union_codec.py` & `json_codec-0.2.0/json_codec/codecs/union_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/json_codec/json_codec.py` & `json_codec-0.2.0/json_codec/json_codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 from dataclasses import MISSING, asdict, dataclass, is_dataclass
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
 from typing import (
     Any,
     Callable,
@@ -67,14 +68,15 @@
     UUID: PrimitiveTypeDecoder(UUID, "UUID"),
     Union: UnionTypeParser(),
     Any: PrimitiveTypeDecoder(lambda x: x, "Any"),
     date: DateTypeDecoder(),
     datetime: DateTimeTypeDecoder(),
     time: TimeTypeParser(),
     type(None): PrimitiveTypeDecoder(lambda x: None, "null"),
+    bytes: PrimitiveTypeDecoder(base64.b64decode, "bytes"),
 }
 
 
 @dataclass
 class LocatedValidationError:
     message: str
     json_path: str
@@ -295,14 +297,16 @@
         return value
     if isinstance(value, (list, tuple)):
         return [__encode(v) for v in value]
     if isinstance(value, dict):
         return {__encode(k): __encode(v) for k, v in value.items()}
     if is_dataclass(value):
         return __encode(asdict(value))
+    if isinstance(value, bytes):
+        return base64.b64encode(value).decode("utf-8")
     if value is None:
         return None
     raise ValueError(f"Unsupported type: {type(value)}")
 
 
 def encode(value: Any) -> Any:
     return __encode(value)
```

### Comparing `json_codec-0.1.5/json_codec/test_json_codec.py` & `json_codec-0.2.0/json_codec/test_json_codec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import base64
 import json
 from dataclasses import dataclass
 from datetime import date, datetime, time, timezone
 from decimal import Decimal
 from enum import Enum
 from typing import Dict, List, NewType, Optional, Union
 
 import pytest
 
 from json_codec.json_codec import (
     LocatedValidationErrorCollection,
     decode,
+    encode,
     optional,
 )
 from json_codec.utils import get_class_or_type_name
 
 
 class TestJsonDeserializerCodec:
     def test_decode_primitives(self) -> None:
@@ -337,7 +339,33 @@
         assert isinstance(parsed.my_int, MyInt)
 
     def test_decode_newtype(self) -> None:
         UserId = NewType("UserId", int)
 
         assert decode(json.loads("1"), UserId) == UserId(1)
         assert isinstance(decode(json.loads("1"), UserId), int)
+
+    def test_encode_and_decode_bytes(self):
+
+        hello_bytes = b"hello"
+
+        base64_hello_bytes = base64.b64encode(hello_bytes).decode("utf-8")
+
+        assert encode(hello_bytes) == base64_hello_bytes
+
+        assert decode(base64_hello_bytes, bytes) == hello_bytes
+
+        @dataclass
+        class Dummy:
+            bytes_: bytes
+
+        dummy_json_text = """
+        {
+            "bytes_": "aGVsbG8="
+        }
+        """
+
+        dummy_json = json.loads(dummy_json_text)
+
+        parsed = decode(dummy_json, Dummy)
+
+        assert parsed.bytes_ == hello_bytes
```

### Comparing `json_codec-0.1.5/json_codec/types.py` & `json_codec-0.2.0/json_codec/types.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.5/setup.py` & `json_codec-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['json_codec', 'json_codec.codecs']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'json-codec',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': '',
     'long_description': '# Json Codec\n\nIt\'s a simple library to encode and decode json to strict python types using dataclasses and builtin python types.\n\n## Installation\n\n```bash\npip install json-codec\n\npoetry add json-codec\n```\n\n## Usage\n\n### Parse a simple primitive type\n\n```python\nfrom json_codec import decode\nimport json\n\nassert decode(json.loads("true"), bool) is True\nassert decode(json.loads("false"), bool) is False\nassert decode(json.loads("null"), Optional[bool]) is None\nassert decode(json.loads("1"), int) == 1\nassert decode(json.loads("1"), Decimal) == Decimal("1")\nassert decode(json.loads(\'"1.1"\'), Decimal) == Decimal("1.1")\nassert decode(json.loads(\'"1.1"\'), float) == 1.1\nassert decode(json.loads(\'"1.1"\'), str) == "1.1"\n\nassert decode(json.loads(\'[1,1]\'), List[int]) == [1, 1]\n```\n\n### Parse a dataclass\n\n```python\nfrom dataclasses import dataclass\nfrom json_codec import decode\nimport json\n\n@dataclass(frozen=True)\nclass User:\n    name: str\n    age: int\n\nassert decode({"name": "John", "age": 30}, User) == User(name="John", age=30)\n\n\n@dataclass\nclass Dummy:\n    text_list: List[str]\n    text_dict: Dict[str, Decimal]\n    optional_text: Optional[str]\n\ndummy_json_text = """\n{\n    "text_list": ["a", "b", "c"],\n    "text_dict": {\n        "a": 1.0,\n        "b": 2,\n        "c": "3.3",\n        "d": 2.2\n    },\n    "optional_text": "hello"\n}\n"""\n\ndummy_json = json.loads(dummy_json_text)\n\nparsed = decode(dummy_json, Dummy)\n\nassert parsed.text_list == ["a", "b", "c"]\nassert parsed.text_dict["a"] == Decimal("1.0")\nassert parsed.text_dict["b"] == Decimal("2.0")\nassert parsed.text_dict["c"] == Decimal("3.3")\nassert parsed.text_dict["d"].quantize(Decimal("1.0")) == Decimal("2.2")\nassert parsed.optional_text == "hello"\n```\n\n### Parse a dataclass with a nested dataclass\n\n```python\nfrom dataclasses import dataclass\nfrom json_codec import decode\nimport json\n\n @dataclass\nclass NestedDummy:\n    text: str\n    number: Decimal\n\n    boolean: bool\n\n@dataclass\nclass Dummy:\n    text_list: List[str]\n    text_dict: Dict[str, Decimal]\n    nested: NestedDummy\n\ndummy_json_text = """\n{\n\n    "text_list": ["a", "b", "c"],\n    "text_dict": {\n        "a": 1.0,\n        "b": 2,\n        "c": "3.3",\n        "d": 2.2\n    },\n    "nested": {\n        "text": "hello",\n        "number": 1.1,\n        "boolean": true\n    }\n}\n"""\n\ndummy_json = json.loads(dummy_json_text)\n\nparsed = decode(dummy_json, Dummy)\n\nassert parsed.text_list == ["a", "b", "c"]\nassert parsed.text_dict["a"] == Decimal("1.0")\nassert parsed.text_dict["b"] == Decimal("2.0")\nassert parsed.text_dict["c"] == Decimal("3.3")\nassert parsed.text_dict["d"].quantize(Decimal("1.0")) == Decimal("2.2")\nassert parsed.nested.text == "hello"\nassert parsed.nested.number.quantize(Decimal("1.0")) == Decimal("1.1")\nassert parsed.nested.boolean is True\n```\n\n### Parse a newtype\n\n```python\nfrom json_codec import decode\nfrom typing import NewType\nimport json\n\nUserId = NewType("UserId", int)\n\nassert decode(json.loads("1"), UserId) == UserId(1)\nassert isinstance(decode(json.loads("1"), UserId), int)\n\n```',
     'author': 'Lucas Silva',
     'author_email': 'lucas76leonardo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/LuscasLeo/json_codec',
```

### Comparing `json_codec-0.1.5/PKG-INFO` & `json_codec-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-codec
-Version: 0.1.5
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/LuscasLeo/json_codec
 Author: Lucas Silva
 Author-email: lucas76leonardo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

