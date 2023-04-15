# Comparing `tmp/traducteur-0.4.6.tar.gz` & `tmp/traducteur-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traducteur-0.4.6.tar", max compression
+gzip compressed data, was "traducteur-0.4.7.tar", max compression
```

## Comparing `traducteur-0.4.6.tar` & `traducteur-0.4.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-04-15 10:09:31.889888 traducteur-0.4.6/LICENSE
--rw-r--r--   0        0        0     3588 2023-04-15 10:09:31.889888 traducteur-0.4.6/README.md
--rw-r--r--   0        0        0      756 2023-04-15 10:09:31.889888 traducteur-0.4.6/pyproject.toml
--rw-r--r--   0        0        0       37 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/__init__.py
--rw-r--r--   0        0        0      253 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/base.py
--rw-r--r--   0        0        0      606 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/mongo.py
--rw-r--r--   0        0        0      523 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/context/sqlite.py
--rw-r--r--   0        0        0       71 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/exceptions/tasks/__init__.py
--rw-r--r--   0        0        0       40 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/exceptions/tasks/base.py
--rw-r--r--   0        0        0       46 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/exceptions/tasks/worker.py
--rw-r--r--   0        0        0       34 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/__init__.py
--rw-r--r--   0        0        0      189 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/base.py
--rw-r--r--   0        0        0      264 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/base.py
--rw-r--r--   0        0        0      206 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/__init__.py
--rw-r--r--   0        0        0       73 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/base.py
--rw-r--r--   0        0        0      133 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/boolean_filter.py
--rw-r--r--   0        0        0      204 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/datetime_filter.py
--rw-r--r--   0        0        0      133 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/exists_filter.py
--rw-r--r--   0        0        0      189 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/number_filter.py
--rw-r--r--   0        0        0      229 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/filters/types/string_filter.py
--rw-r--r--   0        0        0     3041 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/mongo.py
--rw-r--r--   0        0        0       33 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/query/__init__.py
--rw-r--r--   0        0        0     6040 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/query/sql.py
--rw-r--r--   0        0        0     2410 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/managers/sql.py
--rw-r--r--   0        0        0       68 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/models/base/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-15 10:09:31.893888 traducteur-0.4.6/traducteur/models/base/base.py
--rw-r--r--   0        0        0      731 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/base/database.py
--rw-r--r--   0        0        0     2942 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/document/mongo.py
--rw-r--r--   0        0        0      676 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/document/redis.py
--rw-r--r--   0        0        0     2572 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/models/relational/sql.py
--rw-r--r--   0        0        0       27 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/base.py
--rw-r--r--   0        0        0      548 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/lifetime.py
--rw-r--r--   0        0        0      130 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/base/status.py
--rw-r--r--   0        0        0       28 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/task/__init__.py
--rw-r--r--   0        0        0     1991 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/task/redis.py
--rw-r--r--   0        0        0      103 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/worker/base.py
--rw-r--r--   0        0        0     1138 2023-04-15 10:09:31.897889 traducteur-0.4.6/traducteur/tasks/worker/redis.py
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-15 10:43:30.354752 traducteur-0.4.7/LICENSE
+-rw-r--r--   0        0        0     3588 2023-04-15 10:43:30.354752 traducteur-0.4.7/README.md
+-rw-r--r--   0        0        0      756 2023-04-15 10:43:30.354752 traducteur-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/context/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/context/base.py
+-rw-r--r--   0        0        0      606 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/context/mongo.py
+-rw-r--r--   0        0        0      523 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/context/sqlite.py
+-rw-r--r--   0        0        0       71 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/exceptions/tasks/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/exceptions/tasks/base.py
+-rw-r--r--   0        0        0       46 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/exceptions/tasks/worker.py
+-rw-r--r--   0        0        0       34 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/base.py
+-rw-r--r--   0        0        0      264 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/base.py
+-rw-r--r--   0        0        0      206 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/base.py
+-rw-r--r--   0        0        0      133 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/boolean_filter.py
+-rw-r--r--   0        0        0      204 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/datetime_filter.py
+-rw-r--r--   0        0        0      133 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/exists_filter.py
+-rw-r--r--   0        0        0      189 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/number_filter.py
+-rw-r--r--   0        0        0      229 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/filters/types/string_filter.py
+-rw-r--r--   0        0        0     3041 2023-04-15 10:43:30.354752 traducteur-0.4.7/traducteur/managers/mongo.py
+-rw-r--r--   0        0        0       33 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/managers/query/__init__.py
+-rw-r--r--   0        0        0     6040 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/managers/query/sql.py
+-rw-r--r--   0        0        0     2410 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/managers/sql.py
+-rw-r--r--   0        0        0       68 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/models/base/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/models/base/base.py
+-rw-r--r--   0        0        0      731 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/models/base/database.py
+-rw-r--r--   0        0        0     2942 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/models/document/mongo.py
+-rw-r--r--   0        0        0      689 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/models/document/redis.py
+-rw-r--r--   0        0        0     2572 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/models/relational/sql.py
+-rw-r--r--   0        0        0       27 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/base/__init__.py
+-rw-r--r--   0        0        0     1407 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/base/base.py
+-rw-r--r--   0        0        0      548 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/base/lifetime.py
+-rw-r--r--   0        0        0      130 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/base/status.py
+-rw-r--r--   0        0        0       28 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/task/__init__.py
+-rw-r--r--   0        0        0     1997 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/task/redis.py
+-rw-r--r--   0        0        0      103 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/worker/base.py
+-rw-r--r--   0        0        0     1287 2023-04-15 10:43:30.358752 traducteur-0.4.7/traducteur/tasks/worker/redis.py
+-rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.7/PKG-INFO
```

### Comparing `traducteur-0.4.6/LICENSE` & `traducteur-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/README.md` & `traducteur-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/pyproject.toml` & `traducteur-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "traducteur"
-version = "0.4.6"
+version = "0.4.7"
 description = "Traducteur is the middle man to handle your basic data needs."
 authors = ["Seppe De Langhe <seppedelanghe@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.4"
```

### Comparing `traducteur-0.4.6/traducteur/context/mongo.py` & `traducteur-0.4.7/traducteur/context/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/context/sqlite.py` & `traducteur-0.4.7/traducteur/context/sqlite.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/managers/mongo.py` & `traducteur-0.4.7/traducteur/managers/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/managers/query/sql.py` & `traducteur-0.4.7/traducteur/managers/query/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/managers/sql.py` & `traducteur-0.4.7/traducteur/managers/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/models/base/base.py` & `traducteur-0.4.7/traducteur/models/base/base.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/models/base/database.py` & `traducteur-0.4.7/traducteur/models/base/database.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/models/document/mongo.py` & `traducteur-0.4.7/traducteur/models/document/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/models/document/redis.py` & `traducteur-0.4.7/traducteur/models/document/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     @classmethod
     def get(cls, uuid: str):
         r = cls.redis_instance()
         out = r.get(uuid)
         return cls.from_json(out) if isinstance(out, bytes) else None
 
     def save(self):
-        r = self.redis_instance()
+        r: redis.Redis = self.redis_instance()
         r.set(self.id, self.json(), ex=float(os.environ.get('REDIS_TTL', '86400')))
         return self
 
     def delete(self):
         r = self.redis_instance()
         r.delete(self.id)
```

### Comparing `traducteur-0.4.6/traducteur/models/relational/sql.py` & `traducteur-0.4.7/traducteur/models/relational/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/tasks/base/base.py` & `traducteur-0.4.7/traducteur/tasks/base/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import marshal, types
 import logging
 
 from typing import Optional, Callable, Union
 
 from .status import TaskStatus
 from .lifetime import TaskLifetime
 from ...models.base import BaseModel
-from ...exceptions.tasks import TaskException
 
 
 class BaseTask(BaseModel):
     action: Callable
     status: TaskStatus = TaskStatus.NONE
     lifetime: TaskLifetime = TaskLifetime()
     tin: Optional[dict] = None
```

### Comparing `traducteur-0.4.6/traducteur/tasks/base/lifetime.py` & `traducteur-0.4.7/traducteur/tasks/base/lifetime.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.6/traducteur/tasks/task/redis.py` & `traducteur-0.4.7/traducteur/tasks/task/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Optional
 
 import dill as pickle
 from ..base import BaseTask
-from ...models.document import BaseRedisModel
+from ...models.document.redis import BaseRedisModel
 
 
 class RedisTask(BaseTask, BaseRedisModel):
     channel: str
 
     def queue(self, **kwargs):
         self._queue_children()
```

### Comparing `traducteur-0.4.6/traducteur/tasks/worker/redis.py` & `traducteur-0.4.7/traducteur/tasks/worker/redis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import redis
 import time
+import logging
 
 from typing import Optional
 
 from .base import BaseTaskWorker
 from ..task.redis import RedisTask
 from ...exceptions.tasks import TaskWorkerException
 
@@ -20,18 +21,20 @@
         self.r = redis.Redis(**kwargs)
 
     def listen(self):
         sub = self.r.pubsub()
         sub.subscribe(self.channel)
 
         while True:
-            message: Optional[str] = sub.get_message()
-            if isinstance(message, str):
-                message: dict = json.loads(message)
-                task: Optional[bytes] = self.r.get(message['id'])
+            message: Optional[dict] = sub.get_message()
+            if isinstance(message, dict) and message['type'] == 'message':
+                data = json.loads(message['data'])
+                task: Optional[bytes] = self.r.get(data['id'])
                 if isinstance(task, bytes):
                     task: RedisTask = RedisTask.unpickle(task)
                     task.digest()
+                    if task.status == 5:
+                        logging.error(task.lifetime.error)
                 elif self.throws:
-                    raise TaskWorkerException(f"Got message for new task, but no task found with uuid: {message['id']}!")
+                    raise TaskWorkerException(f"Got message for new task, but no task found with uuid: {message['data']}!")
 
-            time.sleep(self.idle)
+            time.sleep(self.idle)
```

### Comparing `traducteur-0.4.6/PKG-INFO` & `traducteur-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traducteur
-Version: 0.4.6
+Version: 0.4.7
 Summary: Traducteur is the middle man to handle your basic data needs.
 Author: Seppe De Langhe
 Author-email: seppedelanghe@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

