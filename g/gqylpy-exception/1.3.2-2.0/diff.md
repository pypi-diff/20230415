# Comparing `tmp/gqylpy_exception-1.3.2.tar.gz` & `tmp/gqylpy_exception-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_exception-1.3.2.tar", last modified: Sun Jan  8 11:07:20 2023, max compression
+gzip compressed data, was "gqylpy_exception-2.0.tar", last modified: Sat Apr 15 04:43:26 2023, max compression
```

## Comparing `gqylpy_exception-1.3.2.tar` & `gqylpy_exception-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:07:20.740630 gqylpy_exception-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-01-08 11:07:08.000000 gqylpy_exception-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-01-08 11:07:20.740630 gqylpy_exception-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-01-08 11:07:08.000000 gqylpy_exception-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:07:20.740630 gqylpy_exception-1.3.2/gqylpy_exception/
--rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-01-08 11:07:08.000000 gqylpy_exception-1.3.2/gqylpy_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-01-08 11:07:08.000000 gqylpy_exception-1.3.2/gqylpy_exception/g exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:07:20.740630 gqylpy_exception-1.3.2/gqylpy_exception.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-01-08 11:07:20.000000 gqylpy_exception-1.3.2/gqylpy_exception.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-08 11:07:20.000000 gqylpy_exception-1.3.2/gqylpy_exception.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 11:07:20.000000 gqylpy_exception-1.3.2/gqylpy_exception.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-08 11:07:20.000000 gqylpy_exception-1.3.2/gqylpy_exception.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 11:07:20.740630 gqylpy_exception-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-08 11:07:08.000000 gqylpy_exception-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:43:26.296699 gqylpy_exception-2.0/gqylpy_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/gqylpy_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/gqylpy_exception/g exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/gqylpy_exception.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/setup.py
```

### Comparing `gqylpy_exception-1.3.2/LICENSE` & `gqylpy_exception-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-1.3.2/PKG-INFO` & `gqylpy_exception-2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy_exception
-Version: 1.3.2
+Version: 2.0
 Summary: 在执行 raise 语句的同时创建异常类，无需事先定义异常类，方便快捷。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Environment :: Web Environment
@@ -73,33 +73,33 @@
 @TryExcept(ValueError)
 def func():
     int('a')
 ```
 默认的处理流程是将异常简要信息输出到终端。当然，也可以输出到文件或做其它处理，通过参数控制：
 ```python
 def TryExcept(
-        etype:          Union[type, Tuple[type, ...]],
-        /, *,
-        ignore:         bool                                       = False,
-        output_raw_exc: bool                                       = False,
-        logger:         logging.Logger                             = None,
-        ereturn:        Any                                        = None,
-        ecallback:      Callable[[Exception, Callable, ...], None] = None,
-        eexit:          bool                                       = False
+        etype:      Union[ExceptionTypes],
+        *,
+        silent_exc: Optional[bool]              = None,
+        raw_exc:    Optional[bool]              = None,
+        logger:     Optional[ExceptionLogger]   = None,
+        ereturn:    Optional[Any]               = None,
+        ecallback:  Optional[ExceptionCallback] = None,
+        eexit:      Optional[bool]              = None
 ):
     ...
 ```
 __参数 `etype`__<br>
 要处理哪种异常，使用元祖传入多个。
 
-__参数 `ingore`__<br>
+__参数 `silent_exc`__<br>
 设为 `True` 将静默处理异常，没有任何输出。
 
-__参数 `output_raw_exc`__<br>
-设为 `True` 将输出完整的异常信息，注意其优先级低于 `ignore`。 
+__参数 `raw_exc`__<br>
+设为 `True` 将输出完整的异常信息，注意其优先级低于 `silent_exc`。 
 
 __参数 `logger`__<br>
 接收一个日志记录器对象，`TryExcept` 希望使用日志记录器输出异常信息，它调用日志记录器的 `error` 方法。<br>
 缺省情况下使用 `sys.stderr` 输出异常信息。
 
 __参数 `ereturn`__<br>
 若被装饰的函数中引发了异常，将返回此参数，默认为 `None`。<br>
@@ -121,21 +121,21 @@
 def func():
     int('a')
 ```
 若被装饰的函数中引发了异常，会尝试重新执行被装饰的函数，默认重试 `Exception` 及其子类的所有异常。
 像上面这样调用 `Retry(count=3, cycle=1)` 表示最大执行3次，每次间隔1秒。完整的参数如下：
 ```python
 def Retry(
-        etype:          Union[type, Tuple[type, ...]] = Exception,
+        etype:      Optional[ExceptionTypes]    = None,
         *,
-        count:          int                           = inf,
-        cycle:          Union[int, float]             = 0,
-        ignore:         bool                          = False,
-        output_raw_exc: bool                          = False,
-        logger:         logging.Logger                = None
+        count:      Optional[int]               = inf,
+        cycle:      Optional[Union[int, float]] = 0,
+        silent_exc: Optional[bool]              = None,
+        raw_exc:    Optional[bool]              = None,
+        logger:     Optional[ExceptionLogger]   = None
 ):
     ...
 ```
 `Retry` 继承 `TryExcept`，你可以在 `TryExcept` 中找到参数说明，但注意 `Retry` 调用日志记录器的 `warning` 方法。
 
 结合 `TryExcept` 使用，既能重试异常又能处理异常：
 ```python
```

