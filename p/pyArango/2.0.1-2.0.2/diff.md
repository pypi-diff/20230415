# Comparing `tmp/pyArango-2.0.1.tar.gz` & `tmp/pyArango-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyArango-2.0.1.tar", last modified: Thu Jan 13 18:48:28 2022, max compression
+gzip compressed data, was "/Users/antoine/workspace/pyArango/dist/.tmp-_y_hacmh/pyArango-2.0.2.tar", last modified: Sat Apr 15 00:06:43 2023, max compression
```

## Comparing `pyArango-2.0.1.tar` & `pyArango-2.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2022-01-13 18:48:28.208567 pyArango-2.0.1/
--rw-r--r--   0 antoine    (501) staff       (20)     3884 2022-01-13 18:46:39.000000 pyArango-2.0.1/CHANGELOG.rst
--rw-r--r--   0 antoine    (501) staff       (20)      919 2022-01-13 18:46:39.000000 pyArango-2.0.1/DESCRIPTION.rst
--rw-r--r--   0 antoine    (501) staff       (20)    11342 2021-03-24 19:31:31.000000 pyArango-2.0.1/LICENSE
--rw-r--r--   0 antoine    (501) staff       (20)       30 2021-03-24 19:31:31.000000 pyArango-2.0.1/MANIFEST.in
--rw-r--r--   0 antoine    (501) staff       (20)     1868 2022-01-13 18:48:28.208672 pyArango-2.0.1/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)    12242 2022-01-13 18:46:39.000000 pyArango-2.0.1/README.rst
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2022-01-13 18:48:28.204102 pyArango-2.0.1/pyArango/
--rw-r--r--   0 antoine    (501) staff       (20)        0 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/__init__.py
--rw-r--r--   0 antoine    (501) staff       (20)     2392 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/action.py
--rw-r--r--   0 antoine    (501) staff       (20)      720 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/admin.py
--rw-r--r--   0 antoine    (501) staff       (20)      962 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/ca_certificate.py
--rw-r--r--   0 antoine    (501) staff       (20)    35991 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/collection.py
--rw-r--r--   0 antoine    (501) staff       (20)    12870 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/connection.py
--rw-r--r--   0 antoine    (501) staff       (20)      204 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/consts.py
--rw-r--r--   0 antoine    (501) staff       (20)    20323 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/database.py
--rw-r--r--   0 antoine    (501) staff       (20)    20250 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/document.py
--rw-r--r--   0 antoine    (501) staff       (20)     1593 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/foxx.py
--rw-r--r--   0 antoine    (501) staff       (20)     4927 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/gevent_session.py
--rw-r--r--   0 antoine    (501) staff       (20)     9731 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/graph.py
--rw-r--r--   0 antoine    (501) staff       (20)     1929 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/index.py
--rw-r--r--   0 antoine    (501) staff       (20)     3002 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/jwauth.py
--rw-r--r--   0 antoine    (501) staff       (20)     8007 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/query.py
--rw-r--r--   0 antoine    (501) staff       (20)     2038 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/tasks.py
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2022-01-13 18:48:28.207583 pyArango-2.0.1/pyArango/tests/
--rw-r--r--   0 antoine    (501) staff       (20)        0 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/tests/__init__.py
--rw-r--r--   0 antoine    (501) staff       (20)     1167 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/tests/doc_save_benchmark.py
--rw-r--r--   0 antoine    (501) staff       (20)     3172 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/tests/doc_save_bulk_benchmark.py
--rw-r--r--   0 antoine    (501) staff       (20)    37206 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/tests/tests.py
--rw-r--r--   0 antoine    (501) staff       (20)     1233 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/tests/validators_tests.py
--rw-r--r--   0 antoine    (501) staff       (20)     7391 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/theExceptions.py
--rw-r--r--   0 antoine    (501) staff       (20)     5657 2021-03-24 19:31:31.000000 pyArango-2.0.1/pyArango/users.py
--rw-r--r--   0 antoine    (501) staff       (20)     3933 2022-01-13 18:46:39.000000 pyArango-2.0.1/pyArango/validation.py
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2022-01-13 18:48:28.205611 pyArango-2.0.1/pyArango.egg-info/
--rw-r--r--   0 antoine    (501) staff       (20)     1868 2022-01-13 18:48:28.000000 pyArango-2.0.1/pyArango.egg-info/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)      832 2022-01-13 18:48:28.000000 pyArango-2.0.1/pyArango.egg-info/SOURCES.txt
--rw-r--r--   0 antoine    (501) staff       (20)        1 2022-01-13 18:48:28.000000 pyArango-2.0.1/pyArango.egg-info/dependency_links.txt
--rw-r--r--   0 antoine    (501) staff       (20)       40 2022-01-13 18:48:28.000000 pyArango-2.0.1/pyArango.egg-info/entry_points.txt
--rw-r--r--   0 antoine    (501) staff       (20)       32 2022-01-13 18:48:28.000000 pyArango-2.0.1/pyArango.egg-info/requires.txt
--rw-r--r--   0 antoine    (501) staff       (20)        9 2022-01-13 18:48:28.000000 pyArango-2.0.1/pyArango.egg-info/top_level.txt
--rw-r--r--   0 antoine    (501) staff       (20)       67 2022-01-13 18:48:28.208977 pyArango-2.0.1/setup.cfg
--rw-r--r--   0 antoine    (501) staff       (20)     1598 2022-01-13 18:46:39.000000 pyArango-2.0.1/setup.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-04-15 00:06:43.883299 pyArango-2.0.2/
+-rw-r--r--   0 antoine    (501) staff       (20)     4058 2023-04-15 00:05:36.000000 pyArango-2.0.2/CHANGELOG.rst
+-rw-r--r--   0 antoine    (501) staff       (20)      919 2023-04-15 00:05:36.000000 pyArango-2.0.2/DESCRIPTION.rst
+-rw-r--r--   0 antoine    (501) staff       (20)    11342 2023-04-15 00:05:36.000000 pyArango-2.0.2/LICENSE
+-rw-r--r--   0 antoine    (501) staff       (20)       30 2023-04-15 00:05:36.000000 pyArango-2.0.2/MANIFEST.in
+-rw-r--r--   0 antoine    (501) staff       (20)     1715 2023-04-15 00:06:43.883372 pyArango-2.0.2/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)    12242 2023-04-15 00:05:36.000000 pyArango-2.0.2/README.rst
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-04-15 00:06:43.881580 pyArango-2.0.2/pyArango/
+-rw-r--r--   0 antoine    (501) staff       (20)        0 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/__init__.py
+-rw-r--r--   0 antoine    (501) staff       (20)     2392 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/action.py
+-rw-r--r--   0 antoine    (501) staff       (20)      720 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/admin.py
+-rw-r--r--   0 antoine    (501) staff       (20)      962 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/ca_certificate.py
+-rw-r--r--   0 antoine    (501) staff       (20)    35673 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/collection.py
+-rw-r--r--   0 antoine    (501) staff       (20)    13947 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/connection.py
+-rw-r--r--   0 antoine    (501) staff       (20)      204 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/consts.py
+-rw-r--r--   0 antoine    (501) staff       (20)    20513 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/database.py
+-rw-r--r--   0 antoine    (501) staff       (20)    20438 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/document.py
+-rw-r--r--   0 antoine    (501) staff       (20)     1593 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/foxx.py
+-rw-r--r--   0 antoine    (501) staff       (20)     4927 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/gevent_session.py
+-rw-r--r--   0 antoine    (501) staff       (20)     9731 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/graph.py
+-rw-r--r--   0 antoine    (501) staff       (20)     1929 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/index.py
+-rw-r--r--   0 antoine    (501) staff       (20)     3002 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/jwauth.py
+-rw-r--r--   0 antoine    (501) staff       (20)     8007 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/query.py
+-rw-r--r--   0 antoine    (501) staff       (20)     2038 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/tasks.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-04-15 00:06:43.883167 pyArango-2.0.2/pyArango/tests/
+-rw-r--r--   0 antoine    (501) staff       (20)        0 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/tests/__init__.py
+-rw-r--r--   0 antoine    (501) staff       (20)     1167 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/tests/doc_save_benchmark.py
+-rw-r--r--   0 antoine    (501) staff       (20)     3172 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/tests/doc_save_bulk_benchmark.py
+-rw-r--r--   0 antoine    (501) staff       (20)    37206 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/tests/tests.py
+-rw-r--r--   0 antoine    (501) staff       (20)     1233 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/tests/validators_tests.py
+-rw-r--r--   0 antoine    (501) staff       (20)     7628 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/theExceptions.py
+-rw-r--r--   0 antoine    (501) staff       (20)     5657 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/users.py
+-rw-r--r--   0 antoine    (501) staff       (20)     3933 2023-04-15 00:05:36.000000 pyArango-2.0.2/pyArango/validation.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-04-15 00:06:43.882379 pyArango-2.0.2/pyArango.egg-info/
+-rw-r--r--   0 antoine    (501) staff       (20)     1715 2023-04-15 00:06:43.000000 pyArango-2.0.2/pyArango.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)      832 2023-04-15 00:06:43.000000 pyArango-2.0.2/pyArango.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        1 2023-04-15 00:06:43.000000 pyArango-2.0.2/pyArango.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       39 2023-04-15 00:06:43.000000 pyArango-2.0.2/pyArango.egg-info/entry_points.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       32 2023-04-15 00:06:43.000000 pyArango-2.0.2/pyArango.egg-info/requires.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        9 2023-04-15 00:06:43.000000 pyArango-2.0.2/pyArango.egg-info/top_level.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       67 2023-04-15 00:06:43.883643 pyArango-2.0.2/setup.cfg
+-rw-r--r--   0 antoine    (501) staff       (20)     1598 2023-04-15 00:05:36.000000 pyArango-2.0.2/setup.py
```

### Comparing `pyArango-2.0.1/CHANGELOG.rst` & `pyArango-2.0.2/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+2.0.2
+=====
+* Fixed contains functions
+* Added UniqueConstrainViolation exception, inherits from CreationError
+
 2.0.1
 =====
 
 * Fixed max retries for write conflicts
