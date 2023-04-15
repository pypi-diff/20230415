# Comparing `tmp/async_state_machine-0.0.3.tar.gz` & `tmp/async_state_machine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_state_machine-0.0.3.tar", max compression
+gzip compressed data, was "async_state_machine-0.0.4.tar", max compression
```

## Comparing `async_state_machine-0.0.3.tar` & `async_state_machine-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/README.md
--rw-r--r--   0        0        0      430 2023-04-01 15:55:42.998340 async_state_machine-0.0.3/async_state_machine/__init__.py
--rw-r--r--   0        0        0      172 2023-04-01 13:02:08.510038 async_state_machine-0.0.3/async_state_machine/const.py
--rw-r--r--   0        0        0     1985 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/exceptions.py
--rw-r--r--   0        0        0      366 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/shared.py
--rw-r--r--   0        0        0      170 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/state/__init__.py
--rw-r--r--   0        0        0      687 2023-04-01 13:14:02.774686 async_state_machine-0.0.3/async_state_machine/state/coro_wrappers.py
--rw-r--r--   0        0        0     4379 2023-04-01 11:50:11.371780 async_state_machine-0.0.3/async_state_machine/state/stage_callbacks.py
--rw-r--r--   0        0        0     6300 2023-04-01 16:06:48.658471 async_state_machine-0.0.3/async_state_machine/state/state.py
--rw-r--r--   0        0        0     3405 2023-04-01 16:05:29.571767 async_state_machine-0.0.3/async_state_machine/state/state_runner.py
--rw-r--r--   0        0        0     3105 2023-04-01 11:48:14.041256 async_state_machine-0.0.3/async_state_machine/state_machine.py
--rw-r--r--   0        0        0      161 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/states_enum.py
--rw-r--r--   0        0        0      216 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/typings.py
--rw-r--r--   0        0        0      880 2023-04-08 18:02:11.166640 async_state_machine-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 async_state_machine-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-31 19:08:14.905097 async_state_machine-0.0.4/README.md
+-rw-r--r--   0        0        0      430 2023-04-01 15:55:42.998340 async_state_machine-0.0.4/async_state_machine/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-15 18:08:30.972485 async_state_machine-0.0.4/async_state_machine/const.py
+-rw-r--r--   0        0        0     1985 2023-03-31 19:08:14.905097 async_state_machine-0.0.4/async_state_machine/exceptions.py
+-rw-r--r--   0        0        0      366 2023-03-31 19:08:14.905097 async_state_machine-0.0.4/async_state_machine/shared.py
+-rw-r--r--   0        0        0      170 2023-03-31 19:08:14.905097 async_state_machine-0.0.4/async_state_machine/state/__init__.py
+-rw-r--r--   0        0        0      687 2023-04-15 18:10:06.787084 async_state_machine-0.0.4/async_state_machine/state/coro_wrappers.py
+-rw-r--r--   0        0        0     4381 2023-04-15 17:55:02.725189 async_state_machine-0.0.4/async_state_machine/state/stage_callbacks.py
+-rw-r--r--   0        0        0     6300 2023-04-15 18:05:24.984270 async_state_machine-0.0.4/async_state_machine/state/state.py
+-rw-r--r--   0        0        0     3405 2023-04-09 15:58:25.354907 async_state_machine-0.0.4/async_state_machine/state/state_runner.py
+-rw-r--r--   0        0        0     3162 2023-04-15 18:12:02.039126 async_state_machine-0.0.4/async_state_machine/state_machine.py
+-rw-r--r--   0        0        0      161 2023-03-31 19:08:14.905097 async_state_machine-0.0.4/async_state_machine/states_enum.py
+-rw-r--r--   0        0        0      212 2023-04-15 18:03:49.262276 async_state_machine-0.0.4/async_state_machine/typings.py
+-rw-r--r--   0        0        0      904 2023-04-15 18:12:55.605951 async_state_machine-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 async_state_machine-0.0.4/PKG-INFO
```

### Comparing `async_state_machine-0.0.3/async_state_machine/exceptions.py` & `async_state_machine-0.0.4/async_state_machine/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_state_machine-0.0.3/async_state_machine/state/coro_wrappers.py` & `async_state_machine-0.0.4/async_state_machine/state/coro_wrappers.py`

 * *Files identical despite different names*

### Comparing `async_state_machine-0.0.3/async_state_machine/state/stage_callbacks.py` & `async_state_machine-0.0.4/async_state_machine/state/stage_callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Запуск функций для этапа состояния."""
 
 import asyncio
-from typing import Any, Callable, Coroutine, Final, Literal, Self
+from collections.abc import Awaitable, Callable
+from typing import Any, Final, Literal, Self
 
 from loguru import logger
 
 from ..exceptions import NewStateData, NewStateException, StateMachineError
 from ..states_enum import StatesEnum
 from ..typings import TCallback, TCallbackCollection
 
-
 EXC_TIMEOUT: Final[str] = "Timeout occur {name}|{stage}"
 EXC_TIMEOUT_WITHOUT_TARGET: Final[
     str
 ] = "{base_msg}, but target state not specified"
 
 
 class StageCallbacks(object):
@@ -22,15 +22,15 @@
     def __init__(
         self,
         callbacks: TCallbackCollection | None,
         timeout: float | None,
         timeout_to_state: StatesEnum | None,
         name: StatesEnum,
         stage: Literal["on_enter", "on_run", "on_exit"],
-        coro_wrapper: Callable[[TCallback], Coroutine[Any, Any, None]],
+        coro_wrapper: Callable[[TCallback], Awaitable[None]],
         logging_level: int = 0,  # TODO - remove
     ) -> None:
         """Запуск функций для этапа состояния."""
         self.__callbacks: TCallbackCollection | None
         self.__coro_wrapper: Any
         self.__name: StatesEnum
         self.__timeout: float | None
@@ -50,15 +50,15 @@
             "{name}|{stage}|start".format(
                 name=self.__name,
                 stage=self.__stage,
             ),
         )
         new_state_data: NewStateData | None = None
         try:
-            await self.__run_taskgroup()
+            await self.__run()
         except* asyncio.TimeoutError:
             self.__except_timeout()
         except* NewStateException as exc:
             new_state_data = self.__except_new_state(exc)
         logger.debug(
             "{name}|{stage}|end".format(
                 name=self.__name,
@@ -69,33 +69,34 @@
             raise NewStateException.reraise(new_state_data, self.__name)
 
     def config_logging(self, logging_level: int) -> Self:
         """Конфигурировать уровень логгирования.
 
         TODO - remove
         """
-        # log.setLevel(logging_level)
         return self
 
-    async def __run_taskgroup(self) -> None:
+    async def __run(self) -> None:
         """Запуск."""
-        async with asyncio.TaskGroup() as tg:
-            self.__create_tasks(tg)
-
-    def __create_tasks(self, tg: asyncio.TaskGroup) -> None:
-        """Создание группы задач."""
         if self.__callbacks is None:
-            return
-        for task in self.__callbacks:
-            tg.create_task(
-                asyncio.wait_for(
-                    fut=self.__coro_wrapper(task),
-                    timeout=self.__timeout,
-                ),
+            return await asyncio.sleep(0)
+        await asyncio.gather(*self.__create_tasks(self.__callbacks))
+
+    def __create_tasks(
+        self,
+        callbacks: TCallbackCollection,
+    ) -> tuple[Awaitable[None], ...]:
+        """Создание коллекцию задач."""
+        return tuple(
+            asyncio.wait_for(
+                fut=self.__coro_wrapper(task),
+                timeout=self.__timeout,
             )
+            for task in callbacks
+        )
 
     def __except_timeout(self) -> None:
         """Обработка превышения времени выполнения."""
         logger.debug(EXC_TIMEOUT.format(name=self.__name, stage=self.__stage))
         if self.__timeout_to_state is None:
             msg = EXC_TIMEOUT_WITHOUT_TARGET.format(
                 base_msg=EXC_TIMEOUT.format(
@@ -107,15 +108,15 @@
             raise StateMachineError(msg)
         raise NewStateException(
             new_state=self.__timeout_to_state,
         )
 
     def __except_new_state(
         self,
-        exc: ExceptionGroup[NewStateException],
+        exc: BaseExceptionGroup[NewStateException],
     ) -> NewStateData:
         """Обработка перехода в новое состояние."""
         new_state_data = exc.exceptions[0]
         if isinstance(new_state_data, NewStateException):
             exc_data = new_state_data.exception_data
             logger.debug(
                 "State {name}, stage {stage}, new state: {new_name}".format(
```

### Comparing `async_state_machine-0.0.3/async_state_machine/state/state.py` & `async_state_machine-0.0.4/async_state_machine/state/state.py`

 * *Files identical despite different names*

### Comparing `async_state_machine-0.0.3/async_state_machine/state/state_runner.py` & `async_state_machine-0.0.4/async_state_machine/state/state_runner.py`

 * *Files identical despite different names*

### Comparing `async_state_machine-0.0.3/async_state_machine/state_machine.py` & `async_state_machine-0.0.4/async_state_machine/state_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Диаграмма состояний."""
 
 import asyncio
 from typing import Final, Iterable, Self, Type
 
