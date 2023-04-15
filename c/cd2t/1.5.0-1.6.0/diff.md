# Comparing `tmp/cd2t-1.5.0.tar.gz` & `tmp/cd2t-1.6.0.tar.gz`

## Comparing `cd2t-1.5.0.tar` & `cd2t-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/DataParser.py
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/References.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/__init__.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/results.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/schema.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/utils.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/List.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/NoneDataType.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/any.py
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/base.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/bool.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/datatype.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/enum.py
--rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/float.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/idlist.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/integer.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/multitype.py
--rw-r--r--   0        0        0    10718 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/object.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/schema.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/string.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.5.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.5.0/LICENSE
--rw-r--r--   0        0        0    17429 2020-02-02 00:00:00.000000 cd2t-1.5.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 cd2t-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/DataParser.py
+-rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/References.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/RunTimeEnv.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/__init__.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/results.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/schema.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/utils.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/List.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/NoneDataType.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/__init__.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/base.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/bool.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/datatype.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/enum.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/float.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/idlist.py
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/integer.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/multitype.py
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/object.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/schema.py
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/string.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.6.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.6.0/LICENSE
+-rw-r--r--   0        0        0    17972 2020-02-02 00:00:00.000000 cd2t-1.6.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 cd2t-1.6.0/PKG-INFO
```

### Comparing `cd2t-1.5.0/cd2t/DataParser.py` & `cd2t-1.6.0/cd2t/DataParser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from cd2t.References import References
 from cd2t.types import *
 from cd2t.schema import Schema, SchemaError
 from cd2t.results import FindingsList
+from cd2t.References import ReferenceFinding
+from cd2t.RunTimeEnv import RunTimeEnv
 import copy
 
 
 BUILTIN_DATA_TYPES = {
-    'any': AnyDataType,
+    'any': BaseDataType,
     'bool': Bool,
     'enum': Enum,
     'float': Float,
     'idlist': IDList,
     'integer': Integer,
     'list': List,
     'multitype': Multitype,
@@ -18,122 +19,124 @@
     'object': Object,
     'schema': SchemaDataType,
     'string': String
 }
 
 class DataParser():
     def __init__(self, namespace='') -> None:
-        self._check_given_namespace(namespace, allow_empty=True)
-        self.references = References(namespace=namespace)
-        self.namespace = namespace
+        self.RTE = RunTimeEnv()
+        self.RTE.change_namespace(namespace=namespace, allow_empty=True)
+        self.RTE.load_data_types(BUILTIN_DATA_TYPES)
         self.current_schema = None
-        self._data_type_classes = copy.copy(BUILTIN_DATA_TYPES)
-
-    @staticmethod
-    def _check_given_namespace(namespace :str, allow_empty=False) -> None:
-        if not isinstance(namespace, str):
-            raise ValueError('namespace has to be a string')
-        if not allow_empty and len(namespace) == 0:
-            raise ValueError('namespace has to be a non empty string')
+    
+    @property
+    def namespace(self):
+        return self.RTE.namespace
         
     def change_namespace(self, namespace :str) -> None:
-        self._check_given_namespace(namespace)
-        self.references.change_namespace(namespace)
-        self.namespace = namespace
+        self.RTE.change_namespace(namespace=namespace)
     
     def _get_schema_object(self, schema) -> Schema:
         if isinstance(schema, Schema):
             if schema.root_data_type is None:
                 if self.current_schema is None:
                     raise SchemaError('need a schema or ' +\
                                             'Validator object loads a schema first')
                 return self.current_schema
             return schema
         raise SchemaError('Given schema is not a valid schema object')
 
     def load_data_type(self, type_name :str, type_class :any) -> None:
-        if type_name in self._data_type_classes.keys():
-            raise ValueError("Data type '%s' already loaded" % type_name)
-        if not issubclass(type_class, BaseDataType):
-            raise ValueError("Loading %s failed - not %s" % (type_class, BaseDataType))
-        self._data_type_classes[type_name] = type_class
+        self.RTE.load_data_type(type_name=type_name, type_class=type_class)
     
     def load_schema(self, schema :dict) -> Schema:
         def verify_schema_format(schema_dic :dict, sub=False, sub_name=''):
             try:
                 if not isinstance(schema_dic, dict):
                     raise SchemaError('needs to be an dictionary')
                 if 'root' not in schema_dic.keys():
                     raise SchemaError("has no key 'root'")
                 root_schema = schema_dic.get('root', None)
                 if not isinstance(root_schema, dict):
-                    raise SchemaError("root is no mapping")
+                    if self.RTE.allow_shortcuts:
+                        if not isinstance(root_schema, str):
+                            raise SchemaError('root needs to be an dictionary or a string')
+                        root_type_name = root_schema
+                        root_schema = dict()
+                    else:
+                        raise SchemaError("root is not a dictionary")
+                else:
+                    root_type_name = root_schema.get('type', None)
                 if len(root_schema) and 'type' not in root_schema.keys():
                     raise SchemaError("option 'type' in root schema missing")
             except SchemaError as se:
                 if sub:
                     raise SchemaError("Subschema '%s' %s" % (sub_name, str(se)))
                 raise SchemaError("Schema %s" % str(se))
-            root_type_name = root_schema.get('type', None)
             if root_type_name is None:
-                root_class = AnyDataType
+                root_class = BaseDataType
             else:
-                if root_type_name not in self._data_type_classes:
+                try:
+                    root_class = self.RTE.get_data_type_class(root_type_name)
+                except SchemaError as se:
                     raise SchemaError("Schema root type '%s' not found" % str(root_type_name))
-                root_class = self._data_type_classes[root_type_name]
             return root_class, root_schema
         
         schema = copy.copy(schema)
+
+        self.RTE.allow_shortcuts = schema.get('allow_data_type_shortcuts', False)
+
         sub_schemas = dict()
         if 'subschemas' in schema.keys():
             sub_schemas = schema['subschemas']
             if not isinstance(sub_schemas, dict):
                 raise SchemaError("Schema subschemas is no mapping")
             for sub_name in sub_schemas.keys():
                 sub_schema = sub_schemas[sub_name]
                 if isinstance(sub_schema, Schema):
                     # This subschema was already verified/translated (recursively)
                     continue
                 sub_type_class, sub_type_schema = verify_schema_format(sub_schema, sub=True, sub_name=sub_name)
