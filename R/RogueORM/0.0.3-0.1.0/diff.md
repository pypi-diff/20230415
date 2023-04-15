# Comparing `tmp/RogueORM-0.0.3.tar.gz` & `tmp/RogueORM-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RogueORM-0.0.3.tar", last modified: Mon Apr 10 23:21:59 2023, max compression
+gzip compressed data, was "RogueORM-0.1.0.tar", last modified: Sat Apr 15 18:18:56 2023, max compression
```

## Comparing `RogueORM-0.0.3.tar` & `RogueORM-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.557810 RogueORM-0.0.3/
--rw-rw-rw-   0        0        0     1093 2022-12-06 23:54:36.000000 RogueORM-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3853 2023-04-10 23:21:59.557810 RogueORM-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2071 2023-04-10 23:07:27.000000 RogueORM-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.537101 RogueORM-0.0.3/RogueORM.egg-info/
--rw-rw-rw-   0        0        0     3853 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      752 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1212 2023-04-10 23:21:29.000000 RogueORM-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.539062 RogueORM-0.0.3/rogue/
--rw-rw-rw-   0        0        0        0 2022-12-07 00:00:53.000000 RogueORM-0.0.3/rogue/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.541991 RogueORM-0.0.3/rogue/backends/
--rw-rw-rw-   0        0        0        0 2022-12-09 00:39:38.000000 RogueORM-0.0.3/rogue/backends/__init__.py
--rw-rw-rw-   0        0        0     4665 2023-04-10 23:21:08.000000 RogueORM-0.0.3/rogue/backends/base.py
--rw-rw-rw-   0        0        0      155 2022-12-21 23:27:34.000000 RogueORM-0.0.3/rogue/backends/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.545971 RogueORM-0.0.3/rogue/backends/sqlite/
--rw-rw-rw-   0        0        0        0 2022-12-09 00:40:15.000000 RogueORM-0.0.3/rogue/backends/sqlite/__init__.py
--rw-rw-rw-   0        0        0      640 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/backends/sqlite/client.py
--rw-rw-rw-   0        0        0     2704 2023-01-05 21:20:18.000000 RogueORM-0.0.3/rogue/backends/sqlite/query.py
--rw-rw-rw-   0        0        0     4277 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/backends/sqlite/schema.py
--rw-rw-rw-   0        0        0       45 2022-12-21 18:46:55.000000 RogueORM-0.0.3/rogue/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.547925 RogueORM-0.0.3/rogue/managers/
--rw-rw-rw-   0        0        0      128 2023-01-05 21:19:29.000000 RogueORM-0.0.3/rogue/managers/__init__.py
--rw-rw-rw-   0        0        0     5853 2023-01-05 21:20:21.000000 RogueORM-0.0.3/rogue/managers/base.py
--rw-rw-rw-   0        0        0      152 2022-12-21 18:47:09.000000 RogueORM-0.0.3/rogue/managers/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.550855 RogueORM-0.0.3/rogue/migrations/
--rw-rw-rw-   0        0        0       86 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/migrations/__init__.py
--rw-rw-rw-   0        0        0     4450 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/migrations/base.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.554873 RogueORM-0.0.3/rogue/models/
--rw-rw-rw-   0        0        0       84 2022-12-18 20:54:58.000000 RogueORM-0.0.3/rogue/models/__init__.py
--rw-rw-rw-   0        0        0     7583 2023-04-10 19:23:26.000000 RogueORM-0.0.3/rogue/models/base.py
--rw-rw-rw-   0        0        0      332 2022-12-21 23:59:31.000000 RogueORM-0.0.3/rogue/models/errors.py
--rw-rw-rw-   0        0        0     8001 2023-04-10 19:33:23.000000 RogueORM-0.0.3/rogue/models/fields.py
--rw-rw-rw-   0        0        0     1920 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/models/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.556832 RogueORM-0.0.3/rogue/settings/
--rw-rw-rw-   0        0        0     1117 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/settings/__init__.py
--rw-rw-rw-   0        0        0       90 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/settings/default_settings.py
--rw-rw-rw-   0        0        0       42 2023-04-10 23:21:59.558789 RogueORM-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.955515 RogueORM-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2022-12-06 23:54:36.000000 RogueORM-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3863 2023-04-15 18:18:56.955515 RogueORM-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2081 2023-04-15 18:17:17.000000 RogueORM-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.894650 RogueORM-0.1.0/RogueORM.egg-info/
+-rw-rw-rw-   0        0        0     3863 2023-04-15 18:18:56.000000 RogueORM-0.1.0/RogueORM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2023-04-15 18:18:56.000000 RogueORM-0.1.0/RogueORM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:18:56.000000 RogueORM-0.1.0/RogueORM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-15 18:18:56.000000 RogueORM-0.1.0/RogueORM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 18:18:56.000000 RogueORM-0.1.0/RogueORM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1212 2023-04-15 18:18:29.000000 RogueORM-0.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.897580 RogueORM-0.1.0/rogue/
+-rw-rw-rw-   0        0        0        0 2022-12-07 00:00:53.000000 RogueORM-0.1.0/rogue/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-10 23:07:27.000000 RogueORM-0.1.0/rogue/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.904950 RogueORM-0.1.0/rogue/backends/
+-rw-rw-rw-   0        0        0        0 2022-12-09 00:39:38.000000 RogueORM-0.1.0/rogue/backends/__init__.py
+-rw-rw-rw-   0        0        0     5056 2023-04-14 21:28:08.000000 RogueORM-0.1.0/rogue/backends/base.py
+-rw-rw-rw-   0        0        0      155 2022-12-21 23:27:34.000000 RogueORM-0.1.0/rogue/backends/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.918182 RogueORM-0.1.0/rogue/backends/sqlite/
+-rw-rw-rw-   0        0        0        0 2022-12-09 00:40:15.000000 RogueORM-0.1.0/rogue/backends/sqlite/__init__.py
+-rw-rw-rw-   0        0        0      640 2023-04-15 15:58:54.000000 RogueORM-0.1.0/rogue/backends/sqlite/client.py
+-rw-rw-rw-   0        0        0     3642 2023-04-14 22:02:10.000000 RogueORM-0.1.0/rogue/backends/sqlite/query.py
+-rw-rw-rw-   0        0        0     4277 2023-04-10 23:07:27.000000 RogueORM-0.1.0/rogue/backends/sqlite/schema.py
+-rw-rw-rw-   0        0        0       45 2023-04-13 02:15:20.000000 RogueORM-0.1.0/rogue/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.926529 RogueORM-0.1.0/rogue/managers/
+-rw-rw-rw-   0        0        0      128 2023-01-05 21:19:29.000000 RogueORM-0.1.0/rogue/managers/__init__.py
+-rw-rw-rw-   0        0        0     7658 2023-04-15 16:12:36.000000 RogueORM-0.1.0/rogue/managers/base.py
+-rw-rw-rw-   0        0        0      152 2022-12-21 18:47:09.000000 RogueORM-0.1.0/rogue/managers/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.928480 RogueORM-0.1.0/rogue/migrations/
+-rw-rw-rw-   0        0        0       86 2023-04-10 23:07:27.000000 RogueORM-0.1.0/rogue/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4450 2023-04-10 23:07:27.000000 RogueORM-0.1.0/rogue/migrations/base.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.939763 RogueORM-0.1.0/rogue/models/
+-rw-rw-rw-   0        0        0       84 2022-12-18 20:54:58.000000 RogueORM-0.1.0/rogue/models/__init__.py
+-rw-rw-rw-   0        0        0     7944 2023-04-14 21:46:46.000000 RogueORM-0.1.0/rogue/models/base.py
+-rw-rw-rw-   0        0        0      332 2022-12-21 23:59:31.000000 RogueORM-0.1.0/rogue/models/errors.py
+-rw-rw-rw-   0        0        0     8476 2023-04-15 16:10:15.000000 RogueORM-0.1.0/rogue/models/fields.py
+-rw-rw-rw-   0        0        0     1920 2023-04-10 19:11:29.000000 RogueORM-0.1.0/rogue/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.952590 RogueORM-0.1.0/rogue/query/
+-rw-rw-rw-   0        0        0      140 2023-04-15 16:12:15.000000 RogueORM-0.1.0/rogue/query/__init__.py
+-rw-rw-rw-   0        0        0      750 2023-04-15 16:11:52.000000 RogueORM-0.1.0/rogue/query/descriptors.py
+-rw-rw-rw-   0        0        0      239 2023-04-15 16:11:29.000000 RogueORM-0.1.0/rogue/query/query.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:18:56.954538 RogueORM-0.1.0/rogue/settings/
+-rw-rw-rw-   0        0        0     1117 2023-04-10 19:11:29.000000 RogueORM-0.1.0/rogue/settings/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-04-10 19:11:29.000000 RogueORM-0.1.0/rogue/settings/default_settings.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:18:56.955515 RogueORM-0.1.0/setup.cfg
```

### Comparing `RogueORM-0.0.3/LICENSE` & `RogueORM-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.3/PKG-INFO` & `RogueORM-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RogueORM
-Version: 0.0.3
+Version: 0.1.0
 Summary: An ORM that strives to eradicate N+1 issues.
 Author-email: Maxime Toussaint <m.toussaint@mail.com>
 License: MIT License
         
         Copyright (c) 2022 Maxime Toussaint
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,16 @@
 ## Development Roadmap
  1. Define a clear syntax taking advantage of Python 3.10 and later's typing syntax. Status: Done
  2. Define models, managers and fields. Status: Done
  3. Add support for basic SQLite operation: SELECT, INSERT, UPDATE, DELETE. Status: Done
  4. Add support for Foreign Keys. Status: Done
  5. Add support for ManyToMany relationships using a joining table. Status: Done (Testing has to be improved)
  6. Add a migration system. Status: Done (Testing has to be improved)
