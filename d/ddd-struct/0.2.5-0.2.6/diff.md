# Comparing `tmp/ddd-struct-0.2.5.tar.gz` & `tmp/ddd-struct-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddd-struct-0.2.5.tar", last modified: Tue Apr 11 16:27:15 2023, max compression
+gzip compressed data, was "ddd-struct-0.2.6.tar", last modified: Sat Apr 15 12:34:55 2023, max compression
```

## Comparing `ddd-struct-0.2.5.tar` & `ddd-struct-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.826456 ddd-struct-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:27:15.826456 ddd-struct-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.802455 ddd-struct-0.2.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/application/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/domain/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/infrastructure/repository_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/lib/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1715 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/common.py
--rw-rw-rw-   0 root         (0) root         (0)     4696 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/thread.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/warning.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.263749 ddd-struct-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-15 12:34:55.263749 ddd-struct-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 12:34:55.263749 ddd-struct-0.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.243748 ddd-struct-0.2.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.259749 ddd-struct-0.2.6/src/ddd_struct/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.259749 ddd-struct-0.2.6/src/ddd_struct/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14104 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/application/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.263749 ddd-struct-0.2.6/src/ddd_struct/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/domain/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.263749 ddd-struct-0.2.6/src/ddd_struct/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/infrastructure/repository_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.263749 ddd-struct-0.2.6/src/ddd_struct/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/lib/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4696 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/lib/thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/lib/warning.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-15 12:34:48.000000 ddd-struct-0.2.6/src/ddd_struct/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:34:55.259749 ddd-struct-0.2.6/src/ddd_struct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-15 12:34:55.000000 ddd-struct-0.2.6/src/ddd_struct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-15 12:34:55.000000 ddd-struct-0.2.6/src/ddd_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 12:34:55.000000 ddd-struct-0.2.6/src/ddd_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-15 12:34:55.000000 ddd-struct-0.2.6/src/ddd_struct.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-15 12:34:55.000000 ddd-struct-0.2.6/src/ddd_struct.egg-info/top_level.txt
```

### Comparing `ddd-struct-0.2.5/LICENSE` & `ddd-struct-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/setup.py` & `ddd-struct-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/src/ddd_struct/application/action.py` & `ddd-struct-0.2.6/src/ddd_struct/application/action.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import copy
 from typing import Optional, List
 from ..domain.repository import TaskQueueRepository, TaskProcessRepository
 
 
 
 
-__all__ = ['CacheQueue', 'SimpleTaskProcessor']
+__all__ = ['CacheQueue', 'SimpleTaskProcessor', 'SequenceTaskProcessor']
 class CacheQueue:
     def __init__(self) -> None:
         self.cache = {}
         self.queue = None
 
 
     def _next(self):
@@ -155,15 +155,15 @@
         # preprocess
         succeed, item = self.preprocess(item, process_repo)
         if not succeed:
             self.process_when_failed(item, 'preprocess')
             return 
 
         # process
-        item = self.process_task(item)
+        item = self.process_task(item, process_repo)
         succeed = self.save_item(item, queue_repo)
         if not succeed:
             self.process_when_failed(item, 'save')
             return 
 
         # postprocess
         succeed, item = self.postprocess(item, process_repo)
@@ -186,15 +186,15 @@
         if failed_items:
             self.process_when_failed_batch(failed_items, 'preprocess')
 
         # process
         items = [i for i,s in zip(items, succeed_symbols) if s]
         if not items:
             return
-        items = self.process_tasks(items)
+        items = self.process_tasks(items, process_repo)
         succeed_symbols = self.save_items(items, queue_repo)
         failed_items = [i for i,s in zip(items, succeed_symbols) if not s]
         if failed_items:
             self.process_when_failed_batch(failed_items, 'save')
 
         # postprocess
         items = [i for i,s in zip(items, succeed_symbols) if s]
@@ -276,7 +276,155 @@
             try:
                 self.process_all_batch(items, process_repo, queue_repo)
             except:
                 self.process_when_failed_batch(items, 'process_all')
 
             
 
