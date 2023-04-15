# Comparing `tmp/datajunction-0.0.1a3.tar.gz` & `tmp/datajunction-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajunction-0.0.1a3.tar", max compression
+gzip compressed data, was "datajunction-0.0.1a4.tar", max compression
```

## Comparing `datajunction-0.0.1a3.tar` & `datajunction-0.0.1a4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1081 2023-03-23 18:47:56.715355 datajunction-0.0.1a3/LICENSE.txt
--rw-r--r--   0        0        0     5589 2023-03-23 18:47:56.715553 datajunction-0.0.1a3/README.rst
--rw-r--r--   0        0        0      384 2023-03-23 18:47:56.716046 datajunction-0.0.1a3/dj/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 18:47:56.716107 datajunction-0.0.1a3/dj/api/__init__.py
--rw-r--r--   0        0        0     4692 2023-04-15 05:07:29.312727 datajunction-0.0.1a3/dj/api/attributes.py
--rw-r--r--   0        0        0     2862 2023-04-15 05:07:29.312961 datajunction-0.0.1a3/dj/api/catalogs.py
--rw-r--r--   0        0        0      654 2023-04-15 05:07:29.313211 datajunction-0.0.1a3/dj/api/cubes.py
--rw-r--r--   0        0        0     4437 2023-04-15 05:07:29.313555 datajunction-0.0.1a3/dj/api/data.py
--rw-r--r--   0        0        0     1457 2023-04-15 05:07:29.313966 datajunction-0.0.1a3/dj/api/engines.py
--rw-r--r--   0        0        0     1220 2023-04-15 05:07:29.314174 datajunction-0.0.1a3/dj/api/health.py
--rw-r--r--   0        0        0    12516 2023-04-15 05:07:29.314478 datajunction-0.0.1a3/dj/api/helpers.py
--rw-r--r--   0        0        0     2995 2023-04-15 05:07:29.315145 datajunction-0.0.1a3/dj/api/main.py
--rw-r--r--   0        0        0     2781 2023-04-15 05:07:29.315496 datajunction-0.0.1a3/dj/api/metrics.py
--rw-r--r--   0        0        0    31233 2023-04-15 05:07:29.316092 datajunction-0.0.1a3/dj/api/nodes.py
--rw-r--r--   0        0        0      702 2023-04-15 05:07:29.316369 datajunction-0.0.1a3/dj/api/query.py
--rw-r--r--   0        0        0     1032 2023-04-15 05:07:29.316543 datajunction-0.0.1a3/dj/api/sql.py
--rw-r--r--   0        0        0     3358 2023-04-15 05:07:29.317020 datajunction-0.0.1a3/dj/api/tags.py
--rw-r--r--   0        0        0     2239 2023-04-12 00:50:10.209059 datajunction-0.0.1a3/dj/config.py
--rw-r--r--   0        0        0      412 2023-03-23 18:47:56.717349 datajunction-0.0.1a3/dj/constants.py
--rwxr-xr-x   0        0        0        0 2023-03-23 18:47:56.717408 datajunction-0.0.1a3/dj/construction/__init__.py
--rwxr-xr-x   0        0        0    16624 2023-04-15 05:07:29.317378 datajunction-0.0.1a3/dj/construction/build.py
--rw-r--r--   0        0        0     6561 2023-04-06 16:56:36.610509 datajunction-0.0.1a3/dj/construction/dj_query.py
--rwxr-xr-x   0        0        0     1495 2023-03-23 18:47:56.717765 datajunction-0.0.1a3/dj/construction/exceptions.py
--rwxr-xr-x   0        0        0     2679 2023-04-13 20:40:03.277515 datajunction-0.0.1a3/dj/construction/utils.py
--rw-r--r--   0        0        0     5900 2023-04-06 16:56:36.610840 datajunction-0.0.1a3/dj/errors.py
--rw-r--r--   0        0        0      518 2023-03-23 19:26:05.392314 datajunction-0.0.1a3/dj/models/__init__.py
--rw-r--r--   0        0        0     2146 2023-03-23 18:47:56.718197 datajunction-0.0.1a3/dj/models/attribute.py
--rw-r--r--   0        0        0     1592 2023-03-23 18:47:56.718254 datajunction-0.0.1a3/dj/models/base.py
--rw-r--r--   0        0        0     2155 2023-03-23 18:47:56.718316 datajunction-0.0.1a3/dj/models/catalog.py
--rw-r--r--   0        0        0     2661 2023-04-06 16:56:36.610968 datajunction-0.0.1a3/dj/models/column.py
--rw-r--r--   0        0        0      858 2023-03-23 18:47:56.718484 datajunction-0.0.1a3/dj/models/cube.py
--rw-r--r--   0        0        0     2019 2023-03-23 19:26:05.392453 datajunction-0.0.1a3/dj/models/database.py
--rw-r--r--   0        0        0      478 2023-03-23 18:47:56.718608 datajunction-0.0.1a3/dj/models/engine.py
--rw-r--r--   0        0        0     1183 2023-04-07 03:44:14.893669 datajunction-0.0.1a3/dj/models/metric.py
--rw-r--r--   0        0        0    20252 2023-04-15 05:07:29.317932 datajunction-0.0.1a3/dj/models/node.py
--rw-r--r--   0        0        0     3711 2023-03-23 19:26:05.392593 datajunction-0.0.1a3/dj/models/query.py
--rw-r--r--   0        0        0     2449 2023-03-23 18:47:56.718891 datajunction-0.0.1a3/dj/models/table.py
--rw-r--r--   0        0        0     2567 2023-03-23 18:47:56.718952 datajunction-0.0.1a3/dj/models/tag.py
--rw-r--r--   0        0        0     4043 2023-04-07 03:44:14.894264 datajunction-0.0.1a3/dj/service_clients.py
--rw-r--r--   0        0        0        0 2023-03-23 18:47:56.719076 datajunction-0.0.1a3/dj/sql/__init__.py
--rw-r--r--   0        0        0     1243 2023-03-23 19:26:05.392954 datajunction-0.0.1a3/dj/sql/dag.py
--rw-r--r--   0        0        0    32092 2023-04-15 05:07:29.318209 datajunction-0.0.1a3/dj/sql/functions.py
--rw-r--r--   0        0        0      644 2023-04-06 16:56:36.611655 datajunction-0.0.1a3/dj/sql/parse.py
--rw-r--r--   0        0        0       55 2023-04-06 16:56:36.611803 datajunction-0.0.1a3/dj/sql/parsing/__init__.py
--rw-r--r--   0        0        0    65122 2023-04-15 05:07:29.318629 datajunction-0.0.1a3/dj/sql/parsing/ast.py
--rw-r--r--   0        0        0        0 2023-03-23 18:47:56.720227 datajunction-0.0.1a3/dj/sql/parsing/backends/__init__.py
--rw-r--r--   0        0        0    30496 2023-04-06 16:56:36.612502 datajunction-0.0.1a3/dj/sql/parsing/backends/antlr4.py
--rw-r--r--   0        0        0      192 2023-03-23 18:47:56.720284 datajunction-0.0.1a3/dj/sql/parsing/backends/exceptions.py
--rw-r--r--   0        0        0     8733 2023-03-27 05:02:19.596790 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
--rw-r--r--   0        0        0    49854 2023-03-27 05:02:19.597040 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
--rw-r--r--   0        0        0        0 2023-03-27 05:02:19.597083 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/__init__.py
--rw-r--r--   0        0        0   117820 2023-03-27 05:02:19.597848 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
--rw-r--r--   0        0        0   114725 2023-03-27 05:02:19.598388 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
--rw-r--r--   0        0        0     8131 2023-03-27 05:02:19.598564 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
--rw-r--r--   0        0        0   142799 2023-03-27 05:02:19.599083 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
--rw-r--r--   0        0        0  1020523 2023-03-27 05:02:19.601075 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
--rw-r--r--   0        0        0     8131 2023-03-27 05:02:19.601243 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
--rw-r--r--   0        0        0   102489 2023-03-27 05:02:19.601505 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
--rw-r--r--   0        0        0    60656 2023-03-27 05:02:19.601711 datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
--rw-r--r--   0        0        0    22205 2023-04-15 05:07:29.319121 datajunction-0.0.1a3/dj/sql/parsing/types.py
--rw-r--r--   0        0        0     3812 2023-03-23 18:47:56.721099 datajunction-0.0.1a3/dj/superset.py
--rw-r--r--   0        0        0     6467 2023-04-06 16:56:36.612795 datajunction-0.0.1a3/dj/typing.py
--rw-r--r--   0        0        0     4042 2023-04-15 05:07:29.319550 datajunction-0.0.1a3/dj/utils.py
--rw-r--r--   0        0        0     1430 2023-04-15 05:08:18.855129 datajunction-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 datajunction-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-23 18:47:56.715355 datajunction-0.0.1a4/LICENSE.txt
+-rw-r--r--   0        0        0     5589 2023-03-23 18:47:56.715553 datajunction-0.0.1a4/README.rst
+-rw-r--r--   0        0        0      384 2023-03-23 18:47:56.716046 datajunction-0.0.1a4/dj/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:47:56.716107 datajunction-0.0.1a4/dj/api/__init__.py
+-rw-r--r--   0        0        0     4692 2023-04-15 05:07:29.312727 datajunction-0.0.1a4/dj/api/attributes.py
+-rw-r--r--   0        0        0     2862 2023-04-15 05:07:29.312961 datajunction-0.0.1a4/dj/api/catalogs.py
+-rw-r--r--   0        0        0      654 2023-04-15 05:07:29.313211 datajunction-0.0.1a4/dj/api/cubes.py
+-rw-r--r--   0        0        0     4437 2023-04-15 05:07:29.313555 datajunction-0.0.1a4/dj/api/data.py
+-rw-r--r--   0        0        0     1457 2023-04-15 05:07:29.313966 datajunction-0.0.1a4/dj/api/engines.py
+-rw-r--r--   0        0        0     1220 2023-04-15 05:07:29.314174 datajunction-0.0.1a4/dj/api/health.py
+-rw-r--r--   0        0        0    12516 2023-04-15 05:07:29.314478 datajunction-0.0.1a4/dj/api/helpers.py
+-rw-r--r--   0        0        0     2995 2023-04-15 05:07:29.315145 datajunction-0.0.1a4/dj/api/main.py
+-rw-r--r--   0        0        0     2781 2023-04-15 05:07:29.315496 datajunction-0.0.1a4/dj/api/metrics.py
+-rw-r--r--   0        0        0    31233 2023-04-15 05:07:29.316092 datajunction-0.0.1a4/dj/api/nodes.py
+-rw-r--r--   0        0        0      702 2023-04-15 05:07:29.316369 datajunction-0.0.1a4/dj/api/query.py
+-rw-r--r--   0        0        0     1032 2023-04-15 05:07:29.316543 datajunction-0.0.1a4/dj/api/sql.py
+-rw-r--r--   0        0        0     3358 2023-04-15 05:07:29.317020 datajunction-0.0.1a4/dj/api/tags.py
+-rw-r--r--   0        0        0     2239 2023-04-12 00:50:10.209059 datajunction-0.0.1a4/dj/config.py
+-rw-r--r--   0        0        0      412 2023-03-23 18:47:56.717349 datajunction-0.0.1a4/dj/constants.py
+-rwxr-xr-x   0        0        0        0 2023-03-23 18:47:56.717408 datajunction-0.0.1a4/dj/construction/__init__.py
+-rwxr-xr-x   0        0        0    16624 2023-04-15 05:07:29.317378 datajunction-0.0.1a4/dj/construction/build.py
+-rw-r--r--   0        0        0     6561 2023-04-06 16:56:36.610509 datajunction-0.0.1a4/dj/construction/dj_query.py
+-rwxr-xr-x   0        0        0     1495 2023-03-23 18:47:56.717765 datajunction-0.0.1a4/dj/construction/exceptions.py
+-rwxr-xr-x   0        0        0     2679 2023-04-13 20:40:03.277515 datajunction-0.0.1a4/dj/construction/utils.py
+-rw-r--r--   0        0        0     5900 2023-04-06 16:56:36.610840 datajunction-0.0.1a4/dj/errors.py
+-rw-r--r--   0        0        0      518 2023-03-23 19:26:05.392314 datajunction-0.0.1a4/dj/models/__init__.py
+-rw-r--r--   0        0        0     2146 2023-03-23 18:47:56.718197 datajunction-0.0.1a4/dj/models/attribute.py
+-rw-r--r--   0        0        0     1592 2023-03-23 18:47:56.718254 datajunction-0.0.1a4/dj/models/base.py
+-rw-r--r--   0        0        0     2155 2023-03-23 18:47:56.718316 datajunction-0.0.1a4/dj/models/catalog.py
+-rw-r--r--   0        0        0     2661 2023-04-06 16:56:36.610968 datajunction-0.0.1a4/dj/models/column.py
+-rw-r--r--   0        0        0      858 2023-03-23 18:47:56.718484 datajunction-0.0.1a4/dj/models/cube.py
+-rw-r--r--   0        0        0     2019 2023-03-23 19:26:05.392453 datajunction-0.0.1a4/dj/models/database.py
+-rw-r--r--   0        0        0      478 2023-03-23 18:47:56.718608 datajunction-0.0.1a4/dj/models/engine.py
+-rw-r--r--   0        0        0     1183 2023-04-07 03:44:14.893669 datajunction-0.0.1a4/dj/models/metric.py
+-rw-r--r--   0        0        0    20252 2023-04-15 05:07:29.317932 datajunction-0.0.1a4/dj/models/node.py
+-rw-r--r--   0        0        0     3711 2023-03-23 19:26:05.392593 datajunction-0.0.1a4/dj/models/query.py
+-rw-r--r--   0        0        0     2449 2023-03-23 18:47:56.718891 datajunction-0.0.1a4/dj/models/table.py
+-rw-r--r--   0        0        0     2567 2023-03-23 18:47:56.718952 datajunction-0.0.1a4/dj/models/tag.py
+-rw-r--r--   0        0        0     4043 2023-04-07 03:44:14.894264 datajunction-0.0.1a4/dj/service_clients.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:47:56.719076 datajunction-0.0.1a4/dj/sql/__init__.py
+-rw-r--r--   0        0        0     1243 2023-03-23 19:26:05.392954 datajunction-0.0.1a4/dj/sql/dag.py
+-rw-r--r--   0        0        0    32092 2023-04-15 05:07:29.318209 datajunction-0.0.1a4/dj/sql/functions.py
+-rw-r--r--   0        0        0      644 2023-04-06 16:56:36.611655 datajunction-0.0.1a4/dj/sql/parse.py
+-rw-r--r--   0        0        0       55 2023-04-06 16:56:36.611803 datajunction-0.0.1a4/dj/sql/parsing/__init__.py
+-rw-r--r--   0        0        0    65122 2023-04-15 05:07:29.318629 datajunction-0.0.1a4/dj/sql/parsing/ast.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:47:56.720227 datajunction-0.0.1a4/dj/sql/parsing/backends/__init__.py
+-rw-r--r--   0        0        0    30496 2023-04-06 16:56:36.612502 datajunction-0.0.1a4/dj/sql/parsing/backends/antlr4.py
+-rw-r--r--   0        0        0      192 2023-03-23 18:47:56.720284 datajunction-0.0.1a4/dj/sql/parsing/backends/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-03-27 05:02:19.596790 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
+-rw-r--r--   0        0        0    49854 2023-03-27 05:02:19.597040 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
+-rw-r--r--   0        0        0        0 2023-03-27 05:02:19.597083 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/__init__.py
+-rw-r--r--   0        0        0   117820 2023-03-27 05:02:19.597848 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
+-rw-r--r--   0        0        0   114725 2023-03-27 05:02:19.598388 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
+-rw-r--r--   0        0        0     8131 2023-03-27 05:02:19.598564 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
+-rw-r--r--   0        0        0   142799 2023-03-27 05:02:19.599083 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
+-rw-r--r--   0        0        0  1020523 2023-03-27 05:02:19.601075 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
+-rw-r--r--   0        0        0     8131 2023-03-27 05:02:19.601243 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
+-rw-r--r--   0        0        0   102489 2023-03-27 05:02:19.601505 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
+-rw-r--r--   0        0        0    60656 2023-03-27 05:02:19.601711 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
+-rw-r--r--   0        0        0    22205 2023-04-15 05:07:29.319121 datajunction-0.0.1a4/dj/sql/parsing/types.py
+-rw-r--r--   0        0        0     3812 2023-03-23 18:47:56.721099 datajunction-0.0.1a4/dj/superset.py
+-rw-r--r--   0        0        0     6467 2023-04-06 16:56:36.612795 datajunction-0.0.1a4/dj/typing.py
+-rw-r--r--   0        0        0     4042 2023-04-15 05:07:29.319550 datajunction-0.0.1a4/dj/utils.py
+-rw-r--r--   0        0        0     1418 2023-04-15 05:53:12.084649 datajunction-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 datajunction-0.0.1a4/PKG-INFO
```

### Comparing `datajunction-0.0.1a3/LICENSE.txt` & `datajunction-0.0.1a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/README.rst` & `datajunction-0.0.1a4/README.rst`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/attributes.py` & `datajunction-0.0.1a4/dj/api/attributes.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/catalogs.py` & `datajunction-0.0.1a4/dj/api/catalogs.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/cubes.py` & `datajunction-0.0.1a4/dj/api/cubes.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/data.py` & `datajunction-0.0.1a4/dj/api/data.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/engines.py` & `datajunction-0.0.1a4/dj/api/engines.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/health.py` & `datajunction-0.0.1a4/dj/api/health.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/helpers.py` & `datajunction-0.0.1a4/dj/api/helpers.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/main.py` & `datajunction-0.0.1a4/dj/api/main.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/metrics.py` & `datajunction-0.0.1a4/dj/api/metrics.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/nodes.py` & `datajunction-0.0.1a4/dj/api/nodes.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/query.py` & `datajunction-0.0.1a4/dj/api/query.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/sql.py` & `datajunction-0.0.1a4/dj/api/sql.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/api/tags.py` & `datajunction-0.0.1a4/dj/api/tags.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/config.py` & `datajunction-0.0.1a4/dj/config.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/construction/build.py` & `datajunction-0.0.1a4/dj/construction/build.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/construction/dj_query.py` & `datajunction-0.0.1a4/dj/construction/dj_query.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/construction/exceptions.py` & `datajunction-0.0.1a4/dj/construction/exceptions.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/construction/utils.py` & `datajunction-0.0.1a4/dj/construction/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/errors.py` & `datajunction-0.0.1a4/dj/errors.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/__init__.py` & `datajunction-0.0.1a4/dj/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/attribute.py` & `datajunction-0.0.1a4/dj/models/attribute.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/base.py` & `datajunction-0.0.1a4/dj/models/base.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/catalog.py` & `datajunction-0.0.1a4/dj/models/catalog.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/column.py` & `datajunction-0.0.1a4/dj/models/column.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/cube.py` & `datajunction-0.0.1a4/dj/models/cube.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/database.py` & `datajunction-0.0.1a4/dj/models/database.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/metric.py` & `datajunction-0.0.1a4/dj/models/metric.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/node.py` & `datajunction-0.0.1a4/dj/models/node.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/query.py` & `datajunction-0.0.1a4/dj/models/query.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/table.py` & `datajunction-0.0.1a4/dj/models/table.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/models/tag.py` & `datajunction-0.0.1a4/dj/models/tag.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/service_clients.py` & `datajunction-0.0.1a4/dj/service_clients.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/dag.py` & `datajunction-0.0.1a4/dj/sql/dag.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/functions.py` & `datajunction-0.0.1a4/dj/sql/functions.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parse.py` & `datajunction-0.0.1a4/dj/sql/parse.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/ast.py` & `datajunction-0.0.1a4/dj/sql/parsing/ast.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/antlr4.py` & `datajunction-0.0.1a4/dj/sql/parsing/backends/antlr4.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/SqlBaseParser.g4` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseParser.g4`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py` & `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/sql/parsing/types.py` & `datajunction-0.0.1a4/dj/sql/parsing/types.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/superset.py` & `datajunction-0.0.1a4/dj/superset.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/typing.py` & `datajunction-0.0.1a4/dj/typing.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/dj/utils.py` & `datajunction-0.0.1a4/dj/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a3/pyproject.toml` & `datajunction-0.0.1a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools_scm]
 # See configuration details in https://github.com/pypa/setuptools_scm
 version_scheme = "no-guess-dev"
 
 [tool.poetry]
 name = "datajunction"
-version = "0.0.1a3"
+version = "0.0.1a4"
 readme = "README.rst"
 repository = "https://github.com/DataJunction/dj"
 description = "DataJunction server library for running to a DataJunction server"
 authors = ["DataJunction Authors"]
 license = "MIT"
 packages = [
     { include = "dj" },
@@ -28,24 +28,23 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyYAML = "^5.4.1"
 SQLAlchemy-Utils = "^0.37.7"
-accept-types = "0.4.1"
+accept-types = "^0.4.1"
 antlr4-python3-runtime = "^4.12.0"
-asciidag = "0.2.0"
+asciidag = "^0.2.0"
 cachelib = "^0.4.0"
 celery = "^5.2.2"
-docopt = "0.6.2"
-fastapi= "0.70.1"
+fastapi= "^0.70.1"
 msgpack = "^1.0.2"
 opentelemetry-instrumentation-fastapi = "0.38b0"
-python-dotenv = "0.19.0"
+python-dotenv = "^0.19.0"
 redis = "^3.5.3"
 requests = "^2.26.0"
 rich = "^10.16.2"
 SQLAlchemy = "<= 1.4.41, >= 1.4.17"
-sqlmodel = "0.0.8"
+sqlmodel = "^0.0.8"
 sqlparse = "^0.3.0"
 yarl = "^1.7.2"
```

