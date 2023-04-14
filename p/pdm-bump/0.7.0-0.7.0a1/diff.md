# Comparing `tmp/pdm-bump-0.7.0.tar.gz` & `tmp/pdm-bump-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-bump-0.7.0.tar", last modified: Fri Apr 14 22:21:45 2023, max compression
+gzip compressed data, was "pdm-bump-0.7.0a1.tar", last modified: Mon Apr 10 20:10:45 2023, max compression
```

## Comparing `pdm-bump-0.7.0.tar` & `pdm-bump-0.7.0a1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1092 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/LICENSE
--rw-r--r--   0        0        0     2397 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/README.md
--rw-r--r--   0        0        0     3888 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      770 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/__init__.py
--rw-r--r--   0        0        0      535 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/actions/__init__.py
--rw-r--r--   0        0        0     6558 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/actions/base.py
--rw-r--r--   0        0        0     1784 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/actions/explicit.py
--rw-r--r--   0        0        0     9062 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/actions/increment.py
--rw-r--r--   0        0        0     8128 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/actions/preview.py
--rw-r--r--   0        0        0     1365 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/actions/vcs.py
--rw-r--r--   0        0        0      864 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/cli.py
--rw-r--r--   0        0        0      251 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/core/__init__.py
--rw-r--r--   0        0        0     7530 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/core/config.py
--rw-r--r--   0        0        0     2079 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/core/loader.py
--rw-r--r--   0        0        0     5982 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/core/logging.py
--rw-r--r--   0        0        0     6908 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/core/version.py
--rw-r--r--   0        0        0     4999 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/dynamic.py
--rw-r--r--   0        0        0     5633 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/plugin.py
--rw-r--r--   0        0        0        0 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/py.typed
--rw-r--r--   0        0        0     2032 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/source.py
--rw-r--r--   0        0        0      783 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/vcs/__init__.py
--rw-r--r--   0        0        0     7057 2023-04-14 22:20:56.431649 pdm-bump-0.7.0/src/pdm_bump/vcs/core.py
--rw-r--r--   0        0        0      948 2023-04-14 22:20:56.435649 pdm-bump-0.7.0/src/pdm_bump/vcs/git.py
--rw-r--r--   0        0        0     6826 2023-04-14 22:20:56.435649 pdm-bump-0.7.0/src/pdm_bump/vcs/gitcli.py
--rw-r--r--   0        0        0     3997 2023-04-14 22:20:56.435649 pdm-bump-0.7.0/src/pdm_bump/vcs/mixins.py
--rw-r--r--   0        0        0    28347 2023-04-14 22:20:56.435649 pdm-bump-0.7.0/tests/action_test.py
--rw-r--r--   0        0        0     4317 2023-04-14 22:20:56.435649 pdm-bump-0.7.0/tests/plugin_test.py
--rw-r--r--   0        0        0    27307 2023-04-14 22:20:56.435649 pdm-bump-0.7.0/tests/version_test.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 pdm-bump-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/LICENSE
+-rw-r--r--   0        0        0     2397 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/README.md
+-rw-r--r--   0        0        0     3890 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/__init__.py
+-rw-r--r--   0        0        0      541 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/__init__.py
+-rw-r--r--   0        0        0     5964 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/base.py
+-rw-r--r--   0        0        0     1784 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/explicit.py
+-rw-r--r--   0        0        0     9068 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/increment.py
+-rw-r--r--   0        0        0     8128 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/preview.py
+-rw-r--r--   0        0        0     1193 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/vcs.py
+-rw-r--r--   0        0        0      864 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/cli.py
+-rw-r--r--   0        0        0      251 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/__init__.py
+-rw-r--r--   0        0        0     7530 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/config.py
+-rw-r--r--   0        0        0     5755 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/logging.py
+-rw-r--r--   0        0        0     6908 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/version.py
+-rw-r--r--   0        0        0     4999 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/dynamic.py
+-rw-r--r--   0        0        0     5347 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/py.typed
+-rw-r--r--   0        0        0     2032 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/source.py
+-rw-r--r--   0        0        0      699 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/__init__.py
+-rw-r--r--   0        0        0     7057 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/core.py
+-rw-r--r--   0        0        0      948 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/git.py
+-rw-r--r--   0        0        0     6826 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/gitcli.py
+-rw-r--r--   0        0        0     3997 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/mixins.py
+-rw-r--r--   0        0        0    28261 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/tests/action_test.py
+-rw-r--r--   0        0        0     4317 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/tests/plugin_test.py
+-rw-r--r--   0        0        0    27307 2023-04-10 20:10:12.668938 pdm-bump-0.7.0a1/tests/version_test.py
+-rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 pdm-bump-0.7.0a1/PKG-INFO
```

### Comparing `pdm-bump-0.7.0/LICENSE` & `pdm-bump-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/README.md` & `pdm-bump-0.7.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/pyproject.toml` & `pdm-bump-0.7.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-bump"
-version = "0.7.0"
+version = "0.7.0a1"
 readme = "README.md"
 description = "A plugin for PDM providing the ability to modify the version according to PEP440"
 authors = [
     { name = "Carsten Igel", email = "cig@bite-that-bit.de" },
 ]
 dependencies = [
     "pdm>=2.00",
```

### Comparing `pdm-bump-0.7.0/src/pdm_bump/__init__.py` & `pdm-bump-0.7.0a1/src/pdm_bump/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/actions/base.py` & `pdm-bump-0.7.0a1/src/pdm_bump/actions/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
-from typing import Any, Callable, Protocol
+from typing import Callable, Protocol
 
 from ..core.logging import logger
 from ..core.version import Pep440VersionFormatter, Version
-from ..vcs.core import VcsProvider
+from ..vcs.core import VcsProvider, VcsProviderAggregator
 
 _formatter = Pep440VersionFormatter()
 
 
 # Justification: Just a protocol
 class _HasAddSubParser(Protocol):  # pylint: disable=R0903
     def add_parser(self, name, **kwargs) -> ArgumentParser:
@@ -29,28 +29,38 @@
 
 # Justification: Just a protocol
 class VersionPersister(Protocol):  # pylint: disable=R0903
     def save_version(self, version: Version) -> None:
         raise NotImplementedError()
 
 
-class _ArgumentParserFactoryMixin:
+class ActionBase(ABC):
     name: str
     description: str
 
+    def __init__(self, **kwargs) -> None:
+        # Just to ignore key word arguments
+        pass
+
+    @abstractmethod
+    def run(self, dry_run: bool = False) -> None:
+        raise NotImplementedError()
+
+    @classmethod
+    def create_from_command(cls, **kwargs) -> "ActionBase":
+        instance: "ActionBase" = cls(**kwargs)
+
+        return instance
+
     @classmethod
     def _update_command(cls, sub_parser: ArgumentParser) -> None:
         # Must be implemented if necessary
         pass
 
     @classmethod
-    def get_allowed_arguments(cls) -> set[str]:
-        return set()
-
-    @classmethod
     def create_command(
         cls, sub_parser_collection: _HasAddSubParser, **kwargs
     ) -> ArgumentParser:
         aliases: list[str] = []
 
         if "aliases" in vars(cls):
             aliases = list(getattr(cls, "aliases"))
@@ -75,42 +85,22 @@
         )
 
         cls._update_command(parser)
 
         return parser
 
 