+* Added parameter ``pool_maxsize`` on class ``Connection`` to allow user configure the http pool size.
+=======
 
 2.0
 =====
 
 * changed the default value of reject_zero in NotNull from True to False
 * added to_default function to reset a document to its default values
 * fixed bug in default documents where default values could be overwritten
 * default value for fields is now None
-* defaual value for fields can now be a callable
 
 1.3.5
 =====
 
 * restoreIndex and restoreIndexes in collection will restore previously deleted indexes
 * added max_conflict_retries to handle arango's 1200
 * added single session so AikidoSessio.Holders can share a single request session
```

### Comparing `pyArango-2.0.1/DESCRIPTION.rst` & `pyArango-2.0.2/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/LICENSE` & `pyArango-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/PKG-INFO` & `pyArango-2.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyArango
-Version: 2.0.1
+Version: 2.0.2
 Summary: An easy to use python driver for ArangoDB with built-in validation
 Home-page: https://github.com/tariqdaouda/pyArango
 Author: Tariq Daouda
 Author-email: tariq.daouda@umontreal.ca
 License: ApacheV2
-Description: Python Object Wrapper for ArangoDB_ with built-in validation
-        =============================================================
-        
-        pyArango aims to be an easy to use driver for ArangoDB with built in validation. Collections are treated as types that apply to the documents within. You can be 100% permissive or enforce schemas and validate fields on set, on save or on both.
-        
-        pyArango supports graphs, indexes and probably everything that arangodb_ can do.
-        
-        pyArango is developed by `Tariq Daouda`_, the full source code is available from github_.
-        
-        .. _Tariq Daouda: http://bioinfo.iric.ca/~daoudat/
-        .. _github: https://github.com/tariqdaouda/pyArango
-        .. _arangodb: http://www.arangodb.com
-        .. _ArangoDB: http://www.arangodb.com
-        
-        For the latest news about pyArango, you can follow me on twitter `@tariqdaouda`_.
-        If you have any issues with it, please file a github issue.
-        
-        .. _@tariqdaouda: https://www.twitter.com/tariqdaouda
-        
 Keywords: database ORM nosql arangodb driver validation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+Python Object Wrapper for ArangoDB_ with built-in validation