### Comparing `gqylpy_exception-1.3.2/README.md` & `gqylpy_exception-2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -46,33 +46,33 @@
 @TryExcept(ValueError)
 def func():
     int('a')
 ```
 默认的处理流程是将异常简要信息输出到终端。当然，也可以输出到文件或做其它处理，通过参数控制：
 ```python
 def TryExcept(
-        etype:          Union[type, Tuple[type, ...]],
-        /, *,
-        ignore:         bool                                       = False,
-        output_raw_exc: bool                                       = False,
-        logger:         logging.Logger                             = None,
-        ereturn:        Any                                        = None,
-        ecallback:      Callable[[Exception, Callable, ...], None] = None,
-        eexit:          bool                                       = False
+        etype:      Union[ExceptionTypes],
+        *,
+        silent_exc: Optional[bool]              = None,
+        raw_exc:    Optional[bool]              = None,
+        logger:     Optional[ExceptionLogger]   = None,
+        ereturn:    Optional[Any]               = None,
+        ecallback:  Optional[ExceptionCallback] = None,
+        eexit:      Optional[bool]              = None
 ):
     ...
 ```
 __参数 `etype`__<br>
 要处理哪种异常，使用元祖传入多个。
 
-__参数 `ingore`__<br>
+__参数 `silent_exc`__<br>
 设为 `True` 将静默处理异常，没有任何输出。
 
-__参数 `output_raw_exc`__<br>
-设为 `True` 将输出完整的异常信息，注意其优先级低于 `ignore`。 
+__参数 `raw_exc`__<br>
+设为 `True` 将输出完整的异常信息，注意其优先级低于 `silent_exc`。 
 
 __参数 `logger`__<br>
 接收一个日志记录器对象，`TryExcept` 希望使用日志记录器输出异常信息，它调用日志记录器的 `error` 方法。<br>
 缺省情况下使用 `sys.stderr` 输出异常信息。
 
 __参数 `ereturn`__<br>
 若被装饰的函数中引发了异常，将返回此参数，默认为 `None`。<br>
@@ -94,21 +94,21 @@
 def func():
     int('a')
 ```
 若被装饰的函数中引发了异常，会尝试重新执行被装饰的函数，默认重试 `Exception` 及其子类的所有异常。
 像上面这样调用 `Retry(count=3, cycle=1)` 表示最大执行3次，每次间隔1秒。完整的参数如下：
 ```python
 def Retry(
-        etype:          Union[type, Tuple[type, ...]] = Exception,
+        etype:      Optional[ExceptionTypes]    = None,
         *,
-        count:          int                           = inf,
-        cycle:          Union[int, float]             = 0,
-        ignore:         bool                          = False,
-        output_raw_exc: bool                          = False,
-        logger:         logging.Logger                = None
+        count:      Optional[int]               = inf,
+        cycle:      Optional[Union[int, float]] = 0,
+        silent_exc: Optional[bool]              = None,
+        raw_exc:    Optional[bool]              = None,
+        logger:     Optional[ExceptionLogger]   = None
 ):
     ...
 ```
 `Retry` 继承 `TryExcept`，你可以在 `TryExcept` 中找到参数说明，但注意 `Retry` 调用日志记录器的 `warning` 方法。
 
 结合 `TryExcept` 使用，既能重试异常又能处理异常：
 ```python
```