- 7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Not started
- 8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started
+ 7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Done
+ 8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started (Not a priority)
  9. Add logic for batch fetching in loops. Status: Not started
  10. Add logic for select_related. By design, prefetch_related will never be part of this ORM, preferring a 'fetch in batch when needed' approach. Status: Not started
  11. Look into supporting up to Python 3.7 by taking into account the possible usage of *Union* and *Optional* Maybe import from future? Status: Not started
  12. Improve testing by adding a way to catch queries made to the database, to make sure we lower them as much as possible. Status: Not started
  13. Add support for postgresql. Status: Not started
  14. Look into the next steps for the project. Status: Not started
```

### Comparing `RogueORM-0.0.3/README.md` & `RogueORM-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 ## Development Roadmap
  1. Define a clear syntax taking advantage of Python 3.10 and later's typing syntax. Status: Done
  2. Define models, managers and fields. Status: Done
  3. Add support for basic SQLite operation: SELECT, INSERT, UPDATE, DELETE. Status: Done
  4. Add support for Foreign Keys. Status: Done
  5. Add support for ManyToMany relationships using a joining table. Status: Done (Testing has to be improved)
  6. Add a migration system. Status: Done (Testing has to be improved)
- 7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Not started
- 8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started
+ 7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Done
+ 8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started (Not a priority)
  9. Add logic for batch fetching in loops. Status: Not started
  10. Add logic for select_related. By design, prefetch_related will never be part of this ORM, preferring a 'fetch in batch when needed' approach. Status: Not started
  11. Look into supporting up to Python 3.7 by taking into account the possible usage of *Union* and *Optional* Maybe import from future? Status: Not started
  12. Improve testing by adding a way to catch queries made to the database, to make sure we lower them as much as possible. Status: Not started
  13. Add support for postgresql. Status: Not started
  14. Look into the next steps for the project. Status: Not started