+=============================================================
+
+pyArango aims to be an easy to use driver for ArangoDB with built in validation. Collections are treated as types that apply to the documents within. You can be 100% permissive or enforce schemas and validate fields on set, on save or on both.
+
+pyArango supports graphs, indexes and probably everything that arangodb_ can do.
+
+pyArango is developed by `Tariq Daouda`_, the full source code is available from github_.
+
+.. _Tariq Daouda: http://bioinfo.iric.ca/~daoudat/
+.. _github: https://github.com/tariqdaouda/pyArango
+.. _arangodb: http://www.arangodb.com
+.. _ArangoDB: http://www.arangodb.com
+
+For the latest news about pyArango, you can follow me on twitter `@tariqdaouda`_.
+If you have any issues with it, please file a github issue.
+
+.. _@tariqdaouda: https://www.twitter.com/tariqdaouda
```

### Comparing `pyArango-2.0.1/README.rst` & `pyArango-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/action.py` & `pyArango-2.0.2/pyArango/action.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/admin.py` & `pyArango-2.0.2/pyArango/admin.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/ca_certificate.py` & `pyArango-2.0.2/pyArango/ca_certificate.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/collection.py` & `pyArango-2.0.2/pyArango/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,17 @@
             dct = {}
         if fields is None:
             fields = self._fields
 
         for k, v in fields.items():
             if isinstance(v, dict):
                 dct[k] = self.getDefaultDocument(fields[k], None)
+            elif isinstance(v, list) or isinstance(v, tuple):
+                dct[k] = []
+
             elif isinstance(v, Field):
                 if callable(v.default):
                     dct[k] = v.default()
                 else :
                     dct[k] = v.default
             else:
                 raise ValueError("Field '%s' is of invalid type '%s'" % (k, type(v)) )
@@ -334,15 +337,15 @@
     def _writeBatch(self):
         if not self._bulkCache:
             return
         if self._bulkMode != BulkMode.INSERT:
             raise UpdateError("Mixed bulk operations not supported - have " + str(self._bulkMode))
         payload = []
         for d in self._bulkCache:
-            if type(d) is dict:
+            if isinstance(d,dict):
                 payload.append(json.dumps(d, default=str))
             else:
                 try:
                     payload.append(d.toJson())
                 except Exception as e:
                     payload.append(json.dumps(d.getStore(), default=str))
 
@@ -351,23 +354,23 @@
         data = r.json()
         if (not isinstance(data, list)):
             raise UpdateError("expected reply to be a json array" + r)
         i = 0
         bulkError = None
         for xd in data:
             if not '_key' in xd and 'error' in xd and 'errorNum' in xd:
-                if bulkError == None:
+                if bulkError is None:
                     bulkError = BulkOperationError("saving failed")
                 bulkError.addBulkError(ArangoError(xd), self._bulkCache[i])
             else:
                 self._bulkCache[i].setPrivates(xd)
                 self._bulkCache[i]._key = \
                     xd['_key']
             i += 1
-        if bulkError != None:
+        if bulkError is not None:
             self._bulkCache = []
             raise bulkError
 
         self._bulkCache = []
 
     def _saveBatch(self, document, params):
         if self._bulkMode != BulkMode.NONE and self._bulkMode != BulkMode.INSERT:
@@ -387,15 +390,15 @@
         payload = []
         for d in self._bulkCache:
             dPayload = d._store.getPatches()
         
             if d.collection._validation['on_save']:
                 d.validate()
 
-            if type(d) is dict:
+            if isinstance(d,dict):
                 payload.append(json.dumps(d, default=str))
             else:
                 try:
                     payload.append(d.toJson())
                 except Exception as e:
                     payload.append(json.dumps(d.getStore(), default=str))
         payload = '[' + ','.join(payload) + ']'