### Comparing `gqylpy_exception-1.3.2/gqylpy_exception/g exception.py` & `gqylpy_exception-2.0/gqylpy_exception/g exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,137 +19,182 @@
 import logging
 import asyncio
 import warnings
 import builtins
 import functools
 import traceback
 
+from typing import TypeVar, Type, Optional, Union, Tuple, Callable, Any
+
+Function = Closure = TypeVar('Function', bound=Callable)
+
+ExceptionTypes    = Union[Type[Exception], Tuple[Type[Exception], ...]]
+ExceptionLogger   = Union[logging.Logger, 'gqylpy_log']
+ExceptionCallback = Callable[[Exception, Function, '...'], None]
+
+warnings.filterwarnings('once', category=DeprecationWarning)
+
 
 class GqylpyException:
     __history__ = {}
 
-    def __getattr__(self, ename: str) -> type:
+    def __getattr__(self, ename: str) -> Type['GqylpyError']:
         try:
             eclass = self.__history__[ename]
         except KeyError:
             if hasattr(builtins, ename):
                 raise self.ExceptionClassIsBuiltinsError(
                     f'exception class "{ename}" is builtins.'
-                )
+                ) from None
             # Some special modules may attempt to call non-built-in magic
             # method, such as `copy`, `pickle`. Compatible for this purpose.
             if ename[:2] == ename[-2:] == '__' and \
                     ename[2] != '_' and ename[-3] != '_':
                 raise AttributeError(
-                    f'"{__package__}" has no attribute "{ename}"'
-                )
+                    f'"{__package__}" has no attribute "{ename}".'
+                ) from None
             if ename[-5:] != 'Error':
                 warnings.warn(
-                    message=f'strange exception class "{ename}", exception '
-                        'class name should end with "Error".',
-                    category=type('ImproperUseWarning', (Warning,), {})
+                    f'strange exception class "{ename}", exception class name '
+                    'should end with "Error".', UserWarning
                 )
             eclass = self.__history__[ename] = type(
                 ename, (self.GqylpyError,), {'__module__': 'builtins'}
             )
             # Compatible with object serialization.
             setattr(builtins, ename, eclass)
         return eclass
 
-    def __getitem__(self, ename: str) -> type:
+    def __getitem__(self, ename: str) -> Type['GqylpyError']:
         return getattr(self, ename)
 
     class GqylpyError(Exception):
         __module__ = 'builtins'
 
         @property
-        def msg(self):
-            args_length: int = len(self.args)
-            if args_length == 0:
-                return ''
-            if args_length == 1:
-                return self.args[0]
-            return self.args
-
+        def msg(self) -> Any:
+            return self.args[0] if len(self.args) == 1 else \
+                self.args if self.args else None
 
 # Compatible with object serialization, for `GqylpyException.GqylpyError`.
 builtins.GqylpyException = GqylpyException
 
 
+def stderr(einfo: str) -> None:
+    now: str = time.strftime('%F %T', time.localtime())
+    sys.stderr.write(f'[{now}] {einfo}\n')
+
+
+def get_logger(logger: logging.Logger) -> Callable[[str], None]:
+    if logger is None:
+        return stderr
+
+    if not (
+            isinstance(logger, logging.Logger) or
+            getattr(logger, '__package__', None) == 'gqylpy_log'
+    ):
+        raise ParameterError(
+            'parameter "logger" must be an instance of "logging.Logger", '
+            f'not "{logger.__class__.__name__}".'
+        )
+
+    if sys._getframe(2).f_code is Retry.__init__.__code__:
+        return logger.warning
+
+    return logger.error
+
+
 class TryExcept:
 
