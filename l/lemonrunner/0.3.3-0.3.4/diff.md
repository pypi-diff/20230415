# Comparing `tmp/lemonrunner-0.3.3.tar.gz` & `tmp/lemonrunner-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonrunner-0.3.3.tar", last modified: Sat Apr 15 13:38:08 2023, max compression
+gzip compressed data, was "lemonrunner-0.3.4.tar", last modified: Sat Apr 15 13:48:57 2023, max compression
```

## Comparing `lemonrunner-0.3.3.tar` & `lemonrunner-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.138696 lemonrunner-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.138696 lemonrunner-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.138696 lemonrunner-0.3.3/lemonrunner/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/lemonrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/lemonrunner/lemonrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/lemonrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/tests/test_lemonrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:57.057797 lemonrunner-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:57.053797 lemonrunner-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:57.053797 lemonrunner-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 13:48:57.053797 lemonrunner-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:57.053797 lemonrunner-0.3.4/lemonrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/lemonrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/lemonrunner/lemonrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:57.053797 lemonrunner-0.3.4/lemonrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 13:48:57.000000 lemonrunner-0.3.4/lemonrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 13:48:57.000000 lemonrunner-0.3.4/lemonrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:48:57.000000 lemonrunner-0.3.4/lemonrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 13:48:57.000000 lemonrunner-0.3.4/lemonrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:48:57.057797 lemonrunner-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:57.053797 lemonrunner-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-15 13:48:43.000000 lemonrunner-0.3.4/tests/test_lemonrunner.py
```

### Comparing `lemonrunner-0.3.3/.github/workflows/python-package.yml` & `lemonrunner-0.3.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `lemonrunner-0.3.3/LICENSE` & `lemonrunner-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonrunner-0.3.3/PKG-INFO` & `lemonrunner-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonrunner
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/sveinrou/lemonrunner
 Author: sveinrou
 Author-email: sveinrou@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `lemonrunner-0.3.3/README.md` & `lemonrunner-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `lemonrunner-0.3.3/lemonrunner/lemonrunner.py` & `lemonrunner-0.3.4/lemonrunner/lemonrunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,19 +55,19 @@
             if self.interval:
                 sleep(self.interval)
 
         self.report(output_queue, "exited", None)
 
 
 class Lemonrunner:
-    def __init__(self):
+    def __init__(self, queue_maxsize=1024):
         self.runnables = {}
         self.procs = {}
         self.runnables_lock = Lock()
-        self.input_queue = Queue()
+        self.input_queue = Queue(queue_maxsize)
         self.output_queue = Queue()
         self.last_seens = defaultdict(time)
 
         Thread(target=self._check, daemon=True).start()
         Thread(target=self._eat, daemon=True).start()
 
     def run(self, id, func, **kwargs):
@@ -81,14 +81,15 @@
             id, topic, timestamp, result = self.output_queue.get()
             if topic in topics:
                 yield id, topic, timestamp, result
 
     def _eat(self):
         while True:
             packet = self.input_queue.get()
+            print(self.input_queue.qsize())
             id, topic, timestamp, result = packet
             self.output_queue.put(packet)
 
             self.last_seens[id] = timestamp
 
     def _check(self):
         while True:
```

### Comparing `lemonrunner-0.3.3/lemonrunner.egg-info/PKG-INFO` & `lemonrunner-0.3.4/lemonrunner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonrunner
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/sveinrou/lemonrunner
 Author: sveinrou
 Author-email: sveinrou@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `lemonrunner-0.3.3/setup.py` & `lemonrunner-0.3.4/setup.py`

 * *Files identical despite different names*