@@ -403,24 +406,24 @@
         data = r.json()
         if (not isinstance(data, list)):
             raise UpdateError("expected reply to be a json array" + dir(r))
         i = 0
         bulkError = None
         for xd in data:
             if not '_key' in xd and 'error' in xd and 'errorNum' in xd:
-                if bulkError == None:
+                if bulkError is None:
                     bulkError = BulkOperationError("patching failed")
                 bulkError.addBulkError(ArangoError(xd), str(self._bulkCache[i]))
             else:
                 self._bulkCache[i].setPrivates(xd)
                 self._bulkCache[i]._key = \
                     xd['_key']
             i += 1
         self._bulkCache = []
-        if bulkError != None:
+        if bulkError is not None:
             raise bulkError
         
         
     def _patchBatch(self, document, params):
         if self._bulkMode != BulkMode.NONE and self._bulkMode != BulkMode.UPDATE:
             raise UpdateError("Mixed bulk operations not supported - have " + str(self._bulkMode))
         self._bulkMode = BulkMode.UPDATE
@@ -433,15 +436,15 @@
     def _removeBatch(self):
         if not self._bulkCache:
             return
         if self._bulkMode != BulkMode.DELETE:
             raise UpdateError("Mixed bulk operations not supported - have " + self._bulkMode)
         payload = []
         for d in self._bulkCache:
-            if type(d) is dict:
+            if isinstance(d,dict):
                 payload.append('"%s"' % d['_key'])
             else:
                 try:
                     payload.append('"%s"' % d['_key'])
                 except Exception as e:
                     payload.append('"%s"' % d['_key'])
 
@@ -450,22 +453,22 @@
         data = r.json()
         if (not isinstance(data, list)):
             raise UpdateError("expected reply to be a json array" + r)
         i = 0
         bulkError = None
         for xd in data:
             if not '_key' in xd and 'error' in xd and 'errorNum' in xd:
-                if bulkError == None:
+                if bulkError is None:
                     bulkError = BulkOperationError("deleting failed")
                 bulkError.addBulkError(ArangoError(xd), self._bulkCache[i])
             else:
                 self._bulkCache[i].reset(self)
             i += 1
         self._bulkCache = []
-        if bulkError != None:
+        if bulkError is not None:
             raise bulkError
 
     def _deleteBatch(self, document, params):
         if self._bulkMode != BulkMode.NONE and self._bulkMode != BulkMode.DELETE:
             raise UpdateError("Mixed bulk operations not supported - have " + str(self._bulkMode))
         self._bulkMode = BulkMode.DELETE
         self._bulkCache.append(document)
@@ -670,30 +673,29 @@
 
         if r.status_code < 400:
             if rawResults:
                 return r.json()
             return self.documentClass(self, r.json(), on_load_validation=self._validation["on_load"])
         elif r.status_code == 404 :
             raise DocumentNotFoundError("Unable to find document with _key: %s" % key, r.json())
-        else:
-            raise DocumentNotFoundError("Unable to find document with _key: %s, response: %s" % (key, r.json()), r.json())
+        raise DocumentNotFoundError("Unable to find document with _key: %s, response: %s" % (key, r.json()), r.json())
 
     def fetchByExample(self, exampleDict, batchSize, rawResults = False, **queryArgs):
         """exampleDict should be something like {'age' : 28}"""
         return self.simpleQuery('by-example', rawResults, example = exampleDict, batchSize = batchSize, **queryArgs)
 
     def fetchFirstExample(self, exampleDict, rawResults = False):
         """exampleDict should be something like {'age' : 28}. returns only a single element but still in a SimpleQuery object.
         returns the first example found that matches the example"""
         return self.simpleQuery('first-example', rawResults = rawResults, example = exampleDict)
 
     def fetchAll(self, rawResults = False, **queryArgs):
         """Returns all the documents in the collection. You can use the optinal arguments 'skip' and 'limit'::
 
-            fetchAlll(limit = 3, shik = 10)"""
+            fetchAll(limit = 3, skip = 10)"""
         return self.simpleQuery('all', rawResults = rawResults, **queryArgs)
 
     def simpleQuery(self, queryType, rawResults = False, **queryArgs):
         """General interface for simple queries. queryType can be something like 'all', 'by-example' etc... everything is in the arango doc.
         If rawResults, the query will return dictionaries instead of Document objetcs.
         """
         return SimpleQuery(self, queryType, rawResults, **queryArgs)
@@ -707,15 +709,15 @@
     def bulkSave(self, docs, onDuplicate="error", **params):
         """Parameter docs must be either an iterrable of documents or dictionnaries.
         This function will return the number of documents, created and updated, and will raise an UpdateError exception if there's at least one error.
         params are any parameters from arango's documentation"""
 
         payload = []
         for d in docs:
-            if type(d) is dict:
+            if isinstance(d,dict):
                 payload.append(json.dumps(d, default=str))
             else:
                 try:
                     payload.append(d.toJson())
                 except Exception as e:
                     payload.append(json.dumps(d.getStore(), default=str))
 
@@ -726,52 +728,47 @@
         params["collection"] = self.name
         url = "%s/import" % self.database.getURL()
 
         r = self.connection.session.post(url, params = params, data = payload)
         data = r.json()
         if (r.status_code == 201) and "error" not in data:
             return True