```

### Comparing `RogueORM-0.0.3/RogueORM.egg-info/PKG-INFO` & `RogueORM-0.1.0/RogueORM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RogueORM
-Version: 0.0.3
+Version: 0.1.0
 Summary: An ORM that strives to eradicate N+1 issues.
 Author-email: Maxime Toussaint <m.toussaint@mail.com>
 License: MIT License
         
         Copyright (c) 2022 Maxime Toussaint
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,16 @@
 ## Development Roadmap
  1. Define a clear syntax taking advantage of Python 3.10 and later's typing syntax. Status: Done
  2. Define models, managers and fields. Status: Done
  3. Add support for basic SQLite operation: SELECT, INSERT, UPDATE, DELETE. Status: Done
  4. Add support for Foreign Keys. Status: Done
  5. Add support for ManyToMany relationships using a joining table. Status: Done (Testing has to be improved)
  6. Add a migration system. Status: Done (Testing has to be improved)
- 7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Not started
- 8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started
+ 7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Done
+ 8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started (Not a priority)
  9. Add logic for batch fetching in loops. Status: Not started
  10. Add logic for select_related. By design, prefetch_related will never be part of this ORM, preferring a 'fetch in batch when needed' approach. Status: Not started
  11. Look into supporting up to Python 3.7 by taking into account the possible usage of *Union* and *Optional* Maybe import from future? Status: Not started
  12. Improve testing by adding a way to catch queries made to the database, to make sure we lower them as much as possible. Status: Not started
  13. Add support for postgresql. Status: Not started
  14. Look into the next steps for the project. Status: Not started
