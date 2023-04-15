# Comparing `tmp/gqylpy_log-1.0.3.tar.gz` & `tmp/gqylpy_log-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_log-1.0.3.tar", last modified: Sun Jan 15 09:42:26 2023, max compression
+gzip compressed data, was "gqylpy_log-1.0.4.tar", last modified: Sat Apr 15 04:48:04 2023, max compression
```

## Comparing `gqylpy_log-1.0.3.tar` & `gqylpy_log-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 09:42:26.626027 gqylpy_log-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-01-15 09:42:09.000000 gqylpy_log-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-15 09:42:26.622027 gqylpy_log-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-01-15 09:42:09.000000 gqylpy_log-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 09:42:26.622027 gqylpy_log-1.0.3/gqylpy_log/
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-01-15 09:42:09.000000 gqylpy_log-1.0.3/gqylpy_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-01-15 09:42:09.000000 gqylpy_log-1.0.3/gqylpy_log/g log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 09:42:26.622027 gqylpy_log-1.0.3/gqylpy_log.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-15 09:42:26.000000 gqylpy_log-1.0.3/gqylpy_log.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-15 09:42:26.000000 gqylpy_log-1.0.3/gqylpy_log.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 09:42:26.000000 gqylpy_log-1.0.3/gqylpy_log.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-15 09:42:26.000000 gqylpy_log-1.0.3/gqylpy_log.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 09:42:26.626027 gqylpy_log-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-01-15 09:42:09.000000 gqylpy_log-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/gqylpy_log/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/gqylpy_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/gqylpy_log/g log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/gqylpy_log.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/setup.py
```

### Comparing `gqylpy_log-1.0.3/LICENSE` & `gqylpy_log-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_log-1.0.3/PKG-INFO` & `gqylpy_log-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy_log
-Version: 1.0.3
+Version: 1.0.4
 Summary: 二次封装 logging，更方便快捷的创建日志记录器。使用 gqylpy_log 模块可以快速创建 logging.Logger 实例并完成一系列的日志配置，使你的代码更简洁。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-log
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_log-1.0.3/README.md` & `gqylpy_log-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gqylpy_log-1.0.3/gqylpy_log/g log.py` & `gqylpy_log-1.0.4/gqylpy_log/g log.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,22 @@
         output:  str = 'stream',
         logfmt:  str = '[%(asctime)s] [%(module)s.%(funcName)s.line%(lineno)d] '
                        '[%(levelname)s] %(message)s',
         datefmt: str = '%F %T',
         logfile: str = None,
         gname:   str = None
 ) -> logging.Logger:
-    if output not in ("stream", "file", "stream,file", "file,stream"):
+    if output.replace(' ', '') not in \
+            ("stream", "file", "stream,file", "file,stream"):
         raise type('ParameterError', (TypeError,), {'__module__': 'builtins'})(
             'parameter "output" can only be "stream", "file", or '
             f'"file,stream", not "{output}"'
         )
 
-    logger = logging.Logger(name, level)
+    logger    = logging.Logger(name, level)
     formatter = logging.Formatter(logfmt, datefmt)
 
     if 'stream' in output:
         handler = logging.StreamHandler()
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
@@ -89,44 +90,46 @@
         elif gname.__class__ is str:
             gobj: logging.Logger = getattr(gpack, gname, None)
             if gobj.__class__ is not logging.Logger:
                 raise NameError(f'gname "{gname}" not found in {__package__}.')
         elif gname.__class__ is logging.Logger:
             gobj: logging.Logger = gname
         else:
-            x: str = gname.__class__.__name__
             raise TypeError(
                 'parameter "gname" type must be a "str" or "logging.Logger", '
-                f'not "{x}".'
+                f'not "{gname.__class__.__name__}".'
             )
 
-        if 'stacklevel' in kw:
-            if kw['stacklevel'].__class__ is not int:
-                if not kw['stacklevel'].isdigit():
-                    x: str = kw['stacklevel'].__class__.__name__
-                    raise TypeError(
-                        'Parameter "stacklevel" type must be a "int", '
-                        f'not "{x}".'
-                    )
-                kw['stacklevel'] = int(kw['stacklevel'])
-            if kw['stacklevel'] < 2:
+        if sys.version_info >= (3, 8):
+            if 'stacklevel' in kw:
+                if kw['stacklevel'].__class__ is not int:
+                    if not kw['stacklevel'].isdigit():
+                        raise TypeError(
+                            'Parameter "stacklevel" type must be a "int", '
+                            f'not "{kw["stacklevel"].__class__.__name__}".'
+                        )
+                    kw['stacklevel'] = int(kw['stacklevel'])
+                if kw['stacklevel'] < 2:
+                    kw['stacklevel'] = 2
+            else:
                 kw['stacklevel'] = 2
-        else:
-            kw['stacklevel'] = 2
+
+        if msg.__class__ is str:
+            msg = msg.strip()
 
         getattr(gobj, func.__name__)(msg, **kw)
 
     return inner
 
 
 @__call__
 def debug(): ...
 @__call__
 def info(): ...
 @__call__
 def warning(): ...
-exception = warning
 @__call__
 def error(): ...
+exception = error
 @__call__
 def critical(): ...
 fatal = critical
```

### Comparing `gqylpy_log-1.0.3/gqylpy_log.egg-info/PKG-INFO` & `gqylpy_log-1.0.4/gqylpy_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-log
-Version: 1.0.3
+Version: 1.0.4
 Summary: 二次封装 logging，更方便快捷的创建日志记录器。使用 gqylpy_log 模块可以快速创建 logging.Logger 实例并完成一系列的日志配置，使你的代码更简洁。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-log
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_log-1.0.3/setup.py` & `gqylpy_log-1.0.4/setup.py`

 * *Files identical despite different names*