-        else:
-            if "errors" in data and data["errors"] > 0:
-                raise UpdateError("%d documents could not be created" % data["errors"], data)
-            elif data["error"]:
-                raise UpdateError("Documents could not be created", data)
+        if "errors" in data and data["errors"] > 0:
+            raise UpdateError("%d documents could not be created" % data["errors"], data)
+        elif data["error"]:
+            raise UpdateError("Documents could not be created", data)
 
         return data["updated"] + data["created"]
 
     def bulkImport_json(self, filename, onDuplicate="error", formatType="auto", **params):
         """bulk import from a file repecting arango's key/value format"""
 
         url = "%s/import" % self.database.getURL()
         params["onDuplicate"] = onDuplicate
         params["collection"] = self.name
         params["type"] = formatType
         with open(filename) as f:
             data = f.read()
             r = self.connection.session.post(url, params = params, data = data)
 
-            try:
-                errorMessage = "At least: %d errors. The first one is: '%s'\n\n more in <this_exception>.data" % (len(data), data[0]["errorMessage"])
-            except KeyError:
-                raise UpdateError(data['errorMessage'], data)
+            if r.status_code != 201:
+                raise UpdateError('Unable to bulk import JSON', r)
 
     def bulkImport_values(self, filename, onDuplicate="error", **params):
         """bulk import from a file repecting arango's json format"""
         
         url = "%s/import" % self.database.getURL()
         params["onDuplicate"] = onDuplicate
         params["collection"] = self.name
         with open(filename) as f:
             data = f.read()
             r = self.connection.session.post(url, params = params, data = data)
 
-            try:
-                errorMessage = "At least: %d errors. The first one is: '%s'\n\n more in <this_exception>.data" % (len(data), data[0]["errorMessage"])
-            except KeyError:
-                raise UpdateError(data['errorMessage'], data)
+            if r.status_code != 201:
+                raise UpdateError('Unable to bulk import values', r)
 
     def truncate(self):
         """deletes every document in the collection"""
         return self.action('PUT', 'truncate')
 
     def empty(self):
         """alias for truncate"""
@@ -807,31 +804,29 @@
 
     def getType(self):
         """returns a word describing the type of the collection (edges or ducments) instead of a number, if you prefer the number it's in self.type"""
         if self.type == CONST.COLLECTION_DOCUMENT_TYPE:
             return "document"
         elif self.type == CONST.COLLECTION_EDGE_TYPE:
             return "edge"
-        else:
-            raise ValueError("The collection is of Unknown type %s" % self.type)
+        raise ValueError("The collection is of Unknown type %s" % self.type)
 
     def getStatus(self):
         """returns a word describing the status of the collection (loaded, loading, deleted, unloaded, newborn) instead of a number, if you prefer the number it's in self.status"""
         if self.status == CONST.COLLECTION_LOADING_STATUS:
             return "loading"
         elif self.status == CONST.COLLECTION_LOADED_STATUS:
             return "loaded"
         elif self.status == CONST.COLLECTION_DELETED_STATUS:
             return "deleted"
         elif self.status == CONST.COLLECTION_UNLOADED_STATUS:
             return "unloaded"
         elif self.status == CONST.COLLECTION_NEWBORN_STATUS:
             return "newborn"
-        else:
-            raise ValueError("The collection has an Unknown status %s" % self.status)
+        raise ValueError("The collection has an Unknown status %s" % self.status)
 
     def __len__(self):
         """returns the number of documents in the collection"""
         return self.count()
 
     def __repr__(self):
         return "ArangoDB collection name: %s, id: %s, type: %s, status: %s" % (self.name, self.id, self.getType(), self.getStatus())
@@ -877,16 +872,15 @@
         for nested dicts ex: {address : { street: xxx} }, fieldName can take the form address.street
         """
         try:
             valValue = Collection.validateField(fieldName, value)
         except SchemaViolation as e:
             if fieldName == "_from" or fieldName == "_to":
                 return True
-            else:
-                raise e
+            raise e
         return valValue
 
     def createEdge(self, initValues = None):
         """Create an edge populated with defaults"""
         return self.createDocument(initValues)
 
     def getInEdges(self, vertex, rawResults = False):
@@ -898,15 +892,15 @@
         return self.getEdges(vertex, inEdges = False, outEdges = True, rawResults = rawResults)
 
     def getEdges(self, vertex, inEdges = True, outEdges = True, rawResults = False):
         """returns in, out, or both edges liked to a given document. vertex can be either a Document object or a string for an _id.
         If rawResults a arango results will be return as fetched, if false, will return a liste of Edge objects"""
         if isinstance(vertex, Document):
             vId = vertex._id
-        elif (type(vertex) is str) or (type(vertex) is bytes):
+        elif isinstance(vertex,str) or isinstance(vertex,bytes):
             vId = vertex
         else:
             raise ValueError("Vertex is neither a Document nor a String")
 
         params = {"vertex" : vId}
         if inEdges and outEdges:
             pass
@@ -921,16 +915,15 @@
         data = r.json()
         if r.status_code == 200:
             if not rawResults:
                 ret = []
                 for e in data["edges"]:
                     ret.append(Edge(self, e))
                 return ret
-            else:
-                return data["edges"]
+            return data["edges"]
         else:
             raise CreationError("Unable to return edges for vertex: %s" % vId, data)
 
 
 class BulkOperation(object):
     def __init__(self, collection, batchSize=100):
         self.coll = collection
```

### Comparing `pyArango-2.0.1/pyArango/connection.py` & `pyArango-2.0.2/pyArango/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import uuid
 import json as json_mod
 from datetime import datetime
 
 import requests
-import base64
-import tempfile
-import shutil
 
 from .action import ConnectionAction
 from .database import Database, DBHandle
 from .theExceptions import CreationError, ConnectionError
 from .users import Users
 
 from .ca_certificate import CA_Certificate
@@ -25,16 +22,18 @@
     def __call__(self, *args, **kwargs):
         try:
             return self.ret.json_originalFct(*args, **kwargs)
         except Exception as e:
             print( "Unable to get json for request: %s. Content: %s" % (self.ret.url, self.ret.content) )
             raise e
 
-class AikidoSession(object):
-    """Magical Aikido being that you probably do not need to access directly that deflects every http request to requests in the most graceful way.
+
+class AikidoSession:
+    """Magical Aikido being that you probably do not need to access directly
+    that deflects every http request to requests in the most graceful way.
     It will also save basic stats on requests in it's attribute '.log'.
     """
 
     class Holder(object):
         def __init__(self, fct, auth, max_conflict_retries=5, verify=True):
             self.fct = fct
             self.auth = auth
