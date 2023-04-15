# Comparing `tmp/np_queuey-0.1.0.tar.gz` & `tmp/np_queuey-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.1.0.tar", last modified: Fri Apr 14 06:35:34 2023, max compression
+gzip compressed data, was "np_queuey-0.1.1.tar", last modified: Sat Apr 15 00:22:18 2023, max compression
```

## Comparing `np_queuey-0.1.0.tar` & `np_queuey-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.0/README.md
--rw-r--r--   0        0        0     2284 2023-04-14 06:35:34.307852 np_queuey-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.0/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.0/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     3927 2023-04-14 06:34:44.441332 np_queuey-0.1.0/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.0/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6580 2023-04-14 03:02:37.309842 np_queuey-0.1.0/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0     3019 2023-04-13 23:41:51.924236 np_queuey-0.1.0/src/np_queuey/queues.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.0/src/np_queuey/tasks.py
--rw-r--r--   0        0        0      138 2023-04-14 05:38:58.270331 np_queuey-0.1.0/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.0/tests/test_huey.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.1/README.md
+-rw-r--r--   0        0        0     2357 2023-04-15 00:22:18.421726 np_queuey-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.1/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.1/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     8490 2023-04-15 00:21:39.512663 np_queuey-0.1.1/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.1/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6771 2023-04-15 00:21:38.677120 np_queuey-0.1.1/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      245 2023-04-15 00:21:39.508662 np_queuey-0.1.1/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0     3019 2023-04-13 23:41:51.924236 np_queuey-0.1.1/src/np_queuey/queues.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.1/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.1/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.1/tests/test_huey.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.1/PKG-INFO
```

### Comparing `np_queuey-0.1.0/pyproject.toml` & `np_queuey-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,63 @@
+[project]
+name = "np_queuey"
+version = "0.1.1"
+description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
+authors = [
+    { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
+]
+dependencies = [
+    "huey>=2.4.5",
+    "np-config>=0.4.17",
+    "np-logging>=0.5.1",
+    "np-tools>=0.1.0",
+    "np-session>=0.5.1",
+]
+requires-python = ">=3.8"
+readme = "README.md"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+]
+
+[project.license]
+text = "MIT"
+
+[project.scripts]
+run_small_jobs = "np_queuey.jobs.run_small_jobs:main"
+
+[project.urls]
+Repository = "https://github.com/AllenInstitute/np_queuey"
+"Bug Tracker" = "https://github.com/AllenInstitute/np_queuey/issues"
+
+[project.optional-dependencies]
+dev = [
+    "blue>=0.9.1",
+    "pytest>=7.2.2",
+    "mypy>=1.1.1",
+    "coverage[toml]>=7.2.2",
+    "pdm>=2.4.9",
+    "pytest-cov>=4.0.0",
+    "bump>=1.3.2",
+    "types-backports>=0.1.3",
+    "ruff>=0.0.260",
+]
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
 [tool.pdm.scripts]
 ruff = "ruff --fix src"
 blue = "blue src"
 pytest = "pytest --cov"
 bump = "pdm bump patch"
 
 [tool.pdm.scripts.prebuild]
@@ -58,60 +114,7 @@
 branch = true
 source = [
     "np_queuey",
 ]
 
 [tool.coverage.report]
 show_missing = true
