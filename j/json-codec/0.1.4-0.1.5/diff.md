# Comparing `tmp/json_codec-0.1.4.tar.gz` & `tmp/json_codec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_codec-0.1.4.tar", max compression
+gzip compressed data, was "json_codec-0.1.5.tar", max compression
```

## Comparing `json_codec-0.1.4.tar` & `json_codec-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     3033 2022-12-10 21:46:23.651234 json_codec-0.1.4/README.md
--rw-r--r--   0        0        0       33 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/__init__.py
--rw-r--r--   0        0        0        0 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/__init__.py
--rw-r--r--   0        0        0      976 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/date_codec.py
--rw-r--r--   0        0        0     1145 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/datetime_codec.py
--rw-r--r--   0        0        0     2297 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/dict_codec.py
--rw-r--r--   0        0        0     1230 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/list_codec.py
--rw-r--r--   0        0        0      856 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/primitive_codec.py
--rw-r--r--   0        0        0     1165 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/set_codec.py
--rw-r--r--   0        0        0      984 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/time_codec.py
--rw-r--r--   0        0        0     1002 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/tuple_codec.py
--rw-r--r--   0        0        0     1007 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/codecs/union_codec.py
--rw-r--r--   0        0        0     9463 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/json_codec.py
--rw-r--r--   0        0        0     8772 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/test_json_codec.py
--rw-r--r--   0        0        0     2272 2022-12-10 21:46:23.651234 json_codec-0.1.4/json_codec/types.py
--rw-r--r--   0        0        0      484 2022-12-10 21:46:23.651234 json_codec-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 json_codec-0.1.4/setup.py
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 json_codec-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3033 2022-12-10 21:43:50.025310 json_codec-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 02:13:43.379791 json_codec-0.1.5/json_codec/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 02:13:43.339791 json_codec-0.1.5/json_codec/codecs/__init__.py
+-rw-r--r--   0        0        0      960 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/date_codec.py
+-rw-r--r--   0        0        0     1111 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/datetime_codec.py
+-rw-r--r--   0        0        0     2211 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/dict_codec.py
+-rw-r--r--   0        0        0     1223 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/list_codec.py
+-rw-r--r--   0        0        0      906 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/primitive_codec.py
+-rw-r--r--   0        0        0     1151 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/set_codec.py
+-rw-r--r--   0        0        0      960 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/time_codec.py
+-rw-r--r--   0        0        0     1002 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/tuple_codec.py
+-rw-r--r--   0        0        0     1000 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/codecs/union_codec.py
+-rw-r--r--   0        0        0     9581 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/json_codec.py
+-rw-r--r--   0        0        0     8691 2023-04-15 02:14:25.229790 json_codec-0.1.5/json_codec/test_json_codec.py
+-rw-r--r--   0        0        0     2272 2023-04-15 02:13:43.439792 json_codec-0.1.5/json_codec/types.py
+-rw-r--r--   0        0        0      502 2023-04-15 02:14:33.609790 json_codec-0.1.5/json_codec/utils.py
+-rw-r--r--   0        0        0      484 2023-04-15 02:15:14.079786 json_codec-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 json_codec-0.1.5/setup.py
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 json_codec-0.1.5/PKG-INFO
```

### Comparing `json_codec-0.1.4/README.md` & `json_codec-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.4/json_codec/codecs/date_codec.py` & `json_codec-0.1.5/json_codec/codecs/date_codec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Any, Callable, Generator, Tuple, Type, TypeVar
+from typing import Any, Generator, Type, TypeVar
 from datetime import date, datetime
+
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeDecoder,
     ValidationError,
 )
```

### Comparing `json_codec-0.1.4/json_codec/codecs/datetime_codec.py` & `json_codec-0.1.5/json_codec/codecs/datetime_codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any, Callable, Generator, Tuple, Type, TypeVar
-from datetime import date, datetime, timedelta, timezone
+from typing import Any, Generator, Type, TypeVar
+from datetime import datetime, timezone
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeDecoder,
     ValidationError,
 )