-                sub_type = sub_type_class().build_schema(
-                                schema=sub_type_schema, path='->' + sub_name, data_types=self._data_type_classes,
+                sub_type = sub_type_class(self.RTE).build_schema(
+                                schema=sub_type_schema, path='<' + sub_name +'>',
                                 subschemas=sub_schemas, subpath=[sub_name]
                             )
                 sub_schema_obj = Schema()
                 sub_schema_obj.set_root_data_type(sub_type)
                 sub_schemas[sub_name] = sub_schema_obj
                 
         root_type_class, root_type_schema = verify_schema_format(schema)
-        root_type = root_type_class().build_schema(
-                schema=root_type_schema, path='', data_types=self._data_type_classes,
+        root_type = root_type_class(self.RTE).build_schema(
+                schema=root_type_schema, path='',
                 subschemas=sub_schemas, subpath=[]
             )
         schema_obj = Schema()
         schema_obj.set_root_data_type(root_type)
         self.current_schema = schema_obj
         return schema_obj
+    
+    def get_reference_findings(self) -> list[ReferenceFinding]:
+        return self.RTE.references.get_producer_consumer_issues()
 
 
 class Autogenerator(DataParser):
     def build_references(self, data :any, schema=Schema()) -> None:
         schema = self._get_schema_object(schema)
         root_data_type = schema.root_data_type
-        root_data_type.build_references(data=data, path='', references=self.references)
+        root_data_type.build_references(data=data, path='')
 
     def autogenerate_data(self, data :any, schema=Schema()) -> any:
         schema = self._get_schema_object(schema)
         root_data_type = schema.root_data_type
-        new_data, FL = root_data_type.autogenerate_data(
-                        data=data, path='', references=self.references)
-        FL.set_namespace(self.namespace)
+        new_data, FL = root_data_type.autogenerate_data(data=data, path='')
+        FL.set_namespace(self.RTE.namespace)
         return new_data, FL
     
     
 class Validator(DataParser):
     def validate_data(self, data :any, schema=Schema()) -> FindingsList:
         schema = self._get_schema_object(schema)
         root_data_type = schema.root_data_type
-        FL = root_data_type.validate_data(
-                        data=data, path='', references=self.references)
-        FL.set_namespace(self.namespace)
+        FL = root_data_type.validate_data(data=data, path='')
+        FL.set_namespace(self.RTE.namespace)
         return FL
```

### Comparing `cd2t-1.5.0/cd2t/References.py` & `cd2t-1.6.0/cd2t/References.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.5.0/cd2t/results.py` & `cd2t-1.6.0/cd2t/results.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.5.0/cd2t/schema.py` & `cd2t-1.6.0/cd2t/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.5.0/cd2t/utils.py` & `cd2t-1.6.0/cd2t/utils.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.5.0/cd2t/types/List.py` & `cd2t-1.6.0/cd2t/types/List.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,77 @@
 from cd2t.types.base import BaseDataType
-from cd2t.types.any import AnyDataType
 from cd2t.results import FindingsList, ValidationFinding, WrongValueFinding
-from cd2t.References import References
 from cd2t.schema import SchemaError
+from cd2t.RunTimeEnv import RunTimeEnv
 import copy
 
 class List(BaseDataType):
     type = 'list'
+    path_symbol = '[]'
     matching_classes = [list]
     options = [
         # option_name, required, class
         ('minimum', False, int, None),
         ('maximum', False, int, None),
         ('allow_duplicates', False, bool, True),
-        ('elements', True, dict, dict()),
+        ('elements', True, [dict, str], dict()),
     ]
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.minimum = None
         self.maximum = None
         self.allow_duplicates = True
         self.elements = dict()
         self.element_data_type = None
     
-    def build_schema(self, schema :dict, path :str,
-                     data_types :dict, subschemas :dict,
-                     subpath :list):
-        self.__init__()
-        path = path + '[]'
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
+        self.__init__(RTE=self.RTE)
+        path = path + self.path_symbol
         self.load_schema_options(schema, path)
-        if len(self.elements) == 0:
-            self.element_data_type = AnyDataType()
-            return
-        if not 'type' in self.elements.keys():
-            raise SchemaError("'elements' need to have a key 'type'", path)
-        element_data_type_name = self.elements['type']
-        if element_data_type_name not in data_types.keys():
-            raise SchemaError("'elements' data type '%s' not found" % 
-                              (element_data_type_name), path)
-        self.element_data_type = data_types[element_data_type_name]()
+
+        self.element_data_type = self._get_data_type('elements', path + 'elements')
         # Save recursively detected data type (i.e. from 'schema' --> subschema)
         self.element_data_type = self.element_data_type.build_schema(
-            schema=self.elements, path=path, data_types=data_types,
+            schema=self.elements, path=path,
             subschemas=subschemas, subpath=subpath)
         return self
     
-    def build_sub_references(self, data :any, path :str, references :References):
+    def build_sub_references(self, data :any, path :str):
         i = 0
         for element in data:
-            self.element_data_type.build_references(element, "%s[%d]" % (path, i), references)
+            self.element_data_type.build_references(element, "%s[%d]" % (path, i))
             i += 1
     
-    def autogenerate_data(self, data :any, path :str, references :References):
+    def autogenerate_data(self, data :any, path :str):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
         new_list = list()
         i = 0
         for element in data:
-            _data, _FL = self.element_data_type.autogenerate_data(
-                element, "%s[%d]" % (path, i), references)
+            _data, _FL = self.element_data_type.autogenerate_data(element, "%s[%d]" % (path, i))
             new_list.append(_data)
             FL += _FL
             i += 1
         return new_list, FL
 
-    def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         FL = FindingsList()
         if self.minimum and len(data) < self.minimum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Length of list is lower than %d' % self.minimum))
         elif self.maximum and len(data) > self.maximum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Length of list is greater than %d' % self.maximum))
         i = 0
         for element in data:
-            FL += self.element_data_type.validate_data(
-                element, "%s[%d]" % (path, i), references)
+            FL += self.element_data_type.validate_data(element, "%s[%d]" % (path, i))
             i += 1
         
         if not self.allow_duplicates:
             remaining_data = copy.copy(data)
             i = 0 
             for element in data:
                 remaining_data = remaining_data[1:]
```

### Comparing `cd2t-1.5.0/cd2t/types/enum.py` & `cd2t-1.6.0/cd2t/types/enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from cd2t.types.base import BaseDataType
-from cd2t.References import References
 from cd2t.results import WrongValueFinding, FindingsList
 from cd2t.schema import SchemaError
+from cd2t.RunTimeEnv import RunTimeEnv
 
 
 class Enum(BaseDataType):
     type = 'enum'
-    multi_type_class = True
+    path_symbol = '<<'
     options = [
         # option_name, required, class
         ('allowed_values', True, list, None),
     ]
     supported_data_types = [int, float, dict, list, str]
 
-    def __init__(self, data_type_classes=dict(), path=str()) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.matching_classes = []
         self.allowed_values = None
         self.data_type_mismatch_message = "None of the allowed value data types matches"
     
     def verify_options(self, path: str):
         if not len(self.allowed_values):
             raise SchemaError("'allowed_values' must have at least one element", path)
         for value in self.allowed_values:
             value_type = type(value)
             if value_type not in self.supported_data_types:
                 raise SchemaError("'allowed_values' contains unsupported data types", path)
             if value_type not in self.matching_classes:
                 self.matching_classes.append(value_type)
 
-    def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         FL = FindingsList()
         if data not in self.allowed_values:
             FL.append(WrongValueFinding(path=path, message='Value not allowed'))
         return FL
```

### Comparing `cd2t-1.5.0/cd2t/types/float.py` & `cd2t-1.6.0/cd2t/types/float.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from cd2t.types.base import BaseDataType
 from cd2t.schema import SchemaError
 from cd2t.results import WrongValueFinding, AutogenerationError, AutogenerationInfo, FindingsList
-from cd2t.References import References, ReferenceElement, OPT
+from cd2t.References import ReferenceElement, OPT
+from cd2t.RunTimeEnv import RunTimeEnv
 import random
 
 
 class Float(BaseDataType):
     type = 'float'
+    path_symbol = '.'
     matching_classes = [float]
     support_reference = True
     options = [
         # option_name, required, class
         ('maximum', False, float, None),
         ('minimum', False, float, None),
         ('maximum_decimals', False, int, None),
@@ -19,16 +21,16 @@
         ('autogenerate', False, bool, False),
         ('autogenerate_default', False, float, None),
         ('autogenerate_ranges', False, list, list()),
         ('autogenerate_random_tries', False, int, 10),
         ('autogenerate_random_decimals', False, int, 2),
     ]
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.minimum = None
         self.maximum = None
         self.maximum_decimals = None
         self.allowed_values = list()
         self.allowed_dic = dict(
             discrete=list(),  # of floats
             round=list(),     # of tuples (decimals :int, matches :float)
@@ -106,15 +108,15 @@
                     and e[min] <= e[max]:
                 self.autogen_ranges.append((e[min], e[max]))
             else:
                 raise SchemaError(
                     "'autogenerate_ranges' contains unsupported directive at position %d" % i, path)
             i += 1
  
-    def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         def matches_values(value :float, value_dic :dict):
             if value in value_dic['discrete']:
                 return True
             for _round, _match in value_dic['round']:
                 if round(value, _round) == _match:
                     return True
             for _min, _max in value_dic['ranges']:
@@ -135,15 +137,15 @@
                 % (data, self.maximum_decimals), path))
         if matches_values(data, self.not_allowed_dic) \
                 or (self.allowed_values and not matches_values(data, self.allowed_dic)):
             FL.append(WrongValueFinding(
                 path=path, message='%s is not allowed' % data))
         return FL
     
-    def autogenerate_data(self, data :any, path :str, references :References):
+    def autogenerate_data(self, data :any, path :str):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         # We need to autogenerate
         new_value = None
         new_element = None
         if self.autogenerate_default:
@@ -154,22 +156,22 @@
                 if not self.autogenerate_ranges:
                     min = self.minimum
                     max = self.maximum
                 else:
                     random_list_key = round(random.uniform(1, len(self.autogen_ranges)))
                     min, max = self.autogen_ranges[random_list_key - 1]
                 random_float = round(random.uniform(min, max), self.autogenerate_random_decimals)
-                results = self.verify_data(random_float, path, references)
+                results = self.verify_data(random_float, path)
                 if not len(results):
                     if not OPT.NONE in self.ref_OPT:
                         new_element = ReferenceElement(self.ref_key, path, random_float, self.ref_OPT)
                         if OPT.UNIQUE in self.ref_OPT and \
-                                references.same_unique(new_element) is not None:
+                                self.RTE.references.same_unique(new_element) is not None:
                             continue
-                        references.add_element(new_element)
+                        self.RTE.references.add_element(new_element)
                     new_value = random_float
                     break
         if new_value is None:
             FL.append(AutogenerationError(
                 path=path,
                 message='Failed to find a valid random value after %d tries.' % self.autogenerate_random_tries))
         else:
```

### Comparing `cd2t-1.5.0/cd2t/types/idlist.py` & `cd2t-1.6.0/cd2t/types/idlist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,76 @@
 from cd2t.types.base import BaseDataType
-from cd2t.types.any import AnyDataType
-from cd2t.References import References, ReferenceElement, OPT
+from cd2t.References import ReferenceElement, OPT
 from cd2t.results import WrongValueFinding, UniqueErrorFinding, FindingsList
 from cd2t.schema import SchemaError
+from cd2t.RunTimeEnv import RunTimeEnv
 import re
 
 
 class IDList(BaseDataType):
     type = 'idlist'
+    path_symbol = '{id}'
     matching_classes = [dict]
     support_reference = True
     options = [
         # option_name, required, class
         ('minimum', False, int, None),
         ('maximum', False, int, None),
-        ('elements', True, dict, None),
+        ('elements', True, [dict, str], None),
         ('id_type', False, str, 'string'),
         ('id_minimum', False, int, None),
         ('id_maximum', False, int, None),
         ('allowed_ids', False, list, None),
         ('not_allowed_ids', False, list, list()),
     ]
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.minimum = None
         self.maximum = None
         self.elements = None
         self.element_type = None
         self.id_type = 'string'
         self.id_minimum = None
         self.id_maximum = None
         self.allowed_ids = None
         self.not_allowed_ids = list()
     
-    def build_schema(self, schema :dict, path :str,
-                     data_types :dict, subschemas :dict,
-                     subpath :list):
-        self.__init__()
-        path = path + '{id}'
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
+        self.__init__(RTE=self.RTE)
+        path = path + self.path_symbol
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
+
         if self.id_type not in ['string', 'integer']:
             raise SchemaError("id_type '%s' is not valid" % self.id_type, path)
-        if 'type' in self.elements.keys():
-            element_type_name = self.elements['type']
-            if element_type_name not in data_types:
-                raise SchemaError("Elements data type '%s' not found" % element_type_name, path)
-            self.element_type = data_types[element_type_name]()
-        elif self.elements:
-            raise SchemaError("'type' not found in elements schema", path)
-        else:
-            self.element_type = AnyDataType()
+        self.element_type = self._get_data_type('elements', path + 'elements')
         # Save recursively detected data type (i.e. from 'schema' --> subschema)
         self.element_type = self.element_type.build_schema(
-            schema=self.elements, path=path,
-            data_types=data_types, subschemas=subschemas, subpath=subpath)
+            schema=self.elements, path=path, subschemas=subschemas, subpath=subpath)
         return self
     
