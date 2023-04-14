# Comparing `tmp/caliper-reader-0.3.0.tar.gz` & `tmp/caliper-reader-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/boehme3/tmp/caliper-reader/dist/tmp7wv8ochr/caliper-reader-0.3.0.tar", last modified: Thu Jul 22 22:03:09 2021, max compression
+gzip compressed data, was "caliper-reader-0.4.0.tar", last modified: Fri Apr 14 23:25:39 2023, max compression
```

## Comparing `caliper-reader-0.3.0.tar` & `caliper-reader-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 boehme3  (37937)    37937        0 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/
--rw-r--r--   0 boehme3  (37937)    37937     1525 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/LICENSE
--rw-r--r--   0 boehme3  (37937)    37937     2757 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/PKG-INFO
--rw-r--r--   0 boehme3  (37937)    37937     2334 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/README.md
-drwxr-xr-x   0 boehme3  (37937)    37937        0 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/caliper_reader.egg-info/
--rw-r--r--   0 boehme3  (37937)    37937     2757 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/caliper_reader.egg-info/PKG-INFO
--rw-r--r--   0 boehme3  (37937)    37937      354 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/caliper_reader.egg-info/SOURCES.txt
--rw-r--r--   0 boehme3  (37937)    37937        1 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/caliper_reader.egg-info/dependency_links.txt
--rw-r--r--   0 boehme3  (37937)    37937       14 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/caliper_reader.egg-info/top_level.txt
-drwxr-xr-x   0 boehme3  (37937)    37937        0 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/caliperreader/
--rw-r--r--   0 boehme3  (37937)    37937      289 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/caliperreader/__init__.py
--rw-r--r--   0 boehme3  (37937)    37937     3046 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/caliperreader/caliperreader.py
--rw-r--r--   0 boehme3  (37937)    37937     4980 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/caliperreader/caliperstreamreader.py
--rw-r--r--   0 boehme3  (37937)    37937     6631 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/caliperreader/metadatadb.py
--rw-r--r--   0 boehme3  (37937)    37937      244 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/caliperreader/readererror.py
--rw-r--r--   0 boehme3  (37937)    37937      226 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/caliperreader/version.py
--rw-r--r--   0 boehme3  (37937)    37937       38 2021-07-22 22:03:09.000000 caliper-reader-0.3.0/setup.cfg
--rw-r--r--   0 boehme3  (37937)    37937     1209 2021-07-22 22:01:27.000000 caliper-reader-0.3.0/setup.py
+drwxr-xr-x   0 david     (1000) users      (100)        0 2023-04-14 23:25:39.949658 caliper-reader-0.4.0/
+-rw-r--r--   0 david     (1000) users      (100)     1525 2022-08-04 05:16:48.000000 caliper-reader-0.4.0/LICENSE
+-rw-r--r--   0 david     (1000) users      (100)     4591 2023-04-14 23:25:39.949658 caliper-reader-0.4.0/PKG-INFO
+-rw-r--r--   0 david     (1000) users      (100)     2334 2022-08-04 05:16:48.000000 caliper-reader-0.4.0/README.md
+drwxr-xr-x   0 david     (1000) users      (100)        0 2023-04-14 23:25:39.937658 caliper-reader-0.4.0/caliper_reader.egg-info/
+-rw-r--r--   0 david     (1000) users      (100)     4591 2023-04-14 23:25:39.000000 caliper-reader-0.4.0/caliper_reader.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) users      (100)      381 2023-04-14 23:25:39.000000 caliper-reader-0.4.0/caliper_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) users      (100)        1 2023-04-14 23:25:39.000000 caliper-reader-0.4.0/caliper_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) users      (100)       14 2023-04-14 23:25:39.000000 caliper-reader-0.4.0/caliper_reader.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) users      (100)        0 2023-04-14 23:25:39.949658 caliper-reader-0.4.0/caliperreader/
+-rw-r--r--   0 david     (1000) users      (100)      289 2022-08-04 05:16:48.000000 caliper-reader-0.4.0/caliperreader/__init__.py
+-rw-r--r--   0 david     (1000) users      (100)     3046 2022-08-04 05:16:48.000000 caliper-reader-0.4.0/caliperreader/caliperreader.py
+-rw-r--r--   0 david     (1000) users      (100)     4547 2023-04-14 21:36:28.000000 caliper-reader-0.4.0/caliperreader/caliperstreamreader.py
+-rw-r--r--   0 david     (1000) users      (100)     8180 2023-04-14 21:36:28.000000 caliper-reader-0.4.0/caliperreader/metadatadb.py
+-rw-r--r--   0 david     (1000) users      (100)      244 2022-08-04 05:16:48.000000 caliper-reader-0.4.0/caliperreader/readererror.py
+-rw-r--r--   0 david     (1000) users      (100)      226 2023-04-14 22:57:47.000000 caliper-reader-0.4.0/caliperreader/version.py
+-rw-r--r--   0 david     (1000) users      (100)      597 2023-04-14 23:15:30.000000 caliper-reader-0.4.0/pyproject.toml
+-rw-r--r--   0 david     (1000) users      (100)       38 2023-04-14 23:25:39.949658 caliper-reader-0.4.0/setup.cfg
+drwxr-xr-x   0 david     (1000) users      (100)        0 2023-04-14 23:25:39.949658 caliper-reader-0.4.0/tests/
+-rw-r--r--   0 david     (1000) users      (100)     3324 2022-08-04 05:16:48.000000 caliper-reader-0.4.0/tests/test_reader.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `caliper-reader-0.3.0/LICENSE` & `caliper-reader-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caliper-reader-0.3.0/PKG-INFO` & `caliper-reader-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: caliper-reader
-Version: 0.3.0
-Summary: A Python library for reading Caliper .cali files
-Home-page: https://github.com/LLNL/Caliper
-Author: David Boehme
-Author-email: boehme3@llnl.gov
-License: BSD-3-Clause
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 caliper-reader: A Python reader for Caliper files
 =================================================
 
 This Python package reads the native .cali files produced by the
 [Caliper](https://github.com/LLNL/Caliper) performance profiling
 library.
 
@@ -86,9 +72,8 @@
 
 Release
 -------------------------------------
 
 Caliper is released under a BSD 3-clause license.
 See [LICENSE](LICENSE) for details.
 
-``LLNL-CODE-678900``
-
+``LLNL-CODE-678900``
```

