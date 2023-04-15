# Comparing `tmp/hagis-0.2.1.tar.gz` & `tmp/hagis-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.1.tar", last modified: Fri Apr 14 13:20:06 2023, max compression
+gzip compressed data, was "hagis-0.2.2.tar", last modified: Sat Apr 15 01:03:29 2023, max compression
```

## Comparing `hagis-0.2.1.tar` & `hagis-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:20:06.679693 hagis-0.2.1/
--rw-rw-rw-   0        0        0      958 2023-04-14 13:20:06.678693 hagis-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 13:20:06.661475 hagis-0.2.1/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.1/hagis/__init__.py
--rw-rw-rw-   0        0        0     8515 2023-04-14 13:00:48.000000 hagis-0.2.1/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:20:06.676699 hagis-0.2.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      958 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 13:20:06.000000 hagis-0.2.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-14 13:19:21.000000 hagis-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 13:20:06.680535 hagis-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:29.855959 hagis-0.2.2/
+-rw-rw-rw-   0        0        0      941 2023-04-15 01:03:29.822446 hagis-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:29.788827 hagis-0.2.2/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.2/hagis/__init__.py
+-rw-rw-rw-   0        0        0     8410 2023-04-15 00:47:32.000000 hagis-0.2.2/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:29.807143 hagis-0.2.2/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-15 01:03:29.000000 hagis-0.2.2/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-15 01:03:29.000000 hagis-0.2.2/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 01:03:29.000000 hagis-0.2.2/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 01:03:29.000000 hagis-0.2.2/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-14 19:19:43.000000 hagis-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 01:03:29.855959 hagis-0.2.2/setup.cfg
```

### Comparing `hagis-0.2.1/PKG-INFO` & `hagis-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.1
+Version: 0.2.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,24 +12,22 @@
 Description-Content-Type: text/markdown
 
 # Hagis
 
 A high availability GIS client
 
 ```python
-from hagis import Mapper, Point
-
-url = "https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0"
+from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
     pop2000: int
     shape: Point
 
-mapper = Mapper(url, City)
+layer = Layer("https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0", City)
 
-for city in mapper.query():
+for city in layer.query():
     print(city.areaname, city.pop2000, city.shape.x, city.shape.y)
 ```
 
 [More examples](https://github.com/jshirota/Hagis/blob/main/demo.ipynb)
```

### Comparing `hagis-0.2.1/hagis/hagis.py` & `hagis-0.2.2/hagis/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 from datetime import datetime
 from json import dumps, loads
 from requests import post
 from types import SimpleNamespace
-from typing import Any, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 
 T = TypeVar("T")
 
 class Layer(Generic[T]):
-    """ 
-
-    Args:
-        Generic (T): Type argument.
-        AttGeoBase: Base class.
-    """
-
     def __init__(self, layer_url: str, model: Type[T] = SimpleNamespace, oid_field: str = "objectid", shape_property_name: str = "shape", **mapping: str) -> None:
-        """ Creates a new instance of the AttGeo class.
+        """ Creates a new instance of the Layer class.
 
         Args:
             layer_url (str): Layer url (e.g. .../FeatureServer/0).
             model (Type[T], optional): Model to map to.  Defaults to SimpleNamespace.
             oid_field (str, optional): Name of the Object ID field.  Defaults to "objectid".
             shape_property_name (str, optional): Name of the shape property.  Defaults to "shape".
         """
@@ -54,15 +47,15 @@
                         self._shape_property_type = property_type
 
         # Add custom properties that have not been handled as dynamically handled propeties.
         for property, field in mapping.items():
             if property not in mapped:
                 self._fields[property.lower()] = field
 
-    def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterator[T]:
+    def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterable[T]:
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
             fields = ",".join([f for (_, f) in self._fields.items() if f != self._shape_property_name.lower()])
 
@@ -164,15 +157,15 @@
         if self._shape_property_type is None or self._shape_property_type in self._unknown_shape_types:
             shape = row.geometry
         else:
             shape = self._shape_property_type()
             shape.__dict__ = row.geometry.__dict__
         return SimpleNamespace(**row.attributes.__dict__, **{self._shape_property_name: shape})
 
-    def _query(self, where_clause: str, fields: str, **kwargs: Any) -> Iterator[SimpleNamespace]:
+    def _query(self, where_clause: str, fields: str, **kwargs: Any) -> Iterable[SimpleNamespace]:
         def get_rows(where_clause: str):
             return self._get_rows(where_clause, fields, **kwargs)
 
         rows, exceededTransferLimit = get_rows(where_clause)
 
         for row in rows:
             yield self._map(row)
```

### Comparing `hagis-0.2.1/hagis.egg-info/PKG-INFO` & `hagis-0.2.2/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.1
+Version: 0.2.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,24 +12,22 @@
 Description-Content-Type: text/markdown
 
 # Hagis
 
 A high availability GIS client
 
 ```python
-from hagis import Mapper, Point
-
-url = "https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0"
+from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
     pop2000: int
     shape: Point
 
-mapper = Mapper(url, City)
+layer = Layer("https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0", City)
 
-for city in mapper.query():
+for city in layer.query():
     print(city.areaname, city.pop2000, city.shape.x, city.shape.y)
 ```
 
 [More examples](https://github.com/jshirota/Hagis/blob/main/demo.ipynb)
```

### Comparing `hagis-0.2.1/pyproject.toml` & `hagis-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