-    def build_sub_references(self, data :any, path :str, references :References):
+    def build_sub_references(self, data :any, path :str):
         for id, element in data.items():
-            self.element_type.build_references(data=element,
-                                            path=path + '{id}',
-                                            references=references)
+            self.element_type.build_references(data=element, path=path + self.path_symbol)
     
-    def autogenerate_data(self, data :any, path :str, references :References):
+    def autogenerate_data(self, data :any, path :str):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
         new_dict = dict()
         for id, element in data.items():
             new_path = path + '{}' + str(id)
             _data, _FL = self.element_type.autogenerate_data(data=element,
-                                                            path=new_path,
-                                                            references=references)
+                                                            path=new_path)
             new_dict[id] = _data
             FL += _FL
         return new_dict, FL
 
-    def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         FL = FindingsList()
         path = path + '{}'
         if self.minimum and len(data) < self.minimum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Attribute count is lower than minimum %d' % self.minimum))
         elif self.maximum is not None and len(data) > self.maximum:
@@ -144,31 +132,30 @@
                         message="Attribute is not allowed"))
                 elif self.allowed_ids and id not in self.allowed_ids:
                     _FL.append(WrongValueFinding(
                         path=id_path,
                         message="Attribute is not an allowed value"))
 
             if not _FL:
-                FL += (self.element_type.validate_data(
-                    data=element, path=id_path, references=references))
+                FL += (self.element_type.validate_data(data=element, path=id_path))
             else:
                 FL += _FL
         return FL
 
-    def verify_reference(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_reference(self, data :any, path :str) -> FindingsList:
         if not self.data_matches_type(data) or OPT.NONE in self.ref_OPT:
             return []
         results = list()
         for id in data.keys():
             id_path = path + '{}' + id
             element = ReferenceElement(self.ref_key, id_path, id, self.ref_OPT)
-            other = references.same_unique(element)
+            other = self.RTE.references.same_unique(element)
             if other is not None:
-                if references.namespace != other.namespace:
+                if self.RTE.namespace != other.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
                 results.append(UniqueErrorFinding(
                     path=id_path, message="ID '%s' already used at '%s'" % (str(id), _path)))
             else:
-                references.add_element(element)
+                self.RTE.references.add_element(element)
         return results
```

### Comparing `cd2t-1.5.0/cd2t/types/integer.py` & `cd2t-1.6.0/cd2t/types/integer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from cd2t.types.base import BaseDataType
 from cd2t.results import FindingsList, WrongValueFinding, AutogenerationError, AutogenerationInfo
-from cd2t.References import References, OPT, ReferenceElement
+from cd2t.References import OPT, ReferenceElement
 from cd2t.schema import SchemaError
+from cd2t.RunTimeEnv import RunTimeEnv
 import itertools
 import random
 
 
 class Integer(BaseDataType):
     type = 'integer'
+    path_symbol = '+'
     matching_classes = [int]
     support_reference = True
     options = [
         # option_name, required, class, default value
         ('maximum', False, int, None),
         ('minimum', False, int, None),
         ('not_allowed_values', False, list, list()),
         ('autogenerate', False, bool, False),
         ('autogenerate_default', False, int, None),
         ('autogenerate_maximum', False, int, None),
         ('autogenerate_minimum', False, int, None),
         ('autogenerate_find', False, str, 'next_higher'),
     ]
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.minimum = None
         self.maximum = None
         self.not_allowed_values = list()
         self.autogenerate = False
         self.autogenerate_default = None
         self.autogenerate_find = 'next_higher'
         self.autogenerate_minimum = None
@@ -51,76 +53,76 @@
             elif self.autogenerate_find == 'random' \
                     and (not (self.autogenerate_minimum or self.minimum) \
                               or not (self.autogenerate_maximum or self.maximum)):
                 raise SchemaError("Option 'autogenerate_find' as 'random' needs " +\
                                   "'minimum' or 'autogenerate_minimum' and " +\
                                   "'maximum' or 'autogenerate_maximum' to be set", path)
     
-    def autogenerate_data(self, data :any, path :str, references :References):
+    def autogenerate_data(self, data :any, path :str):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         # We need to autogenerate
         if self.autogenerate_default is not None:
             data = self.autogenerate_default
         
         elif self.autogenerate_find == 'next_lower':
             start = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
             end = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
             if OPT.UNIQUE not in self.ref_OPT:
                 data = start
             else:
-                all_uniques = references.get_unique_values_by_ref_key(self.ref_key)
+                all_uniques = self.RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 blocked = all_uniques.union(set(self.not_allowed_values))
                 _iter = itertools.filterfalse(blocked.__contains__, itertools.count(start=start, step=-1))
                 data = next(_iter)
                 if end is not None and data < end:
                     data = None
                 else:
                     new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
-                    references.add_element(new_element)
+                    self.RTE.references.add_element(new_element)
                 
         elif self.autogenerate_find == 'next_higher':
             start = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
             end = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
             if OPT.UNIQUE not in self.ref_OPT:
                 data = start
             else:
-                all_uniques = references.get_unique_values_by_ref_key(self.ref_key)
+                all_uniques = self.RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 blocked = all_uniques.union(set(self.not_allowed_values))
                 _iter = itertools.filterfalse(blocked.__contains__, itertools.count(start=start, step=1))
                 data = next(_iter)
                 if end is not None and data > end:
                     data = None
                 else:
                     new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
-                    references.add_element(new_element)
+                    self.RTE.references.add_element(new_element)
         
         elif self.autogenerate_find == 'random':
             start = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
             end = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
             min_max_values = set(range(start, end + 1))
             allowed_values = min_max_values - set(self.not_allowed_values)
             if allowed_values and OPT.UNIQUE in self.ref_OPT:
-                available_values = allowed_values - references.get_unique_values_by_ref_key(self.ref_key)
+                available_values = allowed_values - self.RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 if available_values:
                     data = list(available_values)[random.randint(0, len(available_values)-1)]
                     new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
-                    references.add_element(new_element)
+                    self.RTE.references.add_element(new_element)
             elif allowed_values:
                 data = list(allowed_values)[random.randint(0, len(allowed_values)-1)]
         
         if data is None:
             FL.append(AutogenerationError(path=path, message='All values in use!'))
         else:
             FL.append(AutogenerationInfo(
                 path=path, message='Autogenerated value is %d' % data))
         return data, FL
  
-    def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         FL = FindingsList()
         if self.minimum is not None and self.minimum > data:
             FL.append(WrongValueFinding(
                 path=path, message='%d is lower than minimum %d' % (data, self.minimum)))
         elif self.maximum is not None and self.maximum < data:
             FL.append(WrongValueFinding(
                 path=path, message='%d is higher than maximum %d' % (data, self.maximum)))
```

### Comparing `cd2t-1.5.0/cd2t/types/object.py` & `cd2t-1.6.0/cd2t/types/object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 from cd2t.types.base import BaseDataType
-from cd2t.types.any import AnyDataType
 from cd2t.utils import string_matches_regex_list, regex_matches_in_string_list
-from cd2t.References import References
 from cd2t.results import ValidationFinding, FindingsList
 from cd2t.schema import SchemaError
+from cd2t.RunTimeEnv import RunTimeEnv
 
 
 class Object(BaseDataType):
     type = 'object'
+    path_symbol = '{}'
     matching_classes = [dict]
     support_reference = True
     options = [
         # option_name, required, class, init_value
         ('attributes', False, dict, None),
         ('required_attributes', False, list, list),
         ('dependencies', False, dict, dict()),
         ('reference_attributes', False, list, None),
         ('ignore_undefined_attributes', False, bool, False),
         ('allow_regex_attributes', False, bool, False),
         ('autogenerate', False, bool, True)
     ]
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.attributes = None
         self.attributes_objects = dict()
+        self.tmp_a_schema = None
         self.required_attributes = list()
         self.dependencies = dict()
         self.reference_attributes = None
         self.ignore_undefined_attributes = False
         self.allow_regex_attributes = False
         self.autogenerate = True
         return
     
-    def build_schema(self, schema :dict, path :str,
-                     data_types :dict, subschemas :dict,
-                     subpath :list):
-        self.__init__()
-        path = path + '{}'
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
+        self.__init__(RTE=self.RTE)
+        path = path + self.path_symbol
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
         if self.attributes is None:
             # No other options should be set:
             for option, required, cls, init_value in self.options:
                 if exec("self." + option + " != init_value"):
                     raise SchemaError("Option 'attribute' is omitted, no other option is expected.")
@@ -68,65 +67,56 @@
             for ex_attr in dep_info.get('excludes', []):
                 if not self._attribute_in_list(ex_attr, list(self.attributes.keys()), self.allow_regex_attributes):
                     raise SchemaError("Excluded attribute '%s' " % ex_attr +\
                                       "for dependency '%s' not in attributes" % dep_attr, path)
         #
         for a_name, a_schema in self.attributes.items():
             a_path = path + a_name
-            if not isinstance(a_schema, dict):
-                raise SchemaError("Schema is not a dictionary", a_path)
-            if 'type' in a_schema.keys():
-                type_name = a_schema['type']
-                if type_name not in data_types.keys():
-                    raise SchemaError("Data type '%s' not found" % type_name, a_path)
-                data_type = data_types[type_name]()
-            else:
-                data_type = AnyDataType()
+            self.tmp_a_schema = a_schema
+            data_type = self._get_data_type('tmp_a_schema', a_path)
             # Save recursively detected data type (i.e. from 'schema' --> subschema)
-            _data_type = data_type.build_schema(a_schema, path + a_name, data_types, subschemas, subpath)
-            self.attributes_objects[a_name] = _data_type
+            self.attributes_objects[a_name] = data_type.build_schema(self.tmp_a_schema, a_path, subschemas, subpath)
         return self
     
-    def build_references(self, data :any, path :str, references :References):
+    def build_references(self, data :any, path :str):
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 continue
-            a_path = path + '{}' + a_name
-            data_type.build_references(a_data, a_path, references)
+            a_path = path + self.path_symbol + a_name
+            data_type.build_references(a_data, a_path)
     
-    def autogenerate_data(self, data :any, path :str, references :References):
+    def autogenerate_data(self, data :any, path :str):
         FL = FindingsList()
         if data is None or not self.data_matches_type(data):
             return data, FL
         new_data = dict()
         processed_attributes = list()
         if not self.allow_regex_attributes and self.autogenerate:
             for a_name, data_type in self.attributes_objects.items():
                 processed_attributes.append(a_name)
-                a_path = path + '{}' + a_name
+                a_path = path + self.path_symbol + a_name
                 _FL = FindingsList()
                 if a_name not in data.keys():
-                    _data, _FL = data_type.autogenerate_data(
-                        data=None, path=a_path, references=references)
+                    _data, _FL = data_type.autogenerate_data(data=None, path=a_path)
                     if _FL:
                         new_data[a_name] = _data
                 else:
-                    _data, _FL = data_type.autogenerate_data(data[a_name], a_path, references)
+                    _data, _FL = data_type.autogenerate_data(data[a_name], a_path)
                     new_data[a_name] = _data
                 FL += _FL
         for a_name, a_data in data.items():
             if a_name in processed_attributes:
                 continue
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 new_data[a_name] = a_data
                 continue
-            a_path = path + '{}' + a_name
-            _data, _FL = data_type.autogenerate_data(a_data, a_path, references)
+            a_path = path + self.path_symbol + a_name
+            _data, _FL = data_type.autogenerate_data(a_data, a_path)
             new_data[a_name] = _data
             FL += _FL
         return new_data, FL
     
     @staticmethod
     def _attribute_in_list(attribute :str, attributes :list, regex_allowed=False) -> bool:
         if regex_allowed:
@@ -138,35 +128,35 @@
     def _get_attribute_object(self, name :str, regex_allowed=False) -> bool:
         if regex_allowed:
             name = string_matches_regex_list(string=name,
                                                    regex_list=list(self.attributes_objects.keys()),
                                                    full_match=True)
         return self.attributes_objects.get(name, None)
 
-    def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         FL = FindingsList()
         if self.attributes is None:
             return FL
-        path = path + '{}'
+        path = path + self.path_symbol
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 if self.ignore_undefined_attributes:
                     continue
                 FL.append(ValidationFinding(path=path, message="Invalid attribute '%s'" % a_name))
                 continue
             a_path = path + a_name
-            FL += data_type.validate_data(data=a_data, path=a_path, references=references)
+            FL += data_type.validate_data(data=a_data, path=a_path)
         for req_attr in self.required_attributes:
             found_in_data_keys = False
             if self.allow_regex_attributes:
                 if regex_matches_in_string_list(
-                                                        regex=req_attr,
-                                                        strings=list(data.keys()),
-                                                        full_match=True):
+                                                regex=req_attr,
+                                                strings=list(data.keys()),
+                                                full_match=True):
                     found_in_data_keys = True
             elif req_attr in data.keys():
                 found_in_data_keys = True
             if not found_in_data_keys:
                 FL.append(ValidationFinding(
                     path = path + req_attr,
                     message = "Required attribute missing"))