@@ -72,20 +71,30 @@
                 raise ConnectionError("Empty server response", ret.url, ret.status_code, ret.content)
             elif ret.status_code == 401:
                 raise ConnectionError("Unauthorized access, you must supply a (username, password) with the correct credentials", ret.url, ret.status_code, ret.content)
 
             ret.json = JsonHook(ret)
             return ret
 
-    def __init__(self, username, password, verify=True, max_conflict_retries=5, max_retries=5, single_session=True, log_requests=False):
+    def __init__(
+            self,
+            username,
+            password,
+            verify=True,
+            max_conflict_retries=5,
+            max_retries=5,
+            single_session=True,
+            log_requests=False,
+            pool_maxsize=10
+    ):
         if username:
             self.auth = (username, password)
         else:
             self.auth = None
-
+        self.pool_maxsize = pool_maxsize
         self.verify = verify
         self.max_retries = max_retries
         self.log_requests = log_requests
         self.max_conflict_retries = max_conflict_retries
 
         self.session = None
         if single_session:
@@ -94,25 +103,31 @@
         if log_requests:
             self.log = {}
             self.log["nb_request"] = 0
             self.log["requests"] = {}
 
     def _make_session(self):
         session = requests.Session()
-        http = requests.adapters.HTTPAdapter(max_retries=self.max_retries)
-        https = requests.adapters.HTTPAdapter(max_retries=self.max_retries)
+        kwargs = {
+            'max_retries': self.max_retries,
+            'pool_connections': self.pool_maxsize,
+            'pool_maxsize': self.pool_maxsize,
+            #'pool_block': True  # We don't want to lose connections
+        }
+        http = requests.adapters.HTTPAdapter(**kwargs)
+        https = requests.adapters.HTTPAdapter(**kwargs)
         session.mount('http://', http)
         session.mount('https://', https)
 
         return session
 
     def __getattr__(self, request_function_name):
         if self.session is not None:
             session = self.session
-        else :
+        else:
             session = self._make_session()
 
         try:
             request_function = getattr(session, request_function_name)
         except AttributeError:
             raise AttributeError("Attribute '%s' not found (no Aikido move available)" % request_function_name)
 
@@ -124,14 +139,15 @@
             log["requests"][request_function.__name__] += 1
 
         return AikidoSession.Holder(request_function, auth, max_conflict_retries=self.max_conflict_retries, verify=verify)
 
     def disconnect(self):
         pass
 
+
 class Connection(object):
     """This is the entry point in pyArango and directly handles databases.
     @param arangoURL: can be either a string url or a list of string urls to different coordinators
     @param use_grequests: allows for running concurent requets.
 
     Parameters
     ----------
@@ -158,37 +174,42 @@
         use JWT authentication
     use_lock_for_reseting_jwt: bool
         use lock for reseting gevents authentication
     max_retries: int
         max number of retries for a request
     max_conflict_retries: int
         max number of requests for a conflict error (1200 arangodb error). Does not work with gevents (grequests),
+    pool_maxsize: int
+        max number of open connections. (Not intended for grequest)
     """
 
     LOAD_BLANCING_METHODS = {'round-robin', 'random'}
 
