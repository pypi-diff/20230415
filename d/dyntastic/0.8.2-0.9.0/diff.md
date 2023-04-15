# Comparing `tmp/dyntastic-0.8.2.tar.gz` & `tmp/dyntastic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dyntastic-0.8.2.tar", last modified: Sun Nov 13 04:49:59 2022, max compression
+gzip compressed data, was "dist/dyntastic-0.9.0.tar", last modified: Sat Apr 15 20:57:30 2023, max compression
```

## Comparing `dyntastic-0.8.2.tar` & `dyntastic-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 04:49:59.000000 dyntastic-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-11-13 04:49:39.000000 dyntastic-0.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-11-13 04:49:39.000000 dyntastic-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-13 04:49:39.000000 dyntastic-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10219 2022-11-13 04:49:59.000000 dyntastic-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8009 2022-11-13 04:49:39.000000 dyntastic-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-13 04:49:39.000000 dyntastic-0.8.2/dyntastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9718 2022-11-13 04:49:39.000000 dyntastic-0.8.2/dyntastic/attr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-11-13 04:49:39.000000 dyntastic-0.8.2/dyntastic/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-13 04:49:39.000000 dyntastic-0.8.2/dyntastic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    19904 2022-11-13 04:49:39.000000 dyntastic-0.8.2/dyntastic/main.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-13 04:49:39.000000 dyntastic-0.8.2/dyntastic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10219 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-13 04:49:59.000000 dyntastic-0.8.2/dyntastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-13 04:49:39.000000 dyntastic-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-13 04:49:59.000000 dyntastic-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-11-13 04:49:39.000000 dyntastic-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:57:30.000000 dyntastic-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-15 20:57:13.000000 dyntastic-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 20:57:13.000000 dyntastic-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 20:57:13.000000 dyntastic-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-15 20:57:30.000000 dyntastic-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-15 20:57:13.000000 dyntastic-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-15 20:57:13.000000 dyntastic-0.9.0/dyntastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-15 20:57:13.000000 dyntastic-0.9.0/dyntastic/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-15 20:57:13.000000 dyntastic-0.9.0/dyntastic/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-15 20:57:13.000000 dyntastic-0.9.0/dyntastic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-04-15 20:57:13.000000 dyntastic-0.9.0/dyntastic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:57:13.000000 dyntastic-0.9.0/dyntastic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 20:57:30.000000 dyntastic-0.9.0/dyntastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 20:57:13.000000 dyntastic-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:57:30.000000 dyntastic-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 20:57:13.000000 dyntastic-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:57:30.000000 dyntastic-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_batch_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_batch_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-15 20:57:13.000000 dyntastic-0.9.0/tests/test_update_expressions.py
```

### Comparing `dyntastic-0.8.2/CHANGELOG.md` & `dyntastic-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.9.0 2023-04-15
+
+- Add support for `__table_host__` for local testing
+
 ## 0.8.2 2022-11-12
 
 - Make mypy linting more strict
 
 ## 0.8.1 2022-11-08
 
 - Fixed `batch_read` to support non-string hash keys
```

### Comparing `dyntastic-0.8.2/LICENSE` & `dyntastic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyntastic-0.8.2/PKG-INFO` & `dyntastic-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyntastic
-Version: 0.8.2
+Version: 0.9.0
 Summary: A DynamoDB library on top of Pydantic and boto3.
 Home-page: https://github.com/nayaverdier/dyntastic
 Author: Naya Verdier
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -80,14 +80,18 @@
 # {'product_id': 'd2e91c30-e701-422f-b71b-465b02749f18', 'name': 'bread', 'description': None, 'price': 3.49, 'tax': None}
 
 p.json()
 # '{"product_id": "d2e91c30-e701-422f-b71b-465b02749f18", "name": "bread", "description": null, "price": 3.49, "tax": null}'
 
 ```
 
+To explicitly define an AWS region or DynamoDB endpoint url (for using a local
+dynamodb docker instance, for example), set `__table_region__` or
+`__table_host__`
+
 ### Inserting into DynamoDB
 
 Using the `Product` example from above, simply:
 
 ```python
 product = Product(name="bread", description="Sourdough Bread", price=3.99)
 product.product_id
