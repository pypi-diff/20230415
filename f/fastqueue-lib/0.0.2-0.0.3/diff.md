# Comparing `tmp/fastqueue-lib-0.0.2.tar.gz` & `tmp/fastqueue-lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.2.tar", last modified: Sat Apr 15 06:25:54 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.3.tar", last modified: Sat Apr 15 18:11:25 2023, max compression
```

## Comparing `fastqueue-lib-0.0.2.tar` & `fastqueue-lib-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.721992 fastqueue-lib-0.0.2/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     1096 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.2/LICENSE
--rwxrwxrwx   0 matt      (1000) matt      (1000)       34 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.2/MANIFEST.in
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3374 2023-04-15 06:25:54.718995 fastqueue-lib-0.0.2/PKG-INFO
--rwxrwxrwx   0 matt      (1000) matt      (1000)     2520 2023-04-15 06:21:51.000000 fastqueue-lib-0.0.2/README.md
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.617101 fastqueue-lib-0.0.2/fastqueue/
--rwxrwxrwx   0 matt      (1000) matt      (1000)       67 2023-04-15 04:39:02.000000 fastqueue-lib-0.0.2/fastqueue/__init__.py
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3238 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.2/fastqueue/prototypes.py
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.669049 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3374 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 matt      (1000) matt      (1000)      352 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)        1 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)       39 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/requires.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)       21 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/top_level.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)     1098 2023-04-15 06:25:02.000000 fastqueue-lib-0.0.2/pyproject.toml
--rwxrwxrwx   0 matt      (1000) matt      (1000)       38 2023-04-15 06:25:54.721992 fastqueue-lib-0.0.2/setup.cfg
--rwxrwxrwx   0 matt      (1000) matt      (1000)     1020 2023-04-15 04:36:07.000000 fastqueue-lib-0.0.2/setup.py
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.697020 fastqueue-lib-0.0.2/src/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     2341 2023-04-15 05:18:24.000000 fastqueue-lib-0.0.2/src/ccqueue.cpp
--rwxrwxrwx   0 matt      (1000) matt      (1000)     2177 2023-04-15 05:18:20.000000 fastqueue-lib-0.0.2/src/cllqueue.cpp
--rwxrwxrwx   0 matt      (1000) matt      (1000)    19493 2023-04-15 05:18:04.000000 fastqueue-lib-0.0.2/src/fastqueue.c
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.707007 fastqueue-lib-0.0.2/tests/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3303 2023-04-15 04:44:10.000000 fastqueue-lib-0.0.2/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.428902 fastqueue-lib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/fastqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/fastqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/fastqueue/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 18:11:25.000000 fastqueue-lib-0.0.3/fastqueue_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:11:25.428902 fastqueue-lib-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/src/ccqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/src/cllqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18942 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/src/fastqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:11:25.424902 fastqueue-lib-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-15 18:11:09.000000 fastqueue-lib-0.0.3/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.2/LICENSE` & `fastqueue-lib-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Matthew Andre Taylor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Matthew Andre Taylor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `fastqueue-lib-0.0.2/PKG-INFO` & `fastqueue-lib-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,15 +36,15 @@
 - `python 3.9+`
 
 ## Installation
 
 To install fastqueue, using pip:
 
 ```bash
-pip install fastqueue
+pip install fastqueue-lib
 ```
 
 ## Quickstart
 
 For general use cases `fastqueue.Queue()` objects are tuned to perform well.
 The enqueue and dequeue methods perform well over a large sequence of arbitrary operations.
 `fastqueue.Queue()` supports many standard sequence methods similar to lists.
```