+    def __new__(cls, *a, **kw):
+        if 'ignore' in kw:
+            warnings.warn(DeprecationWarning(
+                'parameter "ignore" deprecated, replaced to "silent_exc".'
+            ), stacklevel=2)
+        if 'output_raw_exc' in kw:
+            warnings.warn(DeprecationWarning(
+                'parameter "output_raw_exc" deprecated, replaced to "raw_exc".'
+            ), stacklevel=2)
+        return object.__new__(cls)
+
     def __init__(
             self,
-            etype:          [type, tuple],
+            etype:      ExceptionTypes,
             *,
-            ignore:         bool          = False,
-            output_raw_exc: bool          = False,
-            logger:         ...           = None,
-            ereturn:        ...           = None,
-            ecallback:      ...           = None,
-            eexit:          bool          = False
+            silent_exc: bool                        = False,
+            raw_exc:    bool                        = False,
+            logger:     Optional[ExceptionLogger]   = None,
+            ereturn:    Optional[Any]               = None,
+            ecallback:  Optional[ExceptionCallback] = None,
+            eexit:      bool                        = False,
+            ignore         = None,
+            output_raw_exc = None
     ):
-        self.etype          = etype
-        self.ignore         = ignore
-        self.output_raw_exc = output_raw_exc
-        self.logger         = logger
-        self.ereturn        = ereturn
-        self.ecallback      = ecallback
-        self.eexit          = eexit
+        self.etype      = etype
+        self.silent_exc = silent_exc
+        self.raw_exc    = raw_exc
+        self.logger     = get_logger(logger)
+        self.ereturn    = ereturn
+        self.ecallback  = ecallback
+        self.eexit      = eexit
+
+        self.local: bool = self.__class__ is TryExcept
+
+    def __call__(self, func: Function) -> Closure:
+        try:
+            core = func.__closure__[1].cell_contents.core.__func__
+        except (TypeError, IndexError, AttributeError):
+            if asyncio.iscoroutinefunction(func):
+                self.core = self.core_async
+        else:
+            if core in (TryExcept.core_async, Retry.core_async):
+                self.core = self.core_async
 
-    def __call__(self, func):
         @functools.wraps(func, updated=('__dict__', '__globals__'))
-        def inner(*a, **kw):
+        def inner(*a, **kw) -> Any:
             return self.core(func, *a, **kw)
+
         return inner
 
-    def core(self, func, *a, **kw):
+    def core(self, func: Function, *a, **kw) -> Any:
         try:
             return func(*a, **kw)
         except self.etype as e:
             self.exception_handling(func, e, *a, **kw)
         return self.ereturn
 
-    def exception_handling(self, func, e: Exception, *a, **kw):
-        local_instance: bool = self.__class__ in (TryExcept, TryExceptAsync)
+    async def core_async(self, func: Function, *a, **kw) -> Any:
+        try:
+            return await func(*a, **kw)
+        except self.etype as e:
+            self.exception_handling(func, e, *a, **kw)
+        return self.ereturn
 
-        if not self.ignore:
+    def exception_handling(
+            self, func: Function, e: Exception, *a, **kw
+    ) -> None:
+        if not self.silent_exc:
             try:
                 einfo: str = self.exception_analysis(func, e)
             except Exception as ee:
                 einfo: str = f'{self.__class__.__name__}Error: {ee}'
+            if not self.local:
+                einfo = f'[try:{kw["count"]}/{self.count}:{self.cycle}] {einfo}'
+            self.logger(einfo)
+
+        if self.local:
+            if self.ecallback:
+                self.ecallback(e, func, *a, **kw)
+            if self.eexit:
+                raise SystemExit(4)
 