@@ -150,14 +154,24 @@
 
 # query an index
 Event.query(A.my_other_field == 12345, index="my_other_field-index")
 
 # note: Must provide a condition expression rather than just the value
 Event.query(123545, index="my_other_field-index")  # errors!
 
+# query an index with an optional filter expression
+filter_expression = None
+if filter_value:
+    filter_expression = A('filter_field').eq(filter_value)
+Event.query(
+    A.my_other_field == 12345, 
+    index="my_other_field-index",
+    filter_expression=filter_expression
+)
+
 # consistent read
 Event.query("some_event_id", consistent_read=True)
 ```
 
 If you need to manually handle pagination, use `query_page`:
 
 ```python
@@ -308,14 +322,18 @@
 
 MyModel.create_table(index1, index2)
 ```
 
 
 # Changelog
 
+## 0.9.0 2023-04-15
+
+- Add support for `__table_host__` for local testing
+
 ## 0.8.2 2022-11-12
 
 - Make mypy linting more strict
 
 ## 0.8.1 2022-11-08
 
 - Fixed `batch_read` to support non-string hash keys
```

### Comparing `dyntastic-0.8.2/README.md` & `dyntastic-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,18 @@
 # {'product_id': 'd2e91c30-e701-422f-b71b-465b02749f18', 'name': 'bread', 'description': None, 'price': 3.49, 'tax': None}
 
 p.json()
 # '{"product_id": "d2e91c30-e701-422f-b71b-465b02749f18", "name": "bread", "description": null, "price": 3.49, "tax": null}'
 
 ```
 
+To explicitly define an AWS region or DynamoDB endpoint url (for using a local
+dynamodb docker instance, for example), set `__table_region__` or
+`__table_host__`
+
 ### Inserting into DynamoDB
 
 Using the `Product` example from above, simply:
 
 ```python
 product = Product(name="bread", description="Sourdough Bread", price=3.99)
 product.product_id
@@ -135,14 +139,24 @@
 
 # query an index
 Event.query(A.my_other_field == 12345, index="my_other_field-index")
 
 # note: Must provide a condition expression rather than just the value
 Event.query(123545, index="my_other_field-index")  # errors!
 
+# query an index with an optional filter expression
+filter_expression = None
+if filter_value:
+    filter_expression = A('filter_field').eq(filter_value)
+Event.query(
+    A.my_other_field == 12345, 
+    index="my_other_field-index",
+    filter_expression=filter_expression
+)
+
 # consistent read
 Event.query("some_event_id", consistent_read=True)
 ```
 
 If you need to manually handle pagination, use `query_page`:
 
 ```python
```

### Comparing `dyntastic-0.8.2/dyntastic/attr.py` & `dyntastic-0.9.0/dyntastic/attr.py`

 * *Files identical despite different names*

### Comparing `dyntastic-0.8.2/dyntastic/batch.py` & `dyntastic-0.9.0/dyntastic/batch.py`

 * *Files identical despite different names*

### Comparing `dyntastic-0.8.2/dyntastic/main.py` & `dyntastic-0.9.0/dyntastic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 _T = TypeVar("_T", bound="Dyntastic")
 
 
 class _TableMetadata:
     # TODO: add __table_host__?
     __table_name__: Union[str, Callable[[], str]]
     __table_region__: Optional[str] = None
+    __table_host__: Optional[str] = None
 
     __hash_key__: str
     __range_key__: Optional[str] = None
 
     _dyntastic_batch_writer: Optional[BatchWriter] = None
 
 
@@ -424,37 +425,43 @@
         key = {self.__hash_key__: self._dyntastic_hash_key}
         if self.__range_key__:
             key[self.__range_key__] = self._dyntastic_range_key
 
         return serialize(key)
 
     @classmethod
+    def _dynamodb_boto3_kwargs(cls):
+        kwargs = {}
+
+        if cls.__table_region__:
+            kwargs["region_name"] = cls.__table_region__
+
+        if cls.__table_host__:
+            kwargs["endpoint_url"] = cls.__table_host__
+
+        return kwargs
+
+    @classmethod
     def _dynamodb_resource(cls):
         if cls._dynamodb_resource_instance is None:  # type: ignore
