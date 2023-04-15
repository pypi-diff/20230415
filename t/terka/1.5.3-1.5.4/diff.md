# Comparing `tmp/terka-1.5.3.tar.gz` & `tmp/terka-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.5.3.tar", last modified: Fri Apr 14 14:20:11 2023, max compression
+gzip compressed data, was "terka-1.5.4.tar", last modified: Sat Apr 15 18:33:04 2023, max compression
```

## Comparing `terka-1.5.3.tar` & `terka-1.5.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.234563 terka-1.5.3/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.5.3/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-14 14:20:11.234563 terka-1.5.3/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.5.3/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-14 14:20:11.234563 terka-1.5.3/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-14 14:20:02.000000 terka-1.5.3/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.230563 terka-1.5.3/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.3/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.230563 terka-1.5.3/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.3/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.5.3/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.5.3/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.230563 terka-1.5.3/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.3/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.5.3/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    36636 2023-04-13 22:07:45.000000 terka-1.5.3/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.5.3/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.5.3/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.5.3/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.5.3/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.5.3/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.5.3/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.5.3/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.5.3/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.5.3/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.5.3/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.5.3/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.5.3/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.230563 terka-1.5.3/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.5.3/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.5.3/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.230563 terka-1.5.3/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.3/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    28255 2023-04-14 14:14:44.000000 terka-1.5.3/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.5.3/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.5.3/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.5.3/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     7088 2023-04-13 19:08:12.000000 terka-1.5.3/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.230563 terka-1.5.3/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-14 14:20:11.000000 terka-1.5.3/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-14 14:20:11.000000 terka-1.5.3/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-14 14:20:11.000000 terka-1.5.3/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-14 14:20:11.000000 terka-1.5.3/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-14 14:20:11.000000 terka-1.5.3/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-14 14:20:11.000000 terka-1.5.3/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-14 14:20:11.234563 terka-1.5.3/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.3/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.5.3/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.5.3/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.5.3/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.5.3/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.5.3/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.5.3/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.860915 terka-1.5.4/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.5.4/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-15 18:33:04.860915 terka-1.5.4/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.5.4/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-15 18:33:04.860915 terka-1.5.4/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-15 18:32:59.000000 terka-1.5.4/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.856915 terka-1.5.4/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.4/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.856915 terka-1.5.4/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.4/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.5.4/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.5.4/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.856915 terka-1.5.4/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.4/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.5.4/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    36942 2023-04-15 18:14:56.000000 terka-1.5.4/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.5.4/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.5.4/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.5.4/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.5.4/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.5.4/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.5.4/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.5.4/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.5.4/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.5.4/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.5.4/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.5.4/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.5.4/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.856915 terka-1.5.4/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.5.4/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.5.4/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.856915 terka-1.5.4/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.4/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27681 2023-04-15 18:17:03.000000 terka-1.5.4/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.5.4/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.5.4/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.5.4/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     7088 2023-04-13 19:08:12.000000 terka-1.5.4/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.860915 terka-1.5.4/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-15 18:33:04.000000 terka-1.5.4/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-15 18:33:04.000000 terka-1.5.4/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-15 18:33:04.000000 terka-1.5.4/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-15 18:33:04.000000 terka-1.5.4/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-15 18:33:04.000000 terka-1.5.4/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-15 18:33:04.000000 terka-1.5.4/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 18:33:04.860915 terka-1.5.4/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.4/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.5.4/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.5.4/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.5.4/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.5.4/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.5.4/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.5.4/tests/test_utils.py
```

### Comparing `terka-1.5.3/LICENSE` & `terka-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/PKG-INFO` & `terka-1.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.5.3
+Version: 1.5.4
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.5.3/README.md` & `terka-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/setup.py` & `terka-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.5.3",
+    version="1.5.4",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.5.3/src/adapters/orm.py` & `terka-1.5.4/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/adapters/repository.py` & `terka-1.5.4/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/collaborators.py` & `terka-1.5.4/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/commands.py` & `terka-1.5.4/src/domain/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -786,25 +786,31 @@
                 self.execute("update", "tasks", task_params)
         elif command == "show":
             print_options = printer.PrintOptions(
                 show_history=bool(kwargs.get("show_history")),
                 show_commentaries=bool(kwargs.get("show_commentaries")),
                 show_completed=bool(kwargs.get("show_completed"))
             )
-            if (task_id := kwargs.get("id")):
-                tasks = get_ids(task_id)
-                for task in tasks:
-                    if task.isdigit():
-                        entities = self.repo.list(entity, {"id": task})
+            if not (task_id := kwargs.get("id")):
+                if entity_type == "sprints":
+                    active_sprint = self.repo.list(Sprint, {"status": "ACTIVE"})
+                    if len(active_sprint) == 1:
+                        task_id = active_sprint[0].id
                     else:
-                        entities = self.repo.list(entity, {"name": task})
-                    self.printer.print_entity(
-                        task, entity_type, entities, self.repo, print_options)
-                    logger.info("<show> %s: %s", entity_type, task_id)
-                return entities, None, None
+                        exit("More than 1 active sprint, please specify the sprint_id")
+            tasks = get_ids(task_id)
+            for task in tasks:
+                if task.isdigit():
+                    entities = self.repo.list(entity, {"id": task})
+                else:
+                    entities = self.repo.list(entity, {"name": task})
+                self.printer.print_entity(
+                    task, entity_type, entities, self.repo, print_options)
+                logger.info("<show> %s: %s", entity_type, task_id)
+            return entities, None, None
         elif command == "done":
             if entity_type not in ("tasks", "sprints"):
                 raise ValueError("can complete only tasks and sprints")
             elif entity_type == "tasks":
                 kwargs.update({"status": "DONE"})
                 self.execute("update", entity_type, kwargs)
                 self.console.print(
```

### Comparing `terka-1.5.3/src/domain/commentary.py` & `terka-1.5.4/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/epic.py` & `terka-1.5.4/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/event_history.py` & `terka-1.5.4/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/project.py` & `terka-1.5.4/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/sprint.py` & `terka-1.5.4/src/domain/sprint.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,40 +2,46 @@
 from enum import Enum
 import logging
 from datetime import datetime
 from dataclasses import dataclass
 
 from src.domain.task import Task
 
-
 logger = logging.getLogger(__name__)
 
 
 class SprintStatus(Enum):
     PLANNED = 1
     ACTIVE = 2
     COMPLETED = 3
 
 
 class Sprint:
 
     def __init__(self,
-                 start_date: datetime,
-                 end_date: datetime,
+                 start_date: datetime = None,
+                 end_date: datetime = None,
                  status: str = "PLANNED",
                  goal: str = None,
                  **kwargs) -> None:
-        # if start_date.date()  < datetime.today().date():
-        #     raise ValueError(f"start date {start_date.date()} cannot be less than today")
-        # else:
+        if start_date.date()  < datetime.today().date():
+            raise ValueError(f"start date cannot be less than today")
+        if not start_date:
+            raise ValueError(
+                "Please provide start date for the sprint in YYYY-MM-DD format"
+            )
         self.start_date = start_date
-        # if end_date.date()  < start_date:
-        #     raise ValueError(f"Sprint end date cannot be less than start date")
-        # else:
+        if not end_date:
+            raise ValueError(
+                "Please provide end date for the sprint in YYYY-MM-DD format")
         self.end_date = end_date
+        if end_date.date() < start_date.date():
+            raise ValueError(f"Sprint end date cannot be less than start date")
+        if end_date.date() < datetime.today().date():
+            raise ValueError(f"Sprint end date cannot be less than today")
         self.status = self._validate_status(status)
         self.goal = goal
         self.tasks: Set[Task, ...] = set()
         self.is_completed = False
 
     def _validate_status(self, status):
         if status and status not in [s.name for s in SprintStatus]:
@@ -57,8 +63,7 @@
 @dataclass
 class SprintTask:
     sprint: int
     task: int
     story_points: int = 0
     #TODO: add actual_time_spent: int = 0
     is_active_link: bool = True
-
```

### Comparing `terka-1.5.3/src/domain/story.py` & `terka-1.5.4/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/tag.py` & `terka-1.5.4/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/task.py` & `terka-1.5.4/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/time_tracker.py` & `terka-1.5.4/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/domain/user.py` & `terka-1.5.4/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/entrypoints/cli.py` & `terka-1.5.4/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/service_layer/printer.py` & `terka-1.5.4/src/service_layer/printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,21 +398,14 @@
                     entity_id = str(entity.id)
             else:
                 entity_id = str(entity.id)
             table.add_row(str(entity_id), entity_name, entity.description,
                           str(story_point), entity.status.name, priority,
                           project, str(entity.due_date), tag_string,
                           collaborator_string, str(time_spent))
-        if printable_entities:
-            if printable_entities == 1:
-                app = TerkaTask(entity=entity,
-                                project=project,
-                                history=history,
-                                commentaries=comments)
-                app.run()
             self.console.print(table)
         if show_completed and completed_tasks:
             table = Table(box=self.box)
             for column in default_columns:
                 table.add_column(column)
             self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
             for entity, story_point in zip(completed_tasks,
@@ -446,20 +439,14 @@
                               collaborator_string, str(time_spent))
             self.console.print(table)
         if len(entities) == 1 and printable_entities == 0:
             table = Table(box=self.box)
             for column in default_columns:
                 table.add_column(column)
             for entity in entities:
-                app = TerkaTask(entity=entity,
-                                project=project,
-                                is_completed=True,
-                                history=history,
-                                commentaries=comments)
-                app.run()
                 table.add_row(str(entity.id), entity.name, entity.description,
                               entity.status.name, priority, project,
                               str(entity.due_date), tag_string,
                               collaborator_string, str(time_spent))
             self.console.print(table)
 
     def print_task(self,
```

### Comparing `terka-1.5.3/src/service_layer/services.py` & `terka-1.5.4/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/service_layer/ui.py` & `terka-1.5.4/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/service_layer/vertical_layout.css` & `terka-1.5.4/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/src/utils.py` & `terka-1.5.4/src/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/terka.egg-info/PKG-INFO` & `terka-1.5.4/terka.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.5.3
+Version: 1.5.4
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.5.3/terka.egg-info/SOURCES.txt` & `terka-1.5.4/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/tests/test_orm.py` & `terka-1.5.4/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/tests/test_task.py` & `terka-1.5.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.3/tests/test_user.py` & `terka-1.5.4/tests/test_user.py`

 * *Files identical despite different names*