-class ActionBase(ABC, _ArgumentParserFactoryMixin):
-    def __init__(self, **kwargs) -> None:
-        # Just to ignore key word arguments
-        pass
-
-    @abstractmethod
-    def run(self, dry_run: bool = False) -> None:
-        raise NotImplementedError()
-
-    @classmethod
-    def create_from_command(cls, **kwargs) -> "ActionBase":
-        instance: "ActionBase" = cls(**kwargs)
-
-        return instance
-
-
 class VersionConsumer(ActionBase):
     def __init__(self, version: Version, **kwargs) -> None:
         self.__version = version
 
     @property
     def current_version(self) -> Version:
         return self.__version
 
-    @classmethod
-    def get_allowed_arguments(cls) -> set[str]:
-        return set(["version"]).union(ActionBase.get_allowed_arguments())
-
 
 class VersionModifier(VersionConsumer):
     def __init__(
         self, version: Version, persister: VersionPersister, **kwargs
     ) -> None:
         super().__init__(version, **kwargs)
         self.__persister = persister
@@ -129,20 +119,14 @@
     def run(self, dry_run: bool = False) -> None:
         next_version: Version = self.create_new_version()
         if not dry_run:
             self.__persister.save_version(next_version)
         else:
             logger.info("Would write new version %s", next_version)
 
