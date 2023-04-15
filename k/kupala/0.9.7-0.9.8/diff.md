# Comparing `tmp/kupala-0.9.7.tar.gz` & `tmp/kupala-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kupala-0.9.7.tar", max compression
+gzip compressed data, was "kupala-0.9.8.tar", max compression
```

## Comparing `kupala-0.9.7.tar` & `kupala-0.9.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1074 2021-11-23 10:14:57.770830 kupala-0.9.7/LICENSE
--rw-r--r--   0        0        0      840 2021-11-23 10:14:57.770830 kupala-0.9.7/README.md
--rw-r--r--   0        0        0        0 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/__init__.py
--rw-r--r--   0        0        0     5702 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/application.py
--rw-r--r--   0        0        0     2656 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/config.py
--rw-r--r--   0        0        0       52 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/constants.py
--rw-r--r--   0        0        0    11056 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/container.py
--rw-r--r--   0        0        0      817 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/contracts.py
--rw-r--r--   0        0        0     4638 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/csrf.py
--rw-r--r--   0        0        0    11976 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/dotenv.py
--rw-r--r--   0        0        0     7150 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/exceptions.py
--rw-r--r--   0        0        0        0 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/ext/__init__.py
--rw-r--r--   0        0        0     2826 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/ext/jinja.py
--rw-r--r--   0        0        0      622 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/ext/storages.py
--rw-r--r--   0        0        0     1222 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/form_errors.py
--rw-r--r--   0        0        0     2303 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/json.py
--rw-r--r--   0        0        0     4174 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/messages.py
--rw-r--r--   0        0        0     1488 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/middleware.py
--rw-r--r--   0        0        0      243 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/providers.py
--rw-r--r--   0        0        0     9371 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/requests.py
--rw-r--r--   0        0        0     1389 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/resources.py
--rw-r--r--   0        0        0     3702 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/response_factories.py
--rw-r--r--   0        0        0     5913 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/responses.py
--rw-r--r--   0        0        0    21151 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/routing.py
--rw-r--r--   0        0        0      560 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/shortcuts.py
--rw-r--r--   0        0        0      214 2021-11-23 10:14:57.770830 kupala-0.9.7/kupala/storages.py
--rw-r--r--   0        0        0     1162 2021-11-23 10:14:57.774830 kupala-0.9.7/kupala/templates/errors/http_error.html
--rw-r--r--   0        0        0     1869 2021-11-23 10:14:57.774830 kupala-0.9.7/kupala/templating.py
--rw-r--r--   0        0        0       70 2021-11-23 10:14:57.774830 kupala-0.9.7/kupala/testclient.py
--rw-r--r--   0        0        0      171 2021-11-23 10:14:57.774830 kupala-0.9.7/kupala/types.py
--rw-r--r--   0        0        0      164 2021-11-23 10:14:57.774830 kupala-0.9.7/kupala/utils.py
--rw-r--r--   0        0        0       51 2021-11-23 10:14:57.774830 kupala-0.9.7/kupala/websockets.py
--rw-r--r--   0        0        0     2627 2021-11-23 10:14:57.774830 kupala-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     1762 2021-11-23 10:15:37.536203 kupala-0.9.7/setup.py
--rw-r--r--   0        0        0     2071 2021-11-23 10:15:37.536504 kupala-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-11-23 16:31:33.146887 kupala-0.9.8/LICENSE
+-rw-r--r--   0        0        0      840 2021-11-23 16:31:33.146887 kupala-0.9.8/README.md
+-rw-r--r--   0        0        0        0 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/__init__.py
+-rw-r--r--   0        0        0     5702 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/application.py
+-rw-r--r--   0        0        0     2656 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/config.py
+-rw-r--r--   0        0        0       52 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/constants.py
+-rw-r--r--   0        0        0    11087 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/container.py
+-rw-r--r--   0        0        0     1058 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/contracts.py
+-rw-r--r--   0        0        0     4638 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/csrf.py
+-rw-r--r--   0        0        0    11976 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/dotenv.py
+-rw-r--r--   0        0        0     7150 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/exceptions.py
+-rw-r--r--   0        0        0        0 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/ext/__init__.py
+-rw-r--r--   0        0        0     2826 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/ext/jinja.py
+-rw-r--r--   0        0        0      622 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/ext/storages.py
+-rw-r--r--   0        0        0     1222 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/form_errors.py
+-rw-r--r--   0        0        0     2303 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/json.py
+-rw-r--r--   0        0        0     4174 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/messages.py
+-rw-r--r--   0        0        0     1488 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/middleware.py
+-rw-r--r--   0        0        0      243 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/providers.py
+-rw-r--r--   0        0        0     9371 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/requests.py
+-rw-r--r--   0        0        0     1389 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/resources.py
+-rw-r--r--   0        0        0     3702 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/response_factories.py
+-rw-r--r--   0        0        0     5913 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/responses.py
+-rw-r--r--   0        0        0    21151 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/routing.py
+-rw-r--r--   0        0        0      560 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/shortcuts.py
+-rw-r--r--   0        0        0      214 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/storages.py
+-rw-r--r--   0        0        0     1162 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/templates/errors/http_error.html
+-rw-r--r--   0        0        0     1869 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/templating.py
+-rw-r--r--   0        0        0       70 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/testclient.py
+-rw-r--r--   0        0        0      171 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/types.py
+-rw-r--r--   0        0        0      164 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/utils.py
+-rw-r--r--   0        0        0       51 2021-11-23 16:31:33.146887 kupala-0.9.8/kupala/websockets.py
+-rw-r--r--   0        0        0     2627 2021-11-23 16:31:33.146887 kupala-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     1762 2021-11-23 16:32:46.708248 kupala-0.9.8/setup.py
+-rw-r--r--   0        0        0     2071 2021-11-23 16:32:46.708661 kupala-0.9.8/PKG-INFO
```

### Comparing `kupala-0.9.7/LICENSE` & `kupala-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/README.md` & `kupala-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/application.py` & `kupala-0.9.8/kupala/application.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/config.py` & `kupala-0.9.8/kupala/config.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/container.py` & `kupala-0.9.8/kupala/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,17 @@
     """Raise if injection cannot be proceed."""
 
     ErrorType = InjectionErrorType
 
     def __init__(
         self, message: str, error_type: InjectionErrorType, invokation_target: t.Union[t.Callable, t.Type]
     ) -> None:
-        class_name = (
-            invokation_target.__class__.__name__ if inspect.isclass(invokation_target) else invokation_target.__name__
-        )
-        addon = f'Tried to invoke: {class_name}{inspect.signature(invokation_target)}.'
+        class_name = invokation_target.__name__ if inspect.isclass(invokation_target) else invokation_target.__name__
+        module_name = invokation_target.__module__
+        addon = f'Tried to invoke: {module_name}.{class_name}{inspect.signature(invokation_target)}.'
         super().__init__(message + f'\n{addon}')
         self.error_type = error_type
 
 
 S = t.TypeVar('S')
 Key = t.Union[str, t.Type[S]]
```

### Comparing `kupala-0.9.7/kupala/contracts.py` & `kupala-0.9.8/kupala/contracts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import typing as t
 
 from kupala.requests import Request
 
 SERVICE = t.TypeVar('SERVICE')
 
 
+class PasswordHasher(t.Protocol):  # pragma: no cover
+    def hash(self, plain_password: str) -> str:
+        ...
+
+
+class PasswordVerifier(t.Protocol):  # pragma: no cover
+    def verify(self, plain: str, hashed: str) -> bool:
+        ...
+
+
 class Resolver(t.Protocol):  # pragma: nocover
     """A service resolver protocol."""
 
     def resolve(self, key: t.Type[SERVICE]) -> SERVICE:
         ...
```

### Comparing `kupala-0.9.7/kupala/csrf.py` & `kupala-0.9.8/kupala/csrf.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/dotenv.py` & `kupala-0.9.8/kupala/dotenv.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/exceptions.py` & `kupala-0.9.8/kupala/exceptions.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/ext/jinja.py` & `kupala-0.9.8/kupala/ext/jinja.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/ext/storages.py` & `kupala-0.9.8/kupala/ext/storages.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/form_errors.py` & `kupala-0.9.8/kupala/form_errors.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/json.py` & `kupala-0.9.8/kupala/json.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/messages.py` & `kupala-0.9.8/kupala/messages.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/middleware.py` & `kupala-0.9.8/kupala/middleware.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/requests.py` & `kupala-0.9.8/kupala/requests.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/resources.py` & `kupala-0.9.8/kupala/resources.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/response_factories.py` & `kupala-0.9.8/kupala/response_factories.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/responses.py` & `kupala-0.9.8/kupala/responses.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/routing.py` & `kupala-0.9.8/kupala/routing.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/shortcuts.py` & `kupala-0.9.8/kupala/shortcuts.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/templates/errors/http_error.html` & `kupala-0.9.8/kupala/templates/errors/http_error.html`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/kupala/templating.py` & `kupala-0.9.8/kupala/templating.py`

 * *Files identical despite different names*

### Comparing `kupala-0.9.7/pyproject.toml` & `kupala-0.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "kupala"
 description = "A modern web framework for Python."
-version = "0.9.7"
+version = "0.9.8"
 authors = ["Alex Oleshkevich <alex.oleshkevich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alex-oleshkevich/kupala"
 repository = "https://github.com/alex-oleshkevich/kupala"
 documentation = "https://github.com/alex-oleshkevich/kupala"
 keywords = []
```

### Comparing `kupala-0.9.7/setup.py` & `kupala-0.9.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'python-dotenv>=0.19.1,<0.20.0',
  'python-multipart>=0.0.5,<0.0.6',
  'starlette>=0.17.0,<0.18.0',
  'starsessions>=1.1.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'kupala',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'A modern web framework for Python.',
     'long_description': '# Kupala Framework\n\nA modern web framework for Python.\n\n![PyPI](https://img.shields.io/pypi/v/kupala)\n![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alex-oleshkevich/kupala/Lint)\n![GitHub](https://img.shields.io/github/license/alex-oleshkevich/kupala)\n![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/kupala)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/kupala)\n![GitHub Release Date](https://img.shields.io/github/release-date/alex-oleshkevich/kupala)\n![Lines of code](https://img.shields.io/tokei/lines/github/alex-oleshkevich/kupala)\n\n## Installation\n\nInstall `kupala` using PIP or poetry:\n\n```bash\npip install kupala\n# or\npoetry add kupala\n```\n\n## Features\n\n-   TODO\n\n## Quick start\n\nSee example application in `examples/` directory of this repository.\n',
     'author': 'Alex Oleshkevich',
     'author_email': 'alex.oleshkevich@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/alex-oleshkevich/kupala',
```

### Comparing `kupala-0.9.7/PKG-INFO` & `kupala-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kupala
-Version: 0.9.7
+Version: 0.9.8
 Summary: A modern web framework for Python.
 Home-page: https://github.com/alex-oleshkevich/kupala
 License: MIT
 Author: Alex Oleshkevich
 Author-email: alex.oleshkevich@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