### Comparing `caliper-reader-0.3.0/caliperreader/caliperreader.py` & `caliper-reader-0.4.0/caliperreader/caliperreader.py`

 * *Files identical despite different names*

### Comparing `caliper-reader-0.3.0/caliperreader/caliperstreamreader.py` & `caliper-reader-0.4.0/caliperreader/caliperstreamreader.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,81 +98,64 @@
 
 
     def _expand_record(self, record):
         result = {}
 
         if 'ref' in record:
             for node_id in record['ref']:
-                for k, v in self._expand_node(int(node_id)).items():
-                    if len(v) > 1:
-                        result[k] = v
-                    else:
-                        result[k] = v[0]
+                result.update(self.db.nodes[int(node_id)].expand())
 
         if 'attr' in record and 'data' in record:
             for attr_id, val in zip(record['attr'], record['data']):
-                attr = Attribute(self.db.nodes[int(attr_id)])
+                attr = self.db.attributes_by_id[int(attr_id)]
                 if not attr.is_hidden():
                     result[attr.name()] = val
 
         return result
 
 
-    def _expand_node(self, node_id):
-        def add(result, key, data):
-            if key not in result:
-                result[key] = []
-            result[key].insert(0, data)
-
-        result = {}
-        node = self.db.nodes[node_id]
-
-        while node is not None:
-            attr = node.attribute()
+def _read_cali_record(line):
+    """ Splits comma-separated Caliper record line into constituent elements
 
-            if not attr.is_hidden():
-                add(result, attr.name(), node.data)
-                if attr.is_nested():
-                    add(result, 'path', node.data)
+        A .cali line has the form
 
-            node = node.parent
+          "__rec=ctx,ref=42=4242,attr=1=2=3,data=11=22=33"
 
-        return result
+        This function splits this into a key-list dict like so:
 
+          {
+            "__rec" : [ "ctx" ],
+            "ref"   : [ "42", "4242" ],
+            "attr"  : [ "1", "2", "3" ],
+            "data"  : [ "11", "22", "33" ]
+          }
 
-def _split_escape_string(input, keep_escape = True, splitchar = ',', escapechar = '\\'):
-    """ Splits a string but allows escape characters """
+        We need to deal with possibly escaped characters in strings so we
+        can't just use str.split().
+    """
 
-    results = []
+    result  = {}
+    entry   = []
     string  = ""
-    escaped = False
 
-    for c in input:
-        if not escaped and c == escapechar:
-            escaped = True
-            if keep_escape:
-                string += c
-        elif not escaped and c == splitchar:
-            results.append(string)
+    iterator = iter(line.strip())
+
+    for c in iterator:
+        if c == '\\':
+            c = next(iterator)
+            string += c
+        elif c == ',':
+            entry.append(string)
+            result[entry[0]] = entry[1:]
+            string = ""
+            entry  = []
+        elif c == '=':
+            entry.append(string)
             string = ""
         else:
             string += c
-            escaped = False
-
-    results.append(string)
-
-    return results
-
-
-def _read_cali_record(line):
-    record  = {}
-    entries = _split_escape_string(line.strip())
-
-    for e in entries:
-        kv = _split_escape_string(e, False, '=')
-
-        if len(kv) < 1:
-            raise ReaderError('Invalid record: {}'.format(line))
 
-        record[kv[0]] = kv[1:]
+    if len(string) > 0:
+        entry.append(string)
+        result[entry[0]] = entry[1:]
 