```

### Comparing `cd2t-1.5.0/cd2t/types/string.py` & `cd2t-1.6.0/cd2t/types/string.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from cd2t.types.base import BaseDataType
 from cd2t.utils import string_matches_regex_list
 from cd2t.schema import SchemaError
 from cd2t.results import FindingsList, WrongValueFinding
-from cd2t.References import References, OPT, ReferenceElement, ConsumerElement
-import re
+from cd2t.References import OPT, ReferenceElement, ConsumerElement
+from cd2t.RunTimeEnv import RunTimeEnv
 
 class String(BaseDataType):
     type = 'string'
+    path_symbol = '#'
     matching_classes = [str]
     support_reference = True
     options = [
         # option_name, required, class
         ('maximum', False, int, None),
         ('minimum', False, int, None),
         ('allowed_values', False, list, None),
         ('not_allowed_values', False, list, list()),
         ('regex_mode', False, bool, False),
         ('regex_multiline', False, bool, False),
         ('regex_fullmatch', False, bool, True),
     ]
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, RTE :RunTimeEnv) -> None:
+        super().__init__(RTE=RTE)
         self.minimum = None
         self.maximum = None
         self.allowed_values = None
         self.not_allowed_values = list()
         self.regex_mode = False
         self.regex_multiline = False
         self.regex_fullmatch = True