+class SequenceTaskProcessor(SimpleTaskProcessor):
+    def __init__(
+        self, 
+        queue_repo:TaskQueueRepository, 
+        process_repos: List[TaskProcessRepository],
+        delay:int = 1,
+        batch_size = 5
+    ) -> None:
+        self.queue_repo = queue_repo
+        self.process_repos = process_repos
+        self.delay = delay
+        self.batch_size = batch_size
+    
+
+    def process_all(
+        self, 
+        item, 
+        process_repos: List[TaskProcessRepository],
+        queue_repo: TaskQueueRepository
+    ):
+        '''处理所有的步骤
+        '''
+        # preprocess
+        for process_repo in process_repos:
+            succeed, item = self.preprocess(item, process_repo)
+            if not succeed:
+                self.process_when_failed(item, 'preprocess')
+                return
+
+            # process
+            item = self.process_task(item, process_repo)
+            succeed = self.save_item(item, queue_repo)
+            if not succeed:
+                self.process_when_failed(item, 'save')
+                return 
+
+            # postprocess
+            succeed, item = self.postprocess(item, process_repo)
+            if not succeed:
+                self.process_when_failed(item, 'postprocess')
+                return 
+            
+    
+    def process_all_batch(
+        self, 
+        items, 
+        process_repos: List[TaskProcessRepository], 
+        queue_repo: TaskQueueRepository
+    ):
+        '''处理所有步骤，并且是批量处理
+        '''
+        # preprocess
+        for process_repo in process_repos:
+            succeed_symbols, items = self.preprocess_batch(items, process_repo)
+            failed_items = [i for i,s in zip(items, succeed_symbols) if not s]
+            if failed_items:
+                self.process_when_failed_batch(failed_items, 'preprocess')
+
+            # process
+            items = [i for i,s in zip(items, succeed_symbols) if s]
+            if not items:
+                return
+            items = self.process_tasks(items, process_repo)
+            succeed_symbols = self.save_items(items, queue_repo)
+            failed_items = [i for i,s in zip(items, succeed_symbols) if not s]
+            if failed_items:
+                self.process_when_failed_batch(failed_items, 'save')
+
+            # postprocess
+            items = [i for i,s in zip(items, succeed_symbols) if s]
+            if not items:
+                return
+            succeed_symbols, items = self.postprocess_batch(items, process_repo)
+            failed_items = [i for i,s in zip(items, succeed_symbols) if not s]
+            if failed_items:
+                self.process_when_failed_batch(failed_items, 'postprocess')
+
+    def run(
+        self, 
+        queue_repo: Optional[TaskQueueRepository]=None, 
+        process_repos: Optional[TaskProcessRepository]=None,
+        delay=None, 
+        n_loop=1000000000,
+        auto_change_delay=True
+    ):
+        queue_repo = queue_repo or self.queue_repo
+        process_repos = process_repos or self.process_repos
+        delay = delay or self.delay
+        ignore_delay = False
+        for i in range(n_loop):
+            if not auto_change_delay or not ignore_delay:
+                time.sleep(delay)
+            request_id, request = self.get_request(queue_repo)
+            if not request:
+                continue
+            else:
+                ignore_delay = True
+
+            # generate item
+            item = self.gen_item(request_id, request)
+            succeed = self.save_item(item, queue_repo)
+            if not succeed:
+                self.process_when_failed(item, 'save')
+                continue
+
+            # process item
+            try:
+                self.process_all(item, process_repos, queue_repo)
+            except:
+                self.process_when_failed(item, 'process_all') 
+                
+    
+
+    def run_batch(
+        self, 
+        queue_repo: Optional[TaskQueueRepository]=None, 
+        process_repos: Optional[TaskProcessRepository]=None,
+        delay=None, 
+        n_loop=1000000000,
+        auto_change_delay=True
+    ):
+        queue_repo = queue_repo or self.queue_repo
+        process_repos = process_repos or self.process_repos
+        delay = delay or self.delay
+        ignore_delay = False
+        for i in range(n_loop):
+            if not auto_change_delay or not ignore_delay:
+                time.sleep(delay)
+            requests = self.get_requests(self.batch_size, queue_repo)
+            if not requests:
+                continue
+            else:
+                ignore_delay = True
+
+            # generate item
+            items = self.gen_items(requests)
+            succeed_symbols = self.save_items(items, queue_repo)
+            failed_items = [i for i,s in zip(items, succeed_symbols) if not s]
+            if failed_items:
+                self.process_when_failed_batch(failed_items, 'save')
+            items = [i for i,s in zip(items, succeed_symbols) if s]
+            if not items:
+                continue
+            try:
+                self.process_all_batch(items, process_repos, queue_repo)
+            except:
+                self.process_when_failed_batch(items, 'process_all')
+
```

### Comparing `ddd-struct-0.2.5/src/ddd_struct/domain/repository.py` & `ddd-struct-0.2.6/src/ddd_struct/domain/repository.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/src/ddd_struct/infrastructure/repository_impl.py` & `ddd-struct-0.2.6/src/ddd_struct/infrastructure/repository_impl.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/src/ddd_struct/lib/common.py` & `ddd-struct-0.2.6/src/ddd_struct/lib/common.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/src/ddd_struct/lib/thread.py` & `ddd-struct-0.2.6/src/ddd_struct/lib/thread.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/src/ddd_struct/lib/warning.py` & `ddd-struct-0.2.6/src/ddd_struct/lib/warning.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.5/src/ddd_struct.egg-info/SOURCES.txt` & `ddd-struct-0.2.6/src/ddd_struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