-    def __init__(self,
-        arangoURL = 'http://127.0.0.1:8529',
-        username = None,
-        password = None,
-        verify = True,
-        verbose = False,
-        statsdClient = None,
-        reportFileName = None,
-        loadBalancing = "round-robin",
-        use_grequests = False,
-        use_jwt_authentication=False,
-        use_lock_for_reseting_jwt=True,
-        max_retries=5,
-        max_conflict_retries=5
+    def __init__(
+            self,
+            arangoURL='http://127.0.0.1:8529',
+            username=None,
+            password=None,
+            verify=True,
+            verbose=False,
+            statsdClient=None,
+            reportFileName=None,
+            loadBalancing="round-robin",
+            use_grequests=False,
+            use_jwt_authentication=False,
+            use_lock_for_reseting_jwt=True,
+            max_retries=5,
+            max_conflict_retries=5,
+            pool_maxsize=10
     ):
 
         if loadBalancing not in Connection.LOAD_BLANCING_METHODS:
             raise ValueError("loadBalancing should be one of : %s, got %s" % (Connection.LOAD_BLANCING_METHODS, loadBalancing) )
 
+        self.pool_maxsize = pool_maxsize
         self.loadBalancing = loadBalancing
         self.currentURLId = 0
         self.username = username
         self.use_grequests = use_grequests
         self.use_jwt_authentication = use_jwt_authentication
         self.use_lock_for_reseting_jwt = use_lock_for_reseting_jwt
         self.max_retries = max_retries
@@ -256,35 +277,60 @@
         r = self.session.get(self.getURL() + "/version")
         data = r.json()
         if r.status_code == 200 and not "error" in data:
             return data
         else:
             raise CreationError(data["errorMessage"], data)
 
+    def create_aikido_session(
+            self,
+            username,
+            password,
+            verify
+    ) -> AikidoSession:
+        return AikidoSession(
+            username=username,
+            password=password,
+            verify=verify,
+            single_session=True,
+            max_conflict_retries=self.max_conflict_retries,
+            max_retries=self.max_retries,
+            log_requests=False,
+            pool_maxsize=self.pool_maxsize
+        )
+
+    def create_grequest_session(
+            self,
+            username,
+            password,
+            verify
+    ):
+        from .gevent_session import AikidoSession_GRequests
+        return AikidoSession_GRequests(
+            username, password, self.arangoURL,
+            self.use_jwt_authentication,
+            self.use_lock_for_reseting_jwt,
+            self.max_retries,
+            verify
+        )
+
     def resetSession(self, username=None, password=None, verify=True):
         """resets the session"""
         self.disconnectSession()
         if self.use_grequests:
-            from .gevent_session import AikidoSession_GRequests
-            self.session = AikidoSession_GRequests(
-                username, password, self.arangoURL,
-                self.use_jwt_authentication,
-                self.use_lock_for_reseting_jwt, self.max_retries,
+            self.session = self.create_grequest_session(
+                username,
+                password,
                 verify
             )
         else:
-            # self.session = AikidoSession(username, password, verify, self.max_retries)
-            self.session = AikidoSession(
-                username=username,
-                password=password,
-                verify=verify,
-                single_session=True,
-                max_conflict_retries=self.max_conflict_retries,
-                max_retries=self.max_retries,
-                log_requests=False
+            self.session = self.create_aikido_session(
+                username,
+                password,
+                verify
             )
 
     def reload(self):
         """Reloads the database list.
         Because loading a database triggers the loading of all collections and graphs within,
         only handles are loaded when this function is called. The full databases are loaded on demand when accessed
         """
@@ -314,14 +360,18 @@
         else:
             raise CreationError(data["errorMessage"], r.content)
 
     def hasDatabase(self, name):
         """returns true/false wether the connection has a database by the name of 'name'"""
         return name in self.databases
 
+    def __contains__(self, name):
+        """Alias for hasDatabase"""
+        return self.hasDatabase(name)
+
     def __getitem__(self, dbName):
         """Collection[dbName] returns a database by the name of 'dbName', raises a KeyError if not found"""
         try:
             return self.databases[dbName]
         except KeyError:
             self.reload()
             try:
```

### Comparing `pyArango-2.0.1/pyArango/database.py` & `pyArango-2.0.2/pyArango/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,14 @@
         """returns true if the databse has a collection by the name of 'name'"""
         return name in self.collections
 
     def hasGraph(self, name):
         """returns true if the databse has a graph by the name of 'name'"""
         return name in self.graphs
 
-    def __contains__(self, name):
-        """if name in database"""
-        return self.hasCollection(name) or self.hasGraph(name)
-
     def dropAllCollections(self):
         """drops all public collections (graphs included) from the database"""
         for graph_name in self.graphs:
             self.graphs[graph_name].delete()
         for collection_name in self.collections:
             # Collections whose name starts with '_' are system collections
             if not collection_name.startswith('_'):
@@ -510,21 +506,29 @@
             return data
         else:
             raise TransactionError(data["errorMessage"], action, data)
 
     def __repr__(self):
         return "ArangoDB database: %s" % self.name
 
-    def __contains__(self, _id):
-        """allows to check if _id:str is the id of an existing document"""
-        col, key = _id.split('/')
-        try:
-            return key in self[col]
-        except KeyError:
-            return False
+    # def __contains__(self, name):
+        # """if name in database"""
+        # return self.hasCollection(name) or self.hasGraph(name)
+
+    def __contains__(self, name_or_id):
+        """allows to check if name_or_id:str is the id of an existing document"""
+        splid = name_or_id.split('/')
+        if len(splid) == 2:
+            col, key = splid
+            try:
+                return key in self[col]
+            except KeyError:
+                return False
+        else:
+            return self.hasCollection(name_or_id) or self.hasGraph(name_or_id)
 
     def __getitem__(self, collectionName):
         """use database[collectionName] to get a collection from the database"""
         try:
             return self.collections[collectionName]
         except KeyError:
             self.reload()
```

### Comparing `pyArango-2.0.1/pyArango/document.py` & `pyArango-2.0.2/pyArango/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json, types
-from .theExceptions import (CreationError, DeletionError, UpdateError, ValidationError, SchemaViolation, InvalidDocument, ArangoError)
+from .theExceptions import (CreationError, UniqueConstrainViolation, DeletionError, UpdateError, ValidationError, SchemaViolation, InvalidDocument, ArangoError)
 
 __all__ = ["DocumentStore", "Document", "Edge"]
 
 class DocumentStore(object):
     """Store all the data of a document in hierarchy of stores and handles validation.
     Does not store private information, these are in the document."""
 
@@ -301,15 +301,18 @@
                     self._rev = data['_rev']
                 else:
                     self.set(data)
             else:
                 if update:
                     raise UpdateError(data['errorMessage'], data)
                 else:
-                    raise CreationError(data['errorMessage'], data)
+                    if data["errorNum"] == 1210:
+                        raise UniqueConstrainViolation(data['errorMessage'], data)
+                    else:
+                        raise CreationError(data['errorMessage'], data)
 
             self.modified = False
 
         self._store.resetPatch()
 
     def forceSave(self, **docArgs):
         "saves even if the document has not been modified since the last save"
```

### Comparing `pyArango-2.0.1/pyArango/foxx.py` & `pyArango-2.0.2/pyArango/foxx.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/gevent_session.py` & `pyArango-2.0.2/pyArango/gevent_session.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/graph.py` & `pyArango-2.0.2/pyArango/graph.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/index.py` & `pyArango-2.0.2/pyArango/index.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/jwauth.py` & `pyArango-2.0.2/pyArango/jwauth.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/query.py` & `pyArango-2.0.2/pyArango/query.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/tasks.py` & `pyArango-2.0.2/pyArango/tasks.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/tests/doc_save_benchmark.py` & `pyArango-2.0.2/pyArango/tests/doc_save_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/tests/doc_save_bulk_benchmark.py` & `pyArango-2.0.2/pyArango/tests/doc_save_bulk_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/tests/tests.py` & `pyArango-2.0.2/pyArango/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/tests/validators_tests.py` & `pyArango-2.0.2/pyArango/tests/validators_tests.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/theExceptions.py` & `pyArango-2.0.2/pyArango/theExceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,21 @@
 class CreationError(pyArangoException):
     """Something went wrong when creating something"""
     def __init__(self, message, errors = None):
         if errors is None:
             errors = {}
         pyArangoException.__init__(self, message, errors)
 
+class UniqueConstrainViolation(CreationError):
+    """Violation of a unique key"""
+    def __init__(self, message, errors = None):
+        if errors is None:
+            errors = {}
+        CreationError.__init__(self, message, errors)
+
 class IndexError(pyArangoException):
     """wasn't able to get the index"""
     def __init__(self, message, errors = None):
         if errors is None:
             errors = {}
         pyArangoException.__init__(self, message, errors)
```

### Comparing `pyArango-2.0.1/pyArango/users.py` & `pyArango-2.0.2/pyArango/users.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango/validation.py` & `pyArango-2.0.2/pyArango/validation.py`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/pyArango.egg-info/PKG-INFO` & `pyArango-2.0.2/pyArango.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyArango
-Version: 2.0.1
+Version: 2.0.2
 Summary: An easy to use python driver for ArangoDB with built-in validation
 Home-page: https://github.com/tariqdaouda/pyArango
 Author: Tariq Daouda
 Author-email: tariq.daouda@umontreal.ca
 License: ApacheV2
-Description: Python Object Wrapper for ArangoDB_ with built-in validation
-        =============================================================
-        
-        pyArango aims to be an easy to use driver for ArangoDB with built in validation. Collections are treated as types that apply to the documents within. You can be 100% permissive or enforce schemas and validate fields on set, on save or on both.
-        
-        pyArango supports graphs, indexes and probably everything that arangodb_ can do.
-        
-        pyArango is developed by `Tariq Daouda`_, the full source code is available from github_.
-        
-        .. _Tariq Daouda: http://bioinfo.iric.ca/~daoudat/
-        .. _github: https://github.com/tariqdaouda/pyArango
-        .. _arangodb: http://www.arangodb.com
-        .. _ArangoDB: http://www.arangodb.com
-        
-        For the latest news about pyArango, you can follow me on twitter `@tariqdaouda`_.
-        If you have any issues with it, please file a github issue.
-        
-        .. _@tariqdaouda: https://www.twitter.com/tariqdaouda
-        
 Keywords: database ORM nosql arangodb driver validation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+Python Object Wrapper for ArangoDB_ with built-in validation
+=============================================================
+
+pyArango aims to be an easy to use driver for ArangoDB with built in validation. Collections are treated as types that apply to the documents within. You can be 100% permissive or enforce schemas and validate fields on set, on save or on both.
+
+pyArango supports graphs, indexes and probably everything that arangodb_ can do.
+
+pyArango is developed by `Tariq Daouda`_, the full source code is available from github_.
+
+.. _Tariq Daouda: http://bioinfo.iric.ca/~daoudat/
+.. _github: https://github.com/tariqdaouda/pyArango
+.. _arangodb: http://www.arangodb.com
+.. _ArangoDB: http://www.arangodb.com
+
+For the latest news about pyArango, you can follow me on twitter `@tariqdaouda`_.
+If you have any issues with it, please file a github issue.
+
+.. _@tariqdaouda: https://www.twitter.com/tariqdaouda
```

### Comparing `pyArango-2.0.1/pyArango.egg-info/SOURCES.txt` & `pyArango-2.0.2/pyArango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyArango-2.0.1/setup.py` & `pyArango-2.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Get the long description from the relevant file
 with open(path.join(here, 'DESCRIPTION.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyArango',
 
-    version='2.0.1',
+    version='2.0.2',
 
     description='An easy to use python driver for ArangoDB with built-in validation',
     long_description=long_description,
 
     url='https://github.com/tariqdaouda/pyArango',
 
     author='Tariq Daouda',
```