+from .const import INFINITE_CORO_SLEEP
 from .exceptions import NewStateException, StateMachineError
 from .state import State, StateRunner
 from .states_enum import StatesEnum
 
 EXC_NAME_NOT_FOUND: Final[str] = "State with name {name} not found."
 EXC_NOT_USED_STATES: Final[str] = "Need to define states: {states}"
 EXC_REUSE_STATE: Final[str] = "Several use state with name: {name}"
@@ -40,15 +41,15 @@
         """Задача для асинхронного выполнения."""
         while True:
             try:
                 await self.__active_state.run()
             except NewStateException as exc:
                 new_state = exc.exception_data.new_state
                 self.__active_state = self.__find_state_by_name(new_state)
-            await asyncio.sleep(0)
+            await asyncio.sleep(INFINITE_CORO_SLEEP)
 
     def config_logging(self, logging_level: int) -> Self:
         """Конфигурировать уровень логгирования."""
         # log.setLevel(logging_level)
         for state in self.__states:
             state.config_logging(logging_level)
         return self
```

### Comparing `async_state_machine-0.0.3/pyproject.toml` & `async_state_machine-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.black]
 line-length = 80
 
 
 [tool.poetry]
 name = "async_state_machine"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["konstantin-dudersky <konstantin.dudersky@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "async_state_machine" }]
 
 
 [tool.poetry.dependencies]
@@ -21,14 +21,15 @@
 loguru = "^0.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pytest = "7.2.0"
 wemake-python-styleguide = "0.17.0"
+flake8-deprecated = "*"
 
 
 [tool.pyright]
 pythonPlatform = "Linux"
 pythonVersion = "3.11"
 reportUnnecessaryTypeIgnoreComment = true
 stubPath = '.venv/typings/'
```

