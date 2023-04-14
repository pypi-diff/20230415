# Comparing `tmp/pipen_cli_require-0.5.0.tar.gz` & `tmp/pipen_cli_require-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_cli_require-0.5.0.tar", max compression
+gzip compressed data, was "pipen_cli_require-0.6.0.tar", max compression
```

## Comparing `pipen_cli_require-0.5.0.tar` & `pipen_cli_require-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2123 2023-03-30 06:16:03.321215 pipen_cli_require-0.5.0/README.md
--rw-r--r--   0        0        0       87 2023-03-30 06:16:03.321215 pipen_cli_require-0.5.0/pipen_cli_require/__init__.py
--rw-r--r--   0        0        0     1945 2023-03-30 06:16:03.321215 pipen_cli_require-0.5.0/pipen_cli_require/entry.py
--rw-r--r--   0        0        0     9797 2023-03-30 06:16:03.321215 pipen_cli_require-0.5.0/pipen_cli_require/require.py
--rw-r--r--   0        0        0       46 2023-03-30 06:16:03.321215 pipen_cli_require-0.5.0/pipen_cli_require/version.py
--rw-r--r--   0        0        0     1028 2023-03-30 06:16:03.321215 pipen_cli_require-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 pipen_cli_require-0.5.0/setup.py
--rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 pipen_cli_require-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2682 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/README.md
+-rw-r--r--   0        0        0      132 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/__init__.py
+-rw-r--r--   0        0        0     2277 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/entry.py
+-rw-r--r--   0        0        0    10514 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/require.py
+-rw-r--r--   0        0        0       46 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/version.py
+-rw-r--r--   0        0        0     1026 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 pipen_cli_require-0.6.0/setup.py
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 pipen_cli_require-0.6.0/PKG-INFO
```

### Comparing `pipen_cli_require-0.5.0/README.md` & `pipen_cli_require-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,25 +39,49 @@
     output = "outfile:file:out.txt"
     envs = {"require_conditional": False}
     lang = "python"
 
 # Setup the pipeline
 # Must be outside __main__
 # Or define a function to return the pipeline
-pipeline = Pipen(...).set_start(P1)
+class Pipeline(Pipen):
+    starts = P1
+
 
 if __name__ == '__main__':
-    # Pipeline must be executed with __main__
-    pipeline.run()
+    # Pipeline must run with __main__
+    Pipeline().run()
+```
+
+### Parsing process requirements using API
+
+```python
+from pipen_cli_require import parse_proc_requirements
+
+
+def parse_proc_requirements(
+    proc: Type[Proc]
+) -> Tuple[OrderedDiot, OrderedDiot]:
+    """Parse the requirements of a process
+
+    Args:
+        proc: The process class
+
+    Returns:
+        A tuple of two OrderedDiot's.
+        The first one is the annotated sections by pipen_annotate
+        The second one is the requirements. The key is the name of the
+            requirement, the value is a dict with message, check and if_ keys.
+    """
 ```
 
 ## Checking the requirements via the CLI
 
 ```shell
-> pipen require --r-verbose --r-ncores 2 example_pipeline.py:pipeline
+> pipen require --verbose --ncores 2 example_pipeline.py:pipeline
 
 Checking requirements for pipeline: PIPEN-0
 │
 └── P1: Process 1
     ├── ✅ pipen
     ├── ✅ liquidpy
     ├── ❎ nonexist: Run `pip install -U nonexist` to install