-            if not local_instance:
-                einfo: str = f'[try:{kw["count"]}/{self.count}:{self.cycle}] ' \
-                             f'{einfo}'
-
-            if self.logger:
-                if not(
-                        isinstance(self.logger, logging.Logger) or
-                        getattr(self.logger, '__name__', None) == 'gqylpy_log'
-                ):
-                    x: str = self.logger.__class__.__name__
-                    raise GqylpyException.ParameterError(
-                        f'parameter "logger" must be an instance '
-                        f'of "logging.Logger", not "{x}".'
-                    )
-                (self.logger.error if local_instance else self.logger.warning)(
-                    einfo, stacklevel=4 if local_instance else 6)
-            else:
-                now: str = time.strftime('%F %T', time.localtime())
-                sys.stderr.write(f'[{now}] {einfo}\n')
-
-        if local_instance:
-            self.ecallback and self.ecallback(e, func, *a, **kw)
-            self.eexit and exit(4)
-
-    def exception_analysis(self, func, e: Exception) -> str:
+    def exception_analysis(self, func: Function, e: Exception) -> str:
         einfo: str = traceback.format_exc()
 
-        if self.output_raw_exc:
+        if self.raw_exc:
             return einfo
 
         filepath: str = func.__globals__['__file__']
         funcpath: str = f'{func.__module__}.{func.__qualname__}'
 
         for line in reversed(einfo.split('\n')[1:-3]):
             if filepath in line:
@@ -163,87 +208,78 @@
         return f'[{funcpath}.{eline}.{e.__class__.__name__}] {e}'
 
 
 class Retry(TryExcept):
 
     def __init__(
             self,
-            etype:          [type, tuple] = Exception,
+            etype:      ExceptionTypes            = Exception,
             *,
-            count:          int           = 0,
-            cycle:          int           = 0,
-            ignore:         bool          = False,
-            output_raw_exc: bool          = False,
-            logger:         ...           = None,
+            count:      int                       = 0,
+            cycle:      int                       = 0,
+            silent_exc: bool                      = False,
+            raw_exc:    bool                      = False,
+            logger:     Optional[ExceptionLogger] = None,
+            ignore         = None,
+            output_raw_exc = None
     ):
         if not (count.__class__ is int and count >= 0):
             if not (count.__class__ is str and count.isdigit()):