```

### Comparing `RogueORM-0.0.3/RogueORM.egg-info/SOURCES.txt` & `RogueORM-0.1.0/RogueORM.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 rogue/migrations/__init__.py
 rogue/migrations/base.py
 rogue/models/__init__.py
 rogue/models/base.py
 rogue/models/errors.py
 rogue/models/fields.py
 rogue/models/utils.py
+rogue/query/__init__.py
+rogue/query/descriptors.py
+rogue/query/query.py
 rogue/settings/__init__.py
 rogue/settings/default_settings.py
```

### Comparing `RogueORM-0.0.3/pyproject.toml` & `RogueORM-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'RogueORM'
-version = '0.0.3'
+version = '0.1.0'
 description = 'An ORM that strives to eradicate N+1 issues.'
 readme = 'README.md'
 authors = [{name = 'Maxime Toussaint', email = 'm.toussaint@mail.com'}]
 license = {file = 'LICENSE'}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `RogueORM-0.0.3/rogue/__main__.py` & `RogueORM-0.1.0/rogue/__main__.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.3/rogue/backends/base.py` & `RogueORM-0.1.0/rogue/backends/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,29 +34,33 @@
     @abstractmethod
     def close(self):  # pragma: no cover
         pass
 
 
 @dataclass
 class WhereStatement:
+    table_name: str
     field: str
     comparison: str
     value: Any
+    relation_descriptor: Any
 
 
 class BaseQueryBuilder(metaclass=ABCMeta):
     SELECT = "SELECT"
     UPDATE = "UPDATE"
     INSERT = "INSERT INTO"
     DELETE = "DELETE"
 
     FROM = "FROM"
     WHERE = "WHERE"
     AND = "AND"
     VALUES = "VALUES"
+    INNER_JOIN = "INNER JOIN"
+    ON = "ON"
 
     EQUAL = "equal"
     IN = "in"
 
     COMPARISON_MAPPING = {
         EQUAL: "=",
         IN: "IN",
@@ -78,15 +82,24 @@
     def table_name(self):
         return self.model.table_name
 
     @property
     def fields(self):
         return self.model.get_fields()
 
-    def where(self, field, comparison, value, not_=False):
+    def where(
+        self,
+        *,
+        table_name,
+        field,
+        comparison,
+        value,
+        not_: bool = False,
+        relation_descriptor=None,
+    ):
         comparison_mapping = (
             self.NOT_COMPARISON_MAPPING if not_ else self.COMPARISON_MAPPING
         )
 
         if not comparison:
             comparison = self.COMPARISON_DEFAULT
 
@@ -94,15 +107,21 @@
             comparison = comparison_mapping[comparison]
         except KeyError:
             raise InvalidComparisonError(
                 f"{comparison} is not a valid comparison operator."
             )
 
         self.where_statements.append(
-            WhereStatement(field=field, comparison=comparison, value=value)
+            WhereStatement(
+                table_name=table_name,
+                field=field,
+                comparison=comparison,
+                value=value,
+                relation_descriptor=relation_descriptor,
+            )
         )
         return self
 
     @abstractmethod
     def fetch_one(self):  # pragma: no cover
         pass
```

