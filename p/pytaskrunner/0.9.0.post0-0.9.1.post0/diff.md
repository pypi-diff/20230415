# Comparing `tmp/pytaskrunner-0.9.0.post0.tar.gz` & `tmp/pytaskrunner-0.9.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytaskrunner-0.9.0.post0.tar", last modified: Sat Nov 12 16:53:47 2022, max compression
+gzip compressed data, was "pytaskrunner-0.9.1.post0.tar", last modified: Fri Feb  3 12:57:36 2023, max compression
```

## Comparing `pytaskrunner-0.9.0.post0.tar` & `pytaskrunner-0.9.1.post0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2022-11-12 16:53:47.368202 pytaskrunner-0.9.0.post0/
--rw-rw-r--   0 omer      (1000) omer      (1000)     1067 2022-02-08 22:33:12.000000 pytaskrunner-0.9.0.post0/LICENSE
--rw-r--r--   0 omer      (1000) omer      (1000)    18823 2022-11-12 16:53:47.368202 pytaskrunner-0.9.0.post0/PKG-INFO
--rw-r--r--   0 omer      (1000) omer      (1000)    18114 2022-11-11 18:57:35.000000 pytaskrunner-0.9.0.post0/README.md
--rw-rw-r--   0 omer      (1000) omer      (1000)       85 2022-08-27 13:25:07.000000 pytaskrunner-0.9.0.post0/pyproject.toml
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2022-11-12 16:53:47.367201 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/
--rw-rw-r--   0 omer      (1000) omer      (1000)    18823 2022-11-12 16:53:47.000000 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/PKG-INFO
--rw-rw-r--   0 omer      (1000) omer      (1000)      369 2022-11-12 16:53:47.000000 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/SOURCES.txt
--rw-rw-r--   0 omer      (1000) omer      (1000)        1 2022-11-12 16:53:47.000000 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/dependency_links.txt
--rw-rw-r--   0 omer      (1000) omer      (1000)       53 2022-11-12 16:53:47.000000 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/entry_points.txt
--rw-rw-r--   0 omer      (1000) omer      (1000)       37 2022-11-12 16:53:47.000000 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/requires.txt
--rw-rw-r--   0 omer      (1000) omer      (1000)        3 2022-11-12 16:53:47.000000 pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/top_level.txt
--rw-r--r--   0 omer      (1000) omer      (1000)      838 2022-11-12 16:53:47.368202 pytaskrunner-0.9.0.post0/setup.cfg
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2022-11-12 16:53:47.367201 pytaskrunner-0.9.0.post0/tr/
--rw-r--r--   0 omer      (1000) omer      (1000)     6849 2022-11-12 16:44:02.000000 pytaskrunner-0.9.0.post0/tr/Task.py
--rw-r--r--   0 omer      (1000) omer      (1000)      217 2022-11-12 16:52:16.000000 pytaskrunner-0.9.0.post0/tr/__init__.py
--rw-r--r--   0 omer      (1000) omer      (1000)     7983 2022-11-11 18:57:35.000000 pytaskrunner-0.9.0.post0/tr/actions.py
--rw-r--r--   0 omer      (1000) omer      (1000)     3322 2022-11-12 14:14:06.000000 pytaskrunner-0.9.0.post0/tr/common.py
--rw-r--r--   0 omer      (1000) omer      (1000)     8261 2022-11-12 16:44:02.000000 pytaskrunner-0.9.0.post0/tr/config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     4032 2022-11-11 18:57:35.000000 pytaskrunner-0.9.0.post0/tr/logTools.py
--rw-r--r--   0 omer      (1000) omer      (1000)     5794 2022-11-12 16:44:02.000000 pytaskrunner-0.9.0.post0/tr/schemas.py
--rw-r--r--   0 omer      (1000) omer      (1000)     7536 2022-11-11 18:57:35.000000 pytaskrunner-0.9.0.post0/tr/taskrun.py
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-03 12:57:36.524449 pytaskrunner-0.9.1.post0/
+-rw-rw-r--   0 omer      (1000) omer      (1000)     1067 2022-02-08 22:33:12.000000 pytaskrunner-0.9.1.post0/LICENSE
+-rw-r--r--   0 omer      (1000) omer      (1000)    18874 2023-02-03 12:57:36.524449 pytaskrunner-0.9.1.post0/PKG-INFO
+-rw-r--r--   0 omer      (1000) omer      (1000)    18114 2022-11-11 18:57:35.000000 pytaskrunner-0.9.1.post0/README.md
+-rw-r--r--   0 omer      (1000) omer      (1000)       85 2023-02-03 11:25:48.000000 pytaskrunner-0.9.1.post0/pyproject.toml
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-03 12:57:36.523450 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/
+-rw-rw-r--   0 omer      (1000) omer      (1000)    18874 2023-02-03 12:57:36.000000 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/PKG-INFO
+-rw-rw-r--   0 omer      (1000) omer      (1000)      369 2023-02-03 12:57:36.000000 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 omer      (1000) omer      (1000)        1 2023-02-03 12:57:36.000000 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 omer      (1000) omer      (1000)       53 2023-02-03 12:57:36.000000 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/entry_points.txt
+-rw-rw-r--   0 omer      (1000) omer      (1000)       37 2023-02-03 12:57:36.000000 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/requires.txt
+-rw-rw-r--   0 omer      (1000) omer      (1000)        3 2023-02-03 12:57:36.000000 pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/top_level.txt
+-rw-r--r--   0 omer      (1000) omer      (1000)      878 2023-02-03 12:57:36.524449 pytaskrunner-0.9.1.post0/setup.cfg
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-03 12:57:36.524449 pytaskrunner-0.9.1.post0/tr/
+-rw-r--r--   0 omer      (1000) omer      (1000)     6849 2022-11-12 16:57:12.000000 pytaskrunner-0.9.1.post0/tr/Task.py
+-rw-r--r--   0 omer      (1000) omer      (1000)      217 2023-02-03 12:56:30.000000 pytaskrunner-0.9.1.post0/tr/__init__.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     7906 2023-02-03 11:22:10.000000 pytaskrunner-0.9.1.post0/tr/actions.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     3322 2022-11-12 14:14:06.000000 pytaskrunner-0.9.1.post0/tr/common.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     8261 2022-11-12 16:57:12.000000 pytaskrunner-0.9.1.post0/tr/config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     4032 2022-11-11 18:57:35.000000 pytaskrunner-0.9.1.post0/tr/logTools.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     5794 2022-11-12 16:57:12.000000 pytaskrunner-0.9.1.post0/tr/schemas.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     7536 2022-11-11 18:57:35.000000 pytaskrunner-0.9.1.post0/tr/taskrun.py
```

### Comparing `pytaskrunner-0.9.0.post0/LICENSE` & `pytaskrunner-0.9.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/PKG-INFO` & `pytaskrunner-0.9.1.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pytaskrunner
-Version: 0.9.0.post0
+Version: 0.9.1.post0
 Summary: Shell tasks managmement tool
 Home-page: https://github.com/omercsp/taskrunner
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Test](https://github.com/omercsp/taskrunner/actions/workflows/test.yml/badge.svg?branch=master)
 
 # What is this?
```

### Comparing `pytaskrunner-0.9.0.post0/README.md` & `pytaskrunner-0.9.1.post0/README.md`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/pytaskrunner.egg-info/PKG-INFO` & `pytaskrunner-0.9.1.post0/pytaskrunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pytaskrunner
-Version: 0.9.0.post0
+Version: 0.9.1.post0
 Summary: Shell tasks managmement tool
 Home-page: https://github.com/omercsp/taskrunner
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Test](https://github.com/omercsp/taskrunner/actions/workflows/test.yml/badge.svg?branch=master)
 
 # What is this?
```

### Comparing `pytaskrunner-0.9.0.post0/setup.cfg` & `pytaskrunner-0.9.1.post0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
 install_requires = 
 	argcomplete>=2.0.0
 	jsonschema>=3.2.0
 python_requires = >=3.6,<4
```

### Comparing `pytaskrunner-0.9.0.post0/tr/Task.py` & `pytaskrunner-0.9.1.post0/tr/Task.py`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/tr/actions.py` & `pytaskrunner-0.9.1.post0/tr/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,41 +80,36 @@
         if task.c_flags:
             print_blob("  Additional flags:", task.c_flags)
         if task.c_cwd:
             print_blob("  Working directory:", _task_str(task.c_cwd))
         if len(task.c_volumes) == 1:
             print_blob("  Volume:", _task_str(task.c_volumes[0]))
         elif len(task.c_volumes) > 1:
-            count = 0
             print("  Volumes:")
-            for vol in task.c_volumes:
-                print_blob(f"       [{count}]", _task_str(vol))
-                count += 1
+            for i ,vol in enumerate(task.c_volumes):
+                print_blob(f"       [{i}]", _task_str(vol))
         if task.c_env:
             print("  Environment:")
-            for k, v in task.c_env.items():
-                print_blob(f"       [{count}]", f"{k}={v}")
-                count += 1
+            for i, (k, v) in enumerate(task.c_env.items()):
+                print_blob(f"       [{i}]", f"{k}={v}")
 
     if len(task.commands) == 0:
         if task.c_image is None:
             print("NOTICE: No commands defined for task")
         else:
             print("NOTICE: Will run the image/container default command")
         return
     if len(task.commands) == 1:
         print_blob("Command:", _task_str(task.commands[0]))
         return
 
     print_bool("Stop on error:", task.stop_on_error)
     print("Commands:")
-    count = 0
-    for cmd in task.commands:
-        print_blob(f"     [{count}]", _task_str(cmd))
-        count += 1
+    for i, cmd in enumerate(task.commands):
+        print_blob(f"     [{i}]", _task_str(cmd))
 
 
 def show_task_info(config: Config) -> None:
     task_name = _active_task_name(config)
     task = Task(task_name, config)
     if config.args.expand:
         task.expand()
```

### Comparing `pytaskrunner-0.9.0.post0/tr/common.py` & `pytaskrunner-0.9.1.post0/tr/common.py`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/tr/config.py` & `pytaskrunner-0.9.1.post0/tr/config.py`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/tr/logTools.py` & `pytaskrunner-0.9.1.post0/tr/logTools.py`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/tr/schemas.py` & `pytaskrunner-0.9.1.post0/tr/schemas.py`

 * *Files identical despite different names*

### Comparing `pytaskrunner-0.9.0.post0/tr/taskrun.py` & `pytaskrunner-0.9.1.post0/tr/taskrun.py`

 * *Files identical despite different names*

