# Comparing `tmp/pipen_lock-0.1.1.tar.gz` & `tmp/pipen_lock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_lock-0.1.1.tar", max compression
+gzip compressed data, was "pipen_lock-0.2.0.tar", max compression
```

## Comparing `pipen_lock-0.1.1.tar` & `pipen_lock-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-04-05 23:33:53.156309 pipen_lock-0.1.1/LICENSE
--rw-r--r--   0        0        0      348 2023-04-05 23:33:53.156309 pipen_lock-0.1.1/README.md
--rw-r--r--   0        0        0     1019 2023-04-05 23:33:53.156309 pipen_lock-0.1.1/pipen_lock.py
--rw-r--r--   0        0        0      669 2023-04-05 23:33:53.156309 pipen_lock-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 pipen_lock-0.1.1/setup.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pipen_lock-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-14 23:48:38.731598 pipen_lock-0.2.0/LICENSE
+-rw-r--r--   0        0        0      348 2023-04-14 23:48:38.731598 pipen_lock-0.2.0/README.md
+-rw-r--r--   0        0        0     1019 2023-04-14 23:48:38.731598 pipen_lock-0.2.0/pipen_lock.py
+-rw-r--r--   0        0        0      667 2023-04-14 23:48:38.731598 pipen_lock-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 pipen_lock-0.2.0/setup.py
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pipen_lock-0.2.0/PKG-INFO
```

### Comparing `pipen_lock-0.1.1/LICENSE` & `pipen_lock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_lock-0.1.1/pipen_lock.py` & `pipen_lock-0.2.0/pipen_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pipen import plugin
 from pipen.utils import get_logger
 from filelock import FileLock, Timeout
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Proc
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 logger = get_logger("lock", "info")
 
 
 class PipenLockPlugin:
     version = __version__
     name = "lock"
```

### Comparing `pipen_lock-0.1.1/pyproject.toml` & `pipen_lock-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pipen-lock"
-version = "0.1.1"
+version = "0.2.0"
 description = "Process lock for pipen to prevent multiple runs at the same time"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
+python = "^3.8"
+pipen = "^0.9"
 filelock = "^3"
 
 [tool.poetry.plugins.pipen]
 lock = "pipen_lock:pipen_lock_plugin"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `pipen_lock-0.1.1/setup.py` & `pipen_lock-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['pipen_lock']
 install_requires = \
-['filelock>=3,<4', 'pipen>=0.7,<0.8']
+['filelock>=3,<4', 'pipen>=0.9,<0.10']
 
 entry_points = \
 {'pipen': ['lock = pipen_lock:pipen_lock_plugin']}
 
 setup_kwargs = {
     'name': 'pipen-lock',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Process lock for pipen to prevent multiple runs at the same time',
     'long_description': '# pipen-lock\n\nProcess lock for pipen to prevent multiple runs at the same time\n\n## Installation\n\n```bash\npip install -U pipen-lock\n```\n\n## Enable/Disable\n\nThe plugin is enabled by default. To disable it, either uninstall it or:\n\n```python\nfrom pipen import Proc, Pipen\n\n# process definition\n\nclass MyPipeline(Pipen):\n    plugins = ["no:lock"]\n\n```\n',
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

### Comparing `pipen_lock-0.1.1/PKG-INFO` & `pipen_lock-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-lock
-Version: 0.1.1
+Version: 0.2.0
 Summary: Process lock for pipen to prevent multiple runs at the same time
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
 Requires-Dist: filelock (>=3,<4)
-Requires-Dist: pipen (>=0.7,<0.8)
+Requires-Dist: pipen (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # pipen-lock
 
 Process lock for pipen to prevent multiple runs at the same time
 
 ## Installation
```

