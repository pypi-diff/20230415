# Comparing `tmp/pipen_args-0.9.0.tar.gz` & `tmp/pipen_args-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_args-0.9.0.tar", max compression
+gzip compressed data, was "pipen_args-0.9.1.tar", max compression
```

## Comparing `pipen_args-0.9.0.tar` & `pipen_args-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2159 2023-04-14 20:12:43.760336 pipen_args-0.9.0/README.md
--rw-r--r--   0        0        0      969 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/__init__.py
--rw-r--r--   0        0        0     3851 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/defaults.py
--rw-r--r--   0        0        0     9490 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/parser_.py
--rw-r--r--   0        0        0     4784 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/plugin.py
--rw-r--r--   0        0        0     3277 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/procgroup.py
--rw-r--r--   0        0        0       22 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/version.py
--rw-r--r--   0        0        0     1185 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 pipen_args-0.9.0/setup.py
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 pipen_args-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2173 2023-04-15 03:36:06.342230 pipen_args-0.9.1/README.md
+-rw-r--r--   0        0        0      969 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pipen_args/__init__.py
+-rw-r--r--   0        0        0     3851 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pipen_args/defaults.py
+-rw-r--r--   0        0        0     9490 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pipen_args/parser_.py
+-rw-r--r--   0        0        0     5335 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pipen_args/plugin.py
+-rw-r--r--   0        0        0     3277 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pipen_args/procgroup.py
+-rw-r--r--   0        0        0       22 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pipen_args/version.py
+-rw-r--r--   0        0        0     1185 2023-04-15 03:36:06.342230 pipen_args-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 pipen_args-0.9.1/setup.py
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pipen_args-0.9.1/PKG-INFO
```

### Comparing `pipen_args-0.9.0/README.md` & `pipen_args-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,26 +46,27 @@
 Optional Arguments:
   -h, --help, -h+, --help+
                         show help message (with + to show more options) and exit
 ```
 
 See more examples in `tests/pipelines/` folder.
 
-## Metadata for env items
+## Metadata for Proc envs items
 
 The metadata in the docstring of env items determines how the arguments are defined.
 
 ```python
 class Process(Proc):
     """My process
 
     # other docstring sections
 
     Envs:
         a (<metadata>): ...
+    """
 ```
 
 The metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to
 separate the key and value. The value is optional. If the value is not specified, it
 will be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.
 
 [1]: https://github.com/pwwang/pipen
```

### Comparing `pipen_args-0.9.0/pipen_args/__init__.py` & `pipen_args-0.9.1/pipen_args/__init__.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.0/pipen_args/defaults.py` & `pipen_args-0.9.1/pipen_args/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.0/pipen_args/parser_.py` & `pipen_args-0.9.1/pipen_args/parser_.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.0/pipen_args/plugin.py` & `pipen_args-0.9.1/pipen_args/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 from argx import Namespace
 from simpleconf import ProfileConfig
 from pipen import plugin
 from pipen.defaults import CONFIG_FILES
-from pipen.utils import copy_dict
+from pipen.utils import copy_dict, get_logger
 
 from .version import __version__
 from .parser_ import Parser
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Pipen
 
+logger = get_logger("args", "info")
+
 
 class ArgsPlugin:
     """Automatically parse arguments and load configs for pipen pipelines"""
     name = "args"
     version = __version__
 
     @plugin.impl
@@ -85,38 +87,48 @@
             config[key] = old
 
         if parser.flatten_proc_args is True:
             parsed = Namespace(**{pipen.procs[0].name: parsed})
 
         for proc in pipen.procs:
             proc_args = vars(getattr(parsed, proc.name))
-            if "in" in proc_args:
-                from pandas import DataFrame
-                from pandas.core.dtypes.api import is_scalar
-
-                indata = vars(proc_args["in"])
-                for key, val in indata.items():
-                    if is_scalar(val):
-                        indata[key] = [val]
-
-                maxlen = max(map(len, indata.values()))
-                input_data = DataFrame(
-                    {
-                        key: (
-                            val * maxlen
-                            if len(val) == 1 and maxlen > 1
-                            else val
-                        )
-                        for key, val in indata.items()
-                        if val is not None and len(val) > 0
-                    }
-                )
-                # only when input data is given
-                if input_data.shape[0] > 0:
-                    proc.input_data = input_data
+            if (
+                "in" in proc_args
+                and not all(v is None for v in vars(proc_args["in"]).values())
+            ):
+                if proc.input_data is not None:
+                    logger.warning(
+                        "[red]![%s] input_data is given, ignore input from "
+                        "parsed arguments[/red]",
+                        proc.name,
+                    )
+                else:
+                    from pandas import DataFrame
+                    from pandas.core.dtypes.api import is_scalar
+
+                    indata = vars(proc_args["in"])
+                    for key, val in indata.items():
+                        if is_scalar(val):
+                            indata[key] = [val]
+
+                    maxlen = max(map(len, indata.values()))
+                    input_data = DataFrame(
+                        {
+                            key: (
+                                val * maxlen
+                                if len(val) == 1 and maxlen > 1
+                                else val
+                            )
+                            for key, val in indata.items()
+                            if val is not None and len(val) > 0
+                        }
+                    )
+                    # only when input data is given and not all None
+                    if input_data.shape[0] > 0:
+                        proc.input_data = input_data
 
             if (
                 "envs" in proc_args
                 and proc.envs is not None
                 and proc_args["envs"] is not None
             ):
                 proc_envs = (
```

### Comparing `pipen_args-0.9.0/pipen_args/procgroup.py` & `pipen_args-0.9.1/pipen_args/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.0/pyproject.toml` & `pipen_args-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-args"
-version = "0.9.0"
+version = "0.9.1"
 description = "Command-line argument parser for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-args"
 repository = "https://github.com/pwwang/pipen-args"
```

### Comparing `pipen_args-0.9.0/setup.py` & `pipen_args-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pipen-annotate>=0.7.1,<0.8.0']
 
 entry_points = \
 {'pipen': ['args = pipen_args.plugin:ArgsPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-args',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Command-line argument parser for pipen.',
-    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for env items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-args',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pipen_args-0.9.0/PKG-INFO` & `pipen_args-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-args
-Version: 0.9.0
+Version: 0.9.1
 Summary: Command-line argument parser for pipen.
 Home-page: https://github.com/pwwang/pipen-args
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -65,26 +65,27 @@
 Optional Arguments:
   -h, --help, -h+, --help+
                         show help message (with + to show more options) and exit
 ```
 
 See more examples in `tests/pipelines/` folder.
 
-## Metadata for env items
+## Metadata for Proc envs items
 
 The metadata in the docstring of env items determines how the arguments are defined.
 
 ```python
 class Process(Proc):
     """My process
 
     # other docstring sections
 
     Envs:
         a (<metadata>): ...
+    """
 ```
 
 The metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to
 separate the key and value. The value is optional. If the value is not specified, it
 will be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.
 
 [1]: https://github.com/pwwang/pipen
```

