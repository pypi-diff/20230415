# Comparing `tmp/essentials-configuration-2.0.2.tar.gz` & `tmp/essentials_configuration-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "essentials-configuration-2.0.2.tar", last modified: Mon Apr 10 11:40:27 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `essentials-configuration-2.0.2.tar` & `essentials_configuration-2.0.3.tar`

### file list

```diff
@@ -1,48 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.531860 essentials-configuration-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.519860 essentials-configuration-2.0.2/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/env/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/env/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/errors/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/ini/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/ini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/ini/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/json/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/json/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/secrets/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/config/toml/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/toml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/toml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/config/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/yaml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/essentials_configuration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:40:27.531860 essentials-configuration-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/tests/test_examples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/cli/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/cli/py.typed
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/common/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/common/files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/common/py.typed
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/env/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/env/py.typed
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/errors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/errors/py.typed
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/ini/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/ini/py.typed
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/json/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/json/py.typed
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/toml/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/toml/py.typed
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/user/__init__.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/user/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/user/py.typed
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/yaml/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/config/yaml/py.typed
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/LICENSE
+-rw-r--r--   0        0        0    12810 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/README.md
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 essentials_configuration-2.0.3/PKG-INFO
```

### Comparing `essentials-configuration-2.0.2/LICENSE` & `essentials_configuration-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials-configuration-2.0.2/PKG-INFO` & `essentials_configuration-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: essentials-configuration
-Version: 2.0.2
+Version: 2.0.3
 Summary: Implementation of key-value pair based configuration for Python applications.
-Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 Project-URL: Homepage, https://github.com/Neoteroi/essentials-configuration
 Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-configuration/issues
-Keywords: configuration,root,management,strategy
+Author-email: Roberto Prevato <roberto.prevato@gmail.com>
+License-File: LICENSE
+Keywords: configuration,management,root,settings,strategy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: yaml
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: tomli; python_version < '3.11'
 Provides-Extra: full