-            if cls.__table_region__:
-                resource = boto3.resource("dynamodb", region_name=cls.__table_region__)
-            else:
-                resource = boto3.resource("dynamodb")
-            cls._dynamodb_resource_instance = resource  # type: ignore
+            kwargs = cls._dynamodb_boto3_kwargs()
+            cls._dynamodb_resource_instance = boto3.resource("dynamodb", **kwargs)  # type: ignore
         return cls._dynamodb_resource_instance  # type: ignore
 
     @classmethod
     def _dynamodb_table(cls):
         if cls._dynamodb_table_instance is None:  # type: ignore
             cls._dynamodb_table_instance = cls._dynamodb_resource().Table(cls._resolve_table_name())  # type: ignore
         return cls._dynamodb_table_instance  # type: ignore
 
     @classmethod
     def _dynamodb_client(cls):
         if cls._dynamodb_client_instance is None:  # type: ignore
-            if cls.__table_region__:
-                client = boto3.client("dynamodb", region_name=cls.__table_region__)
-            else:
-                client = boto3.client("dynamodb")
-            cls._dynamodb_client_instance = client  # type: ignore
+            kwargs = cls._dynamodb_boto3_kwargs()
+            cls._dynamodb_client_instance = boto3.client("dynamodb", **kwargs)  # type: ignore
         return cls._dynamodb_client_instance  # type: ignore
 
     @classmethod
     def _wait_until_exists(cls):
         # wait a maximum of 15 * 2 = 30 seconds
         for _ in range(15):  # pragma: no cover
             response = cls._dynamodb_client().describe_table(TableName=cls._resolve_table_name())
```

### Comparing `dyntastic-0.8.2/dyntastic.egg-info/PKG-INFO` & `dyntastic-0.9.0/dyntastic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyntastic
-Version: 0.8.2
+Version: 0.9.0
 Summary: A DynamoDB library on top of Pydantic and boto3.
 Home-page: https://github.com/nayaverdier/dyntastic
 Author: Naya Verdier
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -80,14 +80,18 @@
 # {'product_id': 'd2e91c30-e701-422f-b71b-465b02749f18', 'name': 'bread', 'description': None, 'price': 3.49, 'tax': None}
 
 p.json()
 # '{"product_id": "d2e91c30-e701-422f-b71b-465b02749f18", "name": "bread", "description": null, "price": 3.49, "tax": null}'
 
 ```
 
+To explicitly define an AWS region or DynamoDB endpoint url (for using a local
+dynamodb docker instance, for example), set `__table_region__` or
+`__table_host__`
+
 ### Inserting into DynamoDB
 
 Using the `Product` example from above, simply:
 
 ```python
 product = Product(name="bread", description="Sourdough Bread", price=3.99)
 product.product_id
@@ -150,14 +154,24 @@
 
 # query an index
 Event.query(A.my_other_field == 12345, index="my_other_field-index")
 
 # note: Must provide a condition expression rather than just the value
 Event.query(123545, index="my_other_field-index")  # errors!
 
+# query an index with an optional filter expression
+filter_expression = None
+if filter_value:
+    filter_expression = A('filter_field').eq(filter_value)
+Event.query(
+    A.my_other_field == 12345, 
+    index="my_other_field-index",
+    filter_expression=filter_expression
+)
+
 # consistent read
 Event.query("some_event_id", consistent_read=True)
 ```
 
 If you need to manually handle pagination, use `query_page`:
 
 ```python
@@ -308,14 +322,18 @@
 
 MyModel.create_table(index1, index2)
 ```
 
 
 # Changelog
 
+## 0.9.0 2023-04-15
+
+- Add support for `__table_host__` for local testing
+
 ## 0.8.2 2022-11-12
 
 - Make mypy linting more strict
 
 ## 0.8.1 2022-11-08
 
 - Fixed `batch_read` to support non-string hash keys
```

### Comparing `dyntastic-0.8.2/setup.py` & `dyntastic-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "pytest==7.1.2",
     "pytest-cov==3.0.0",
     "pytest-mock==3.7.0",
 ]
 
 setup(
     name="dyntastic",
-    version="0.8.2",
+    version="0.9.0",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
```

