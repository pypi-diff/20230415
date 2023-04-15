# Comparing `tmp/traducteur-0.4.5.tar.gz` & `tmp/traducteur-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traducteur-0.4.5.tar", max compression
+gzip compressed data, was "traducteur-0.4.6.tar", max compression
```

## Comparing `traducteur-0.4.5.tar` & `traducteur-0.4.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-04-11 20:42:57.015424 traducteur-0.4.5/LICENSE
--rw-r--r--   0        0        0     3588 2023-04-11 20:42:57.015424 traducteur-0.4.5/README.md
--rw-r--r--   0        0        0      756 2023-04-11 20:42:57.015424 traducteur-0.4.5/pyproject.toml
--rw-r--r--   0        0        0       37 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/__init__.py
--rw-r--r--   0        0        0      253 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/base.py
--rw-r--r--   0        0        0      606 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/mongo.py
--rw-r--r--   0        0        0      523 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/sqlite.py
--rw-r--r--   0        0        0       71 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/exceptions/tasks/__init__.py
--rw-r--r--   0        0        0       40 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/exceptions/tasks/base.py
--rw-r--r--   0        0        0       46 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/exceptions/tasks/worker.py
--rw-r--r--   0        0        0       34 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/__init__.py
--rw-r--r--   0        0        0      189 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/base.py
--rw-r--r--   0        0        0      264 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/base.py
--rw-r--r--   0        0        0      164 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/__init__.py
--rw-r--r--   0        0        0       73 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/base.py
--rw-r--r--   0        0        0      204 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/datetime_filter.py
--rw-r--r--   0        0        0      133 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/exists_filter.py
--rw-r--r--   0        0        0      189 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/number_filter.py
--rw-r--r--   0        0        0      229 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/string_filter.py
--rw-r--r--   0        0        0     3041 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/mongo.py
--rw-r--r--   0        0        0       33 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/query/__init__.py
--rw-r--r--   0        0        0     3798 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/query/sql.py
--rw-r--r--   0        0        0     2136 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/sql.py
--rw-r--r--   0        0        0       68 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/base/__init__.py
--rw-r--r--   0        0        0      805 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/base/base.py
--rw-r--r--   0        0        0      731 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/base/database.py
--rw-r--r--   0        0        0     2942 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/document/mongo.py
--rw-r--r--   0        0        0      676 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/document/redis.py
--rw-r--r--   0        0        0     2495 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/relational/sql.py
--rw-r--r--   0        0        0       27 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/base.py
--rw-r--r--   0        0        0      548 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/lifetime.py
--rw-r--r--   0        0        0      130 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/status.py
--rw-r--r--   0        0        0       28 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/task/__init__.py
--rw-r--r--   0        0        0     1991 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/task/redis.py
--rw-r--r--   0        0        0      103 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/worker/base.py
--rw-r--r--   0        0        0     1138 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/worker/redis.py
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-15 10:09:31.889888 traducteur-0.4.6/LICENSE
+-rw-r--r--   0        0        0     3588 2023-04-15 10:09:31.889888 traducteur-0.4.6/README.md
+-rw-r--r--   0        0        0      756 2023-04-15 10:09:31.889888 traducteur-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/base.py
+-rw-r--r--   0        0        0      606 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/mongo.py
+-rw-r--r--   0        0        0      523 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/sqlite.py
+-rw-r--r--   0        0        0       71 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/exceptions/tasks/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/exceptions/tasks/base.py
+-rw-r--r--   0        0        0       46 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/exceptions/tasks/worker.py
+-rw-r--r--   0        0        0       34 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/base.py
+-rw-r--r--   0        0        0      264 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/base.py
+-rw-r--r--   0        0        0      206 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/base.py
+-rw-r--r--   0        0        0      133 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/boolean_filter.py
+-rw-r--r--   0        0        0      204 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/datetime_filter.py
+-rw-r--r--   0        0        0      133 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/exists_filter.py
+-rw-r--r--   0        0        0      189 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/number_filter.py
+-rw-r--r--   0        0        0      229 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/string_filter.py
+-rw-r--r--   0        0        0     3041 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/mongo.py
+-rw-r--r--   0        0        0       33 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/query/__init__.py
+-rw-r--r--   0        0        0     6040 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/query/sql.py
+-rw-r--r--   0        0        0     2410 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/sql.py
+-rw-r--r--   0        0        0       68 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/models/base/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/models/base/base.py
+-rw-r--r--   0        0        0      731 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/base/database.py
+-rw-r--r--   0        0        0     2942 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/document/mongo.py
+-rw-r--r--   0        0        0      676 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/document/redis.py
+-rw-r--r--   0        0        0     2572 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/relational/sql.py
+-rw-r--r--   0        0        0       27 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/base.py
+-rw-r--r--   0        0        0      548 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/lifetime.py
+-rw-r--r--   0        0        0      130 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/status.py
+-rw-r--r--   0        0        0       28 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/task/__init__.py
+-rw-r--r--   0        0        0     1991 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/task/redis.py
+-rw-r--r--   0        0        0      103 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/worker/base.py
+-rw-r--r--   0        0        0     1138 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/worker/redis.py
+-rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.6/PKG-INFO
```

### Comparing `traducteur-0.4.5/LICENSE` & `traducteur-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/README.md` & `traducteur-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/pyproject.toml` & `traducteur-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "traducteur"
-version = "0.4.5"
+version = "0.4.6"
 description = "Traducteur is the middle man to handle your basic data needs."
 authors = ["Seppe De Langhe <seppedelanghe@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.4"
```

### Comparing `traducteur-0.4.5/traducteur/context/mongo.py` & `traducteur-0.4.6/traducteur/context/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/context/sqlite.py` & `traducteur-0.4.6/traducteur/context/sqlite.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/managers/mongo.py` & `traducteur-0.4.6/traducteur/managers/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/managers/query/sql.py` & `traducteur-0.4.6/traducteur/managers/query/sql.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import Sequence, Any, Optional
+from typing import Sequence, Any, Optional, Union
 
-from sqlalchemy.orm import Session
 from sqlalchemy import Column
+from sqlalchemy.orm import Session
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 
 from ..filters.base import BaseFilter
-from ..filters.types import StringFilter, DatetimeFilter, NumberFilter, ExistsFilter
+from ..filters.types import StringFilter, DatetimeFilter, NumberFilter, ExistsFilter, BooleanFilter
 from ..filters.types.base import BaseTypeFilter
 
 
 class QueryBuilderException(Exception):
     pass
 
 
 class SQLQueryBuilder:
     def __init__(self, session: Session, cls):
         self.session = session
         self.cls = cls
+        self.joined = []
 
         self.query = self.session.query(self.cls)
 
     def _add_string(self, str_filter: StringFilter, col: Column):
         if str_filter.exact:
             self.query = self.query.filter(col == str_filter.exact)
             return  # no more need for other filters
@@ -49,60 +50,101 @@
         if number_filter.gt:
             self.query = self.query.filter(col > number_filter.gt)
 
         if number_filter.lt:
             self.query = self.query.filter(col < number_filter.lt)
 
     def _add_exists(self, exists_filter: ExistsFilter, col: Column):
-        pass
+        if isinstance(exists_filter.exists, bool):
+            self.query = self.query.filter(col != None) if exists_filter.exists else self.query.filter(col == None)
+            self.query = self.query.filter(col != "") if exists_filter.exists else self.query.filter(col == "")
+
+    def __add_bool(self, boolean_filter: BooleanFilter, col: Column):
+        if isinstance(boolean_filter.value, bool):
+            self.query = self.query.filter(col == boolean_filter.value)
 
-    def add(self, filter_cls: BaseTypeFilter, col: str):
+    def add(self, filter_cls: BaseTypeFilter, col: str, join_cls=None):
         try:
-            prop: Column = getattr(self.cls, col)
-            if not isinstance(prop, InstrumentedAttribute):
-                raise Exception()
-        except Exception:
-            raise QueryBuilderException(f"{self.cls} has no column {col}!")
+            if join_cls is not None:
+                prop: Column = getattr(join_cls, col)
+                if not isinstance(prop, InstrumentedAttribute):
+                    raise Exception()
+                if join_cls.classname not in self.joined:
+                    self.query = self.query.join(join_cls)
+                    self.joined.append(join_cls.classname)
+            else:
+                prop: Column = getattr(self.cls, col)
+                if not isinstance(prop, InstrumentedAttribute):
+                    raise Exception()
+        except Exception as e:
+            raise QueryBuilderException(f"{join_cls} has no column {col}!" if join_cls is not None else f"{self.cls} has no column {col}!")
 
         if isinstance(filter_cls, StringFilter):
             self._add_string(filter_cls, prop)
         elif isinstance(filter_cls, DatetimeFilter):
             self._add_datetime(filter_cls, prop)
         elif isinstance(filter_cls, NumberFilter):
             self._add_number(filter_cls, prop)
         elif isinstance(filter_cls, ExistsFilter):
             self._add_exists(filter_cls, prop)
+        elif isinstance(filter_cls, BooleanFilter):
+            self.__add_bool(filter_cls, prop)
         else:
             raise QueryBuilderException(f"Invalid filter provided: {type(filter_cls)}!")
 
         return self
 
     def add_multiple(self, filters: Sequence[BaseTypeFilter], columns: Sequence[str]):
         if len(filters) != len(columns):
             raise QueryBuilderException(f"Inconsistent lengths between filters and columns: {len(filters)} != {len(columns)}!")
 
         for f, c in zip(filters, columns):
             self.add(f, c)
 
         return self
 
-    def build(self, **kwargs):
-        if 'filter' in kwargs:
-            f: BaseFilter = kwargs.get('filter')
-            if f is None:
-                raise QueryBuilderException(f"Query filter is set but is None!")
-
-            for col, type_filter in f.for_query().items():
-                if type_filter is None:
+    def _apply_sort(self, **kwargs):
+        sort_by = kwargs.get('sort', None)
+        if isinstance(sort_by, str):
+            desc = kwargs.get('desc', False)
+            self.query = self.query.order_by(getattr(self.cls, sort_by)) if not desc else self.query.order_by(getattr(self.cls, sort_by).desc())
+
+    def _apply_filters(self, **kwargs):
+        filters = kwargs.get('filters', None)
+        if isinstance(filters, list):
+            for fil in filters:
+                if isinstance(fil, tuple) or isinstance(fil, list):
+                    join_cls, f = fil
+                    if not isinstance(f, BaseFilter):
+                        raise QueryBuilderException(f"Query filter is set but is of invalid type!")
+
+                    for col, type_filter in f.for_query().items():
+                        if type_filter is None:
+                            continue
+                        self.add(type_filter, col, join_cls)
+
+                elif isinstance(fil, BaseFilter):
+                    for col, type_filter in fil.for_query().items():
+                        if type_filter is None:
+                            continue
+                        self.add(type_filter, col)
+                elif fil is None:
                     continue
-                self.add(type_filter, col)
+                else:
+                    raise QueryBuilderException('Invalid filter provided!')
 
+    def build(self, **kwargs):
+        self._apply_filters(**kwargs)
+        self._apply_sort(**kwargs)
         return self
 
     def all(self) -> Sequence[Sequence[Any]]:
         return self.query.all()
 
     def paginate(self, page: int, per_page: int = 30) -> Sequence[Sequence[Any]]:
-        return self.query.limit(per_page).offset((page - 1) * per_page).all()
+        return self.query.limit(per_page).offset(page * per_page).all()
 
     def first(self) -> Optional[Sequence[Any]]:
         return self.query.first()
+
+    def get(self, id: Union[int, str]) -> Optional[Any]:
+        return self.query.get(id)
```

### Comparing `traducteur-0.4.5/traducteur/managers/sql.py` & `traducteur-0.4.6/traducteur/managers/sql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+import json
+
 from typing import List, TypeVar, Optional, Generic, Union, Iterable
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
 from sqlalchemy.sql import exists
 
 from .query import SQLQueryBuilder
 
 T = TypeVar("T")
 
 
 class SQLModelManager(Generic[T]):
-    def __init__(self, connection_string):
+    def __init__(self, connection_string, connect_args: Optional[str] = None):
         self.connection_string = connection_string
+        self.connect_args = json.loads(connect_args) if connect_args else None
 
     @property
     def engine(self):
+        if self.connect_args:
+            return create_engine(self.connection_string, connect_args=self.connect_args, echo=False, future=False)
+
         return create_engine(self.connection_string, echo=False, future=False)
 
     def session(self) -> Session:
         return Session(self.engine)
 
     def insert(self, item: T) -> T:
         with self.session() as session:
```

### Comparing `traducteur-0.4.5/traducteur/models/base/database.py` & `traducteur-0.4.6/traducteur/models/base/database.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/models/document/mongo.py` & `traducteur-0.4.6/traducteur/models/document/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/models/document/redis.py` & `traducteur-0.4.6/traducteur/models/document/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/models/relational/sql.py` & `traducteur-0.4.6/traducteur/models/relational/sql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 
 from uuid import uuid4
 from datetime import datetime
-from typing import TypeVar, List
+from pydantic import BaseModel
+from typing import TypeVar, List, Type
 
 from sqlalchemy.orm import declarative_base
 from sqlalchemy import String, Column, DATETIME
 
 from ..base import BaseDatabaseModel
 from ...managers.sql import SQLModelManager
 
@@ -41,16 +42,16 @@
             self.created_at = datetime.utcnow()
             self.updated_at = datetime.utcnow()
             return self.manager().insert(self)
 
     def delete(self):
         return self.manager().delete(self)
 
-    def map_to(self, cls: 'BaseSQLModel'):
-        return cls.from_dict(self.dict())
+    def map_to(self, cls: Type[BaseModel]):
+        return cls(**self.dict())
 
     def dict(self):
         return self.__dict__
 
     """
         Properties
     """
@@ -87,11 +88,11 @@
 
     @classmethod
     def exists(cls, id: str) -> bool:
         return cls.manager().exists(cls, id)
 
     @classmethod
     def manager(cls) -> SQLModelManager:
-        return SQLModelManager[cls](os.environ.get('SQL_CONNECTION_STRING'))
+        return SQLModelManager[cls](os.environ.get('SQL_CONNECTION_STRING'), os.environ.get('SQL_CONNECTION_PARAMS', None))
 
 
 SQLBase = declarative_base(cls=BaseSQLModel)
```

### Comparing `traducteur-0.4.5/traducteur/tasks/base/base.py` & `traducteur-0.4.6/traducteur/tasks/base/base.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/tasks/base/lifetime.py` & `traducteur-0.4.6/traducteur/tasks/base/lifetime.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/tasks/task/redis.py` & `traducteur-0.4.6/traducteur/tasks/task/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/traducteur/tasks/worker/redis.py` & `traducteur-0.4.6/traducteur/tasks/worker/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.5/PKG-INFO` & `traducteur-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traducteur
-Version: 0.4.5
+Version: 0.4.6
 Summary: Traducteur is the middle man to handle your basic data needs.
 Author: Seppe De Langhe
 Author-email: seppedelanghe@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