### Comparing `datajunction-0.0.1a3/PKG-INFO` & `datajunction-0.0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datajunction
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: DataJunction server library for running to a DataJunction server
 Home-page: https://github.com/DataJunction/dj
 License: MIT
 Author: DataJunction Authors
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,28 +17,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.17,<=1.4.41)
 Requires-Dist: SQLAlchemy-Utils (>=0.37.7,<0.38.0)
-Requires-Dist: accept-types (==0.4.1)
+Requires-Dist: accept-types (>=0.4.1,<0.5.0)
 Requires-Dist: antlr4-python3-runtime (>=4.12.0,<5.0.0)
-Requires-Dist: asciidag (==0.2.0)
+Requires-Dist: asciidag (>=0.2.0,<0.3.0)
 Requires-Dist: cachelib (>=0.4.0,<0.5.0)
 Requires-Dist: celery (>=5.2.2,<6.0.0)
-Requires-Dist: docopt (==0.6.2)
-Requires-Dist: fastapi (==0.70.1)
+Requires-Dist: fastapi (>=0.70.1,<0.71.0)
 Requires-Dist: msgpack (>=1.0.2,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.38b0)
-Requires-Dist: python-dotenv (==0.19.0)
+Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: redis (>=3.5.3,<4.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: rich (>=10.16.2,<11.0.0)
-Requires-Dist: sqlmodel (==0.0.8)
+Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: sqlparse (>=0.3.0,<0.4.0)
 Requires-Dist: yarl (>=1.7.2,<2.0.0)
 Project-URL: Repository, https://github.com/DataJunction/dj
 Description-Content-Type: text/x-rst
 
 ------------
 DataJunction
```

