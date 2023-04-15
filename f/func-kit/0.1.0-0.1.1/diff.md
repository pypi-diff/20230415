# Comparing `tmp/func_kit-0.1.0.tar.gz` & `tmp/func_kit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_kit-0.1.0.tar", max compression
+gzip compressed data, was "func_kit-0.1.1.tar", max compression
```

## Comparing `func_kit-0.1.0.tar` & `func_kit-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-15 12:00:29.180320 func_kit-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      106 2023-04-15 12:10:01.485691 func_kit-0.1.0/README.md
--rw-r--r--   0        0        0       75 2023-04-15 11:23:57.226908 func_kit-0.1.0/func_kit/__init__.py
--rw-r--r--   0        0        0     2821 2023-04-15 11:21:50.096941 func_kit-0.1.0/func_kit/cache.py
--rw-r--r--   0        0        0     1997 2023-04-15 11:21:52.066940 func_kit-0.1.0/func_kit/log.py
--rw-r--r--   0        0        0      441 2023-04-15 09:36:33.598532 func_kit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 func_kit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-15 12:00:29.180320 func_kit-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      106 2023-04-15 12:10:01.485691 func_kit-0.1.1/README.md
+-rw-r--r--   0        0        0       75 2023-04-15 11:23:57.226908 func_kit-0.1.1/func_kit/__init__.py
+-rw-r--r--   0        0        0     2848 2023-04-15 12:43:39.221285 func_kit-0.1.1/func_kit/cache.py
+-rw-r--r--   0        0        0     1997 2023-04-15 11:21:52.066940 func_kit-0.1.1/func_kit/log.py
+-rw-r--r--   0        0        0      441 2023-04-15 13:32:22.638224 func_kit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 func_kit-0.1.1/PKG-INFO
```

### Comparing `func_kit-0.1.0/LICENSE.txt` & `func_kit-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `func_kit-0.1.0/func_kit/cache.py` & `func_kit-0.1.1/func_kit/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 from functools import wraps
 import time
 
 
-def memory_limited_cache(max_memory: int = 8 * 1024 * 8):
+def cache_decorator(max_memory: float = 1024):
     """memory limited cache decorator.
 
-    `max_memory`: maximum memory in bytes.
+    `max_memory`: maximum memory in KB.
 
     This decorator can be used to cache the result of a function.
     The result of the function is cached in a dictionary,
     and the dictionary is evicted from the cache if the memory usage
     of the dictionary exceeds the given maximum memory.
 
     The decorator can be used as follows:
 
     ``` code-block:: python
 
-        @memory_limited_cache(max_memory=100)
+        @cache_decorator(max_memory=100)
         def expensive_function(a, b):
             return a + b
     ```
 
     The function can be called as follows:
 
     ``` code-block:: python
@@ -37,35 +37,36 @@
     of the dictionary exceeds the given maximum memory.
 
     The decorator can also be used as a function:
 
     """
     cache = {}
     current_memory = 0
+    max_memory_bit = max_memory * 8 * 1024
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             nonlocal current_memory
             key = (args, tuple(kwargs.items()))
             if key in cache:
                 # Cache hit
                 cache[key]["last_used_time"] = time.time()
                 return cache[key]["result"]
 
             result = func(*args, **kwargs)
             result_size = sys.getsizeof(result)
-            if current_memory + result_size <= max_memory:
+            if current_memory + result_size <= max_memory_bit:
                 # Cache miss, add to cache and increase memory usage.
                 cache[key] = {"result": result, "last_used_time": time.time()}
                 current_memory += result_size
             else:
                 # Cache miss, but not enough memory. Evict the least recently used entry.
                 # This is done by finding the key with the lowest last_used_time value.
-                while current_memory + result_size > max_memory and cache:
+                while current_memory + result_size > max_memory_bit and cache:
                     lru_key = min(
                         cache.keys(), key=lambda k: cache[k]["last_used_time"]
                     )
                     lru_value = cache.pop(lru_key)
                     current_memory -= sys.getsizeof(lru_value["result"])
                 # Add to cache and increase memory usage.
                 cache[key] = {"result": result, "last_used_time": time.time()}
@@ -76,14 +77,14 @@
         return wrapper
 
     return decorator
 
 
 if __name__ == "__main__":
 
-    @memory_limited_cache(100)
+    @cache_decorator(100)
     def time_consuming_func(t):
         time.sleep(t)
         return t
 
     for i in range(10):
         print(time_consuming_func(i))
```

### Comparing `func_kit-0.1.0/func_kit/log.py` & `func_kit-0.1.1/func_kit/log.py`

 * *Files identical despite different names*

### Comparing `func_kit-0.1.0/PKG-INFO` & `func_kit-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-kit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of useful function kits.
 License: MIT
 Author: ranguiquan
 Author-email: ranguiquan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