-                raise GqylpyException.ParameterError(
-                    'parameter "count" must be a '
-                    f'positive integer or 0, not "{count}".'
+                raise ParameterError(
+                    'parameter "count" must be a positive integer or 0, '
+                    f'not "{count}".'
                 )
             count = int(count)
 
         if cycle.__class__ not in (int, float):
             try:
                 cycle = float(cycle)
             except (TypeError, ValueError):
-                raise GqylpyException.ParameterError(
-                    'parameter "cycle" must be a '
-                    f'positive number or 0, not "{cycle}"'
-                )
+                raise ParameterError(
+                    'parameter "count" must be a positive integer or 0, '
+                    f'not "{count}".'
+                ) from None
         if cycle < 0:
-            raise GqylpyException.ParameterError(
-                'parameter "cycle" must be a '
-                f'positive number or 0, not "{cycle}"'
+            raise ParameterError(
+                'parameter "count" must be a positive integer or 0, '
+                f'not "{count}".'
             )
 
         self.count = count or 'N'
         self.cycle = cycle
 
-        super().__init__(
-            etype,
-            ignore=ignore,
-            output_raw_exc=output_raw_exc,
-            logger=logger
+        TryExcept.__init__(
+            self, etype, silent_exc=silent_exc, raw_exc=raw_exc, logger=logger
         )
 
-    def core(self, func, *a, **kw):
+    def core(self, func: Function, *a, **kw) -> Any:
         count = 0
 
         while True:
             try:
                 return func(*a, **kw)
             except self.etype as e:
                 count += 1
                 self.exception_handling(func, e, count=count)
                 if count == self.count:
                     raise e
 
             time.sleep(self.cycle)
 
-
-class TryExceptAsync(TryExcept):
-
-    async def core(self, func, *a, **kw):
-        try:
-            return await func(*a, **kw)
-        except self.etype as e:
-            self.exception_handling(func, e, *a, **kw)
-        return self.ereturn
-
-
-class RetryAsync(Retry):
-
-    async def core(self, func, *a, **kw):
+    async def core_async(self, func: Function, *a, **kw) -> Any:
         count = 0
 
         while True:
             try:
                 return await func(*a, **kw)
             except self.etype as e:
                 count += 1
                 self.exception_handling(func, e, count=count)
                 if count == self.count:
                     raise e
 
             await asyncio.sleep(self.cycle)
+
+
+TryExceptAsync, RetryAsync = TryExcept, Retry
+
+ParameterError = GqylpyException().ParameterError
```

### Comparing `gqylpy_exception-1.3.2/gqylpy_exception.egg-info/PKG-INFO` & `gqylpy_exception-2.0/gqylpy_exception.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-exception
-Version: 1.3.2
+Version: 2.0
 Summary: 在执行 raise 语句的同时创建异常类，无需事先定义异常类，方便快捷。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Environment :: Web Environment
@@ -73,33 +73,33 @@
 @TryExcept(ValueError)
 def func():
     int('a')
 ```
 默认的处理流程是将异常简要信息输出到终端。当然，也可以输出到文件或做其它处理，通过参数控制：
 ```python
 def TryExcept(
-        etype:          Union[type, Tuple[type, ...]],
-        /, *,
-        ignore:         bool                                       = False,
-        output_raw_exc: bool                                       = False,
-        logger:         logging.Logger                             = None,
-        ereturn:        Any                                        = None,
-        ecallback:      Callable[[Exception, Callable, ...], None] = None,
-        eexit:          bool                                       = False
+        etype:      Union[ExceptionTypes],
+        *,
+        silent_exc: Optional[bool]              = None,
+        raw_exc:    Optional[bool]              = None,
+        logger:     Optional[ExceptionLogger]   = None,
+        ereturn:    Optional[Any]               = None,
+        ecallback:  Optional[ExceptionCallback] = None,
+        eexit:      Optional[bool]              = None
 ):
     ...
 ```
 __参数 `etype`__<br>
 要处理哪种异常，使用元祖传入多个。
 
-__参数 `ingore`__<br>
+__参数 `silent_exc`__<br>
 设为 `True` 将静默处理异常，没有任何输出。
 
-__参数 `output_raw_exc`__<br>
-设为 `True` 将输出完整的异常信息，注意其优先级低于 `ignore`。 
+__参数 `raw_exc`__<br>
+设为 `True` 将输出完整的异常信息，注意其优先级低于 `silent_exc`。 
 
 __参数 `logger`__<br>
 接收一个日志记录器对象，`TryExcept` 希望使用日志记录器输出异常信息，它调用日志记录器的 `error` 方法。<br>
 缺省情况下使用 `sys.stderr` 输出异常信息。
 
 __参数 `ereturn`__<br>
 若被装饰的函数中引发了异常，将返回此参数，默认为 `None`。<br>
@@ -121,21 +121,21 @@
 def func():
     int('a')
 ```
 若被装饰的函数中引发了异常，会尝试重新执行被装饰的函数，默认重试 `Exception` 及其子类的所有异常。
 像上面这样调用 `Retry(count=3, cycle=1)` 表示最大执行3次，每次间隔1秒。完整的参数如下：
 ```python
 def Retry(
-        etype:          Union[type, Tuple[type, ...]] = Exception,
+        etype:      Optional[ExceptionTypes]    = None,
         *,
-        count:          int                           = inf,
-        cycle:          Union[int, float]             = 0,
-        ignore:         bool                          = False,
-        output_raw_exc: bool                          = False,
-        logger:         logging.Logger                = None
+        count:      Optional[int]               = inf,
+        cycle:      Optional[Union[int, float]] = 0,
+        silent_exc: Optional[bool]              = None,
+        raw_exc:    Optional[bool]              = None,
+        logger:     Optional[ExceptionLogger]   = None
 ):
     ...
 ```
 `Retry` 继承 `TryExcept`，你可以在 `TryExcept` 中找到参数说明，但注意 `Retry` 调用日志记录器的 `warning` 方法。
 
 结合 `TryExcept` 使用，既能重试异常又能处理异常：
 ```python
```

### Comparing `gqylpy_exception-1.3.2/setup.py` & `gqylpy_exception-2.0/setup.py`

 * *Files identical despite different names*