-    @classmethod
-    def get_allowed_arguments(cls) -> set[str]:
-        return set(["persister"]).union(
-            VersionConsumer.get_allowed_arguments()
-        )
-
 
 class ActionRegistry:
     def __init__(self) -> None:
         self.__items: dict[str, type[ActionBase]] = {}
 
     def register(self) -> Callable:
         def decorator(clazz: type[ActionBase]):
@@ -175,17 +159,15 @@
 
         for key in keys:
             clazz = self.__items[key]
             clazz.create_command(parsers, exit_on_error=exit_on_error)
 
     def execute(
         self,
-        /,
         args: Namespace,
-        *,
         version: Version,
         persister: VersionPersister,
         vcs_provider: VcsProvider,
     ) -> None:
         kwargs: dict = {}
 
         kwargs.update(vars(args))
@@ -200,34 +182,28 @@
         if "dry_run" in kwargs:
             dry_run = bool(kwargs.pop("dry_run"))
 
         selected_command: str = kwargs.pop("selected_command")
 
         if selected_command not in self.__items:
             raise ValueError(
-                f"Failed to get command {selected_command}. "
+                f"´Failed to get command {selected_command}. "
                 + "Valid values are {', '.join(self.__items.keys())}."
             )
 
         clazz: type[ActionBase] = self.__items[selected_command]
 
-        allowed_args: set[str] = clazz.get_allowed_arguments()
-        allowed_kwargs: dict[str, Any] = {
-            "version": version,
-            "persister": persister,
-            "vcs_provider": vcs_provider,
-        }
+        if issubclass(clazz, VersionConsumer):
+            kwargs["version"] = version
 
-        allowed_kwargs = {
-            key: value
-            for key, value in allowed_kwargs.items()
-            if key in allowed_args
-        }
+        if issubclass(clazz, VersionModifier):
+            kwargs["persister"] = persister
 
-        kwargs.update(allowed_kwargs)
+        if issubclass(clazz, VcsProviderAggregator):
+            kwargs["vcs_provider"] = vcs_provider
 
         command: "ActionBase" = clazz.create_from_command(**kwargs)
         command.run(dry_run=dry_run)
 
 
 actions = ActionRegistry()
 action = actions.register()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pdm-bump-0.7.0/src/pdm_bump/actions/explicit.py` & `pdm-bump-0.7.0a1/src/pdm_bump/actions/explicit.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/actions/increment.py` & `pdm-bump-0.7.0a1/src/pdm_bump/actions/increment.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 class FinalizingVersionModifier(_NonFinalPartsRemovingVersionModifier):
     name: str = "no-pre-release"
     description: str = "Remove all pre-release parts from the version"
 
     def __init__(
         self, version: Version, persister: VersionPersister, **kwargs
     ) -> None:
-        super().__init__(version, persister, **kwargs)
+        super().__init__(version, persister, True, **kwargs)
 
     @traced_function
     def create_new_version(self) -> Version:
         constructional_args: dict[
             str,
             Any
             # Using type alias due to line length enforced by black
```

### Comparing `pdm-bump-0.7.0/src/pdm_bump/actions/preview.py` & `pdm-bump-0.7.0a1/src/pdm_bump/actions/preview.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/actions/vcs.py` & `pdm-bump-0.7.0a1/src/pdm_bump/actions/vcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,13 +34,7 @@
         if not dry_run:
             self.vcs_provider.create_tag_from_version(self.current_version)
         else:
             logger.info(
                 "Would create tag v%s",
                 Pep440VersionFormatter().format(self.current_version),
             )
-
-    @classmethod
-    def get_allowed_arguments(cls) -> set[str]:
-        return set(["vcs_provider"]).union(
-            VersionConsumer.get_allowed_arguments()
-        )
```

### Comparing `pdm-bump-0.7.0/src/pdm_bump/cli.py` & `pdm-bump-0.7.0a1/src/pdm_bump/cli.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/core/config.py` & `pdm-bump-0.7.0a1/src/pdm_bump/core/config.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/core/logging.py` & `pdm-bump-0.7.0a1/src/pdm_bump/core/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,26 +185,14 @@
     for handler in list(logger.handlers):
         logger.removeHandler(handler)
 
     new_handler: Handler = TermUIHandler(ui_instance)
     logger.addHandler(new_handler)
 
 
-def setup_logger(level: int) -> None:
-    if 0 > level:
-        return
-
-    if level == 0:
-        logger.setLevel(INFO)
-    elif level == 1:
-        logger.setLevel(DEBUG)
-    elif level == 2:
-        logger.setLevel(TRACE)
-
-
 def traced_function(fun):
     def tracing_function(*args, **kwargs):
         try:
             logger.trace(
                 "%s: Entering function", fun.__qualname__ or fun.__name__
             )
             return fun(*args, **kwargs)
```

### Comparing `pdm-bump-0.7.0/src/pdm_bump/core/version.py` & `pdm-bump-0.7.0a1/src/pdm_bump/core/version.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/dynamic.py` & `pdm-bump-0.7.0a1/src/pdm_bump/dynamic.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/plugin.py` & `pdm-bump-0.7.0a1/src/pdm_bump/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from pdm.cli.commands.base import BaseCommand  # type: ignore
 from pdm.termui import UI  # type: ignore
 
 from .actions import actions
 from .core.config import Config, ConfigHolder, ConfigKeys, ConfigSections
 from .core.logging import (
     logger,
-    setup_logger,
     traced_function,
     update_logger_from_project_ui,
 )
 from .core.version import Pep440VersionFormatter, Version
 from .dynamic import DynamicVersionSource
 from .source import StaticPep621VersionSource
 from .vcs import (
@@ -95,19 +94,14 @@
             logger.error(msg)
             return
 
         self.__backend.current_version = version
 
     @traced_function
     def handle(self, project: _ProjectLike, options: Namespace) -> None:
-        # This will not handling tracing or related parts
-        # Should be evaluated at start-up time
-        if hasattr(options, "verbose"):
-            setup_logger(options.verbose)
-
         config: Config = Config(project)
         update_logger_from_project_ui(project.core.ui)
 
         selected_backend: Optional[_VersionSource] = self._select_backend(
             project, config
         )
 
@@ -119,18 +113,15 @@
             return
 
         backend: _VersionSource = cast(_VersionSource, selected_backend)
         vcs_provider: VcsProvider = self._get_vcs_provider(project)
 
         try:
             actions.execute(
-                options,
-                version=backend.current_version,
-                persister=self,
-                vcs_provider=vcs_provider,
+                options, backend.current_version, self, vcs_provider
             )
         except ValueError as exc:
             logger.exception("Failed to execute action", exc_info=True)
             logger.debug("Exception occurred: %s", get_traceback())
             raise SystemExit(1) from exc
 
     @traced_function
```

### Comparing `pdm-bump-0.7.0/src/pdm_bump/source.py` & `pdm-bump-0.7.0a1/src/pdm_bump/source.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/vcs/core.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/core.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/vcs/git.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/vcs/gitcli.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/gitcli.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/src/pdm_bump/vcs/mixins.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/mixins.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/tests/action_test.py` & `pdm-bump-0.7.0a1/tests/action_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,33 +10,27 @@
 # Refer to LICENSE for more information
 #
 
 import unittest
 from typing import Callable
 
 from pdm_bump.actions import (
+    PreviewMismatchError,
     VersionModifier,
-)
-from pdm_bump.actions.increment import (
     MajorIncrementingVersionModifier,
     MinorIncrementingVersionModifier,
     MicroIncrementingVersionModifier,
+    AlphaIncrementingVersionModifier,
+    BetaIncrementingVersionModifier,
+    ReleaseCandidateIncrementingVersionModifier,
     FinalizingVersionModifier,
     EpochIncrementingVersionModifier,
     DevelopmentVersionIncrementingVersionModifier,
     PostVersionIncrementingVersionModifier,
 )
-from pdm_bump.actions.preview import (
-    PreviewMismatchError,
-    AlphaIncrementingVersionModifier,
-    BetaIncrementingVersionModifier,
-    ReleaseCandidateIncrementingVersionModifier,
-)
-
-
 from pdm_bump.core.version import Version
 
 
 class _UnitTestPersister:
     def save_version(self, version: Version) -> None:
         # Just for testing
         pass
```

### Comparing `pdm-bump-0.7.0/tests/plugin_test.py` & `pdm-bump-0.7.0a1/tests/plugin_test.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/tests/version_test.py` & `pdm-bump-0.7.0a1/tests/version_test.py`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0/PKG-INFO` & `pdm-bump-0.7.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-bump
-Version: 0.7.0
+Version: 0.7.0a1
 Summary: A plugin for PDM providing the ability to modify the version according to PEP440
 License: MIT
 Author-email: Carsten Igel <cig@bite-that-bit.de>
 Requires-Python: >=3.9
 Project-URL: homepage, https://github.com/carstencodes/pdm-bump
 Description-Content-Type: text/markdown
```