```

### Comparing `pipen_cli_require-0.5.0/pipen_cli_require/entry.py` & `pipen_cli_require-0.6.0/pipen_cli_require/entry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Provides PipenCliRequire"""
 from __future__ import annotations
-from typing import TYPE_CHECKING
 
+import sys
 import asyncio
+from typing import TYPE_CHECKING
+
 from pipen.cli import CLIPlugin
 
 from .require import PipenRequire
 from .version import __version__
 
 if TYPE_CHECKING:  # pragma: no cover
     from argx import ArgumentParser, Namespace
@@ -21,22 +23,22 @@
     def __init__(
         self,
         parser: ArgumentParser,
         subparser: ArgumentParser,
     ) -> None:
         super().__init__(parser, subparser)
         subparser.add_argument(
-            "--r-ncores",
+            "--ncores",
             type=int,
             default=1,
             dest="ncores",
             help="Number of cores to use to check the requirements",
         )
         subparser.add_argument(
-            "--r-verbose",
+            "--verbose",
             action="store_true",
             default=False,
             dest="verbose",
             help="Show verbosal error when checking failed",
         )
         subparser.add_argument(
             "pipeline",
@@ -57,10 +59,17 @@
                 args.pipeline_args,
                 args.ncores,
                 args.verbose,
             ).run()
         )
 
     def parse_args(self) -> Namespace:
-        parsed, rest = self.parser.parse_known_args(fromfile_keep=True)
+        """Parse the arguments"""
+        # split the args into two parts, separated by `--`
+        # the first part is the args for pipen_cli_config
+        # the second part is the args for the pipeline
+        args = sys.argv[1:]
+        idx = args.index("--") if "--" in args else len(args)
+        args, rest = args[:idx], args[idx + 1 :]
+        parsed = self.parser.parse_args(args=args)
         parsed.pipeline_args = rest
         return parsed
```

### Comparing `pipen_cli_require-0.5.0/pipen_cli_require/require.py` & `pipen_cli_require-0.6.0/pipen_cli_require/require.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import List, Mapping, Tuple, Type
 
 from diot import Diot, OrderedDiot
 from rich.tree import Tree
 from rich.live import Live
 from rich.status import Status
 from liquid import Liquid
-from pipen import Pipen, Proc
+from pipen import Pipen, Proc, ProcGroup
 from pipen_annotate import annotate
 
 PROC_SUMMARY_NAME = "_SUMMARY"
 # Cache the status of the checks: check => status
 # When status is SUCESS, then the check is successful
 # Otherwise, it is the error
 STATUSES = Manager().dict()
@@ -43,18 +43,28 @@
     if s is None:
         return None
 
     liq = Liquid(s, from_file=False, mode="wild")
     return liq.render(proc=proc, envs=proc.envs)
 
 
-def _parse_proc_requirements(
+def parse_proc_requirements(
     proc: Type[Proc]
 ) -> Tuple[OrderedDiot, OrderedDiot]:
-    """Parse the requirements of a process"""
+    """Parse the requirements of a process
+
+    Args:
+        proc: The process class
+
+    Returns:
+        A tuple of two OrderedDiot's.
+        The first one is the annotated sections by pipen_annotate
+        The second one is the requirements. The key is the name of the
+            requirement, the value is a dict with message, check and if_ keys.
+    """
     annotated = annotate(proc)
 
     out = OrderedDiot()
     # No requirements specified
     if "Requires" not in annotated:
         return annotated, out
 
@@ -105,67 +115,74 @@
         if STATUSES[check] != CheckingStatus.SUCCESS.value:
             errors[f"{pname}/{name}"] = STATUSES[check]
             raise RuntimeError(STATUSES[check])
         else:
             STATUSES[check] = CheckingStatus.SUCCESS.value
 
 
+def parse_pipeline(pipeline: str) -> Pipen:
+    """Parse the pipeline"""
+    modpath, sep, name = pipeline.rpartition(":")
+    if sep != ":":
+        raise ValueError(
+            f"Invalid pipeline: {pipeline}.\n"
+            "It must be in the format '<module[.submodule]>:pipeline' or \n"
+            "'/path/to/pipeline.py:pipeline'"
+        )
+
+    path = Path(modpath)
+    if path.is_file():
+        spec = importlib.util.spec_from_file_location(path.stem, modpath)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+    else:
+        module = importlib.import_module(modpath)
+
+    try:
+        pipeline = getattr(module, name)
+    except AttributeError:
+        raise ValueError(f"Invalid pipeline: {pipeline}") from None
+
+    if isinstance(pipeline, type) and issubclass(pipeline, Proc):
+        pipeline = Pipen(name=f"{pipeline.name}Pipeline").set_starts(pipeline)
+
+    if isinstance(pipeline, type) and issubclass(pipeline, Pipen):
+        pipeline = pipeline()
+
+    if isinstance(pipeline, type) and issubclass(pipeline, ProcGroup):
+        pipeline = pipeline().as_pipen()
+
+    if not isinstance(pipeline, Pipen):
+        raise ValueError(
+            f"Invalid pipeline: {pipeline}\n"
+            "It must be a `pipen.Pipen` instance"
+        )
+
+    return pipeline
+
+
 class PipenRequire:
     """The class to extract and check requirements"""
 
     def __init__(
         self,
         pipeline: str,
         pipeline_args: List[str],
         ncores: int,
         verbose: bool,
     ):
-        self.pipeline = self._parse_pipeline(pipeline)
+        self.pipeline = parse_pipeline(pipeline)
         self.pipeline_args = pipeline_args
         self.ncores = ncores
         self.verbose = verbose
         self.status = Manager().dict()
         self.errors = Manager().dict()
         self.pool = None
         self.results = OrderedDiot()
 
-    def _parse_pipeline(self, pipeline: str) -> Pipen:
-        """Parse the pipeline"""
-        modpath, sep, name = pipeline.rpartition(":")
-        if sep != ":":
-            raise ValueError(
-                f"Invalid pipeline: {pipeline}.\n"
-                "It must be in the format '<module[.submodule]>:pipeline' or \n"
-                "'/path/to/pipeline.py:pipeline'"
-            )
-
-        path = Path(modpath)
-        if path.is_file():
-            spec = importlib.util.spec_from_file_location(path.stem, modpath)
-            module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(module)
-        else:
-            module = importlib.import_module(modpath)
-
-        try:
-            pipeline = getattr(module, name)
-        except AttributeError:
-            raise ValueError(f"Invalid pipeline: {pipeline}") from None
-
-        if isinstance(pipeline, type) and issubclass(pipeline, Pipen):
-            pipeline = pipeline()
-
-        if not isinstance(pipeline, Pipen):
-            raise ValueError(
-                f"Invalid pipeline: {pipeline}\n"
-                "It must be a `pipen.Pipen` instance"
-            )
-
-        return pipeline
-
     def _generate_tree(self, all_reqs: Mapping[str, Mapping[str, str]]):
         """Generate a tree to show requirements checking"""
 
         self._update_status()
         tree = Tree(
             "\nChecking requirements for pipeline: "
             f"[bold]{self.pipeline.name.upper()}[/bold]\n│",
@@ -269,19 +286,24 @@
 
     async def run(self):
         """Run the pipeline"""
         # Inject the cli arguments to the pipeline
         sys.argv = [self.pipeline.name] + self.pipeline_args
         # Initialize the pipeline so that the arguments definied by
         # other plugins (i.e. pipen-args) to take in place.
+        # Make sure the workdir is created, in case other plugins need it
+        self.pipeline.workdir = Path(self.pipeline.config.workdir).joinpath(
+            self.pipeline.name
+        )
+        self.pipeline.workdir.mkdir(parents=True, exist_ok=True)
         await self.pipeline._init()
         self.pipeline.build_proc_relationships()
         all_reqs = OrderedDiot()
         for proc in self.pipeline.procs:
-            anno, requires = _parse_proc_requirements(proc)
+            anno, requires = parse_proc_requirements(proc)
             all_reqs[proc.name] = requires
             all_reqs[proc.name][PROC_SUMMARY_NAME] = anno.Summary.short
 
         self._start_requirements_check(all_reqs)
 
         with Live(self._generate_tree(all_reqs)) as live:
             while not self.all_done():
```

### Comparing `pipen_cli_require-0.5.0/pyproject.toml` & `pipen_cli_require-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "pipen-cli-require"
-version = "0.5.0"
+version = "0.6.0"
 description = "A pipen cli plugin to check requirements for processes of a pipeline"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen-annotate = "^0.6"
+python = "^3.8"
+pipen-annotate = "^0.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-asyncio = "^0.20"
 pytest-cov = "^4"
 pytest-xdist = "^3"
 cmdy = "^0.5"
-pipen-args = "^0.8"
+pipen-args = "^0.9"
 
 [tool.poetry.plugins.pipen_cli]
 cli-require = "pipen_cli_require:PipenCliRequirePlugin"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pipen_cli_require-0.5.0/PKG-INFO` & `pipen_cli_require-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pipen-cli-require
-Version: 0.5.0
+Version: 0.6.0
 Summary: A pipen cli plugin to check requirements for processes of a pipeline
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pipen-annotate (>=0.6,<0.7)
+Requires-Dist: pipen-annotate (>=0.7,<0.8)
 Description-Content-Type: text/markdown
 
 # pipen-cli-require
 
 Checking the requirements for processes of a [pipen][1] pipeline
 
 ## Install
@@ -56,25 +56,49 @@
     output = "outfile:file:out.txt"
     envs = {"require_conditional": False}
     lang = "python"
 
 # Setup the pipeline
 # Must be outside __main__
 # Or define a function to return the pipeline
-pipeline = Pipen(...).set_start(P1)
+class Pipeline(Pipen):
+    starts = P1
+
 
 if __name__ == '__main__':
-    # Pipeline must be executed with __main__
-    pipeline.run()
+    # Pipeline must run with __main__
+    Pipeline().run()
+```
+
+### Parsing process requirements using API
+
+```python
+from pipen_cli_require import parse_proc_requirements
+
+
+def parse_proc_requirements(
+    proc: Type[Proc]
+) -> Tuple[OrderedDiot, OrderedDiot]:
+    """Parse the requirements of a process
+
+    Args:
+        proc: The process class
+
+    Returns:
+        A tuple of two OrderedDiot's.
+        The first one is the annotated sections by pipen_annotate
+        The second one is the requirements. The key is the name of the
+            requirement, the value is a dict with message, check and if_ keys.
+    """
 ```
 
 ## Checking the requirements via the CLI
 
 ```shell
-> pipen require --r-verbose --r-ncores 2 example_pipeline.py:pipeline
+> pipen require --verbose --ncores 2 example_pipeline.py:pipeline
 
 Checking requirements for pipeline: PIPEN-0
 │
 └── P1: Process 1
     ├── ✅ pipen
     ├── ✅ liquidpy
     ├── ❎ nonexist: Run `pip install -U nonexist` to install
```