@@ -57,15 +58,15 @@
             if OPT.CONSUMER not in self.ref_OPT:
                 raise SchemaError("Namespace lookup needs 'mode' == 'consumer'", path)
             if self.namespace_separator_char is None:
                 raise SchemaError("Namespace lookup requires 'namespace_separator_char' to be set", path)
             if not self.namespace_separator_char:
                 raise SchemaError("'namespace_separator_char' mustn't be '' (empty)", path)
         
-    def verify_data(self, data :any, path :str, reference=References()) -> FindingsList:
+    def verify_data(self, data :any, path :str) -> FindingsList:
         FL = FindingsList()
         if self.minimum is not None and self.minimum > len(data):
             FL.append(WrongValueFinding(
                 path=path, message='String length is lower than minimum %d' % self.minimum))
         elif self.maximum is not None and self.maximum < len(data):
             FL.append(WrongValueFinding(
                 path=path, message='String length is greater than maximum %d' % self.maximum))
```

### Comparing `cd2t-1.5.0/LICENSE` & `cd2t-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cd2t-1.5.0/README.md` & `cd2t-1.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.6.0**:
+- *Changed*: Python 3.9 or higher required
+- *New*: Data Type Shortcuts - Specify data type with defaults as string only
+- *Add*: Validator API - Method to get reference findings
+- *Changed*: Multitype Data Type - Enhanced data type support
+
 **Version 1.5.0**:
 - *New*: Integer Data Type - Autogenerate random value
 - *New*: Integer Data Type - Autogenerate default value
 - *New*: Improved Reference Findings
 - *Changed*: All Data Types - Schema and data path adjustment
 
 **Version 1.4.0**:
@@ -58,14 +64,18 @@
 
 **Version 1.0**: *withdrawn form pypi.org*
 
 ## Data Structure Schema
 ```yaml
 name: < str >
 description: < str >
+allow_data_type_shortcuts: < bool | default -> false >
+# Shortcuts are Data Type strings instead of dictionaries.
+# Corresponding data type with default options is used.
+
 root: { data type schema }
 
 subschemas:
   < sub schema name >: { data type schema }
 ```
 
 ## Data Type Options
