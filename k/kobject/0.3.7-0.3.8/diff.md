# Comparing `tmp/kobject-0.3.7.tar.gz` & `tmp/kobject-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobject-0.3.7.tar", max compression
+gzip compressed data, was "kobject-0.3.8.tar", max compression
```

## Comparing `kobject-0.3.7.tar` & `kobject-0.3.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-01-20 00:17:09.918528 kobject-0.3.7/LICENSE
--rw-r--r--   0        0        0     8449 2023-02-01 20:08:26.032815 kobject-0.3.7/README.md
--rw-r--r--   0        0        0      166 2023-02-01 20:08:26.032815 kobject-0.3.7/kobject/__init__.py
--rw-r--r--   0        0        0     5556 2023-04-05 00:27:13.208245 kobject-0.3.7/kobject/from_json/__init__.py
--rw-r--r--   0        0        0     2576 2023-03-23 00:05:46.802055 kobject-0.3.7/kobject/to_json/__init__.py
--rw-r--r--   0        0        0     5026 2023-02-03 11:43:50.229615 kobject-0.3.7/kobject/validator/__init__.py
--rw-r--r--   0        0        0      539 2023-04-05 00:23:33.396951 kobject-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     9424 1970-01-01 00:00:00.000000 kobject-0.3.7/setup.py
--rw-r--r--   0        0        0     8935 1970-01-01 00:00:00.000000 kobject-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-20 00:17:09.918528 kobject-0.3.8/LICENSE
+-rw-r--r--   0        0        0     8449 2023-02-01 20:08:26.032815 kobject-0.3.8/README.md
+-rw-r--r--   0        0        0      166 2023-02-01 20:08:26.032815 kobject-0.3.8/kobject/__init__.py
+-rw-r--r--   0        0        0     5625 2023-04-15 16:35:58.060636 kobject-0.3.8/kobject/from_json/__init__.py
+-rw-r--r--   0        0        0     2576 2023-03-23 00:05:46.802055 kobject-0.3.8/kobject/to_json/__init__.py
+-rw-r--r--   0        0        0     5026 2023-02-03 11:43:50.229615 kobject-0.3.8/kobject/validator/__init__.py
+-rw-r--r--   0        0        0      539 2023-04-15 16:35:58.060636 kobject-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     9424 1970-01-01 00:00:00.000000 kobject-0.3.8/setup.py
+-rw-r--r--   0        0        0     8935 1970-01-01 00:00:00.000000 kobject-0.3.8/PKG-INFO
```

### Comparing `kobject-0.3.7/LICENSE` & `kobject-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kobject-0.3.7/README.md` & `kobject-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `kobject-0.3.7/kobject/from_json/__init__.py` & `kobject-0.3.8/kobject/from_json/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,18 +139,21 @@
     def type_caster(cls, attr_type, attr_value):  # pylint: disable=R1710
         """
         Returns the result of cast attribute type for the attribute type
         """
         for map_attr_type, resolver in cls.types_resolver:
             if inspect.isclass(attr_type) and issubclass(attr_type, map_attr_type):
                 return resolver(attr_type, attr_value)
+        return attr_value
 
 
 FromJSON.set_decoder_resolver(bool, lambda attr_type, value: value)
-FromJSON.set_decoder_resolver(float, lambda attr_type, value: float(value))
+FromJSON.set_decoder_resolver(
+    float, lambda attr_type, value: float(value) if isinstance(value, int) else value
+)
 FromJSON.set_decoder_resolver(int, lambda attr_type, value: value)
 FromJSON.set_decoder_resolver(str, lambda attr_type, value: value)
 FromJSON.set_decoder_resolver(
     FromJSON,
     lambda attr_type, value: attr_type.from_dict(value)
     if isinstance(value, dict)
     else value,
```

### Comparing `kobject-0.3.7/kobject/to_json/__init__.py` & `kobject-0.3.8/kobject/to_json/__init__.py`

 * *Files identical despite different names*