### Comparing `RogueORM-0.0.3/rogue/backends/sqlite/client.py` & `RogueORM-0.1.0/rogue/backends/sqlite/client.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.3/rogue/backends/sqlite/schema.py` & `RogueORM-0.1.0/rogue/backends/sqlite/schema.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.3/rogue/managers/base.py` & `RogueORM-0.1.0/rogue/managers/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from collections.abc import Iterable
 
 from rogue.backends.sqlite.client import DatabaseClient
 from rogue.backends.sqlite.query import QueryBuilder
+from rogue.query import Lookup, RelationDescriptor
 
 from .errors import ManagerValidationError
 
 
 LOOKUP_SEPARATOR = "__"
 
 
 class Manager:
-    def __init__(self, model):
-        self.model = model
+    def __init__(self, model_class, parent=None):
+        self.model_class = model_class
+        self._parent = None
 
-        self._client = DatabaseClient(self.model.db_name)
-        self._query = QueryBuilder(self._client, model)
+        self._client = DatabaseClient(self.model_class.db_name)
+        self._query = QueryBuilder(self._client, self.model_class)
         self._cache = None
         self._is_none = False
 
+        self._joins = {}
+
     def first(self):
         if self._is_none:
             return
 
         self._base_filtering()
 
         data = self._build_models(self._query.fetch_one())
@@ -29,21 +33,33 @@
             return data[0]
         except (IndexError, TypeError):
             return
 
     def all(self):
         return self
 
-    def where(self, not_=False, **where):
+    def where(self, not_=False, table_name=None, **where):
         where = self._deconstruct_where(where)
         if where:
             # TODO: Filter the data instead of forcing a refetch
             self._cache = None
-            for lookup, comparison, value in where:
-                self._query = self._query.where(lookup, comparison, value, not_)
+            for lookup in where:
+                relation_descriptor = (
+                    RelationDescriptor(*lookup.tracking)
+                    if len(lookup.tracking) > 1
+                    else None
+                )
+                self._query = self._query.where(
+                    table_name=table_name or lookup.parent.get_query_table_name(),
+                    field=lookup.parent.name,
+                    comparison=lookup.comparison,
+                    value=lookup.value,
+                    not_=not_,
+                    relation_descriptor=relation_descriptor,
+                )
         return self
 
     def where_not(self, **where):
         return self.where(not_=True, **where)
 
     def insert(self, data):
         self.validate_data(data)
@@ -62,66 +78,94 @@
 
     def validate_data(self, data):
         if data is None:
             raise ManagerValidationError(
                 "The data argument must be passed for insert or update."
             )
 
-        model_fields = self.model.get_fields()
+        model_fields = self.model_class.get_fields()
 
         for field_name in data:
-            if field_name not in self.model.get_field_names():
+            if field_name not in self.model_class.get_field_names():
                 raise ManagerValidationError(
-                    f"{self.model.table_name} has no field named {field_name}."
+                    f"{self.model_class.table_name} has no field named {field_name}."
                 )
             model_fields[field_name].validate(data[field_name])
 
+    def available_lookups(self):
+        return self.model_class.available_lookups()
+
     def _deconstruct_where(self, where):
         formatted_where = []
 