@@ -84,27 +94,31 @@
 - [String Data Type](#string-data-type)
 - [Reference Options](#reference-options)
 
 ### Any Data Type
 **Description**  
 This data type represents any data. The validator stops further data validation or autogeneration.
 
+>Schema Path Sympbol: **\***
+
 **Limitations**  
 - *referencing* is not supported
 - *autogeneration* is not supported
 
 **Any Schema Keys**  
 ```yaml
 type: 'any' # If type is omitted, validator uses Any Data Type
 ```
 
 ### Bool Data Type
 **Description**  
 This data type represents a boolean values (true/false).
 
+>Schema Path Sympbol: **!**
+
 **Limitations**  
 - *referencing* is not supported
 
 **Bool Schema Keys**  
 ```yaml
 type: 'bool'
 
@@ -117,14 +131,16 @@
 autogenerate_default: < bool > # true or false; must match 'allowed_value' (if set)
 ```
 
 ### Enum Data Type
 **Description**  
 This data type represents a selection of allowed values.
 
+>Schema Path Sympbol: **<<**
+
 **Limitations**  
 - *referencing* is not supported
 - *autogeneration* is not supported
 
 **Enum Schema Keys**  
 ```yaml
 type: 'enum'
@@ -133,14 +149,16 @@
 - < value >
 ```
 
 ### Float Data Type
 **Description**  
 This data type represents float values.
 
+>Schema Path Sympbol: **.**
+
 **Float Schema Keys**
 ```yaml
 type: 'float'
 
 reference: { unique options }
 
 maximum: < float >
@@ -208,14 +226,16 @@
 5. value is in allowed_values
 
 ### ID-List Data Type
 **Description**  
 This data type represents a dictionary, where keys are IDs.
 IDs can be strings or integer.
 
+>Schema Path Sympbol: **{id}**
+
 **Limitations**  
 - *autogeneration* is not supported
 
 **ID-List Schema Keys**  
 ```yaml
 type: 'id_list'
 
@@ -254,14 +274,16 @@
 # 'not_allowed_ids' are test before 'allowed_ids'.
 ```
 
 ### Integer Data Type
 **Description**  
 This data type represents integer values.
 
+>Schema Path Sympbol: **+**
+
 **Integer Schema Keys**  
 ```yaml
 type: 'integer'
 
 reference: { unique options }
 
 maximum: < int >
@@ -299,14 +321,16 @@
 
 ### List Data Type
 **Description**  
 This data type represents a list of same data types.  
 If different data types are allowed in the list,
 use data type 'multitype' as elements.
 
+>Schema Path Sympbol: **[]**
+
 **Limitations**  
 - *referencing* is not supported - use referencing in the 'elements' data type
 - *autogeneration* of list elements is not supported - but autogeneration within existing elements data structure is supported (pass-through).
 
 **List Schema Keys**  
 ```yaml
 type: 'list' # required
@@ -324,48 +348,51 @@
 # Allow same element data multiple times
 ```
 
 ### Multitype Data Type
 **Description**  
 This data type represents a selection of allowed data types.
 
+>Schema Path Sympbol: **?**
+
 **Limitations**  
 - *referencing* is not supported - use referencing in the 'elements' data type
 - *autogeneration* of data types is not supported - but autogeneration within existing data structure is supported (pass-through).
-- Data Type Selection Rules:
-  - Data type *Schema* is not allowed - use *schema* in first place and use *Multitype* in subschema's root data type.
-  - Each data type is allowed only once.
-  - *ID-List* and *Object* are treated as the same data type as both rely on dictionaries.
+- *Multitype* in * Multiype* is not allowed
 
 **Multitype Schema Keys**  
 ```yaml
 type: 'multitype'
 types: # required
 - { data type schema }
 # List of data type schemas.
 ```
 
 ### None Data Type
 **Description**  
 This data type represents a none or null value.
 
+>Schema Path Sympbol: **°**
+
 **Limitations**  
 - *referencing* is not supported
 - *autogeneration* of data types is not supported - it is already none :wink:
 
 **Multitype Schema Keys**  
 ```yaml
 type: 'none'
 ```
 
 ### Object Data Type
 **Description**  
 This data type represents an object with attributes. Technically its a dictionary in Python.  
 Attributes of the object are keys in the dictionary.
 
+>Schema Path Sympbol: **{}**
+
 **Limitations**  
 - *autogeneration* of missing keys is supported, if value data type supports autogeneration
 
 **Object Schema Keys**  
 ```yaml
 type: 'object'
 
@@ -413,26 +440,30 @@
 ```
 
 ### Schema Data Type
 **Description**  
 This data type does not represents an expected data value.  
 It uses a subschema's root data type to process the data structure.
 
+>Schema Path Sympbol: **\<** *name* **\>**
+
 **Schema Schema Keys**  
 ```yaml
 type: 'schema'
 
 subschema: < str >
 # Name of the subschema, which is defined under 'subschemas' in schema.
 ```
 
 ### String Data Type
 **Description**  
 This data type represents a string.
 
+>Schema Path Sympbol: **#**
+
 **Limitations**  
 - *autogeneration* is not supported.
 
 **String Schema Keys**  
 ```yaml
 type: 'string'
 
@@ -516,12 +547,13 @@
 results = list()
 for filename in os.listdir('./my_data_folder'):
     with open(filename) as f:
         test_data = yaml.load(f)
     validator.change_namespace(filename)
     _results = validator.validate_data(test_data)
     results.extend(_results)
-    _results = validator.references.get_producer_consumer_issues()
-    results.extend(_results)
+
+_results = validator.get_reference_findings()
+results.extend(_results)
 
 print('\n'.join(results))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cd2t-1.5.0/pyproject.toml` & `cd2t-1.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 [tool.hatch.build]
 include = [
   "/cd2t",
 ]
 
 [project]
 name = "cd2t"
-version = "1.5.0"
+version = "1.6.0"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "cd2t validates data structure, data types and values with templates"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Intended Audience :: Developers",
 ]
```

### Comparing `cd2t-1.5.0/PKG-INFO` & `cd2t-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: cd2t
-Version: 1.5.0
+Version: 1.6.0
 Summary: cd2t validates data structure, data types and values with templates
 Project-URL: Homepage, https://gitlab.com/ko.no/cd2t
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/cd2t/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # cd2t
 
 **repository**:   https://gitlab.com/ko.no/cd2t
 
 **Table of Content**
@@ -33,14 +33,20 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.6.0**:
+- *Changed*: Python 3.9 or higher required
+- *New*: Data Type Shortcuts - Specify data type with defaults as string only
+- *Add*: Validator API - Method to get reference findings
+- *Changed*: Multitype Data Type - Enhanced data type support
+
 **Version 1.5.0**:
 - *New*: Integer Data Type - Autogenerate random value
 - *New*: Integer Data Type - Autogenerate default value
 - *New*: Improved Reference Findings
 - *Changed*: All Data Types - Schema and data path adjustment
 
 **Version 1.4.0**:
@@ -74,14 +80,18 @@
 
 **Version 1.0**: *withdrawn form pypi.org*
 
 ## Data Structure Schema
 ```yaml
 name: < str >
 description: < str >
+allow_data_type_shortcuts: < bool | default -> false >
+# Shortcuts are Data Type strings instead of dictionaries.
+# Corresponding data type with default options is used.
+
 root: { data type schema }
 
 subschemas:
   < sub schema name >: { data type schema }
 ```
 
 ## Data Type Options
@@ -100,27 +110,31 @@
 - [String Data Type](#string-data-type)
 - [Reference Options](#reference-options)
 
 ### Any Data Type
 **Description**  
 This data type represents any data. The validator stops further data validation or autogeneration.
 
+>Schema Path Sympbol: **\***
+
 **Limitations**  
 - *referencing* is not supported
 - *autogeneration* is not supported
 
 **Any Schema Keys**  
 ```yaml
 type: 'any' # If type is omitted, validator uses Any Data Type
 ```
 
 ### Bool Data Type
 **Description**  
 This data type represents a boolean values (true/false).
 
+>Schema Path Sympbol: **!**
+
 **Limitations**  
 - *referencing* is not supported
 
 **Bool Schema Keys**  
 ```yaml
 type: 'bool'
 
@@ -133,14 +147,16 @@
 autogenerate_default: < bool > # true or false; must match 'allowed_value' (if set)
 ```
 
 ### Enum Data Type
 **Description**  
 This data type represents a selection of allowed values.
 
+>Schema Path Sympbol: **<<**
+
 **Limitations**  
 - *referencing* is not supported
 - *autogeneration* is not supported
 
 **Enum Schema Keys**  
 ```yaml
 type: 'enum'
@@ -149,14 +165,16 @@
 - < value >
 ```
 
 ### Float Data Type
 **Description**  
 This data type represents float values.
 
+>Schema Path Sympbol: **.**
+
 **Float Schema Keys**
 ```yaml
 type: 'float'
 
 reference: { unique options }
 
 maximum: < float >
@@ -224,14 +242,16 @@
 5. value is in allowed_values
 
 ### ID-List Data Type
 **Description**  
 This data type represents a dictionary, where keys are IDs.
 IDs can be strings or integer.
 
+>Schema Path Sympbol: **{id}**
+
 **Limitations**  
 - *autogeneration* is not supported
 
 **ID-List Schema Keys**  
 ```yaml
 type: 'id_list'
 
@@ -270,14 +290,16 @@
 # 'not_allowed_ids' are test before 'allowed_ids'.
 ```
 
 ### Integer Data Type
 **Description**  
 This data type represents integer values.
 
+>Schema Path Sympbol: **+**
+
 **Integer Schema Keys**  
 ```yaml
 type: 'integer'
 
 reference: { unique options }
 
 maximum: < int >
@@ -315,14 +337,16 @@
 
 ### List Data Type
 **Description**  
 This data type represents a list of same data types.  
 If different data types are allowed in the list,
 use data type 'multitype' as elements.
 
+>Schema Path Sympbol: **[]**
+
 **Limitations**  
 - *referencing* is not supported - use referencing in the 'elements' data type
 - *autogeneration* of list elements is not supported - but autogeneration within existing elements data structure is supported (pass-through).
 
 **List Schema Keys**  
 ```yaml
 type: 'list' # required
@@ -340,48 +364,51 @@
 # Allow same element data multiple times
 ```
 
 ### Multitype Data Type
 **Description**  
 This data type represents a selection of allowed data types.
 
+>Schema Path Sympbol: **?**
+
 **Limitations**  
 - *referencing* is not supported - use referencing in the 'elements' data type
 - *autogeneration* of data types is not supported - but autogeneration within existing data structure is supported (pass-through).
-- Data Type Selection Rules:
-  - Data type *Schema* is not allowed - use *schema* in first place and use *Multitype* in subschema's root data type.
-  - Each data type is allowed only once.
-  - *ID-List* and *Object* are treated as the same data type as both rely on dictionaries.
+- *Multitype* in * Multiype* is not allowed
 
 **Multitype Schema Keys**  
 ```yaml
 type: 'multitype'
 types: # required
 - { data type schema }
 # List of data type schemas.
 ```
 
 ### None Data Type
 **Description**  
 This data type represents a none or null value.
 
+>Schema Path Sympbol: **°**
+
 **Limitations**  
 - *referencing* is not supported
 - *autogeneration* of data types is not supported - it is already none :wink:
 
 **Multitype Schema Keys**  
 ```yaml
 type: 'none'
 ```
 
 ### Object Data Type
 **Description**  
 This data type represents an object with attributes. Technically its a dictionary in Python.  
 Attributes of the object are keys in the dictionary.
 
+>Schema Path Sympbol: **{}**
+
 **Limitations**  
 - *autogeneration* of missing keys is supported, if value data type supports autogeneration
 
 **Object Schema Keys**  
 ```yaml
 type: 'object'
 
@@ -429,26 +456,30 @@
 ```
 
 ### Schema Data Type
 **Description**  
 This data type does not represents an expected data value.  
 It uses a subschema's root data type to process the data structure.
 
+>Schema Path Sympbol: **\<** *name* **\>**
+
 **Schema Schema Keys**  
 ```yaml
 type: 'schema'
 
 subschema: < str >
 # Name of the subschema, which is defined under 'subschemas' in schema.
 ```
 
 ### String Data Type
 **Description**  
 This data type represents a string.
 
+>Schema Path Sympbol: **#**
+
 **Limitations**  
 - *autogeneration* is not supported.
 
 **String Schema Keys**  
 ```yaml
 type: 'string'
 
@@ -532,12 +563,13 @@
 results = list()
 for filename in os.listdir('./my_data_folder'):
     with open(filename) as f:
         test_data = yaml.load(f)
     validator.change_namespace(filename)
     _results = validator.validate_data(test_data)
     results.extend(_results)
-    _results = validator.references.get_producer_consumer_issues()
-    results.extend(_results)
+
+_results = validator.get_reference_findings()
+results.extend(_results)
 
 print('\n'.join(results))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

