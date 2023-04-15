# Comparing `tmp/osintbuddy-0.0.2rc15.post1.tar.gz` & `tmp/osintbuddy-0.0.2rc16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.2rc15.post1.tar", last modified: Sat Apr 15 20:24:06 2023, max compression
+gzip compressed data, was "osintbuddy-0.0.2rc16.post1.tar", last modified: Sat Apr 15 21:20:22 2023, max compression
```

## Comparing `osintbuddy-0.0.2rc15.post1.tar` & `osintbuddy-0.0.2rc16.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      274 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      447 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/.pypirc
--rw-r--r--   0        0        0      444 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/Dockerfile
--rw-r--r--   0        0        0       11 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/LICENSE
--rw-r--r--   0        0        0     5859 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/README.md
--rw-r--r--   0        0        0       47 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/docs/workflows.md
--rw-r--r--   0        0        0     6714 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/pyproject.toml
--rw-r--r--   0        0        0      251 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/src/README.md
--rw-r--r--   0        0        0      374 2023-04-15 20:24:06.216672 osintbuddy-0.0.2rc15.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      527 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/src/osintbuddy/examples/ip-plugin.py
--rw-r--r--   0        0        0      206 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/src/osintbuddy/manager.py
--rw-r--r--   0        0        0     1284 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     6498 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      989 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/tests/conftest.py
--rw-r--r--   0        0        0      715 2023-04-15 20:24:03.616503 osintbuddy-0.0.2rc15.post1/tests/test_methods.py
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc15.post1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      447 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/Dockerfile
+-rw-r--r--   0        0        0       11 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/LICENSE
+-rw-r--r--   0        0        0      809 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/README.md
+-rw-r--r--   0        0        0       47 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6726 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/README.md
+-rw-r--r--   0        0        0      374 2023-04-15 21:20:22.593318 osintbuddy-0.0.2rc16.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      527 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/examples/ip-plugin.py
+-rw-r--r--   0        0        0      206 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/manager.py
+-rw-r--r--   0        0        0     1219 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     6498 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/tests/conftest.py
+-rw-r--r--   0        0        0      664 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc16.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.2rc15.post1/.gitignore` & `osintbuddy-0.0.2rc16.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc15.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.2rc16.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc15.post1/docs/pylint.md` & `osintbuddy-0.0.2rc16.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc15.post1/pyproject.toml` & `osintbuddy-0.0.2rc16.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "pytest==7.2.2",
     "pytest-github-actions-annotate-failures",
     "shellcheck-py==0.9.0.2"
 ]
 
 [project.urls]
 Documentation = "https://docs-osintbuddy-com.vercel.app/"
-Source = "https://github.com/jerlendds/osintbuddy"
+Source = "https://github.com/jerlendds/plugins.osintbuddy.com"
 Tracker = "https://github.com/jerlendds/osintbuddy/issues"
 
 [tool.flit.module]
 name = "osintbuddy"
 
 [tool.bandit]
 exclude_dirs = ["build","dist","tests","scripts"]
```

### Comparing `osintbuddy-0.0.2rc15.post1/src/osintbuddy/examples/ip-plugin.py` & `osintbuddy-0.0.2rc16.post1/src/osintbuddy/examples/ip-plugin.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc15.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.2rc16.post1/src/osintbuddy/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,30 @@
         self.transforms: dict = None
         self.node: dict = None
         self.node_name: str = None
         self.settings: dict = None
         self.repository: str = None
         self.authors = List[str]
         self._base_plugin_endpoint = slugify(self.node_name)
-        self._endpoints = self.generate_endpoints()
         self._router: APIRouter = APIRouter(prefix=self._base_plugin_endpoint)
+        self._generate_endpoints()
 
     def request(self, transform: str, **kwargs):
         return self.transforms[transform](**kwargs)
 
     def _generate_endpoints(self):
         if self.transforms is None:
             return
-        endpoints = []
         for transform in self.transforms.keys():
             route = str.encode(
                 f"{self._base_plugin_endpoint}{transform}{self.repository}"
             )
             endpoint_route = hashlib.md5(route).hexdigest()
             self._router.add_api_route(
                 endpoint_route,
                 endpoint=self.transforms[transform]
             )
-        return endpoints
 
 
 class Plugin(BasePlugin):
     def __init__(self):
         pass
```

### Comparing `osintbuddy-0.0.2rc15.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.2rc16.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc15.post1/tests/conftest.py` & `osintbuddy-0.0.2rc16.post1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 This is a configuration file for pytest containing customizations and fixtures.
 
 In VSCode, Code Coverage is recorded in config.xml. Delete this file to reset reporting.
 """
 
 from __future__ import annotations
 
-from typing import List
-
 import pytest
 from _pytest.nodes import Item
 
 
 def pytest_collection_modifyitems(items: list[Item]):
     for item in items:
         if "spark" in item.nodeid:
```