```

### Comparing `json_codec-0.1.4/json_codec/codecs/dict_codec.py` & `json_codec-0.1.5/json_codec/codecs/dict_codec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Any, Callable, Dict, Generator, List, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, Generator, Type, TypeVar
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeArgsLengthMismatch,
     TypeDecoder,
     ValidationError,
-    ValidationErrorBase,
-    ValidationErrorCollection,
 )
 
 K = TypeVar("K")
 V = TypeVar("V")
 
 
 class DictKeyError(Exception):
```

### Comparing `json_codec-0.1.4/json_codec/codecs/list_codec.py` & `json_codec-0.1.5/json_codec/codecs/list_codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Generator, List, Tuple, Type, TypeVar, cast
+from typing import Any, Generator, List, Type, TypeVar, cast
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeArgsLengthMismatch,
     TypeDecoder,
     ValidationError,
```

### Comparing `json_codec-0.1.4/json_codec/codecs/primitive_codec.py` & `json_codec-0.1.5/json_codec/codecs/primitive_codec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from typing import Any, Callable, Generator, Tuple, Type, TypeVar
+from typing import Any, Callable, Generator, Type, TypeVar
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeDecoder,
     ValidationError,
 )
 
 T = TypeVar("T")
 
 
 class PrimitiveTypeDecoder(TypeDecoder[T]):
-    def __init__(self, type_: Callable[..., T]) -> None:
+    def __init__(self, type_: Callable[..., T], type_name: str) -> None:
         self.type_ = type_
+        self.type_name = type_name
 
     def parse(
         self, value: Any, *types: Type[Any]
     ) -> Generator[
         ParseProcessYield[Any], ParseProcessResult[Any], ParseProcessResult[T]
     ]:
         try:
             return self._success(self.type_(value))
         except ValueError:
             return self._failure(
                 ValidationError(
-                    f"Expected type {self.type_}, but {value} is not a valid value"
+                    f"Expected type {self.type_name}, but '{value}' is not a valid value"
                 )
             )
         yield
 
 
 def serialize_primitive(value: Any) -> Any:
     return str(value)
```

### Comparing `json_codec-0.1.4/json_codec/codecs/set_codec.py` & `json_codec-0.1.5/json_codec/codecs/set_codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Generator, List, Set, Tuple, Type, TypeVar
+from typing import Any, Generator, Set, Type, TypeVar
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeArgsLengthMismatch,
     TypeDecoder,
     ValidationError,
@@ -15,15 +15,14 @@
     def parse(
         self, value: Any, *types: Type[Any]
     ) -> Generator[
         ParseProcessYield[Any],
         ParseProcessResult[Any],
         ParseProcessResult[Set[T]],
     ]:
-
         if not isinstance(value, list):
             return self._failure(ValidationError(f"Expected list, got {value}"))
 
         if len(types) != 1:
             return self._failure(
                 TypeArgsLengthMismatch(f"Expected 1 type argument, got {len(types)}")
             )
```

### Comparing `json_codec-0.1.4/json_codec/codecs/time_codec.py` & `json_codec-0.1.5/json_codec/codecs/time_codec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any, Callable, Generator, Tuple, Type, TypeVar
-from datetime import date, datetime, time
+from typing import Any, Generator, Type, TypeVar
+from datetime import datetime, time
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeDecoder,
     ValidationError,
 )
@@ -17,15 +17,14 @@
     ) -> Generator[
         ParseProcessYield[Any], ParseProcessResult[Any], ParseProcessResult[time]
     ]:
         if not isinstance(value, str):
             return self._failure(ValidationError(f"Expected string, got {value}"))
 
         try:
-
             return self._success(datetime.strptime(value, "%H:%M:%S").time())
         except ValueError:
             return self._failure(
                 ValidationError(
                     f"Expected date in format YYYY-MM-DD, but {value} is not a valid value"
                 )
             )
```

### Comparing `json_codec-0.1.4/json_codec/codecs/tuple_codec.py` & `json_codec-0.1.5/json_codec/codecs/tuple_codec.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.4/json_codec/codecs/union_codec.py` & `json_codec-0.1.5/json_codec/codecs/union_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Generator, Tuple, Type, TypeVar
+from typing import Any, Generator, Type, TypeVar
 
 from json_codec.types import (
     ParseProcessResult,
     ParseProcessYield,
     TypeDecoder,
     ValidationError,
 )