-        for lookup, value in where.items():
-            comparison = ""
+        for lookup_str, value in where.items():
+            lookup = self._get_lookup_object(lookup_str, value)
+            formatted_where.append(lookup)
+
+        return formatted_where
+
+    def _get_lookup_object(self, lookup: str, value):
+        available_lookups = self.available_lookups()
+        prev_obj = None
+        obj = None
+
+        tracking = []
+        for item in lookup.split(LOOKUP_SEPARATOR):
+            try:
+                prev_obj = obj
+                obj = available_lookups[item]
+                tracking.append(obj)
+            except KeyError:
+                raise LookupError(
+                    f"{item} is not a valid lookup. Options are {', '.join(available_lookups)}."
+                )
 
-            if LOOKUP_SEPARATOR in lookup:
-                lookup, comparison = lookup.split(LOOKUP_SEPARATOR)
+            if not hasattr(obj, "available_lookups"):
+                break
 
-            formatted_where.append((lookup, comparison, value))
+            available_lookups = obj.available_lookups()
 
-        return formatted_where
+        if isinstance(obj, type) and issubclass(obj, Lookup):
+            return obj(prev_obj, value, tracking)
+
+        return Lookup(obj, value, tracking)
 
     def _build_models(self, data):
         models = []
         for row in data:
             row = self._build_relations(row)
             model_class = self.get_returned_model_class()
-            models.append(model_class(**row))
+            models.append(model_class(id_=row.get("id"), parent=self, **row))
 
         return models
 
     def _build_relations(self, row):
-        for field_name, field in self.model.get_related_fields().items():
+        for field_name, field in self.model_class.get_related_fields().items():
             if field.name in row:
                 row[field_name] = row[field.name]
             elif hasattr(field, "_through_model"):
                 relation_manager = field.get_relation_wrapper(field_name, None)
                 relation_manager.id = row.get("id")
                 row[field_name] = relation_manager
         return row
 
     def get_returned_model_class(self):
-        return self.model
+        return self.model_class
+
+    def get_query_table_name(self):
+        return self.model_class.table_name
 
     def __iter__(self):
         return iter(self.all_models)
 
     @property
     def all_data(self):
         obj = self._base_filtering()
 
-        if self._is_none or self.model.get_field_names() == ["id"]:
+        if self._is_none or self.model_class.get_field_names() == ["id"]:
             return []
 
         if obj._cache is not None:
             data = obj._cache
         else:
             data = obj._query.fetch_all()
             obj._cache = data
@@ -138,30 +182,30 @@
     def __eq__(self, other):
         return self.all_data == other.all_data
 
     def __len__(self):
         return len(list(self.__iter__()))
 
     def __contains__(self, other):
-        if not isinstance(other, self.model):
+        if not isinstance(other, self.model_class):
             return False
 
         for data in self.all_data:
             if other.id == data["id"]:
                 return True
 
         return False
 
     def __repr__(self):
         return f"<{self.__class__.__name__} [{', '.join(str(model) for model in self.all_models)}]>"
 
 
 class RelationManager(Manager):
