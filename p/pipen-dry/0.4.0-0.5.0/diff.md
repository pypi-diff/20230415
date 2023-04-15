# Comparing `tmp/pipen_dry-0.4.0.tar.gz` & `tmp/pipen_dry-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_dry-0.4.0.tar", max compression
+gzip compressed data, was "pipen_dry-0.5.0.tar", max compression
```

## Comparing `pipen_dry-0.4.0.tar` & `pipen_dry-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      416 2023-03-29 23:58:05.174136 pipen_dry-0.4.0/README.md
--rw-r--r--   0        0        0     2760 2023-03-29 23:58:05.174136 pipen_dry-0.4.0/pipen_dry.py
--rw-r--r--   0        0        0      638 2023-03-29 23:58:05.174136 pipen_dry-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 pipen_dry-0.4.0/setup.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pipen_dry-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      416 2023-04-15 03:45:37.241097 pipen_dry-0.5.0/README.md
+-rw-r--r--   0        0        0     2711 2023-04-15 03:45:37.241097 pipen_dry-0.5.0/pipen_dry.py
+-rw-r--r--   0        0        0      628 2023-04-15 03:45:37.241097 pipen_dry-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 pipen_dry-0.5.0/setup.py
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pipen_dry-0.5.0/PKG-INFO
```

### Comparing `pipen_dry-0.4.0/pipen_dry.py` & `pipen_dry-0.5.0/pipen_dry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 
 """Dry run a pipeline for pipen"""
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
-from slugify import slugify
 from xqute.scheduler import Scheduler
 from xqute.defaults import JobStatus
 from xqute.utils import a_mkdir
 from pipen import plugin
 from pipen.scheduler import get_scheduler
 from pipen.job import Job
 from pipen.defaults import ProcOutputType
 from pipen.utils import get_logger
 
 if TYPE_CHECKING:
     from pipen import Proc
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 SCHEDULER_NAME = "dry"
 
 logger = get_logger("dry", "info")
 
 
 class DryJob(Job):
@@ -80,16 +79,15 @@
             proc.scheduler or proc.pipeline.config.scheduler
         )
 
         if sched.name != SCHEDULER_NAME:
             return
 
         proc.__class__.workdir = (
-            Path(proc.pipeline.workdir)
-            / f"{slugify(proc.name)}.dry"
+            Path(proc.pipeline.workdir) / f"{proc.name}.dry"
         )
 
         proc.cache = False
         proc.export = False
 
     @plugin.impl
     async def on_proc_start(self, proc: Proc) -> None:
```

### Comparing `pipen_dry-0.4.0/pyproject.toml` & `pipen_dry-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pipen-dry"
-version = "0.4.0"
+version = "0.5.0"
 description = "Dry runner for pipen pipelines"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
+python = "^3.8"
+pipen = "^0.9"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.plugins.pipen_sched]
@@ -23,9 +23,9 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
```

### Comparing `pipen_dry-0.4.0/setup.py` & `pipen_dry-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['pipen_dry']
 install_requires = \
-['pipen>=0.7,<0.8']
+['pipen>=0.9,<0.10']
 
 entry_points = \
 {'pipen': ['dry = pipen_dry:PipenDry'],
  'pipen_sched': ['dry = pipen_dry:PipenDryScheduler']}
 
 setup_kwargs = {
     'name': 'pipen-dry',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Dry runner for pipen pipelines',
     'long_description': '# pipen-dry\n\nDry runner for [pipen][1]\n\nIt is useful to quickly check if there are misconfigurations for your pipeline without actually running it.\n\n## Install\n\n```shell\npip install -U pipen-dry\n```\n\n## Usage\n\n- Use it for process\n\n    ```python\n    class P1(Proc):\n        scheduler = "dry"\n    ```\n\n- Use it for pipeline\n\n    ```python\n    Pipen(scheduler="dry", ...)\n    ```\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen_dry-0.4.0/PKG-INFO` & `pipen_dry-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pipen-dry
-Version: 0.4.0
+Version: 0.5.0
 Summary: Dry runner for pipen pipelines
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
-Requires-Dist: pipen (>=0.7,<0.8)
+Requires-Dist: pipen (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # pipen-dry
 
 Dry runner for [pipen][1]
 
 It is useful to quickly check if there are misconfigurations for your pipeline without actually running it.
```