```

### Comparing `json_codec-0.1.4/json_codec/json_codec.py` & `json_codec-0.1.5/json_codec/json_codec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,87 @@
-from dataclasses import MISSING, asdict, is_dataclass
+from dataclasses import MISSING, asdict, dataclass, is_dataclass
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Callable, Dict, List, Tuple, TypeVar, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 from uuid import UUID
 
-from typing_extensions import Type
-from json_codec.codecs.date_codec import DateTypeDecoder, serialize_date
+from json_codec.codecs.date_codec import (
+    DateTypeDecoder,
+    serialize_date,
+)
 from json_codec.codecs.datetime_codec import (
     DateTimeTypeDecoder,
     serialize_datetime,
 )
-
 from json_codec.codecs.dict_codec import DictTypeDecoder
-from json_codec.codecs.list_codec import ListTypeDecoder as ListTypeParser
-from json_codec.codecs.primitive_codec import (
-    PrimitiveTypeDecoder,
+from json_codec.codecs.list_codec import (
+    ListTypeDecoder as ListTypeParser,
+)
+from json_codec.codecs.primitive_codec import PrimitiveTypeDecoder
+from json_codec.codecs.set_codec import (
+    SetTypeDecoder as SetTypeParser,
 )
-from json_codec.codecs.set_codec import SetTypeDecoder as SetTypeParser
 from json_codec.codecs.time_codec import (
     TimeTypeDecoder as TimeTypeParser,
-    serialize_time,
 )
+from json_codec.codecs.time_codec import serialize_time
 from json_codec.codecs.tuple_codec import (
     TupleTypeDecoder as TupleTypeParser,
 )
 from json_codec.codecs.union_codec import (
     UnionTypeDecoder as UnionTypeParser,
 )
 from json_codec.types import (
     AssumeDataclass,
     AssumeGeneric,
     AssumeNewType,
     ParseProcessResult,
     TypeDecoder,
     ValidationError,
-    ValidationErrorBase,
 )
+from json_codec.utils import is_generic
 
 T = TypeVar("T")
 
 typers_parsers: Dict[Any, TypeDecoder[Any]] = {
-    Decimal: PrimitiveTypeDecoder(Decimal),
-    str: PrimitiveTypeDecoder(str),
-    int: PrimitiveTypeDecoder(int),
-    float: PrimitiveTypeDecoder(float),
-    bool: PrimitiveTypeDecoder(bool),
+    Decimal: PrimitiveTypeDecoder(Decimal, "Decimal"),
+    str: PrimitiveTypeDecoder(str, "string"),
+    int: PrimitiveTypeDecoder(int, "int"),
+    float: PrimitiveTypeDecoder(float, "float"),
+    bool: PrimitiveTypeDecoder(bool, "bool"),
     dict: DictTypeDecoder(),
     list: ListTypeParser(),
     tuple: TupleTypeParser(),
     set: SetTypeParser(),
-    UUID: PrimitiveTypeDecoder(UUID),
+    UUID: PrimitiveTypeDecoder(UUID, "UUID"),
     Union: UnionTypeParser(),
-    Any: PrimitiveTypeDecoder(lambda x: x),
+    Any: PrimitiveTypeDecoder(lambda x: x, "Any"),
     date: DateTypeDecoder(),
     datetime: DateTimeTypeDecoder(),
     time: TimeTypeParser(),
-    type(None): PrimitiveTypeDecoder(lambda x: None),
+    type(None): PrimitiveTypeDecoder(lambda x: None, "null"),
 }
 
 
-def is_generic(type_: Type[Any]) -> bool:
-    return (
-        hasattr(type_, "__origin__")
-        and cast(AssumeGeneric, type_).__origin__ is not None
-    )
-
-
-class LocatedValidationError(Exception):
-    def __init__(self, message: str, json_path: str) -> None:
-        super().__init__(message)
-        self.json_path = json_path
+@dataclass
+class LocatedValidationError:
+    message: str
+    json_path: str
 
 
 class LocatedValidationErrorCollection(Exception):
     def __init__(self, errors: List[LocatedValidationError]) -> None:
         super().__init__("Located validation errors: %s" % errors)
         self.errors = errors
 
@@ -97,25 +104,31 @@
     return hasattr(type_, "__supertype__")
 
 
 def get_new_type_supertype(type_: Type[Any]) -> Type[Any]:
     return cast(AssumeNewType, type_).__supertype__
 
 
+def is_typing_unmappable(type_: Type[Any]) -> bool:
+    return type_ is Any or type_ is type(None)
+
+
 def __parse_value(
     value: Any,
     type_: Type[T],
     json_path: str = "$",
     located_errors: List[LocatedValidationError] = [],
     skip_raise: bool = False,
 ) -> ParseProcessResult[T]:
     real_type = type_
     target_type = type_
     type_args: Tuple[Type[Any], ...] = ()
-    if is_generic(type_):
+    if is_typing_unmappable(type_):
+        ...
+    elif is_generic(type_):
         real_type = cast(AssumeGeneric, type_).__origin__
         target_type = real_type
         type_args = cast(AssumeGeneric, type_).__args__
     elif is_new_type(type_):
         target_type = get_new_type_supertype(type_)
     elif not is_dataclass(type_) and not issubclass(real_type, Enum):
         target_type = __get_recursive_mapped_type(type_)
@@ -131,45 +144,48 @@
                     parsed_yield.type_,
                     "{}{}".format(json_path, parsed_yield.json_path),
                     located_errors,
                     parsed_yield.skip_raise,
                 )
                 parsed_yield = parser_generator.send(parsed_value)
         except StopIteration as e:
-
             final = e.value
             if not isinstance(final, ParseProcessResult):
                 raise ValueError(f"Parser {parser} did not return a ParseProcessResult")
             if isinstance(final.result, Exception) and not skip_raise:
                 located_errors.append(
                     LocatedValidationError(
                         message=str(final.result),
                         json_path=json_path,
                     )
                 )
 
             if target_type != real_type:
-                final = ParseProcessResult(
-                    result=cast(Type[Any], real_type)(final.result),
-                )
+                if not isinstance(final.result, Exception):
+                    final = ParseProcessResult(
+                        result=cast(Type[Any], real_type)(final.result),
+                    )
+                else:
+                    final = ParseProcessResult(
+                        result=None,
+                    )
 
             return cast(ParseProcessResult[T], final)
 
     elif is_dataclass(real_type):
         try:
             return ParseProcessResult(
                 __parse_dataclass(
                     value,
                     real_type,
                     json_path,
                     located_errors,
                 )
             )
         except AssertionError as e:
-
             error = ValidationError(
                 str(e),
             )
             if not skip_raise:
                 located_errors.append(
                     LocatedValidationError(
                         message=str(error),
@@ -177,15 +193,15 @@
                     )
                 )
             return ParseProcessResult(error)
     elif issubclass(real_type, Enum):
         try:
             value = real_type(value)
             return ParseProcessResult(value)
-        except ValueError as e:
+        except ValueError:
             error = ValidationError(
                 "Invalid enum value for {}: {} | valid types: {}".format(
                     real_type,
                     value,
                     ", ".join(k for k, v in real_type.__members__.items()),
                 )
             )
@@ -213,15 +229,14 @@
     assert is_dataclass(type_), "Type must be a dataclass"
 
     fields = cast(AssumeDataclass, type_).__dataclass_fields__
 
     kwargs: Dict[str, Any] = {}
 
     for field_name, field in fields.items():
-
         field_json_path = "{}.{}".format(json_path, field_name)
 
         if field_name not in value:
             if field.default is not None and field.default is not MISSING:
                 kwargs[field_name] = field.default
             elif field.default_factory is not None and field.default_factory is not MISSING:  # type: ignore
                 kwargs[field_name] = field.default_factory()  # type: ignore