### Comparing `kobject-0.3.7/kobject/validator/__init__.py` & `kobject-0.3.8/kobject/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `kobject-0.3.7/pyproject.toml` & `kobject-0.3.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kobject"
-version = "0.3.7"
+version = "0.3.8"
 description = "Know your object is a attribute type checker"
 authors = ["Marco Sievers de Almeida Ximit Gaia <im.ximit@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "kobject"},
     { include = "kobject/**/*.py" },
```

### Comparing `kobject-0.3.7/setup.py` & `kobject-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['kobject', 'kobject.from_json', 'kobject.to_json', 'kobject.validator']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'kobject',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': 'Know your object is a attribute type checker',
     'long_description': '```\n                       ▄▄          ▄▄                      \n▀████▀ ▀███▀          ▄██          ██                 ██   \n  ██   ▄█▀             ██                             ██   \n  ██ ▄█▀      ▄██▀██▄  ██▄████▄  ▀███  ▄▄█▀██ ▄██▀████████ \n  █████▄     ██▀   ▀██ ██    ▀██   ██ ▄█▀   ███▀  ██  ██   \n  ██  ███    ██     ██ ██     ██   ██ ██▀▀▀▀▀▀█       ██   \n  ██   ▀██▄  ██▄   ▄██ ██▄   ▄██   ██ ██▄    ▄█▄    ▄ ██   \n▄████▄   ███▄ ▀█████▀  █▀█████▀    ██  ▀█████▀█████▀  ▀████\n                                ██ ██                      \n                                ▀███                       By CenturyBoys\n                                \nKnow your object is a __init__ type validator for class and dataclass\n```\n\n## Usage\n\nKobject can be use inside default class declaration and with dataclasses. Kobject uses the ```__init__``` signature to check types.\n\n### Default classes\n\n```python\nfrom kobject import Kobject\n\nclass StubClass(Kobject):\n    a_int: int\n    a_bool: bool\n    \n    def __init__(\n        self,\n        a_int: int,\n        a_bool: bool\n    ):\n        self.a_int = a_int\n        self.a_bool = a_bool\n        self.__post_init__()\n\ninstance = StubClass(a_int=1, a_bool=True)\n```\nNotice that in the default class declaration you need to call ```self.__post_init__()``` at the end of the ```__init__``` declaration.\n\n\n### Dataclass\n\n```python\nfrom dataclasses import dataclass\nfrom kobject import Kobject\n\n@dataclass\nclass StubClass(Kobject):\n    a_int: int\n    a_bool: bool\n\ninstance = StubClass(a_int=1, a_bool=True)\n```\nBy default, dataclass calls ```self.__post_init__()``` at the end of the ```__init__``` declaration.\n\n\n### Exception\n\nKobject raises ```TypeError``` with all validation errors, that means it checks all your object\'s attributes before raising the ```TypeError```. Types like List and Tuple will have all their elements checked.\n\n```python\nfrom dataclasses import dataclass\nfrom kobject import Kobject\nfrom typing import List, Tuple\n\n@dataclass\nclass StubClass(Kobject):\n    a_list_int: List[int]\n    a_tuple_bool: Tuple[bool]\n\ninstance = StubClass(a_list_int=[1, "", 2, ""], a_tuple_bool=["", True])\n```\n```bash\nTraceback (most recent call last):\n  File "/snap/pycharm-community/312/plugins/python-ce/helpers/pydev/pydevconsole.py", line 364, in runcode\n    coro = func()\n  File "<input>", line 10, in <module>\n  File "<string>", line 5, in __init__\n  File "/home/marco/projects/kobject/kobject/__init__.py", line 67, in __post_init__\n    raise TypeError(message)\nTypeError: Validation Errors:\n    \'a_list_int\' : Wrong type! Expected (<class \'int\'>,) but giving <class \'str\'> on index 1\n    \'a_list_int\' : Wrong type! Expected (<class \'int\'>,) but giving <class \'str\'> on index 3\n    \'a_tuple_bool\' : Wrong type! Expected <class \'tuple\'> but giving <class \'list\'>\n    \'a_tuple_bool\' : Wrong type! Expected (<class \'bool\'>,) but giving <class \'str\'> on index 0\n```\n\n### Default value\n\nKobject supports default values and will check them before any validation, that means if you declare a ```a_bool: bool = None``` it will not raise an error.\n\n```python\nfrom dataclasses import dataclass\nfrom kobject import Kobject\n\nclass StubClass(Kobject):\n    a_bool: bool = None\n\n    def __init__(self, a_bool: bool = 2):\n        self.a_bool = a_bool\n        self.__post_init__()\n\n@dataclass\nclass StubDataClass(Kobject):\n    a_bool: bool = None\n```\n\n### Custom exception\n\nBy default Kobject raise a ```TypeError``` but you can override this exception using ```set_custom_exception```\n\n```python\nfrom dataclasses import dataclass\nfrom kobject import Kobject\n\nclass CustomException(Exception):\n    pass\n\n\nKobject.set_custom_exception(CustomException)\n\n\n@dataclass\nclass StubClass(Kobject):\n    a__int: int\n\ninstance = StubClass(a__int="")\n```\n```bash\nTraceback (most recent call last):\n  File "/snap/pycharm-community/312/plugins/python-ce/helpers/pydev/pydevconsole.py", line 364, in runcode\n    coro = func()\n  File "<input>", line 15, in <module>\n  File "<string>", line 4, in __init__\n  File "/home/marco/projects/kobject/kobject/__init__.py", line 79, in __post_init__\n    raise exception(message)\n__main__.CustomException: Validation Errors:\n    \'a__int\' : Wrong type! Expected <class \'int\'> but giving <class \'str\'>\n```\n\n### ToJSON\n\nKobject has his own implementation to parse class instance to a JSON representation. \n\n```python\nfrom dataclasses import dataclass\nfrom typing import List, Tuple\n\nfrom kobject import Kobject, ToJSON\n    \n@dataclass\nclass BaseC(Kobject, ToJSON):\n    a_int: int\n    a_str: str\n    a_list_of_int: List[int]\n    a_tuple_of_bool: Tuple[bool]\n    \ninstance = BaseC(\n    a_int=1,\n    a_str="lala",\n    a_list_of_int=[1, 2, 3],\n    a_tuple_of_bool=(True,)\n)\n\njson_bytes = instance.to_json()\n\nprint(json_bytes)\n```\n```bash\nb\'{"a_int": 1, "a_str": "lala", "a_list_of_int": [1, 2, 3], "a_tuple_of_bool": [true]}\'\n```\n\nFor complex values ToJSON expose ```set_encoder_resolver``` to handler it.\n\n```python\nfrom dataclasses import dataclass\nfrom datetime import datetime\nfrom typing import List\nfrom uuid import UUID\n\nfrom kobject import Kobject, ToJSON, FromJSON\n\n\n@dataclass\nclass BaseA(Kobject, ToJSON):\n    a_datetime: datetime\n\n\n@dataclass\nclass BaseB:\n    a_uuid: UUID\n\n\n@dataclass\nclass BaseC(Kobject, ToJSON, FromJSON):\n    a_base_a: BaseA\n    a_base_b: BaseB\n    a_list_of_base_a: List[BaseA]\n\nToJSON.set_encoder_resolver(datetime, lambda value: str(value))\nToJSON.set_encoder_resolver(BaseB, lambda value: {"a_uuid": str(value.a_uuid)})\n\ninstance = BaseC(\n    a_base_a=BaseA(a_datetime=datetime.fromisoformat("2023-02-01 17:38:45.389426")),\n    a_base_b=BaseB(a_uuid=UUID("1d9cf695-c917-49ce-854b-4063f0cda2e7")),\n    a_list_of_base_a=[BaseA(a_datetime=datetime.fromisoformat("2023-02-01 17:38:45.389426"))]\n)\n\njson_bytes = instance.to_json()\n\nprint(json_bytes)\n```\n```bash\nb\'{"a_base_a": {"a_datetime": "2023-02-01 17:38:45.389426"}, "a_base_b": {"a_uuid": "1d9cf695-c917-49ce-854b-4063f0cda2e7"}, "a_list_of_base_a": [{"a_datetime": "2023-02-01 17:38:45.389426"}]}\'\n```\n\n### FromJSON\n\nKobject has his own implementation to parse JSON to a class instance. \n\n```python\nfrom dataclasses import dataclass\nfrom typing import List, Tuple\n\nfrom kobject import Kobject\nfrom kobject.from_json import FromJSON\n\n\n@dataclass\nclass BaseC(Kobject, FromJSON):\n    a_int: int\n    a_str: str\n    a_list_of_int: List[int]\n    a_tuple_of_bool: Tuple[bool]\n\npayload = (\n    b\'{"a_int": 1,"a_str": "lala","a_list_of_int": [1,2,3],\'\n    b\'"a_tuple_of_bool": [true]}\'\n)\ninstance = BaseC.from_json(payload=payload)\n\nprint(instance)\n```\n```bash\nBaseC(a_int=1, a_str=\'lala\', a_list_of_int=[1, 2, 3], a_tuple_of_bool=(True,))\n```\n\nFor complex values FromJSON expose ```set_decoder_resolver``` to handler it.\n\n```python\nfrom datetime import datetime\nfrom dataclasses import dataclass\nfrom typing import List\nfrom uuid import UUID\n\nfrom kobject import Kobject\nfrom kobject.from_json import FromJSON\n\n\n@dataclass\nclass BaseA(Kobject, FromJSON):\n    a_datetime: datetime\n\n\n@dataclass\nclass BaseB:\n    a_uuid: UUID\n\n\n@dataclass\nclass BaseC(Kobject, FromJSON):\n    a_base_a: BaseA\n    a_base_b: BaseB\n    a_list_of_base_a: List[BaseA]\n\nFromJSON.set_decoder_resolver(\n    datetime,\n    lambda attr_type, value: datetime.fromisoformat(value)\n    if isinstance(value, str)\n    else value,\n)\nFromJSON.set_decoder_resolver(\n    BaseB,\n    lambda attr_type, value: attr_type(a_uuid=UUID(value["a_uuid"]))\n    if isinstance(value, dict)\n    else value,\n)\npayload = (\n    b\'{"a_base_a": {"a_datetime": "2023-02-01 17:38:45.389426"},"a_base_b": {"a_\'\n    b\'uuid":"1d9cf695-c917-49ce-854b-4063f0cda2e7"}, "a_lis\'\n    b\'t_of_base_a": [{"a_datetime": "2023-02-01 17:38:45.389426"}]}\'\n)\ninstance = BaseC.from_json(payload=payload)\n\nprint(instance)\n```\n```bash\nBaseC(a_base_a=BaseA(a_datetime=datetime.datetime(2023, 2, 1, 17, 38, 45, 389426)), a_base_b=BaseB(a_uuid=UUID(\'1d9cf695-c917-49ce-854b-4063f0cda2e7\')), a_list_of_base_a=[BaseA(a_datetime=datetime.datetime(2023, 2, 1, 17, 38, 45, 389426))])\n```',
     'author': 'Marco Sievers de Almeida Ximit Gaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kobject-0.3.7/PKG-INFO` & `kobject-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobject
-Version: 0.3.7
+Version: 0.3.8
 Summary: Know your object is a attribute type checker
 License: Apache-2.0
 Author: Marco Sievers de Almeida Ximit Gaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

