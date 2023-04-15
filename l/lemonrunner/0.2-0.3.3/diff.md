# Comparing `tmp/lemonrunner-0.2.tar.gz` & `tmp/lemonrunner-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonrunner-0.2.tar", last modified: Fri Apr 14 16:14:41 2023, max compression
+gzip compressed data, was "lemonrunner-0.3.3.tar", last modified: Sat Apr 15 13:38:08 2023, max compression
```

## Comparing `lemonrunner-0.2.tar` & `lemonrunner-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1071 2023-04-14 15:50:11.000000 lemonrunner-0.2/LICENSE
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1365 2023-04-14 16:14:41.494033 lemonrunner-0.2/PKG-INFO
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      975 2023-04-14 16:14:04.000000 lemonrunner-0.2/README.md
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/lemonrunner/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       48 2023-04-14 16:05:34.000000 lemonrunner-0.2/lemonrunner/__init__.py
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     3606 2023-04-14 16:05:54.000000 lemonrunner-0.2/lemonrunner/lemonrunner.py
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/lemonrunner.egg-info/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1365 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/PKG-INFO
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      260 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/SOURCES.txt
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)        1 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/dependency_links.txt
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       18 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/top_level.txt
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       38 2023-04-14 16:14:41.494033 lemonrunner-0.2/setup.cfg
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      705 2023-04-14 16:13:45.000000 lemonrunner-0.2/setup.py
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/tests/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 11:43:06.000000 lemonrunner-0.2/tests/__init__.py
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      542 2023-04-14 16:06:28.000000 lemonrunner-0.2/tests/test_definitely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.138696 lemonrunner-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.138696 lemonrunner-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.138696 lemonrunner-0.3.3/lemonrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/lemonrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/lemonrunner/lemonrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/lemonrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 13:38:08.000000 lemonrunner-0.3.3/lemonrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:38:08.142696 lemonrunner-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-15 13:37:50.000000 lemonrunner-0.3.3/tests/test_lemonrunner.py
```

### Comparing `lemonrunner-0.2/LICENSE` & `lemonrunner-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonrunner-0.2/PKG-INFO` & `lemonrunner-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonrunner
-Version: 0.2
-Summary: UNKNOWN
-Home-page: https://github.com/sveinrou/definitively
+Version: 0.3.3
+Home-page: https://github.com/sveinrou/lemonrunner
 Author: sveinrou
 Author-email: sveinrou@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lemonrunner
@@ -47,9 +44,7 @@
 runner.run('foo', foo, interval=1)
 runner.run('bar', bar, interval=1, timeout=2)
 runner.run('baaz', baaz, times=2)
 
 for id, message_type, timestamp, return_value in runner.monitor():
 	print(id, message_type, timestamp, return_value)
 ```
-
-
```

### Comparing `lemonrunner-0.2/README.md` & `lemonrunner-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `lemonrunner-0.2/lemonrunner/lemonrunner.py` & `lemonrunner-0.3.3/lemonrunner/lemonrunner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,66 @@
-from dataclasses import dataclass
 from itertools import repeat
 from collections import defaultdict
 from multiprocessing import Process, Queue
 from threading import Thread, Lock
 from inspect import isgeneratorfunction
 from time import time, sleep
-from copy import copy
+
 
 class Runnable:
-    def __init__(self, id, *, target, args=tuple(), kwargs=dict(), timeout=None, times=None, interval=None):
+    def __init__(
+        self,
+        id,
+        *,
+        target,
+        args=tuple(),
+        kwargs=dict(),
+        timeout=None,
+        times=None,
+        interval=None
+    ):
         self.id = id
         self.target = target
         self.args = args
         self.kwargs = kwargs
         self.timeout = timeout
         self.times = times
         self.interval = interval
 
     def report(self, queue, kind, data):
         queue.put((self.id, kind, time(), data))
 
     def _loop_iteration(self, output_queue: Queue):
         if isgeneratorfunction(self.target):
             for result in self.target(*self.args, **self.kwargs):
-                self.report(output_queue, 'yield', result)
+                self.report(output_queue, "yield", result)
         else:
             result = self.target(*self.args, **self.kwargs)
-            self.report(output_queue, 'return', result)
+            self.report(output_queue, "return", result)
 
     def run(self, output_queue: Queue):
         if self.times:
             runs = repeat(None, self.times)
         else:
             runs = repeat(None)
 
         for _ in runs:
-            self.report(output_queue, 'start', None)
+            self.report(output_queue, "start", None)
 
             try:
                 self._loop_iteration(output_queue)
             except Exception as e:
-                self.report(output_queue, 'exception', e)
+                self.report(output_queue, "exception", e)
 
-            self.report(output_queue, 'finish', None)
+            self.report(output_queue, "finish", None)
             if self.interval:
                 sleep(self.interval)
 
-        self.report(output_queue, 'exited', None)
+        self.report(output_queue, "exited", None)
+
 
 class Lemonrunner:
     def __init__(self):
         self.runnables = {}
         self.procs = {}
         self.runnables_lock = Lock()
         self.input_queue = Queue()
@@ -62,15 +72,15 @@
 
     def run(self, id, func, **kwargs):
         runnable = Runnable(id, target=func, **kwargs)
         with self.runnables_lock:
             self.runnables[id] = runnable
         self._start(runnable.id)
 
-    def monitor(self, topics=('return', 'yield')):
+    def monitor(self, topics=("return", "yield", "exception")):
         while True:
             id, topic, timestamp, result = self.output_queue.get()
             if topic in topics:
                 yield id, topic, timestamp, result
 
     def _eat(self):
         while True:
@@ -78,33 +88,39 @@
             id, topic, timestamp, result = packet
             self.output_queue.put(packet)
 
             self.last_seens[id] = timestamp
 
     def _check(self):
         while True:
-            # Use 40% of lowest timeout as sleep duration, or clamp to at most 1 sec
+            # Use 40% of lowest timeout as sleep duration, or clamp to at most
+            # 1 sec
             minimal_timeout = 1
             with self.runnables_lock:
                 runnables = self.runnables
 
             for id, runnable in runnables.items():
                 if runnable.timeout is not None:
-                    minimal_timeout = min(minimal_timeout, runnable.timeout or 0)
+                    minimal_timeout = min(minimal_timeout,
+                                          runnable.timeout or 0)
                     last_seen = self.last_seens[id]
                     if time() - last_seen > runnable.timeout:
                         self._stop(id)
                         self._start(id)
-            sleep(0.4*minimal_timeout)
+            sleep(0.4 * minimal_timeout)
 
     def _start(self, id):
         with self.runnables_lock:
             runnable = self.runnables[id]
-        self.procs[id] = Process(target=runnable.run, args=(self.input_queue,),  daemon=True)
+        self.procs[id] = Process(
+            target=runnable.run, args=(self.input_queue,), daemon=True
+        )
         self.procs[id].start()
 
     def _stop(self, id):
         proc = self.procs[id]
         proc.terminate()
+        proc.close()
+
 
-if __name__=='__main__':
+if __name__ == "__main__":
     pass
```

### Comparing `lemonrunner-0.2/lemonrunner.egg-info/PKG-INFO` & `lemonrunner-0.3.3/lemonrunner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonrunner
-Version: 0.2
-Summary: UNKNOWN
-Home-page: https://github.com/sveinrou/definitively
+Version: 0.3.3
+Home-page: https://github.com/sveinrou/lemonrunner
 Author: sveinrou
 Author-email: sveinrou@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lemonrunner
@@ -47,9 +44,7 @@
 runner.run('foo', foo, interval=1)
 runner.run('bar', bar, interval=1, timeout=2)
 runner.run('baaz', baaz, times=2)
 
 for id, message_type, timestamp, return_value in runner.monitor():
 	print(id, message_type, timestamp, return_value)
 ```
-
-
```

### Comparing `lemonrunner-0.2/setup.py` & `lemonrunner-0.3.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import setuptools
 
-version = "0.2"
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-requirements = []
-
-if __name__=='__main__':
+if __name__ == '__main__':
     setuptools.setup(
         name="lemonrunner",
-        version=version,
+        use_scm_version=True,
+        setup_requires=['setuptools_scm'],
         author="sveinrou",
         author_email="sveinrou@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        url="https://github.com/sveinrou/definitively",
+        url="https://github.com/sveinrou/lemonrunner",
         packages=setuptools.find_packages(),
-        install_requires=requirements,
         classifiers=[
             "Programming Language :: Python :: 3",
             "Operating System :: OS Independent",
         ],
         python_requires=">=3.6",
     )
```