-License-File: LICENSE
+Requires-Dist: pyyaml; extra == 'full'
+Requires-Dist: rich-click; extra == 'full'
+Provides-Extra: yaml
+Requires-Dist: pyyaml; extra == 'yaml'
+Description-Content-Type: text/markdown
 
 ![Build](https://github.com/Neoteroi/essentials-configuration/workflows/Build/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/essentials-configuration.svg)](https://pypi.python.org/pypi/essentials-configuration)
 [![versions](https://img.shields.io/pypi/pyversions/essentials-configuration.svg)](https://github.com/Neoteroi/essentials-configuration)
 [![codecov](https://codecov.io/gh/Neoteroi/essentials-configuration/branch/main/graph/badge.svg?token=VzAnusWIZt)](https://codecov.io/gh/Neoteroi/essentials-configuration)
 [![license](https://img.shields.io/github/license/Neoteroi/essentials-configuration.svg)](https://github.com/Neoteroi/essentials-configuration/blob/main/LICENSE)
 
@@ -287,16 +292,16 @@
 
 The library provides a strategy to handle secrets during local development,
 storing them into the user folder.
 
 The following example shows how secrets can be configured for a project:
 
 ```bash
-config secrets init
-config secrets set "Foo" "Some secret value"
+config settings init
+config settings set "Foo" "Some secret value"
 ```
 
 Secrets are organized by project, and the project information is obtained from
 `pyproject.toml` files (from the `project.name` property). If `pyproject.toml`
 file does not exist, one is generated automatically with a random name.
 
 ---
@@ -321,37 +326,21 @@
 stored in unencrypted form in the user's folder.
 
 Production apps should use dedicated services to handle secrets, like
 [Azure Key Vault](https://docs.microsoft.com/en-us/azure/key-vault/general/basic-concepts),
 [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/), or similar services.
 For Azure Key Vault, an implementation is provided in [essentials-configuration-keyvault](https://github.com/Neoteroi/essentials-configuration-keyvault).
 
-## Handling user secrets
+## Handling user settings
 
-User secrets can be handled using the provided `config` CLI.
+User settings (stored in the user's folder) can be handled using the provided `config` CLI.
 
-```
-config secrets
-Usage: config secrets [OPTIONS] COMMAND [ARGS]...
+![Rich CLI](https://gist.githubusercontent.com/RobertoPrevato/38a0598b515a2f7257c614938843b99b/raw/a83facd6eb4ddc1dc8552a5f5f073278470010c2/config-settings-rich-cli.png)
 
-  Commands to handle user secrets, for local development.
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  del       Delete a secret for a project, by key.
-  get       Get a secret in a user file by key.
-  info      Show information about secrets for a project.
-  init      Initialize user secrets for the current folder.
-  list      List all projects configured for secrets stored in the user...
-  set       Set a secret in a user file by key and value.
-  set-many  Set many secrets read from a JSON file passed through stdin.
-  show      Show the local secrets for a project.
-```
+These settings can be useful to store secrets and other values during local development, or in general when working with desktop applications.
 
 ### Overriding nested values
 
 It is possible to override nested values by environment variables or
 dictionary keys using the following notation for sub properties:
 
 * keys separated by colon ":", such as `a:d:e`
```

### Comparing `essentials-configuration-2.0.2/README.md` & `essentials_configuration-2.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -265,16 +265,16 @@
 
 The library provides a strategy to handle secrets during local development,
 storing them into the user folder.
 
 The following example shows how secrets can be configured for a project:
 
 ```bash
-config secrets init
-config secrets set "Foo" "Some secret value"
+config settings init
+config settings set "Foo" "Some secret value"
 ```
 
 Secrets are organized by project, and the project information is obtained from
 `pyproject.toml` files (from the `project.name` property). If `pyproject.toml`
 file does not exist, one is generated automatically with a random name.
 
 ---
@@ -299,37 +299,21 @@
 stored in unencrypted form in the user's folder.
 
 Production apps should use dedicated services to handle secrets, like
 [Azure Key Vault](https://docs.microsoft.com/en-us/azure/key-vault/general/basic-concepts),
 [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/), or similar services.
 For Azure Key Vault, an implementation is provided in [essentials-configuration-keyvault](https://github.com/Neoteroi/essentials-configuration-keyvault).
 
-## Handling user secrets
+## Handling user settings
 
-User secrets can be handled using the provided `config` CLI.
+User settings (stored in the user's folder) can be handled using the provided `config` CLI.
 
-```
-config secrets
-Usage: config secrets [OPTIONS] COMMAND [ARGS]...
-
-  Commands to handle user secrets, for local development.
+![Rich CLI](https://gist.githubusercontent.com/RobertoPrevato/38a0598b515a2f7257c614938843b99b/raw/a83facd6eb4ddc1dc8552a5f5f073278470010c2/config-settings-rich-cli.png)
 
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  del       Delete a secret for a project, by key.
-  get       Get a secret in a user file by key.
-  info      Show information about secrets for a project.
-  init      Initialize user secrets for the current folder.
-  list      List all projects configured for secrets stored in the user...
-  set       Set a secret in a user file by key and value.
-  set-many  Set many secrets read from a JSON file passed through stdin.
-  show      Show the local secrets for a project.
-```
+These settings can be useful to store secrets and other values during local development, or in general when working with desktop applications.
 
 ### Overriding nested values
 
 It is possible to override nested values by environment variables or
 dictionary keys using the following notation for sub properties:
 
 * keys separated by colon ":", such as `a:d:e`
```

### Comparing `essentials-configuration-2.0.2/config/common/__init__.py` & `essentials_configuration-2.0.3/config/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from config.errors import ConfigurationOverrideError
 
 T = TypeVar("T")
 
 
 def apply_key_value(obj, key, value):
-    key = key.strip("_:")  # remove special characters from both ends
-    for token in (":", "__"):
+    key = key.strip("_:.")  # remove special characters from both ends
+    for token in (":", "__", "."):
         if token in key:
             parts = key.split(token)
 
             sub_property = obj
             last_part = parts[-1]
             for part in parts[:-1]:
                 if isinstance(sub_property, abc.MutableSequence):
```

### Comparing `essentials-configuration-2.0.2/config/common/files.py` & `essentials_configuration-2.0.3/config/common/files.py`

 * *Files identical despite different names*

### Comparing `essentials-configuration-2.0.2/config/env/__init__.py` & `essentials_configuration-2.0.3/config/env/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials-configuration-2.0.2/config/ini/__init__.py` & `essentials_configuration-2.0.3/config/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials-configuration-2.0.2/config/secrets/__init__.py` & `essentials_configuration-2.0.3/config/user/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-This module provides support for user secrets stored locally, for development.
+This module provides support for user settings stored locally, for development, or for
+CLIs.
 """
 from pathlib import Path
 from typing import Any, Dict, Optional
 from uuid import uuid4
 
 from config.common import ConfigurationSource
 from config.json import JSONFile
@@ -26,37 +27,39 @@
             return data["project"]["name"]
         except KeyError:  # pragma: no cover
             pass
 
     return uuid4().hex
 
 
-class UserSecrets(ConfigurationSource):
+class UserSettings(ConfigurationSource):
     """
-    Reads values stored in a file inside the user's folder.
+    This class reads settings stored in a file inside the user's folder.
     """
 
     def __init__(
         self, project_name: Optional[str] = None, optional: bool = True
     ) -> None:
         """
-        Configures an instance of UserSecrets that obtains values from a project file
+        Configures an instance of UserSettings that obtains values from a project file
         stored in the user's folder. If a project name is not provided, it is
         automatically inferred from a `pyproject.toml` file, if present, otherwise a
         random value is generated.
         """
         if not project_name:
             project_name = get_project_name()
         self.project_name = project_name
-        self._secrets_file_path = self.get_base_folder() / project_name / "secrets.json"
-        self._source = JSONFile(self.secrets_file_path, optional)
+        self._settings_file_path = (
+            self.get_base_folder() / project_name / "settings.json"
+        )
+        self._source = JSONFile(self.settings_file_path, optional)
 
     def get_base_folder(self) -> Path:
         return Path.home() / ".neoteroi" / "ec"
 
     @property
-    def secrets_file_path(self) -> Path:
-        return self._secrets_file_path
+    def settings_file_path(self) -> Path:
+        return self._settings_file_path
 
     def get_values(self) -> Dict[str, Any]:
         """Returns the values read from this source."""
         return self._source.get_values()
```

### Comparing `essentials-configuration-2.0.2/config/toml/__init__.py` & `essentials_configuration-2.0.3/config/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials-configuration-2.0.2/config/yaml/__init__.py` & `essentials_configuration-2.0.3/config/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials-configuration-2.0.2/pyproject.toml` & `essentials_configuration-2.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "essentials-configuration"
-version = "2.0.2"
+version = "2.0.3"
 authors = [{ name = "Roberto Prevato", email = "roberto.prevato@gmail.com" }]
 description = "Implementation of key-value pair based configuration for Python applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-keywords = ["configuration", "root", "management", "strategy"]
+keywords = ["configuration", "root", "management", "strategy", "settings"]
 
 dependencies = ["tomli; python_version < '3.11'", "python-dotenv~=1.0.0"]
 
 [project.optional-dependencies]
 yaml = ["PyYAML"]
-full = ["PyYAML", "click"]
+full = ["PyYAML", "rich-click"]
 
 [project.scripts]
 config = "config.cli.main:main"
 
-[tool.setuptools.package-data]
-config = ["*/py.typed"]
+[tool.hatch.build.targets.wheel]
+packages = ["config"]
+
+[tool.hatch.build.targets.sdist]
+exclude = ["tests"]
+
+[tool.hatch.build]
+only-packages = true
 
 [project.urls]
 "Homepage" = "https://github.com/Neoteroi/essentials-configuration"
 "Bug Tracker" = "https://github.com/Neoteroi/essentials-configuration/issues"
```