@@ -243,36 +258,30 @@
         )
 
         kwargs[field_name] = parsed_value.result
 
     return cast(Callable[..., T], type_)(**kwargs)
 
 
-def get_class_or_type_name(type_: Type[Any]) -> str:
-    if is_generic(type_):
-        return cast(AssumeGeneric, type_).__repr__()
-
-    if is_dataclass(type_):
-        return type_.__name__
-
-    return type_.__qualname__
-
-
 def decode(value: Any, type_: Type[T]) -> T:
     errors: List[LocatedValidationError] = []
     parsed_value = __parse_value(value, type_, located_errors=errors)
     if len(errors):
         raise LocatedValidationErrorCollection(errors)
 
     if isinstance(parsed_value.result, Exception):
         raise parsed_value.result
 
     return parsed_value.result
 
 
+def optional(T: Type[T]) -> Type[T]:
+    return Optional[T]  # type: ignore
+
+
 def __encode(value: Any) -> Any:
     if isinstance(value, Enum):
         return value.value
     if isinstance(value, datetime):
         return serialize_datetime(value)
     if isinstance(value, date):
         return serialize_date(value)
```

### Comparing `json_codec-0.1.4/json_codec/test_json_codec.py` & `json_codec-0.1.5/json_codec/test_json_codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from datetime import date, datetime, time, timezone
-from enum import Enum
 import json
 from dataclasses import dataclass
+from datetime import date, datetime, time, timezone
 from decimal import Decimal
-from this import d
+from enum import Enum
 from typing import Dict, List, NewType, Optional, Union
 
 import pytest
 
 from json_codec.json_codec import (
     LocatedValidationErrorCollection,
-    get_class_or_type_name,
     decode,
+    optional,
 )
+from json_codec.utils import get_class_or_type_name
 
 
 class TestJsonDeserializerCodec:
     def test_decode_primitives(self) -> None:
         assert decode(json.loads("true"), bool) is True
         assert decode(json.loads("false"), bool) is False
-        assert decode(json.loads("null"), Optional[bool]) is None
+        assert decode(json.loads("null"), optional(bool)) is None
         assert decode(json.loads("1"), int) == 1
         assert decode(json.loads("1"), Decimal) == Decimal("1")
         assert decode(json.loads('"1.1"'), Decimal) == Decimal("1.1")
         assert decode(json.loads('"1.1"'), float) == 1.1
         assert decode(json.loads('"1.1"'), str) == "1.1"
-        
-        assert decode(json.loads('[1,1]'), List[int]) == [1, 1]
 
+        assert decode(json.loads("[1,1]"), List[int]) == [1, 1]
 
     def test_frozen_dataclass(self) -> None:
         @dataclass(frozen=True)
         class User:
             name: str
             age: int
 
@@ -110,15 +109,14 @@
         assert parsed.text_dict["c"] == Decimal("3.3")
         assert parsed.text_dict["d"].quantize(Decimal("1.0")) == Decimal("2.2")
         assert parsed.nested.text == "hello"
         assert parsed.nested.number.quantize(Decimal("1.0")) == Decimal("1.1")
         assert parsed.nested.boolean is True
 
     def test_raise_when_type_not_mapped(self) -> None:
-
         with pytest.raises(ValueError):
 
             class NonMappedDummy:
                 pass
 
             @dataclass
             class Dummy:
@@ -133,15 +131,14 @@
             """
 
             dummy_json = json.loads(dummy_json_text)
 
             decode(dummy_json, Dummy)
 
     def test_raise_when_missing_field(self) -> None:
-
         with pytest.raises(LocatedValidationErrorCollection):
 
             @dataclass
             class Dummy:
                 text: int
 
             dummy_json_text = """
@@ -167,15 +164,14 @@
             NormalClass
         ) == "{cls_name}.{method_name}.<locals>.NormalClass".format(
             cls_name=TestJsonDeserializerCodec.__name__,
             method_name=TestJsonDeserializerCodec.test_get_class_or_type_name.__name__,
         )
 
     def test_type_not_in_union(self) -> None:
-
         with pytest.raises(LocatedValidationErrorCollection):
 
             @dataclass
             class Dummy:
                 text: Union[List[str], Dict[str, str]]
 
             dummy_json_text = """
@@ -186,15 +182,14 @@
             """
 
             dummy_json = json.loads(dummy_json_text)
 
             decode(dummy_json, Dummy)
 
     def test_dict_with_wrong_type(self) -> None:
-
         with pytest.raises(LocatedValidationErrorCollection) as e:
 
             @dataclass
             class Dummy:
                 text: Dict[int, int]
 
             dummy_json_text = """
@@ -204,15 +199,15 @@
                 }
             }
 
             """
 
             dummy_json = json.loads(dummy_json_text)
 
-            a = decode(dummy_json, Dummy)
+            decode(dummy_json, Dummy)
 
         assert e.value is not None
 
     def test_enum(self) -> None:
         class MyEnum(Enum):
             A = "A"
             B = "B"
@@ -231,15 +226,14 @@
         dummy_json = json.loads(dummy_json_text)
 
         a = decode(dummy_json, Dummy)
 
         assert a.my_enum == MyEnum.A
 
     def test_enum_with_wrong_value(self) -> None:
-
         with pytest.raises(LocatedValidationErrorCollection):
 
             class MyEnum(Enum):
                 A = "A"
                 B = "B"
 
             @dataclass
@@ -251,15 +245,15 @@
                 "my_enum": "C"
             }
 
             """
 
             dummy_json = json.loads(dummy_json_text)
 
-            a = decode(dummy_json, Dummy)
+            decode(dummy_json, Dummy)
 
     def test_date(self) -> None:
         @dataclass
         class Dummy:
             date_time: datetime
             date_: date
             time_: time
@@ -278,31 +272,31 @@
         a = decode(dummy_json, Dummy)
 
         assert a.date_ == date(2020, 1, 1)
         assert a.date_time == datetime(2020, 1, 1, 0, 0, 0, tzinfo=timezone.utc)
         assert a.time_ == time(0, 0, 0)
 
     def test_date_with_wrong_value(self) -> None:
-            
-            with pytest.raises(LocatedValidationErrorCollection):
-    
-                @dataclass
-                class Dummy:
-                    date_time: datetime
-    
-                dummy_json_text = """
+        with pytest.raises(LocatedValidationErrorCollection):
+
+            @dataclass
+            class Dummy:
+                date_time: datetime
+
+            dummy_json_text = """
                 {
                     "date_time": "2020-01-01T00:00:00"
                 }
     
                 """
-    
-                dummy_json = json.loads(dummy_json_text)
-    
-                a = decode(dummy_json, Dummy)
+
+            dummy_json = json.loads(dummy_json_text)
+
+            decode(dummy_json, Dummy)
+
     def test_primitive_class_inheritance(self) -> None:
         class MyInt(int):
             pass
 
         @dataclass
         class Dummy:
             my_int: MyInt