-
-[project]
-name = "np_queuey"
-version = "0.1.0"
-description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
-authors = [
-    { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
-]
-dependencies = [
-    "huey>=2.4.5",
-    "np-config>=0.4.17",
-    "np-logging>=0.5.1",
-    "np-tools>=0.1.0",
-    "np-session>=0.5.1",
-]
-requires-python = ">=3.8"
-readme = "README.md"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
-]
-
-[project.license]
-text = "MIT"
-
-[project.urls]
-Repository = "https://github.com/AllenInstitute/np_queuey"
-"Bug Tracker" = "https://github.com/AllenInstitute/np_queuey/issues"
-
-[project.optional-dependencies]
-dev = [
-    "blue>=0.9.1",
-    "pytest>=7.2.2",
-    "mypy>=1.1.1",
-    "coverage[toml]>=7.2.2",
-    "pdm>=2.4.9",
-    "pytest-cov>=4.0.0",
-    "bump>=1.3.2",
-    "types-backports>=0.1.3",
-    "ruff>=0.0.260",
-]
-
-[build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
```

### Comparing `np_queuey-0.1.0/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.1/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,56 +16,73 @@
 import sqlite3
 
 DB_PATH = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/.tasks.db'
 SESSION_UPLOAD_TABLE = 'behavior_session_mtrain_upload_queue'
 COLUMNS_TO_DEFINITIONS = {
     'foraging_id': 'TEXT PRIMARY KEY NOT NULL',
     'filename': 'TEXT NOT NULL',
-    'added': 'TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL',  #YYYY-MM-DD HH:MM:SS
+    'added': 'TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL',  # YYYY-MM-DD HH:MM:SS
     'processing': 'INTEGER',  # [None] 0 or 1
     'uploaded': 'INTEGER',  # [None] 0 or 1
 }
 
+
 def table_sql(column_name_to_definition_mapping):
     """
     >>> table_sql({'col1': 'TEXT PRIMARY KEY NOT NULL', 'col2': 'INTEGER'})
     '(col1 TEXT PRIMARY KEY NOT NULL, col2 INTEGER)'
     """
-    return '(' + ', '.join([f'{col} {defn}' for col, defn in column_name_to_definition_mapping.items()]) + ')'
+    return (
+        '('
+        + ', '.join(
+            [
+                '{} {}'.format(col, defn)
+                for col, defn in column_name_to_definition_mapping.items()
+            ]
+        )
+        + ')'
+    )
+
 
 def initialize_mtrain_upload_queue_in_db():
     """
     >>> initialize_mtrain_upload_queue_in_db()
     """
     with task_db_cursor() as c:
         c.execute(
-            'CREATE TABLE IF NOT EXISTS behavior_session_mtrain_upload_queue ' + table_sql(COLUMNS_TO_DEFINITIONS)
+            'CREATE TABLE IF NOT EXISTS behavior_session_mtrain_upload_queue '
+            + table_sql(COLUMNS_TO_DEFINITIONS)
         )
 
+
 def parse_filename(filename):
     """
     >>> (task, mouse_id, date, time) = parse_filename('DynamicRouting1_664566_20230328_151155.hdf5')
     >>> '_'.join((task, mouse_id, date, time))
     'DynamicRouting1_664566_20230328_151155'
     """
     return filename.split('.')[0].split('_')
 
+
 def add_behavior_session_to_mtrain_upload_queue(foraging_id, filename):
     """
     >>> add_behavior_session_to_mtrain_upload_queue('test', 'test.hdf5')
     >>> with task_db_cursor() as c:
     ...   sessions = c.execute('SELECT * FROM behavior_session_mtrain_upload_queue').fetchall()
     ...   assert 'test' in (s[0] for s in sessions), 'Test foraging_id = test not added to db'
     >>> add_behavior_session_to_mtrain_upload_queue('test', 'test.hdf5') # accidental repeat should not raise
     """
     initialize_mtrain_upload_queue_in_db()
     with task_db_cursor() as c:
         c.execute(
             'INSERT OR IGNORE INTO behavior_session_mtrain_upload_queue (foraging_id, filename) VALUES (?, ?)',
-            (foraging_id, filename,),
+            (
+                foraging_id,
+                filename,
+            ),
         )
 
 
 def dynamic_routing_task_db():
     """
     >>> conn = dynamic_routing_task_db()
     >>> _ = conn.cursor()
@@ -91,15 +108,14 @@
         raise
     else:
         conn.commit()
     finally:
         cursor.close()
 
 
-
 def remove_behavior_session_from_mtrain_upload_queue(foraging_id):
     """
     >>> remove_behavior_session_from_mtrain_upload_queue('test')
     >>> with task_db_cursor() as c:
     ...   sessions = c.execute('SELECT * FROM behavior_session_mtrain_upload_queue').fetchall()
     ...   assert 'test' not in (s[0] for s in sessions), 'Test foraging_id = "test" not removed from db'
     >>> remove_behavior_session_from_mtrain_upload_queue('test') # accidental repeat should not raise
@@ -134,15 +150,15 @@
     Sets processing = 1.
 
     >>> remove_behavior_session_from_mtrain_upload_queue('test')
     >>> add_behavior_session_to_mtrain_upload_queue('test', 'test.hdf5')
     >>> mark_behavior_session_as_processing('test')
     >>> with task_db_cursor() as c:
     ...   result = c.execute('SELECT processing FROM behavior_session_mtrain_upload_queue WHERE foraging_id = "test"').fetchall()[0][0]
-    ...   assert result == 1, f'Test result (processing, ) returned {result}: expected 1 (True)'
+    ...   assert result == 1, 'Test result (processing, ) returned {}: expected 1 (True)'.format(result)
     """
     with task_db_cursor() as c:
         c.execute(
             'UPDATE behavior_session_mtrain_upload_queue SET processing = 1 WHERE foraging_id = ?',
             (foraging_id,),
         )
 
@@ -152,19 +168,20 @@
     Sets processing to 0 and uploaded to 1.
 
     >>> remove_behavior_session_from_mtrain_upload_queue('test')
     >>> add_behavior_session_to_mtrain_upload_queue('test', 'test.hdf5')
     >>> mark_behavior_session_as_uploaded('test')
     >>> with task_db_cursor() as c:
     ...   result = c.execute('SELECT processing, uploaded FROM behavior_session_mtrain_upload_queue WHERE foraging_id = "test"').fetchall()[0]
-    ...   assert result == (0, 1), f'Test result (processing, uploaded) returned {result}: expected (0, 1) (False, True)'
+    ...   assert result == (0, 1), 'Test result (processing, uploaded) returned {}: expected (0, 1) (False, True)'.format(result)
     """
     with task_db_cursor() as c:
         c.execute(
             'UPDATE behavior_session_mtrain_upload_queue SET processing = 0, uploaded = 1 WHERE foraging_id = ?',
             (foraging_id,),
         )
 
 
 if __name__ == '__main__':
     import doctest
-    doctest.testmod(verbose=True, raise_on_error=False)
+
+    doctest.testmod(verbose=False, raise_on_error=False)
```

### Comparing `np_queuey-0.1.0/src/np_queuey/queues.py` & `np_queuey-0.1.1/src/np_queuey/queues.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.0/tests/test_huey.py` & `np_queuey-0.1.1/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.0/PKG-INFO` & `np_queuey-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