-    def __init__(self, model, lookup_field):
-        super().__init__(model)
+    def __init__(self, lookup_field, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.lookup_field = lookup_field
         self.id = None
 
     def _base_filtering(self):
         if self.id is None:
             return self.none()
 
@@ -177,15 +221,15 @@
         self.relation_model = relation_model
 
     def _base_filtering(self):
         if self.id is None:
             return self.none()
 
         self._query.model = self.relation_model
-        return self.where(id=self.id)
+        return self.where(table_name=self.get_query_table_name(), id=self.id)
 
     def add(self, data):
         # TODO: Add a way to insert many with one query
         if isinstance(data, Iterable):
             all_data = []
             for row in data:
                 insert_data = self._get_ids_from_row(row)
@@ -199,7 +243,10 @@
         if not row:
             return {}
 
         return {row.table_name + "_id": row.id, self.lookup_field: self.id}
 
     def get_returned_model_class(self):
         return self.relation_model
+
+    def get_query_table_name(self):
+        return self.relation_model.table_name
```

### Comparing `RogueORM-0.0.3/rogue/migrations/base.py` & `RogueORM-0.1.0/rogue/migrations/base.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.3/rogue/models/base.py` & `RogueORM-0.1.0/rogue/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     def _get_table_name(cls, name):
         return "_".join(re.sub(r"([A-Z])", r" \1", name).split()).lower()
 
 
 class Model(metaclass=ModelMeta):
     db_name = settings.DATABASE_NAME
 
-    def __init__(self, **kwargs):
-        self._foreign_relations = {}
+    def __init__(self, id_=None, parent=None, **kwargs):
+        self._parent = parent
 
-        id_ = kwargs.get("id")
+        self._foreign_relations = {}
 
         self._set_related_managers()
         self._set_related_managers_id(id_)
 
         for field_name, field in self.get_model_fields().items():
             value = field.clean_value(kwargs.pop(field_name, None))
             value = field.build_for_model(value)
@@ -165,14 +165,26 @@
         return {
             field_name: field
             for field_name, field in cls.__dict__.items()
             if isinstance(field, BaseField)
         }
 
     @classmethod
+    def available_lookups(cls):
+        available_lookups = {}
+
+        for field_name, field in cls.get_model_fields().items():
+            available_lookups[field_name] = field
+
+            if field.name != field_name:
+                available_lookups[field.name] = field
+
+        return available_lookups
+
+    @classmethod
     def get_field_names(cls):
         return list(cls.get_fields())
 
     @classmethod
     def get_related_fields(cls):
         return {
             field_name: field
```

### Comparing `RogueORM-0.0.3/rogue/models/fields.py` & `RogueORM-0.1.0/rogue/models/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections.abc import Iterable
 from typing import get_args
 
 from rogue.managers import RelationManager, ManyToManyManager
+from rogue.query import InLookup, Lookup
 
 from .errors import FieldValidationError
 from .utils import get_through_model
 
 
 UNKNOWN_VALUE = "__UNKNOWN_VALUE__"
 
@@ -97,14 +98,20 @@
 
     def build_for_model(self, value):
         return value
 
     def get_relation_wrapper(self, field_name, value):
         return
 
+    def available_lookups(self):
+        return {"equal": Lookup, "in": InLookup}
+
+    def get_query_table_name(self):
+        return self._parent.table_name
+
 
 class StringField(BaseField):
     PYTHON_TYPE = str
 
     def __init__(self, *args, **kwargs):
         self.max_char = kwargs.pop("max_char")
         super().__init__(*args, **kwargs)
@@ -174,27 +181,32 @@
     def _get_field_name(self):
         return self._model_field_name + "_id"
 
     def _get_default_reverse_relation_name(self):
         return self._parent.table_name + "_set"
 
     def _get_reverse_relation(self, field_name):
-        return RelationManager(self._parent, field_name)
+        return RelationManager(field_name, self._parent, self._parent)
 
     def clean_value(self, value):
         if value is not None and hasattr(value, "id") and hasattr(value, "save"):
             if value.id is None:
                 value.save()
 
             value = value.id
         return super().clean_value(value)
 
     def get_relation_wrapper(self, field_name, value):
         return ForeignKeyWrapper(self._foreign_model, value)
 
+    def available_lookups(self):
+        model_lookups = super().available_lookups()
+
+        return {**model_lookups, **self._foreign_model.available_lookups()}
+
 
 class OneToOneWrapper(BaseWrapper):
     def __init__(self, foreign_model):
         self._foreign_model = foreign_model
         self._cache = None
         self.id = None
 
@@ -259,9 +271,12 @@
             return
 
         if not isinstance(value, Iterable):
             value = [value]
 
         return value
 
+    def get_query_table_name(self):
+        return self._foreign_model.table_name
+
 
 FIELD_MAPPING = {str: StringField, int: IntegerField, float: FloatField}
```

### Comparing `RogueORM-0.0.3/rogue/models/utils.py` & `RogueORM-0.1.0/rogue/models/utils.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.3/rogue/settings/__init__.py` & `RogueORM-0.1.0/rogue/settings/__init__.py`

 * *Files identical despite different names*