@@ -332,21 +326,18 @@
         {
             "my_int": "1"
         }
 
         """
 
         dummy_json = json.loads(dummy_json_text)
-        
+
         parsed = decode(dummy_json, Dummy)
 
         assert parsed.my_int == MyInt(1)
         assert isinstance(parsed.my_int, MyInt)
-        
-
-        
-    def test_decode_newtype(self):
 
+    def test_decode_newtype(self) -> None:
         UserId = NewType("UserId", int)
 
         assert decode(json.loads("1"), UserId) == UserId(1)
-        assert isinstance(decode(json.loads("1"), UserId), int)
+        assert isinstance(decode(json.loads("1"), UserId), int)
```

### Comparing `json_codec-0.1.4/json_codec/types.py` & `json_codec-0.1.5/json_codec/types.py`

 * *Files identical despite different names*

### Comparing `json_codec-0.1.4/setup.py` & `json_codec-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['json_codec', 'json_codec.codecs']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'json-codec',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': '# Json Codec\n\nIt\'s a simple library to encode and decode json to strict python types using dataclasses and builtin python types.\n\n## Installation\n\n```bash\npip install json-codec\n\npoetry add json-codec\n```\n\n## Usage\n\n### Parse a simple primitive type\n\n```python\nfrom json_codec import decode\nimport json\n\nassert decode(json.loads("true"), bool) is True\nassert decode(json.loads("false"), bool) is False\nassert decode(json.loads("null"), Optional[bool]) is None\nassert decode(json.loads("1"), int) == 1\nassert decode(json.loads("1"), Decimal) == Decimal("1")\nassert decode(json.loads(\'"1.1"\'), Decimal) == Decimal("1.1")\nassert decode(json.loads(\'"1.1"\'), float) == 1.1\nassert decode(json.loads(\'"1.1"\'), str) == "1.1"\n\nassert decode(json.loads(\'[1,1]\'), List[int]) == [1, 1]\n```\n\n### Parse a dataclass\n\n```python\nfrom dataclasses import dataclass\nfrom json_codec import decode\nimport json\n\n@dataclass(frozen=True)\nclass User:\n    name: str\n    age: int\n\nassert decode({"name": "John", "age": 30}, User) == User(name="John", age=30)\n\n\n@dataclass\nclass Dummy:\n    text_list: List[str]\n    text_dict: Dict[str, Decimal]\n    optional_text: Optional[str]\n\ndummy_json_text = """\n{\n    "text_list": ["a", "b", "c"],\n    "text_dict": {\n        "a": 1.0,\n        "b": 2,\n        "c": "3.3",\n        "d": 2.2\n    },\n    "optional_text": "hello"\n}\n"""\n\ndummy_json = json.loads(dummy_json_text)\n\nparsed = decode(dummy_json, Dummy)\n\nassert parsed.text_list == ["a", "b", "c"]\nassert parsed.text_dict["a"] == Decimal("1.0")\nassert parsed.text_dict["b"] == Decimal("2.0")\nassert parsed.text_dict["c"] == Decimal("3.3")\nassert parsed.text_dict["d"].quantize(Decimal("1.0")) == Decimal("2.2")\nassert parsed.optional_text == "hello"\n```\n\n### Parse a dataclass with a nested dataclass\n\n```python\nfrom dataclasses import dataclass\nfrom json_codec import decode\nimport json\n\n @dataclass\nclass NestedDummy:\n    text: str\n    number: Decimal\n\n    boolean: bool\n\n@dataclass\nclass Dummy:\n    text_list: List[str]\n    text_dict: Dict[str, Decimal]\n    nested: NestedDummy\n\ndummy_json_text = """\n{\n\n    "text_list": ["a", "b", "c"],\n    "text_dict": {\n        "a": 1.0,\n        "b": 2,\n        "c": "3.3",\n        "d": 2.2\n    },\n    "nested": {\n        "text": "hello",\n        "number": 1.1,\n        "boolean": true\n    }\n}\n"""\n\ndummy_json = json.loads(dummy_json_text)\n\nparsed = decode(dummy_json, Dummy)\n\nassert parsed.text_list == ["a", "b", "c"]\nassert parsed.text_dict["a"] == Decimal("1.0")\nassert parsed.text_dict["b"] == Decimal("2.0")\nassert parsed.text_dict["c"] == Decimal("3.3")\nassert parsed.text_dict["d"].quantize(Decimal("1.0")) == Decimal("2.2")\nassert parsed.nested.text == "hello"\nassert parsed.nested.number.quantize(Decimal("1.0")) == Decimal("1.1")\nassert parsed.nested.boolean is True\n```\n\n### Parse a newtype\n\n```python\nfrom json_codec import decode\nfrom typing import NewType\nimport json\n\nUserId = NewType("UserId", int)\n\nassert decode(json.loads("1"), UserId) == UserId(1)\nassert isinstance(decode(json.loads("1"), UserId), int)\n\n```',
     'author': 'Lucas Silva',
     'author_email': 'lucas76leonardo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/LuscasLeo/json_codec',
```

### Comparing `json_codec-0.1.4/PKG-INFO` & `json_codec-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-codec
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/LuscasLeo/json_codec
 Author: Lucas Silva
 Author-email: lucas76leonardo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