### Comparing `fastqueue-lib-0.0.2/README.md` & `fastqueue-lib-0.0.3/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,97 @@
-# fastqueue
-
-[![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
-[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
-
-
-Single ended fast queue's built in C tuned for python.
-
-## Requirements
-
-- `python 3.9+`
-
-## Installation
-
-To install fastqueue, using pip:
-
-```bash
-pip install fastqueue
-```
-
-## Quickstart
-
-For general use cases `fastqueue.Queue()` objects are tuned to perform well.
-The enqueue and dequeue methods perform well over a large sequence of arbitrary operations.
-`fastqueue.Queue()` supports many standard sequence methods similar to lists.
-`fastqueue.Queue()` minimizes memory usage but maintains the fast queue speeds.
-
-```py
->>> from fastqueue import Queue
->>> queue = Queue()
->>> queue.extend(['🚒', '🛴'])
->>> queue[0]
-'🚒'
->>> '🛴' in queue
-True
->>> queue.enqueue('🚅')
->>> queue.enqueue('🚗')
->>> queue[-1]
-'🚗'
->>> [queue.dequeue() for _ in range(len(queue)) ]
-['🚒', '🛴', '🚅', '🚗']
-```
-
-
-For more specialized cases `fastqueue.QueueC()` objects are tuned to perform well.
-The interface for `fastqueue.QueueC()` is identical to `fastqueue.Queue()`.
-The enqueue and dequeue methods perform similarly well over a large sequence of arbitrary operations.
-`fastqueue.QueueC()` handles memory differently by doubling the capacity when full.
-This increases the complexity but maintains fast amortized cost.
-The benefit of this approach is even faster `__getitem__` and `__setitem__` speeds
-
-```py
->>> from fastqueue import QueueC
->>> queue_c = QueueC()
->>> queue_c.extend(['🚒', '🛴'])
->>> queue_c[0]
-'🚒'
->>> '🛴' in queue_c
-True
->>> queue_c.enqueue('🚅')
->>> queue_c.enqueue('🚗')
->>> queue_c[-1]
-'🚗'
->>> [queue_c.dequeue() for _ in range(len(queue_c)) ]
-['🚒', '🛴', '🚅', '🚗']
-```
-
-## Example Benchmarks
-![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
-![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
-
-
+Metadata-Version: 2.1
+Name: fastqueue-lib
+Version: 0.0.3
+Summary: Fast single ended queue library for python
+Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
+Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
+Keywords: Queue
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: examples
+Provides-Extra: tests
+License-File: LICENSE
+
+# fastqueue
+
+[![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
+[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
+[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
+
+
+Single ended fast queue's built in C tuned for python.
+
+## Requirements
+
+- `python 3.9+`
+
+## Installation
+
+To install fastqueue, using pip:
+
+```bash
+pip install fastqueue-lib
+```
+
+## Quickstart
+
+For general use cases `fastqueue.Queue()` objects are tuned to perform well.
+The enqueue and dequeue methods perform well over a large sequence of arbitrary operations.
+`fastqueue.Queue()` supports many standard sequence methods similar to lists.
+`fastqueue.Queue()` minimizes memory usage but maintains the fast queue speeds.
+
+```py
+>>> from fastqueue import Queue
+>>> queue = Queue()
+>>> queue.extend(['🚒', '🛴'])
+>>> queue[0]
+'🚒'
+>>> '🛴' in queue
+True
+>>> queue.enqueue('🚅')
+>>> queue.enqueue('🚗')
+>>> queue[-1]
+'🚗'
+>>> [queue.dequeue() for _ in range(len(queue)) ]
+['🚒', '🛴', '🚅', '🚗']
+```
+
+
+For more specialized cases `fastqueue.QueueC()` objects are tuned to perform well.
+The interface for `fastqueue.QueueC()` is identical to `fastqueue.Queue()`.
+The enqueue and dequeue methods perform similarly well over a large sequence of arbitrary operations.
+`fastqueue.QueueC()` handles memory differently by doubling the capacity when full.
+This increases the complexity but maintains fast amortized cost.
+The benefit of this approach is even faster `__getitem__` and `__setitem__` speeds
+
+```py
+>>> from fastqueue import QueueC
+>>> queue_c = QueueC()
+>>> queue_c.extend(['🚒', '🛴'])
+>>> queue_c[0]
+'🚒'
+>>> '🛴' in queue_c
+True
+>>> queue_c.enqueue('🚅')
+>>> queue_c.enqueue('🚗')
+>>> queue_c[-1]
+'🚗'
+>>> [queue_c.dequeue() for _ in range(len(queue_c)) ]
+['🚒', '🛴', '🚅', '🚗']
+```
+
+## Example Benchmarks
+![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
+![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
+
+
```

### Comparing `fastqueue-lib-0.0.2/fastqueue/prototypes.py` & `fastqueue-lib-0.0.3/fastqueue/prototypes.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from ctypes import *
-from pathlib import *
-from typing import Any
-
-
-# Matt's Linked List Queue
-class LLNode(Structure):
-    pass
-
-
-LLNode._fields_ = [
-    ('val', py_object),
-    ('next', POINTER(LLNode))
-]
-
-
-class LLNodeQueue(Structure):
-    _fields_ = [
-        ('front', POINTER(LLNode)),
-        ('back', POINTER(LLNode)),
-        ('length', c_uint)
-    ]
-
-
-__libfile = Path(__file__).parent / "cllqueue.so"
-llqueue_lib = CDLL(str(__libfile))
-
-llqueue_lib.new_node_queue.argtypes = []
-llqueue_lib.new_node_queue.restype = POINTER(LLNodeQueue)
-
-llqueue_lib.is_empty.argtypes = [POINTER(LLNodeQueue)]
-llqueue_lib.is_empty.restype = c_bool
-
-llqueue_lib.enqueue.argtypes = [POINTER(LLNodeQueue), py_object]
-llqueue_lib.enqueue.restype = None
-
-llqueue_lib.dequeue.argtypes = [POINTER(LLNodeQueue)]
-llqueue_lib.dequeue.restype = py_object
-
-llqueue_lib.free_q.argtypes = [POINTER(LLNodeQueue)]
-llqueue_lib.free_q.restype = None
-
-
-class LLQueue:
-    __slots__ = "queue"
-    queue: POINTER(LLNodeQueue)
-
-    def __init__(self):
-        self.queue = llqueue_lib.new_node_queue()
-
-    def is_empty(self) -> bool:
-        return llqueue_lib.is_empty(self.queue)
-
-    def __len__(self) -> int:
-        return self.queue.contents.length
-
-    def enqueue(self, item: Any) -> None:
-        llqueue_lib.enqueue(self.queue, item)
-
-    def dequeue(self) -> Any:
-        if self.is_empty():
-            raise IndexError
-        return llqueue_lib.dequeue(self.queue)
-
-    def clear(self):
-        llqueue_lib.free_q(self.queue)
-        self.queue = llqueue_lib.new__queue()
-
-    def __del__(self):
-        llqueue_lib.free_q(self.queue)
-
-
-# Matt's Contiguous Queue
-class ContiguousQueue(Structure):
-    _fields_ = [
-        ('objects', POINTER(py_object)),
-        ('length', c_int),
-        ('capacity', c_int),
-        ('front', c_int),
-        ('back', c_int)
-    ]
-
-
-__libfile = Path(__file__).parent / "ccqueue.so"
-cqueue_lib = CDLL(str(__libfile))
-
-cqueue_lib.new__queue.argtypes = []
-cqueue_lib.new__queue.restype = POINTER(ContiguousQueue)
-
-cqueue_lib.is_empty.argtypes = [POINTER(ContiguousQueue)]
-cqueue_lib.is_empty.restype = c_bool
-
-cqueue_lib.enqueue.argtypes = [POINTER(ContiguousQueue), py_object]
-cqueue_lib.enqueue.restype = None
-
-cqueue_lib.dequeue.argtypes = [POINTER(ContiguousQueue)]
-cqueue_lib.dequeue.restype = py_object
-
-cqueue_lib.free_q.argtypes = [POINTER(ContiguousQueue)]
-cqueue_lib.free_q.restype = None
-
-
-class ContQueue:
-    __slots__ = "queue"
-    queue: POINTER(ContiguousQueue)
-
-    def __init__(self):
-        self.queue = cqueue_lib.new__queue()
-
-    def is_empty(self) -> bool:
-        return cqueue_lib.is_empty(self.queue)
-
-    def __len__(self) -> int:
-        return self.queue.contents.length
-
-    def enqueue(self, item: Any) -> None:
-        cqueue_lib.enqueue(self.queue, item)
-
-    def dequeue(self) -> Any:
-        if self.is_empty():
-            raise IndexError
-        return cqueue_lib.dequeue(self.queue)
-
-    def clear(self):
-        cqueue_lib.free_q(self.queue)
-        self.queue = cqueue_lib.new__queue()
-
-    def __del__(self):
-        cqueue_lib.free_q(self.queue)
+from ctypes import *
+from pathlib import *
+from typing import Any
+
+
+# Matt's Linked List Queue
+class LLNode(Structure):
+    pass
+
+
+LLNode._fields_ = [
+    ('val', py_object),
+    ('next', POINTER(LLNode))
+]
+
+
+class LLNodeQueue(Structure):
+    _fields_ = [
+        ('front', POINTER(LLNode)),
+        ('back', POINTER(LLNode)),
+        ('length', c_uint)
+    ]
+
+
+__libfile = Path(__file__).parent / "cllqueue.so"
+llqueue_lib = CDLL(str(__libfile))
+
+llqueue_lib.new_node_queue.argtypes = []
+llqueue_lib.new_node_queue.restype = POINTER(LLNodeQueue)
+
+llqueue_lib.is_empty.argtypes = [POINTER(LLNodeQueue)]
+llqueue_lib.is_empty.restype = c_bool
+
+llqueue_lib.enqueue.argtypes = [POINTER(LLNodeQueue), py_object]
+llqueue_lib.enqueue.restype = None
+
+llqueue_lib.dequeue.argtypes = [POINTER(LLNodeQueue)]
+llqueue_lib.dequeue.restype = py_object
+
+llqueue_lib.free_q.argtypes = [POINTER(LLNodeQueue)]
+llqueue_lib.free_q.restype = None
+
+
+class LLQueue:
+    __slots__ = "queue"
+    queue: POINTER(LLNodeQueue)
+
+    def __init__(self):
+        self.queue = llqueue_lib.new_node_queue()
+
+    def is_empty(self) -> bool:
+        return llqueue_lib.is_empty(self.queue)
+
+    def __len__(self) -> int:
+        return self.queue.contents.length
+
+    def enqueue(self, item: Any) -> None:
+        llqueue_lib.enqueue(self.queue, item)
+
+    def dequeue(self) -> Any:
+        if self.is_empty():
+            raise IndexError
+        return llqueue_lib.dequeue(self.queue)
+
+    def clear(self):
+        llqueue_lib.free_q(self.queue)
+        self.queue = llqueue_lib.new__queue()
+
+    def __del__(self):
+        llqueue_lib.free_q(self.queue)
+
+
+# Matt's Contiguous Queue
+class ContiguousQueue(Structure):
+    _fields_ = [
+        ('objects', POINTER(py_object)),
+        ('length', c_int),
+        ('capacity', c_int),
+        ('front', c_int),
+        ('back', c_int)
+    ]
+
+
+__libfile = Path(__file__).parent / "ccqueue.so"
+cqueue_lib = CDLL(str(__libfile))
+
+cqueue_lib.new__queue.argtypes = []
+cqueue_lib.new__queue.restype = POINTER(ContiguousQueue)
+
+cqueue_lib.is_empty.argtypes = [POINTER(ContiguousQueue)]
+cqueue_lib.is_empty.restype = c_bool
+
+cqueue_lib.enqueue.argtypes = [POINTER(ContiguousQueue), py_object]
+cqueue_lib.enqueue.restype = None
+
+cqueue_lib.dequeue.argtypes = [POINTER(ContiguousQueue)]
+cqueue_lib.dequeue.restype = py_object
+
+cqueue_lib.free_q.argtypes = [POINTER(ContiguousQueue)]
+cqueue_lib.free_q.restype = None
+
+
+class ContQueue:
+    __slots__ = "queue"
+    queue: POINTER(ContiguousQueue)
+
+    def __init__(self):
+        self.queue = cqueue_lib.new__queue()
+
+    def is_empty(self) -> bool:
+        return cqueue_lib.is_empty(self.queue)
+
+    def __len__(self) -> int:
+        return self.queue.contents.length
+
+    def enqueue(self, item: Any) -> None:
+        cqueue_lib.enqueue(self.queue, item)
+
+    def dequeue(self) -> Any:
+        if self.is_empty():
+            raise IndexError
+        return cqueue_lib.dequeue(self.queue)
+
+    def clear(self):
+        cqueue_lib.free_q(self.queue)
+        self.queue = cqueue_lib.new__queue()
+
+    def __del__(self):
+        cqueue_lib.free_q(self.queue)
```

### Comparing `fastqueue-lib-0.0.2/src/ccqueue.cpp` & `fastqueue-lib-0.0.3/src/ccqueue.cpp`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-/**
- * Copyright (c) 2023 Matthew Andre Taylor
- */
-#ifdef _WIN32
-#define QUEUE_LIBRARY_API extern "C" __declspec(dllexport)
-#else
-#define QUEUE_LIBRARY_API extern "C"
-#endif
-
-#include <Python.h>
-#include <stdlib.h>
-#include <stdio.h>
-
-// Matt's C Contiguous Queue
-QUEUE_LIBRARY_API typedef struct queue {
-    PyObject** objects;
-    int length;
-    int capacity;
-    int front;
-    int back;
-} queue_t;
-
-QUEUE_LIBRARY_API int is_empty(queue_t* queue) {
-    if (queue == NULL) {
-        perror("Queue not allocated");
-        return 1;
-    }
-    return queue->length == 0;
-}
-
-QUEUE_LIBRARY_API queue_t* new__queue() {
-    queue_t* queue = (queue_t*) malloc(sizeof(queue_t));
-    queue->length = 0;
-    queue->capacity = 256;
-    queue->front = 0;
-    queue->back = queue->capacity -1;
-    queue->objects = (PyObject**) malloc(256 * sizeof(PyObject*));
-    return queue;
-}
-
-void resize(queue_t* queue, int newCapacity) {
-    PyObject** newObjects = (PyObject**) malloc(newCapacity * sizeof(PyObject*));
-    for (int i = 0; i < queue->length; ++i) {
-        newObjects[i] = queue->objects[(queue->front + i) % queue->capacity];
-    }
-
-    free(queue->objects);
-    queue->objects = newObjects;
-    queue->front = 0;
-    queue->back = queue->length - 1;
-    queue->capacity = newCapacity;
-}
-
-QUEUE_LIBRARY_API void enqueue(queue_t* queue, PyObject* object) {
-    if (object == Py_None)
-        return;
-
-    if (queue->length == queue->capacity)
-        resize(queue, queue->capacity * 2);
-
-    Py_INCREF(object);
-    queue->front = (queue->front + queue->capacity - 1) % queue->capacity;
-    queue->objects[queue->front] = object;
-    queue->length++;
-}
-
-QUEUE_LIBRARY_API PyObject* dequeue(queue_t* queue) {
-    if (is_empty(queue))
-        return NULL;
-
-    PyObject* object = queue->objects[queue->back];
-    queue->back = (queue->back + queue->capacity - 1) % queue->capacity;
-    queue->length--;
-    return object;
-}
-
-QUEUE_LIBRARY_API void free_q(queue_t* queue) {
-    if (queue == NULL) {
-        perror("Queue not allocated");
-        return;
-    }
-
-    for (int i = 0; i < queue->length; i++) {
-        int index = (queue->front + i) % queue->capacity;
-        Py_DECREF(queue->objects[index]);
-    }
-    free(queue->objects);
-    free(queue);
-}
+/**
+ * Copyright (c) 2023 Matthew Andre Taylor
+ */
+#ifdef _WIN32
+#define QUEUE_LIBRARY_API extern "C" __declspec(dllexport)
+#else
+#define QUEUE_LIBRARY_API extern "C"
+#endif
+
+#include <Python.h>
+#include <stdlib.h>
+#include <stdio.h>
+
+// Matt's C Contiguous Queue
+QUEUE_LIBRARY_API typedef struct queue {
+    PyObject** objects;
+    int length;
+    int capacity;
+    int front;
+    int back;
+} queue_t;
+
+QUEUE_LIBRARY_API int is_empty(queue_t* queue) {
+    if (queue == NULL) {
+        perror("Queue not allocated");
+        return 1;
+    }
+    return queue->length == 0;
+}
+
+QUEUE_LIBRARY_API queue_t* new__queue() {
+    queue_t* queue = (queue_t*) malloc(sizeof(queue_t));
+    queue->length = 0;
+    queue->capacity = 256;
+    queue->front = 0;
+    queue->back = queue->capacity -1;
+    queue->objects = (PyObject**) malloc(256 * sizeof(PyObject*));
+    return queue;
+}
+
+void resize(queue_t* queue, int newCapacity) {
+    PyObject** newObjects = (PyObject**) malloc(newCapacity * sizeof(PyObject*));
+    for (int i = 0; i < queue->length; ++i) {
+        newObjects[i] = queue->objects[(queue->front + i) % queue->capacity];
+    }
+
+    free(queue->objects);
+    queue->objects = newObjects;
+    queue->front = 0;
+    queue->back = queue->length - 1;
+    queue->capacity = newCapacity;
+}
+
+QUEUE_LIBRARY_API void enqueue(queue_t* queue, PyObject* object) {
+    if (object == Py_None)
+        return;
+
+    if (queue->length == queue->capacity)
+        resize(queue, queue->capacity * 2);
+
+    Py_INCREF(object);
+    queue->front = (queue->front + queue->capacity - 1) % queue->capacity;
+    queue->objects[queue->front] = object;
+    queue->length++;
+}
+
+QUEUE_LIBRARY_API PyObject* dequeue(queue_t* queue) {
+    if (is_empty(queue))
+        return NULL;
+
+    PyObject* object = queue->objects[queue->back];
+    queue->back = (queue->back + queue->capacity - 1) % queue->capacity;
+    queue->length--;
+    return object;
+}
+
+QUEUE_LIBRARY_API void free_q(queue_t* queue) {
+    if (queue == NULL) {
+        perror("Queue not allocated");
+        return;
+    }
+
+    for (int i = 0; i < queue->length; i++) {
+        int index = (queue->front + i) % queue->capacity;
+        Py_DECREF(queue->objects[index]);
+    }
+    free(queue->objects);
+    free(queue);
+}
```

### Comparing `fastqueue-lib-0.0.2/src/cllqueue.cpp` & `fastqueue-lib-0.0.3/src/cllqueue.cpp`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-/**
- * Copyright (c) 2023 Matthew Andre Taylor
- */
-#ifdef _WIN32
-#define QUEUE_LIBRARY_API extern "C" __declspec(dllexport)
-#else
-#define QUEUE_LIBRARY_API extern "C"
-#endif
-
-#include <Python.h>
-#include <stdlib.h>
-#include <stdio.h>
-
-// Matt's C Linked List Queue
-
-QUEUE_LIBRARY_API typedef struct node {
-    PyObject* object;
-    struct node* next;
-} node_t;
-
-QUEUE_LIBRARY_API typedef struct queue {
-    node_t* front;
-    node_t* back;
-    unsigned int length;
-} queue_t;
-
-node_t* new_node(PyObject* object) {
-    node_t* node = (node_t*) malloc(sizeof(node_t));
-    if (node == NULL) return NULL;
-
-    Py_INCREF(object);
-    node->object = object;
-    node->next = NULL;
-    return node;
-}
-
-QUEUE_LIBRARY_API queue_t* new_node_queue() {
-    queue_t* queue = (queue_t*) malloc(sizeof(queue_t));
-    queue->front = NULL;
-    queue->back = NULL;
-    queue->length = 0;
-    return queue;
-}
-
-QUEUE_LIBRARY_API int is_empty(queue_t* queue) {
-    if (queue == NULL) {
-        perror("Queue not allocated");
-        return 1;
-    }
-    return queue->length == 0;
-}
-
-QUEUE_LIBRARY_API void enqueue(queue_t* queue, PyObject* object) {
-    if (object == Py_None)
-        return;
-
-    node_t* node = new_node(object);
-    if (queue->back == NULL) {
-        queue->front = node;
-        queue->back = node;
-    } else {
-        queue->back->next = node;
-        queue->back = node;
-    }
-    queue->length++;
-}
-
-QUEUE_LIBRARY_API PyObject* dequeue(queue_t* queue) {
-    if (is_empty(queue))
-        return NULL;
-
-    node_t* temp = queue->front;
-    PyObject* object = temp->object;
-    queue->front = temp->next;
-    free(temp);
-    if (queue->front == NULL)
-        queue->back = NULL;
-    queue->length--;
-    return object;
-}
-
-QUEUE_LIBRARY_API void free_q(queue_t* queue) {
-    if (queue == NULL) {
-        perror("Queue not allocated");
-        return;
-    }
-
-    node_t* current = queue->front;
-    node_t* next;
-    while (current != NULL) {
-        next = current->next;
-        Py_DECREF(current->object);
-        free(current);
-        current = next;
-    }
-    free(queue);
-}
+/**
+ * Copyright (c) 2023 Matthew Andre Taylor
+ */
+#ifdef _WIN32
+#define QUEUE_LIBRARY_API extern "C" __declspec(dllexport)
+#else
+#define QUEUE_LIBRARY_API extern "C"
+#endif
+
+#include <Python.h>
+#include <stdlib.h>
+#include <stdio.h>
+
+// Matt's C Linked List Queue
+
+QUEUE_LIBRARY_API typedef struct node {
+    PyObject* object;
+    struct node* next;
+} node_t;
+
+QUEUE_LIBRARY_API typedef struct queue {
+    node_t* front;
+    node_t* back;
+    unsigned int length;
+} queue_t;
+
+node_t* new_node(PyObject* object) {
+    node_t* node = (node_t*) malloc(sizeof(node_t));
+    if (node == NULL) return NULL;
+
+    Py_INCREF(object);
+    node->object = object;
+    node->next = NULL;
+    return node;
+}
+
+QUEUE_LIBRARY_API queue_t* new_node_queue() {
+    queue_t* queue = (queue_t*) malloc(sizeof(queue_t));
+    queue->front = NULL;
+    queue->back = NULL;
+    queue->length = 0;
+    return queue;
+}
+
+QUEUE_LIBRARY_API int is_empty(queue_t* queue) {
+    if (queue == NULL) {
+        perror("Queue not allocated");
+        return 1;
+    }
+    return queue->length == 0;
+}
+
+QUEUE_LIBRARY_API void enqueue(queue_t* queue, PyObject* object) {
+    if (object == Py_None)
+        return;
+
+    node_t* node = new_node(object);
+    if (queue->back == NULL) {
+        queue->front = node;
+        queue->back = node;
+    } else {
+        queue->back->next = node;
+        queue->back = node;
+    }
+    queue->length++;
+}
+
+QUEUE_LIBRARY_API PyObject* dequeue(queue_t* queue) {
+    if (is_empty(queue))
+        return NULL;
+
+    node_t* temp = queue->front;
+    PyObject* object = temp->object;
+    queue->front = temp->next;
+    free(temp);
+    if (queue->front == NULL)
+        queue->back = NULL;
+    queue->length--;
+    return object;
+}
+
+QUEUE_LIBRARY_API void free_q(queue_t* queue) {
+    if (queue == NULL) {
+        perror("Queue not allocated");
+        return;
+    }
+
+    node_t* current = queue->front;
+    node_t* next;
+    while (current != NULL) {
+        next = current->next;
+        Py_DECREF(current->object);
+        free(current);
+        current = next;
+    }
+    free(queue);
+}
```

### Comparing `fastqueue-lib-0.0.2/src/fastqueue.c` & `fastqueue-lib-0.0.3/src/fastqueue.c`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,551 +1,551 @@
-/**
- * Copyright (c) 2023 Matthew Andre Taylor
- */
-#include <Python.h>
-
-/**
- * Single ended Contiguous Python Queue
- * --- fastqueue.QueueC ---
- */
-typedef struct {
-    PyObject_VAR_HEAD
-    PyObject** objects;
-    int length;
-    int capacity;
-    int front;
-    int back;
-} QueueC;
-
-static PyObject* QueueC_is_empty(QueueC* self, PyObject* args) {
-    if (self->length == 0)
-        Py_RETURN_TRUE;
-    else
-        Py_RETURN_FALSE;
-}
-
-static PyObject* QueueC_new(PyTypeObject* type, PyObject* args, PyObject* kwargs) {
-    QueueC* self = (QueueC*)type->tp_alloc(type, 0);
-    if (self == NULL)
-        return PyErr_NoMemory();
-
-    self->objects = (PyObject**) malloc(1024 * sizeof(PyObject*));
-    if (self->objects == NULL) {
-        Py_DECREF(self);
-        return PyErr_NoMemory();
-    }
-
-    self->length = 0;
-    self->capacity = 1024;
-    self->front = 1023;
-    self->back = 0;
-    return (PyObject*)self;
-}
-
-static void QueueC_dealloc(QueueC* self) {
-    if (self == NULL)
-        return;
-    PyObject_GC_UnTrack(self);
-    free(self->objects);
-    self->objects = NULL;
-    Py_TYPE(self)->tp_free(self);
-}
-
-static int QueueC_clear(QueueC* self) {
-    if (self->length == 0)
-        return 0;
-
-    for (int i = 0; i < self->length; ++i) {
-        int index = (self->back + i) % self->capacity;
-        if (self->objects[index] != NULL && !PyObject_IS_GC(self->objects[index])) {
-            Py_DECREF(self->objects[index]);
-            self->objects[index] = NULL;
-        }
-    }
-    self->length = 0;
-    self->front = self->capacity - 1;
-    self->back = 0;
-    return 0;
-}
-
-static int QueueC_traverse(QueueC* self, visitproc visit, void* arg) {
-    for (int i = 0; i < self->length; ++i) {
-        int index = (self->back + i) % self->capacity;
-        Py_VISIT(self->objects[index]);
-    }
-    return 0;
-}
-
-static void QueueC_resize(QueueC* self, int newCapacity) {
-    PyObject** newObjects = (PyObject**) malloc(newCapacity * sizeof(PyObject*));
-    if (newObjects == NULL) {
-        PyErr_NoMemory();
-        return;
-    }
-    for (int i = 0; i < self->length; ++i) {
-        newObjects[i] = self->objects[(self->back + i) % self->capacity];
-    }
-
-    free(self->objects);
-    self->objects = newObjects;
-    self->capacity = newCapacity;
-}
-
-static PyObject* QueueC_enqueue(QueueC* self, PyObject* object) {
-    if (object == Py_None)
-        Py_RETURN_NONE;
-    if (self->length == self->capacity)
-        QueueC_resize(self, self->capacity * 2);
-
-    Py_INCREF(object);
-    self->front = (self->front + 1) % self->capacity;
-    self->objects[self->front] = object;
-    self->length++;
-    Py_RETURN_NONE;
-}
-
-static PyObject* QueueC_dequeue(QueueC* self) {
-    if (self->length == 0) {
-        PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
-        return NULL;
-    }
-
-    PyObject* object = self->objects[self->back];
-    self->back = (self->back + 1) % self->capacity;
-    self->length--;
-    return object;
-}
-
-static PyObject* QueueC_extend(QueueC* self, PyObject* iterator) {
-    PyObject* iterable = PyObject_GetIter(iterator);
-    if (iterable == NULL)
-        return NULL;
-
-    PyObject* py_object;
-    PyObject* (*next)(PyObject*);
-    next = *Py_TYPE(iterable)->tp_iternext;
-    while ((py_object = next(iterable)) != NULL) {
-        QueueC_enqueue(self, py_object);
-    }
-    Py_DECREF(iterable);
-    Py_RETURN_NONE;
-}
-
-static Py_ssize_t QueueC_len(QueueC* self) {
-    return (Py_ssize_t)self->length;
-}
-
-static PyObject* QueueC_item(QueueC* self, Py_ssize_t index) {
-    if (index < 0)
-        index = index + QueueC_len(self);
-    if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
-        return NULL;
-    }
-    PyObject* object = self->objects[(self->back + index) % self->capacity];
-    Py_INCREF(object);
-    return object;
-}
-
-static int QueueC_setitem(QueueC* self, Py_ssize_t index, PyObject* object) {
-    if (index < 0)
-        index = QueueC_len(self) + index;
-
-    if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
-        return -1;
-    }
-
-    PyObject* oldObject = self->objects[(self->back + index) % self->capacity];
-    Py_DECREF(oldObject);
-    if (object == NULL) {
-        self->objects[(self->back + index) % self->capacity] = Py_None;
-    }
-    else {
-        Py_INCREF(object);
-        self->objects[(self->back + index) % self->capacity] = object;
-    }
-    return 0;
-}
-
-static int QueueC_contains(QueueC* self, PyObject* object) {
-    for (int i = 0; i < self->length; ++i) {
-        int index = (self->back + i) % self->capacity;
-        if (self->objects[index] != NULL && PyObject_RichCompareBool(object, self->objects[index], Py_EQ))
-            return 1;
-    }
-    return 0;
-}
-
-static PySequenceMethods QueueC_sequence_methods = {
-    (lenfunc)QueueC_len,                  /* sq_length */
-    NULL,                                 /* sq_concat */
-    NULL,                                 /* sq_repeat */
-    (ssizeargfunc)QueueC_item,            /* sq_item */
-    NULL,                                 /* sq_slice */
-    (ssizeobjargproc)QueueC_setitem,      /* sq_as_item */
-    NULL,                                 /* sq_as_slice */
-    (objobjproc)QueueC_contains,          /* sq_contains */
-    (binaryfunc)QueueC_extend             /* sq_inplace_concat */
-};
-
-static PyMethodDef QueueC_methods[] = {
-    {"enqueue", (PyCFunction)QueueC_enqueue, METH_O, "Add an object to the front of the QueueC."},
-    {"dequeue", (PyCFunction)QueueC_dequeue, METH_NOARGS, "Remove and return an object from the back of the QueueC."},
-    {"is_empty", (PyCFunction)QueueC_is_empty, METH_NOARGS, "Check if the QueueC is empty."},
-    {"extend", (PyCFunction)QueueC_extend, METH_O, "Add an objects from an iterator front of the QueueC."},
-    {NULL, NULL, 0, NULL}
-};
-
-PyDoc_STRVAR(queuec_doc, "QueueC() -> Contiguous Single ended Queue object.");
-static PyTypeObject QueueCType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "QueueC",                                   /* tp_name */
-    sizeof(QueueC),                             /* tp_basicsize */
-    0,                                          /* tp_itemsize */
-    (destructor)QueueC_dealloc,                 /* tp_dealloc */
-    0,                                          /* tp_print */
-    0,                                          /* tp_getattr */
-    0,                                          /* tp_setattr */
-    0,                                          /* tp_reserved */
-    0,                                          /* tp_repr */
-    0,                                          /* tp_as_number */
-    &QueueC_sequence_methods,                   /* tp_as_sequence */
-    0,                                          /* tp_as_mapping */
-    PyObject_HashNotImplemented,                /* tp_hash */
-    0,                                          /* tp_call */
-    0,                                          /* tp_str */
-    0,                                          /* tp_getattro */
-    0,                                          /* tp_setattro */
-    0,                                          /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,    /* tp_flags */
-    queuec_doc,                                 /* tp_doc */
-    (traverseproc)QueueC_traverse,              /* tp_traverse */
-    (inquiry)QueueC_clear,                      /* tp_clear */
-    0,                                          /* tp_richcompare */
-    0,                                          /* tp_weaklistoffset */
-    0,                                          /* tp_iter */
-    0,                                          /* tp_iternext */
-    QueueC_methods,                             /* tp_methods */
-    0,                                          /* tp_members */
-    0,                                          /* tp_getset */
-    0,                                          /* tp_base */
-    0,                                          /* tp_dict */
-    0,                                          /* tp_descr_get */
-    0,                                          /* tp_descr_set */
-    0,                                          /* tp_dictoffset */
-    0,                                          /* tp_init */
-    PyType_GenericAlloc,                        /* tp_alloc */
-    QueueC_new,                                 /* tp_new */
-    PyObject_GC_Del,                            /* tp_free */
-};
-
-
-/**
- * Single ended Python Queue with subqueue chunks
- * --- fastqueue.QueueC ---
- */
-typedef struct QueueNode {
-    PyObject* py_objects[256];
-    int numEntries; // Number of entries into this node
-    int front;
-    int back;
-    struct QueueNode* next;
-} QueueNode_t;
-
-typedef struct Queue {
-    PyObject_HEAD
-    QueueNode_t* head;
-    QueueNode_t* tail;
-    int length; // Total number of py_objects stored in the queue
-} Queue_t;
-
-PyDoc_STRVAR(is_empty_doc, "Returns whether the queue is empty.");
-static PyObject* Queue_is_empty(Queue_t* self, PyObject* args) {
-    if (self->length == 0)
-        Py_RETURN_TRUE;
-    else
-        Py_RETURN_FALSE;
-}
-
-// Initialize a new QueueNode
-static QueueNode_t* QueueNode_new() {
-    QueueNode_t* node = (QueueNode_t*) malloc(sizeof(QueueNode_t));
-    node->numEntries = 0;
-    node->front = 255;
-    node->back = 0;
-    node->next = NULL;
-    return node;
-}
-
-static PyObject* Queue_new(PyTypeObject* type, PyObject* args, PyObject* kwargs) {
-    Queue_t* self = (Queue_t*)type->tp_alloc(type, 0);
-    if (self == NULL)
-        return PyErr_NoMemory();
-
-    self->head = NULL;
-    self->tail = NULL;
-    self->length = 0;
-    return (PyObject*)self;
-}
-
-// Add a py_object to the front of the QueueNode
-static inline void QueueNode_put(QueueNode_t* queue_node, PyObject* py_object) {
-    Py_INCREF(py_object);
-    queue_node->front = (queue_node->front + 1) & 255;
-    queue_node->py_objects[queue_node->front] = py_object;
-    queue_node->numEntries++;
-}
-
-// Add a py_object to the last QueueNode in the Queue
-PyDoc_STRVAR(enqueue_doc, "Add an item to the front of the queue.");
-static PyObject* Queue_enqueue(Queue_t* self, PyObject* object) {
-    if (object == Py_None)
-        Py_RETURN_NONE;
-
-    if (self->tail == NULL) {
-        self->head = QueueNode_new();
-        self->tail = self->head;
-    } else {
-        if (self->tail->numEntries >= 256) {
-            if (self->tail->next == NULL) {
-                QueueNode_t* node = QueueNode_new();
-                self->tail->next = node;
-                self->tail = node;
-            }
-        }
-    }
-
-    QueueNode_put(self->tail, object);
-    self->length++;
-    Py_RETURN_NONE;
-}
-
-// Remove a py_object from the first QueueNode in the Queue
-PyDoc_STRVAR(dequeue_doc, "Remove and return an item from the end of the queue.");
-static PyObject* Queue_dequeue(Queue_t* self) {
-    if (self->length == 0) {
-        PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
-        return NULL;
-    }
-
-    PyObject* py_object = self->head->py_objects[self->head->back];
-    self->head->back = (self->head->back + 1) & 255;
-    self->head->numEntries--;
-    self->length--;
-
-    if (self->head->numEntries <= 0) {
-        QueueNode_t* oldHead = self->head;
-        self->head = self->head->next;
-        free(oldHead);
-    }
-
-    if (self->head == NULL)
-        self->tail = NULL;
-
-    return py_object;
-}
-
-static int Queue_clear(Queue_t *self) {
-    if (self->length == 0)
-        return 0;
-
-    QueueNode_t* current = self->head;
-    QueueNode_t* next;
-    while (current != NULL) {
-        for (int i = 0; i < current->numEntries; ++i) {
-            int index = (current->back + i) & 255;
-            if (current->py_objects[index] != NULL && !PyObject_IS_GC(current->py_objects[index])) {
-                Py_DECREF(current->py_objects[index]);
-                current->py_objects[index] = NULL;
-            }
-        }
-        next = current->next;
-        free(current);
-        current = next;
-    }
-    self->length = 0;
-    self->head = NULL;
-    self->tail = NULL;
-    return 0;
-}
-
-// Deallocate the Queue
-static void Queue_dealloc(Queue_t* self) {
-    if (self == NULL)
-        return;
-    PyObject_GC_UnTrack(self);
-    if (self->head != NULL)
-        Queue_clear(self);
-    Py_TYPE(self)->tp_free((PyObject*)self);
-}
-
-static int Queue_traverse(Queue_t* self, visitproc visit, void* arg) {
-    QueueNode_t* current = self->head;
-    while (current != NULL) {
-        for (int i = 0; i < current->numEntries; ++i) {
-            int index = (current->back + i) & 255;
-            Py_VISIT(current->py_objects[index]);
-        }
-        current = current->next;
-    }
-    return 0;
-}
-
-PyDoc_STRVAR(extend_doc, "Enqueue a sequence of elements from an iterator.");
-static PyObject* Queue_extend(Queue_t* self, PyObject* iterator) {
-    PyObject* iterable = PyObject_GetIter(iterator);
-    if (iterable == NULL)
-        return NULL;
-
-    PyObject* py_object;
-    PyObject* (*next)(PyObject*);
-    next = *Py_TYPE(iterable)->tp_iternext;
-    while ((py_object = next(iterable)) != NULL) {
-        Queue_enqueue(self, py_object);
-    }
-    Py_DECREF(iterable);
-    Py_RETURN_NONE;
-}
-
-static Py_ssize_t Queue_len(Queue_t* self) {
-    return (Py_ssize_t)self->length;
-}
-
-static PyObject* Queue_item(Queue_t* self, Py_ssize_t index) {
-    if (index < 0)
-        index = Queue_len(self) + index;
-
-    if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
-        return NULL;
-    }
-
-    QueueNode_t* current = self->head;
-    for (int i = 0; i < (int)(index / 256); ++i) {
-        current = current->next;
-    }
-    PyObject* object = current->py_objects[(current->back + index) & 255];
-    Py_INCREF(object);
-    return object;
-}
-
-static int Queue_setitem(Queue_t* self, Py_ssize_t index, PyObject* object) {
-    if (index < 0)
-        index = Queue_len(self) + index;
-
-    if (index >= self->length) {
-        PyErr_SetString(PyExc_IndexError, "queue index out of range");
-        return -1;
-    }
-
-    QueueNode_t* current = self->head;
-    for (int i = 0; i < (int)(index / 256); ++i) {
-        current = current->next;
-    }
-    PyObject* oldObject = current->py_objects[(current->back + index) & 255];
-    Py_DECREF(oldObject);
-    if (object == NULL) {
-        current->py_objects[(current->back + index) & 255] = Py_None;
-    }
-    else {
-        Py_INCREF(object);
-        current->py_objects[(current->back + index) & 255] = object;
-    }
-    return 0;
-}
-
-static int Queue_contains(Queue_t* self, PyObject* object) {
-    QueueNode_t* current = self->head;
-    while (current != NULL) {
-        for (int i = 0; i < current->numEntries; ++i) {
-            if (PyObject_RichCompareBool(object, current->py_objects[(current->back + i) & 255], Py_EQ))
-                return 1;
-        }
-        current = current->next;
-    }
-    return 0;
-}
-
-static PySequenceMethods Queue_sequence_methods = {
-    (lenfunc)Queue_len,                  /* sq_length */
-    NULL,                                 /* sq_concat */
-    NULL,                                 /* sq_repeat */
-    (ssizeargfunc)Queue_item,             /* sq_item */
-    NULL,                                 /* sq_slice */
-    (ssizeobjargproc)Queue_setitem,       /* sq_as_item */
-    NULL,                                 /* sq_as_slice */
-    (objobjproc)Queue_contains,           /* sq_contains */
-    (binaryfunc)Queue_extend              /* sq_inplace_concat */
-};
-
-static PyMethodDef Queue_methods[] = {
-    {"enqueue", (PyCFunction)Queue_enqueue, METH_O, enqueue_doc},
-    {"dequeue", (PyCFunction)Queue_dequeue, METH_NOARGS, dequeue_doc},
-    {"is_empty", (PyCFunction)Queue_is_empty, METH_NOARGS, is_empty_doc},
-    {"extend", (PyCFunction)Queue_extend, METH_O, extend_doc},
-    {NULL, NULL, 0, NULL}
-};
-
-PyDoc_STRVAR(queue_doc,"Queue() -> Single ended Queue object.");
-static PyTypeObject QueueType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "Queue",                                    /* tp_name */
-    sizeof(Queue_t),                            /* tp_basicsize */
-    0,                                          /* tp_itemsize */
-    (destructor)Queue_dealloc,                  /* tp_dealloc */
-    0,                                          /* tp_print */
-    0,                                          /* tp_getattr */
-    0,                                          /* tp_setattr */
-    0,                                          /* tp_reserved */
-    0,                                          /* tp_repr */
-    0,                                          /* tp_as_number */
-    &Queue_sequence_methods,                    /* tp_as_sequence */
-    0,                                          /* tp_as_mapping */
-    PyObject_HashNotImplemented,                /* tp_hash */
-    0,                                          /* tp_call */
-    0,                                          /* tp_str */
-    PyObject_GenericGetAttr,                    /* tp_getattro */
-    0,                                          /* tp_setattro */
-    0,                                          /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,    /* tp_flags */
-    queue_doc,                                  /* tp_doc */
-    (traverseproc)Queue_traverse,               /* tp_traverse */
-    (inquiry)Queue_clear,                       /* tp_clear */
-    0,                                          /* tp_richcompare */
-    0,                                          /* tp_weaklistoffset */
-    0,                                          /* tp_iter */
-    0,                                          /* tp_iternext */
-    Queue_methods,                              /* tp_methods */
-    0,                                          /* tp_members */
-    0,                                          /* tp_getset */
-    0,                                          /* tp_base */
-    0,                                          /* tp_dict */
-    0,                                          /* tp_descr_get */
-    0,                                          /* tp_descr_set */
-    0,                                          /* tp_dictoffset */
-    0,                                          /* tp_init */
-    PyType_GenericAlloc,                        /* tp_alloc */
-    (newfunc)Queue_new,                         /* tp_new */
-    PyObject_GC_Del,                            /* tp_free */
-};
-
-static PyModuleDef QueueModuleDef = {
-    PyModuleDef_HEAD_INIT,
-    "_fastqueue",
-    "Singly linked, small overhead implementations of the Queue data structure.",
-    -1,
-    NULL, NULL, NULL, NULL, NULL
-};
-
-PyMODINIT_FUNC PyInit__fastqueue(void) {
-    PyObject* module;
-    if (PyType_Ready(&QueueType) < 0 || PyType_Ready(&QueueCType) < 0)
-        return NULL;
-
-    module = PyModule_Create(&QueueModuleDef);
-    if (module == NULL)
-        return NULL;
-    PyModule_AddType(module, &QueueCType);
-    PyModule_AddType(module, &QueueType);
-    return module;
-}
+/**
+ * Copyright (c) 2023 Matthew Andre Taylor
+ */
+#include <Python.h>
+
+/**
+ * Single ended Contiguous Python Queue
+ * --- fastqueue.QueueC ---
+ */
+typedef struct {
+    PyObject_VAR_HEAD
+    PyObject** objects;
+    int length;
+    int capacity;
+    int front;
+    int back;
+} QueueC;
+
+static PyObject* QueueC_is_empty(QueueC* self, PyObject* args) {
+    if (self->length == 0)
+        Py_RETURN_TRUE;
+    else
+        Py_RETURN_FALSE;
+}
+
+static PyObject* QueueC_new(PyTypeObject* type, PyObject* args, PyObject* kwargs) {
+    QueueC* self = (QueueC*)type->tp_alloc(type, 0);
+    if (self == NULL)
+        return PyErr_NoMemory();
+
+    self->objects = (PyObject**) malloc(1024 * sizeof(PyObject*));
+    if (self->objects == NULL) {
+        Py_DECREF(self);
+        return PyErr_NoMemory();
+    }
+
+    self->length = 0;
+    self->capacity = 1024;
+    self->front = 1023;
+    self->back = 0;
+    return (PyObject*)self;
+}
+
+static void QueueC_dealloc(QueueC* self) {
+    if (self == NULL)
+        return;
+    PyObject_GC_UnTrack(self);
+    free(self->objects);
+    self->objects = NULL;
+    Py_TYPE(self)->tp_free(self);
+}
+
+static int QueueC_clear(QueueC* self) {
+    if (self->length == 0)
+        return 0;
+
+    for (int i = 0; i < self->length; ++i) {
+        int index = (self->back + i) % self->capacity;
+        if (self->objects[index] != NULL && !PyObject_IS_GC(self->objects[index])) {
+            Py_DECREF(self->objects[index]);
+            self->objects[index] = NULL;
+        }
+    }
+    self->length = 0;
+    self->front = self->capacity - 1;
+    self->back = 0;
+    return 0;
+}
+
+static int QueueC_traverse(QueueC* self, visitproc visit, void* arg) {
+    for (int i = 0; i < self->length; ++i) {
+        int index = (self->back + i) % self->capacity;
+        Py_VISIT(self->objects[index]);
+    }
+    return 0;
+}
+
+static void QueueC_resize(QueueC* self, int newCapacity) {
+    PyObject** newObjects = (PyObject**) malloc(newCapacity * sizeof(PyObject*));
+    if (newObjects == NULL) {
+        PyErr_NoMemory();
+        return;
+    }
+    for (int i = 0; i < self->length; ++i) {
+        newObjects[i] = self->objects[(self->back + i) % self->capacity];
+    }
+
+    free(self->objects);
+    self->objects = newObjects;
+    self->capacity = newCapacity;
+}
+
+static PyObject* QueueC_enqueue(QueueC* self, PyObject* object) {
+    if (object == Py_None)
+        Py_RETURN_NONE;
+    if (self->length == self->capacity)
+        QueueC_resize(self, self->capacity * 2);
+
+    Py_INCREF(object);
+    self->front = (self->front + 1) % self->capacity;
+    self->objects[self->front] = object;
+    self->length++;
+    Py_RETURN_NONE;
+}
+
+static PyObject* QueueC_dequeue(QueueC* self) {
+    if (self->length == 0) {
+        PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
+        return NULL;
+    }
+
+    PyObject* object = self->objects[self->back];
+    self->back = (self->back + 1) % self->capacity;
+    self->length--;
+    return object;
+}
+
+static PyObject* QueueC_extend(QueueC* self, PyObject* iterator) {
+    PyObject* iterable = PyObject_GetIter(iterator);
+    if (iterable == NULL)
+        return NULL;
+
+    PyObject* py_object;
+    PyObject* (*next)(PyObject*);
+    next = *Py_TYPE(iterable)->tp_iternext;
+    while ((py_object = next(iterable)) != NULL) {
+        QueueC_enqueue(self, py_object);
+    }
+    Py_DECREF(iterable);
+    Py_RETURN_NONE;
+}
+
+static Py_ssize_t QueueC_len(QueueC* self) {
+    return (Py_ssize_t)self->length;
+}
+
+static PyObject* QueueC_item(QueueC* self, Py_ssize_t index) {
+    if (index < 0)
+        index = index + QueueC_len(self);
+    if (index >= self->length) {
+        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        return NULL;
+    }
+    PyObject* object = self->objects[(self->back + index) % self->capacity];
+    Py_INCREF(object);
+    return object;
+}
+
+static int QueueC_setitem(QueueC* self, Py_ssize_t index, PyObject* object) {
+    if (index < 0)
+        index = QueueC_len(self) + index;
+
+    if (index >= self->length) {
+        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        return -1;
+    }
+
+    PyObject* oldObject = self->objects[(self->back + index) % self->capacity];
+    Py_DECREF(oldObject);
+    if (object == NULL) {
+        self->objects[(self->back + index) % self->capacity] = Py_None;
+    }
+    else {
+        Py_INCREF(object);
+        self->objects[(self->back + index) % self->capacity] = object;
+    }
+    return 0;
+}
+
+static int QueueC_contains(QueueC* self, PyObject* object) {
+    for (int i = 0; i < self->length; ++i) {
+        int index = (self->back + i) % self->capacity;
+        if (self->objects[index] != NULL && PyObject_RichCompareBool(object, self->objects[index], Py_EQ))
+            return 1;
+    }
+    return 0;
+}
+
+static PySequenceMethods QueueC_sequence_methods = {
+    (lenfunc)QueueC_len,                  /* sq_length */
+    NULL,                                 /* sq_concat */
+    NULL,                                 /* sq_repeat */
+    (ssizeargfunc)QueueC_item,            /* sq_item */
+    NULL,                                 /* sq_slice */
+    (ssizeobjargproc)QueueC_setitem,      /* sq_as_item */
+    NULL,                                 /* sq_as_slice */
+    (objobjproc)QueueC_contains,          /* sq_contains */
+    (binaryfunc)QueueC_extend             /* sq_inplace_concat */
+};
+
+static PyMethodDef QueueC_methods[] = {
+    {"enqueue", (PyCFunction)QueueC_enqueue, METH_O, "Add an object to the front of the QueueC."},
+    {"dequeue", (PyCFunction)QueueC_dequeue, METH_NOARGS, "Remove and return an object from the back of the QueueC."},
+    {"is_empty", (PyCFunction)QueueC_is_empty, METH_NOARGS, "Check if the QueueC is empty."},
+    {"extend", (PyCFunction)QueueC_extend, METH_O, "Add an objects from an iterator front of the QueueC."},
+    {NULL, NULL, 0, NULL}
+};
+
+PyDoc_STRVAR(queuec_doc, "QueueC() -> Contiguous Single ended Queue object.");
+static PyTypeObject QueueCType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "QueueC",                                   /* tp_name */
+    sizeof(QueueC),                             /* tp_basicsize */
+    0,                                          /* tp_itemsize */
+    (destructor)QueueC_dealloc,                 /* tp_dealloc */
+    0,                                          /* tp_print */
+    0,                                          /* tp_getattr */
+    0,                                          /* tp_setattr */
+    0,                                          /* tp_reserved */
+    0,                                          /* tp_repr */
+    0,                                          /* tp_as_number */
+    &QueueC_sequence_methods,                   /* tp_as_sequence */
+    0,                                          /* tp_as_mapping */
+    PyObject_HashNotImplemented,                /* tp_hash */
+    0,                                          /* tp_call */
+    0,                                          /* tp_str */
+    0,                                          /* tp_getattro */
+    0,                                          /* tp_setattro */
+    0,                                          /* tp_as_buffer */
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,    /* tp_flags */
+    queuec_doc,                                 /* tp_doc */
+    (traverseproc)QueueC_traverse,              /* tp_traverse */
+    (inquiry)QueueC_clear,                      /* tp_clear */
+    0,                                          /* tp_richcompare */
+    0,                                          /* tp_weaklistoffset */
+    0,                                          /* tp_iter */
+    0,                                          /* tp_iternext */
+    QueueC_methods,                             /* tp_methods */
+    0,                                          /* tp_members */
+    0,                                          /* tp_getset */
+    0,                                          /* tp_base */
+    0,                                          /* tp_dict */
+    0,                                          /* tp_descr_get */
+    0,                                          /* tp_descr_set */
+    0,                                          /* tp_dictoffset */
+    0,                                          /* tp_init */
+    PyType_GenericAlloc,                        /* tp_alloc */
+    QueueC_new,                                 /* tp_new */
+    PyObject_GC_Del,                            /* tp_free */
+};
+
+
+/**
+ * Single ended Python Queue with subqueue chunks
+ * --- fastqueue.QueueC ---
+ */
+typedef struct QueueNode {
+    PyObject* py_objects[256];
+    int numEntries; // Number of entries into this node
+    int front;
+    int back;
+    struct QueueNode* next;
+} QueueNode_t;
+
+typedef struct Queue {
+    PyObject_HEAD
+    QueueNode_t* head;
+    QueueNode_t* tail;
+    int length; // Total number of py_objects stored in the queue
+} Queue_t;
+
+PyDoc_STRVAR(is_empty_doc, "Returns whether the queue is empty.");
+static PyObject* Queue_is_empty(Queue_t* self, PyObject* args) {
+    if (self->length == 0)
+        Py_RETURN_TRUE;
+    else
+        Py_RETURN_FALSE;
+}
+
+// Initialize a new QueueNode
+static QueueNode_t* QueueNode_new() {
+    QueueNode_t* node = (QueueNode_t*) malloc(sizeof(QueueNode_t));
+    node->numEntries = 0;
+    node->front = 255;
+    node->back = 0;
+    node->next = NULL;
+    return node;
+}
+
+static PyObject* Queue_new(PyTypeObject* type, PyObject* args, PyObject* kwargs) {
+    Queue_t* self = (Queue_t*)type->tp_alloc(type, 0);
+    if (self == NULL)
+        return PyErr_NoMemory();
+
+    self->head = NULL;
+    self->tail = NULL;
+    self->length = 0;
+    return (PyObject*)self;
+}
+
+// Add a py_object to the front of the QueueNode
+static inline void QueueNode_put(QueueNode_t* queue_node, PyObject* py_object) {
+    Py_INCREF(py_object);
+    queue_node->front = (queue_node->front + 1) & 255;
+    queue_node->py_objects[queue_node->front] = py_object;
+    queue_node->numEntries++;
+}
+
+// Add a py_object to the last QueueNode in the Queue
+PyDoc_STRVAR(enqueue_doc, "Add an item to the front of the queue.");
+static PyObject* Queue_enqueue(Queue_t* self, PyObject* object) {
+    if (object == Py_None)
+        Py_RETURN_NONE;
+
+    if (self->tail == NULL) {
+        self->head = QueueNode_new();
+        self->tail = self->head;
+    } else {
+        if (self->tail->numEntries >= 256) {
+            if (self->tail->next == NULL) {
+                QueueNode_t* node = QueueNode_new();
+                self->tail->next = node;
+                self->tail = node;
+            }
+        }
+    }
+
+    QueueNode_put(self->tail, object);
+    self->length++;
+    Py_RETURN_NONE;
+}
+
+// Remove a py_object from the first QueueNode in the Queue
+PyDoc_STRVAR(dequeue_doc, "Remove and return an item from the end of the queue.");
+static PyObject* Queue_dequeue(Queue_t* self) {
+    if (self->length == 0) {
+        PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
+        return NULL;
+    }
+
+    PyObject* py_object = self->head->py_objects[self->head->back];
+    self->head->back = (self->head->back + 1) & 255;
+    self->head->numEntries--;
+    self->length--;
+
+    if (self->head->numEntries <= 0) {
+        QueueNode_t* oldHead = self->head;
+        self->head = self->head->next;
+        free(oldHead);
+    }
+
+    if (self->head == NULL)
+        self->tail = NULL;
+
+    return py_object;
+}
+
+static int Queue_clear(Queue_t *self) {
+    if (self->length == 0)
+        return 0;
+
+    QueueNode_t* current = self->head;
+    QueueNode_t* next;
+    while (current != NULL) {
+        for (int i = 0; i < current->numEntries; ++i) {
+            int index = (current->back + i) & 255;
+            if (current->py_objects[index] != NULL && !PyObject_IS_GC(current->py_objects[index])) {
+                Py_DECREF(current->py_objects[index]);
+                current->py_objects[index] = NULL;
+            }
+        }
+        next = current->next;
+        free(current);
+        current = next;
+    }
+    self->length = 0;
+    self->head = NULL;
+    self->tail = NULL;
+    return 0;
+}
+
+// Deallocate the Queue
+static void Queue_dealloc(Queue_t* self) {
+    if (self == NULL)
+        return;
+    PyObject_GC_UnTrack(self);
+    if (self->head != NULL)
+        Queue_clear(self);
+    Py_TYPE(self)->tp_free((PyObject*)self);
+}
+
+static int Queue_traverse(Queue_t* self, visitproc visit, void* arg) {
+    QueueNode_t* current = self->head;
+    while (current != NULL) {
+        for (int i = 0; i < current->numEntries; ++i) {
+            int index = (current->back + i) & 255;
+            Py_VISIT(current->py_objects[index]);
+        }
+        current = current->next;
+    }
+    return 0;
+}
+
+PyDoc_STRVAR(extend_doc, "Enqueue a sequence of elements from an iterator.");
+static PyObject* Queue_extend(Queue_t* self, PyObject* iterator) {
+    PyObject* iterable = PyObject_GetIter(iterator);
+    if (iterable == NULL)
+        return NULL;
+
+    PyObject* py_object;
+    PyObject* (*next)(PyObject*);
+    next = *Py_TYPE(iterable)->tp_iternext;
+    while ((py_object = next(iterable)) != NULL) {
+        Queue_enqueue(self, py_object);
+    }
+    Py_DECREF(iterable);
+    Py_RETURN_NONE;
+}
+
+static Py_ssize_t Queue_len(Queue_t* self) {
+    return (Py_ssize_t)self->length;
+}
+
+static PyObject* Queue_item(Queue_t* self, Py_ssize_t index) {
+    if (index < 0)
+        index = Queue_len(self) + index;
+
+    if (index >= self->length) {
+        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        return NULL;
+    }
+
+    QueueNode_t* current = self->head;
+    for (int i = 0; i < (int)(index / 256); ++i) {
+        current = current->next;
+    }
+    PyObject* object = current->py_objects[(current->back + index) & 255];
+    Py_INCREF(object);
+    return object;
+}
+
+static int Queue_setitem(Queue_t* self, Py_ssize_t index, PyObject* object) {
+    if (index < 0)
+        index = Queue_len(self) + index;
+
+    if (index >= self->length) {
+        PyErr_SetString(PyExc_IndexError, "queue index out of range");
+        return -1;
+    }
+
+    QueueNode_t* current = self->head;
+    for (int i = 0; i < (int)(index / 256); ++i) {
+        current = current->next;
+    }
+    PyObject* oldObject = current->py_objects[(current->back + index) & 255];
+    Py_DECREF(oldObject);
+    if (object == NULL) {
+        current->py_objects[(current->back + index) & 255] = Py_None;
+    }
+    else {
+        Py_INCREF(object);
+        current->py_objects[(current->back + index) & 255] = object;
+    }
+    return 0;
+}
+
+static int Queue_contains(Queue_t* self, PyObject* object) {
+    QueueNode_t* current = self->head;
+    while (current != NULL) {
+        for (int i = 0; i < current->numEntries; ++i) {
+            if (PyObject_RichCompareBool(object, current->py_objects[(current->back + i) & 255], Py_EQ))
+                return 1;
+        }
+        current = current->next;
+    }
+    return 0;
+}
+
+static PySequenceMethods Queue_sequence_methods = {
+    (lenfunc)Queue_len,                  /* sq_length */
+    NULL,                                 /* sq_concat */
+    NULL,                                 /* sq_repeat */
+    (ssizeargfunc)Queue_item,             /* sq_item */
+    NULL,                                 /* sq_slice */
+    (ssizeobjargproc)Queue_setitem,       /* sq_as_item */
+    NULL,                                 /* sq_as_slice */
+    (objobjproc)Queue_contains,           /* sq_contains */
+    (binaryfunc)Queue_extend              /* sq_inplace_concat */
+};
+
+static PyMethodDef Queue_methods[] = {
+    {"enqueue", (PyCFunction)Queue_enqueue, METH_O, enqueue_doc},
+    {"dequeue", (PyCFunction)Queue_dequeue, METH_NOARGS, dequeue_doc},
+    {"is_empty", (PyCFunction)Queue_is_empty, METH_NOARGS, is_empty_doc},
+    {"extend", (PyCFunction)Queue_extend, METH_O, extend_doc},
+    {NULL, NULL, 0, NULL}
+};
+
+PyDoc_STRVAR(queue_doc,"Queue() -> Single ended Queue object.");
+static PyTypeObject QueueType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "Queue",                                    /* tp_name */
+    sizeof(Queue_t),                            /* tp_basicsize */
+    0,                                          /* tp_itemsize */
+    (destructor)Queue_dealloc,                  /* tp_dealloc */
+    0,                                          /* tp_print */
+    0,                                          /* tp_getattr */
+    0,                                          /* tp_setattr */
+    0,                                          /* tp_reserved */
+    0,                                          /* tp_repr */
+    0,                                          /* tp_as_number */
+    &Queue_sequence_methods,                    /* tp_as_sequence */
+    0,                                          /* tp_as_mapping */
+    PyObject_HashNotImplemented,                /* tp_hash */
+    0,                                          /* tp_call */
+    0,                                          /* tp_str */
+    PyObject_GenericGetAttr,                    /* tp_getattro */
+    0,                                          /* tp_setattro */
+    0,                                          /* tp_as_buffer */
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,    /* tp_flags */
+    queue_doc,                                  /* tp_doc */
+    (traverseproc)Queue_traverse,               /* tp_traverse */
+    (inquiry)Queue_clear,                       /* tp_clear */
+    0,                                          /* tp_richcompare */
+    0,                                          /* tp_weaklistoffset */
+    0,                                          /* tp_iter */
+    0,                                          /* tp_iternext */
+    Queue_methods,                              /* tp_methods */
+    0,                                          /* tp_members */
+    0,                                          /* tp_getset */
+    0,                                          /* tp_base */
+    0,                                          /* tp_dict */
+    0,                                          /* tp_descr_get */
+    0,                                          /* tp_descr_set */
+    0,                                          /* tp_dictoffset */
+    0,                                          /* tp_init */
+    PyType_GenericAlloc,                        /* tp_alloc */
+    (newfunc)Queue_new,                         /* tp_new */
+    PyObject_GC_Del,                            /* tp_free */
+};
+
+static PyModuleDef QueueModuleDef = {
+    PyModuleDef_HEAD_INIT,
+    "_fastqueue",
+    "Singly linked, small overhead implementations of the Queue data structure.",
+    -1,
+    NULL, NULL, NULL, NULL, NULL
+};
+
+PyMODINIT_FUNC PyInit__fastqueue(void) {
+    PyObject* module;
+    if (PyType_Ready(&QueueType) < 0 || PyType_Ready(&QueueCType) < 0)
+        return NULL;
+
+    module = PyModule_Create(&QueueModuleDef);
+    if (module == NULL)
+        return NULL;
+    PyModule_AddType(module, &QueueCType);
+    PyModule_AddType(module, &QueueType);
+    return module;
+}
```