-    return record
+    return result
```

### Comparing `caliper-reader-0.3.0/caliperreader/metadatadb.py` & `caliper-reader-0.4.0/caliperreader/metadatadb.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
         self.id           = id
         self.attribute_id = attribute_id
         self.data         = data
 
         self.metadb       = metadb
 
+        self.attribute_ob = None
+        self.record       = None
 
     def append(self, child):
         """ Append a child node to this node.
         """
 
         child.parent = self
         self.children.append(child)
@@ -44,16 +46,51 @@
             node = node.parent
 
         return node.data if node else None
 
     def attribute(self):
         """ Return the Caliper attribute object for this node.
         """
-        return Attribute(self.metadb.nodes[self.attribute_id])
+        if self.attribute_ob is None:
+            self.attribute_ob = Attribute(self.metadb.nodes[self.attribute_id])
 
+        return self.attribute_ob
+
+    def expand(self):
+        """ Return the expanded dict for this node.
+        """
+
+        if self.record is None:
+            self.record = self._expand()
+
+        return self.record
+
+    def _expand(self):
+        record = {}
+
+        if self.parent is not None:
+            record.update(self.parent.expand())
+
+        attr = self.attribute()
+
+        if not attr.is_hidden():
+            key = attr.name()
+            val = record.get(key)
+
+            if val is None:
+                record[key] = self.data
+            elif isinstance(val, list):
+                record[key] = val + [ self.data ]
+            else:
+                record[key] = [ val, self.data ]
+
+            if attr.is_nested():
+                record['path'] = record.get('path', []) + [ self.data ]
+
+        return record
 
 class Attribute:
     """ A Caliper attribute key.
 
     Provides information about Caliper attribute keys.
     """
 
@@ -61,26 +98,27 @@
     type_attribute_id =   9
     prop_attribute_id =  10
 
     CALI_ATTR_ASVALUE =   1
     CALI_ATTR_HIDDEN  = 128
     CALI_ATTR_NESTED  = 256
     CALI_ATTR_GLOBAL  = 512
+    CALI_ATTR_AGGREGATABLE = 2048
 
     SCOPE_PROCESS     =  12
     SCOPE_THREAD      =  20
     SCOPE_TASK        =  24
 
     SCOPE_MASK        =  60
 
     def __init__(self, node):
-        prop = node.get(self.prop_attribute_id)
+        prop = node.parent.get(self.prop_attribute_id)
 
         self.node = node
-        self.prop = int(prop) if prop is not None else 0
+        self.prop = 0 if prop is None else int(prop)
 
     def name(self):
         """ Return the name of the Caliper attribute. """
         return self.node.data
 
     def id(self):
         """ Return the node ID of the Caliper attribute. """
@@ -134,14 +172,20 @@
 
     def is_hidden(self):
         """ Is this a hidden attribute?
         """
 
         return (self.prop & self.CALI_ATTR_HIDDEN) != 0
 
+    def is_aggregatable(self):
+        """ Is this an aggregatable attribute (i.e., a metric)?
+        """
+
+        return (self.prop & self.CALI_ATTR_AGGREGATABLE) != 0
+
     def scope(self):
         """ Returns the attribute's scope ("process", "thread", or "task")
         """
 
         scopemap = {
             self.SCOPE_THREAD  : "thread"  ,
             self.SCOPE_PROCESS : "process" ,
@@ -155,14 +199,16 @@
         """
 
         node = self.node
         result = {
             "is_global" : self.is_global() ,
             "is_value"  : self.is_value()  ,
             "is_nested" : self.is_nested() ,
+            "is_aggregatable"    : self.is_aggregatable() ,
+            "class.aggregatable" : self.is_aggregatable() , # legacy support
             "type"      : self.attribute_type()
         }
 
         while node is not None:
             result[node.attribute().name()] = node.data
             node = node.parent
 
@@ -205,24 +251,31 @@
         }
 
         # Append bootstrap node children to parents
         self.nodes[3].append(self.nodes[ 8])
         self.nodes[7].append(self.nodes[ 9])
         self.nodes[1].append(self.nodes[10])
 
-        # Initialize the attributes dict
+        # Initialize the attribute dicts
         self.attributes = {
             'cali.attribute.name': Attribute(self.nodes[ 8]),
             'cali.attribute.type': Attribute(self.nodes[ 9]),
             'cali.attribute.prop': Attribute(self.nodes[10])
         }
 
+        self.attributes_by_id = {
+             8: Attribute(self.nodes[ 8]),
+             9: Attribute(self.nodes[ 9]),
+            10: Attribute(self.nodes[10])
+        }
 
     def import_node(self, node_id, attribute_id, data, parent_id = Node.CALI_INV_ID):
         node = Node(self, node_id, attribute_id, data)
         self.nodes[node_id] = node
 
         if parent_id in self.nodes:
             self.nodes[parent_id].append(node)
 
         if attribute_id == Attribute.attr_attribute_id:
-            self.attributes[data] = Attribute(node)
+            attr = Attribute(node)
+            self.attributes[data] = attr
+            self.attributes_by_id[node_id] = attr
```

