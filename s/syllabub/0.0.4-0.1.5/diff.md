# Comparing `tmp/syllabub-0.0.4.tar.gz` & `tmp/syllabub-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syllabub-0.0.4.tar", last modified: Wed Mar 29 12:11:04 2023, max compression
+gzip compressed data, was "syllabub-0.1.5.tar", last modified: Sat Apr 15 21:08:03 2023, max compression
```

## Comparing `syllabub-0.0.4.tar` & `syllabub-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    34020 2023-03-29 12:06:29.085182 syllabub-0.0.4/COPYING
--rw-r--r--   0        0        0    34020 2022-09-20 10:56:30.499965 syllabub-0.0.4/LICENSES/AGPL-3.0-or-later.txt
--rw-r--r--   0        0        0    17023 2022-11-22 13:53:30.786895 syllabub-0.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0    21305 2022-11-22 13:53:30.786895 syllabub-0.0.4/LICENSES/CC-BY-SA-3.0.txt
--rw-r--r--   0        0        0    18375 2023-03-23 19:07:45.171020 syllabub-0.0.4/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2022-09-20 10:56:30.835967 syllabub-0.0.4/LICENSES/CC0-1.0.txt
--rwxr-xr-x   0        0        0      119 2023-03-29 12:06:29.085182 syllabub-0.0.4/LICENSES/LicenseRef-DCO-1.1-license.txt
--rw-r--r--   0        0        0     3439 2023-03-29 12:10:54.868869 syllabub-0.0.4/README.md
--rw-r--r--   0        0        0      854 2023-03-29 12:11:04.576850 syllabub-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/__init__.py
--rw-r--r--   0        0        0      143 2023-03-29 12:10:26.916921 syllabub-0.0.4/src/syllabub/builtin/.gitignore.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/.gitignore.mustache.license
--rw-r--r--   0        0        0     5488 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONDUCT.COVENANT
--rw-r--r--   0        0        0      136 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONDUCT.COVENANT.license
--rw-r--r--   0        0        0     8579 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONDUCT.UBUNTU
--rw-r--r--   0        0        0      134 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONDUCT.UBUNTU.license
--rwxr-xr-x   0        0        0     1421 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONTRIBUTING.DCO
--rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF
--rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF.license
--rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/CONTRIBUTING.DCO.license
--rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt
--rwxr-xr-x   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt.license
--rw-r--r--   0        0        0     1000 2023-03-29 12:10:26.916921 syllabub-0.0.4/src/syllabub/builtin/Makefile.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/Makefile.mustache.license
--rw-r--r--   0        0        0     1374 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/README.md.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/README.md.mustache.license
--rw-r--r--   0        0        0        0 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/__init__.py
--rw-r--r--   0        0        0      174 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/cli.py.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/cli.py.mustache.license
--rw-r--r--   0        0        0    10442 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/logo.png
--rw-r--r--   0        0        0      193 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/logo.png.license
--rw-r--r--   0        0        0       87 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/pdm.lock.license.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/pdm.lock.license.mustache.license
--rw-r--r--   0        0        0      739 2023-03-29 12:10:26.916921 syllabub-0.0.4/src/syllabub/builtin/pyproject.toml.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/pyproject.toml.mustache.license
--rw-r--r--   0        0        0      197 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/test_cli.py.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.0.4/src/syllabub/builtin/test_cli.py.mustache.license
--rw-r--r--   0        0        0     2722 2023-03-23 20:59:58.039494 syllabub-0.0.4/src/syllabub/cli.py
--rw-r--r--   0        0        0     5018 2023-03-23 20:59:58.039494 syllabub-0.0.4/src/syllabub/metadata.py
--rw-r--r--   0        0        0      232 2023-03-23 19:07:45.179020 syllabub-0.0.4/tests/test_cli.py
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 syllabub-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34020 2023-04-15 20:57:16.685095 syllabub-0.1.5/COPYING
+-rw-r--r--   0        0        0    34020 2022-09-20 10:56:30.499965 syllabub-0.1.5/LICENSES/AGPL-3.0-or-later.txt
+-rw-r--r--   0        0        0    17023 2022-11-22 13:53:30.786895 syllabub-0.1.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0    21305 2022-11-22 13:53:30.786895 syllabub-0.1.5/LICENSES/CC-BY-SA-3.0.txt
+-rw-r--r--   0        0        0    18375 2023-03-23 19:07:45.171020 syllabub-0.1.5/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2022-09-20 10:56:30.835967 syllabub-0.1.5/LICENSES/CC0-1.0.txt
+-rwxr-xr-x   0        0        0      119 2023-04-15 20:57:16.685095 syllabub-0.1.5/LICENSES/LicenseRef-DCO-1.1-license.txt
+-rw-r--r--   0        0        0     3500 2023-04-15 21:07:50.942381 syllabub-0.1.5/README.md
+-rw-r--r--   0        0        0      946 2023-04-15 21:08:03.222410 syllabub-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:16:16.766703 syllabub-0.1.5/src/syllabub/__init__.py
+-rw-r--r--   0        0        0      145 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/builtin/.gitignore.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/.gitignore.mustache.license
+-rw-r--r--   0        0        0     5488 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.COVENANT
+-rw-r--r--   0        0        0      136 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.COVENANT.license
+-rw-r--r--   0        0        0     8579 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.UBUNTU
+-rw-r--r--   0        0        0      134 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.UBUNTU.license
+-rwxr-xr-x   0        0        0     1421 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO
+-rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF
+-rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF.license
+-rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO.license
+-rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt
+-rwxr-xr-x   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt.license
+-rw-r--r--   0        0        0     1000 2023-03-29 12:10:26.916921 syllabub-0.1.5/src/syllabub/builtin/Makefile.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/Makefile.mustache.license
+-rw-r--r--   0        0        0     1374 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/builtin/README.md.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/README.md.mustache.license
+-rw-r--r--   0        0        0        0 2023-04-03 16:49:55.680967 syllabub-0.1.5/src/syllabub/builtin/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/cli.py.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/cli.py.mustache.license
+-rw-r--r--   0        0        0    10442 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/logo.png
+-rw-r--r--   0        0        0      193 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/logo.png.license
+-rw-r--r--   0        0        0       87 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/pdm.lock.license.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/pdm.lock.license.mustache.license
+-rw-r--r--   0        0        0      810 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/builtin/pyproject.toml.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/pyproject.toml.mustache.license
+-rw-r--r--   0        0        0      197 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/test_cli.py.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/test_cli.py.mustache.license
+-rw-r--r--   0        0        0     2686 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/cli.py
+-rw-r--r--   0        0        0     5180 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/metadata.py
+-rw-r--r--   0        0        0      232 2023-03-23 19:07:45.179020 syllabub-0.1.5/tests/test_cli.py
+-rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 syllabub-0.1.5/PKG-INFO
```

### Comparing `syllabub-0.0.4/COPYING` & `syllabub-0.1.5/COPYING`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/LICENSES/AGPL-3.0-or-later.txt` & `syllabub-0.1.5/LICENSES/AGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/LICENSES/CC-BY-4.0.txt` & `syllabub-0.1.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/LICENSES/CC-BY-SA-3.0.txt` & `syllabub-0.1.5/LICENSES/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/LICENSES/CC-BY-SA-4.0.txt` & `syllabub-0.1.5/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/LICENSES/CC0-1.0.txt` & `syllabub-0.1.5/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/README.md` & `syllabub-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,42 +3,44 @@
 Keep Python project conventions up-to-date and worry less about trifling
 matters. 🍰
 
 ## Status
 
 Unstable prototype. Please wear goggles.
 
-TODO:
-
-- Replace with pdm scripts: https://pdm.fming.dev/latest/usage/scripts/
-- Just use https://pyscaffold.org
-- Add Gherkin, Mermaid, FAQ?
-
 ## Background
 
-High-quality software projects demand more effort to contribute. Syllabub makes
-simplifying assumptions and toolchain/workflow decisions, so that:
+High-quality software projects demand more contribution effort. Syllabub makes
+assumptions so that:
 
 - maintainers make fewer, less frequent project-level decisions
 - contributors require less up-front learning, but can dive into detail when
-  required
-- syllabub can be used as a bolt-on, not a dependency (maintainers can declare
-  it as a dependency if they prefer)
+    required
+- Syllabub is not required as a dependency
+
+## Alternatives
+
+Other Python
+[scaffolding tools](<https://en.wikipedia.org/wiki/Scaffold_(programming)>)
+include:
 
-## Usage (syllabub tool)
+- [Cookiecutter](https://www.cookiecutter.io)
+- [Copier](https://copier.readthedocs.io)
+- [PyScaffold](https://pyscaffold.org)
+
+These tools are general-purpose, allowing a maintainer to define an entire
+project template. Syllabub has fewer options and uses a built-in template.
+
+## Usage
 
 - Set values in `pyproject.toml`.
 - Invoke `syllabub` to overwrite boilerplate files.
-- Review diff.
+- Review and modify diff.
 - Commit changes.
 
-## Usage (syllabub workflow)
-
-See "Development environment" below.
-
 ## Use case scenarios
 
 ```gherkin
 Feature: Syllabub Project Generation
 
   Scenario: Create a new Syllabub-style project
```

### Comparing `syllabub-0.0.4/pyproject.toml` & `syllabub-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 [project]
 name = "syllabub"
-version = "0.0.4"
 description = "Keep Python project conventions up-to-date and worry less about trifling matters. 🍰"
 authors = [
     { name = "David Seaward", email = "david@librem.one" },
 ]
 dependencies = [
     "chevron>=0.14.0",
     "tomli>=2.0.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
+dynamic = []
+version = "0.1.5"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.optional-dependencies]
 
 [project.scripts]
 syllabub = "syllabub.cli:invoke"
 
+[project.urls]
+Source = "https://gitlab.com/lfdo/syllabub"
+Project = "https://lofidevops.neocities.org"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "carmine>=0.0.3",
 ]
 
+[tool.pdm.version]
+source = "scm"
+
 [tool.syllabub.project]
 conduct = "contributor-covenant-2.1"
 copyright = "Copyright 2022 David Seaward and contributors"
 origin = "DCO-1.1-git-signoff"
-sbom = "reuse spdx"
 title = "Syllabub project bolt-on"
-url = "https://lofidevops.neocities.org"
```

### Comparing `syllabub-0.0.4/src/syllabub/builtin/CONDUCT.COVENANT` & `syllabub-0.1.5/src/syllabub/builtin/CONDUCT.COVENANT`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/src/syllabub/builtin/CONDUCT.UBUNTU` & `syllabub-0.1.5/src/syllabub/builtin/CONDUCT.UBUNTU`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/src/syllabub/builtin/CONTRIBUTING.DCO` & `syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/src/syllabub/builtin/Makefile.mustache` & `syllabub-0.1.5/src/syllabub/builtin/Makefile.mustache`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/src/syllabub/builtin/README.md.mustache` & `syllabub-0.1.5/src/syllabub/builtin/README.md.mustache`

 * *Files 10% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 publish : Upload build artefacts to PyPI.
 ```
 
 # Sharing and contributions
 
 ```
 {{ full_title }}
-{{ url }}
+{{ url_project }}
 {{ copyright }}
 SPDX-License-Identifier: {{ spdx_identifier }}
 ```
 
 Shared under {{ spdx_identifier }}. We adhere to the {{ conduct }}, and
 certify origin per {{ origin }}. Contributions under the
 same terms are welcome.
 
 Submit security and conduct issues as private tickets. Sign commits with
-`{{ origin_command }}`. For a software bill of materials run `{{ sbom_command }}`. For
+`{{ origin_command }}`. For a software bill of materials run `reuse spdx`. For
 more details see CONDUCT, COPYING and CONTRIBUTING.
```

### Comparing `syllabub-0.0.4/src/syllabub/builtin/logo.png` & `syllabub-0.1.5/src/syllabub/builtin/logo.png`

 * *Files identical despite different names*

### Comparing `syllabub-0.0.4/src/syllabub/cli.py` & `syllabub-0.1.5/src/syllabub/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 import logging
 import os.path
 import shutil
 
 from syllabub.metadata import Project, validate_environment
 
 
-def version():
-    return "0.0.2"
-
-
 def invoke():
     # retrieve available data from pyproject.toml
     validate_environment()
     project = Project()
     project.load()
     project.clean()
```

### Comparing `syllabub-0.0.4/src/syllabub/metadata.py` & `syllabub-0.1.5/src/syllabub/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import shutil
 import sys
 from importlib import resources
 
 import chevron
 import tomli
 
+import syllabub
+
 LOOKUP = {
     "DCO-1.1-git-signoff": {
         "text": "DCO 1.1 with a signed-off-by line",
         "command": "git commit --signoff",
     },
     "DCO-1.1-git-gpg-sign": {
         "text": "DCO 1.1 with a GPG signature",
@@ -26,15 +28,19 @@
 
 def bad_key_returns_default(value, default):
     """Decorated function will avoid KeyErrors and instead return a default value."""
 
     def decorator(function):
         def wrapper(*args, **kwargs):
             try:
-                return function(*args, **kwargs)
+                result = function(*args, **kwargs)
+                if result in ["UNKNOWN", "MISSING"]:
+                    raise KeyError("Unknown or missing value.")
+                else:
+                    return result
             except KeyError:
                 logging.error(f"{value} not found, using {default}")
                 return default
 
         return wrapper
 
     return decorator
@@ -73,15 +79,15 @@
         for path in ["COPYING", "LICENSE"]:
             try:
                 os.remove(path)
             except OSError:
                 pass  # skip missing files
 
     @property
-    @bad_key_returns_default("Project name", "new-project")
+    @bad_key_returns_default("Project name", "UNKNOWN")
     def short_name(self):
         return self._pyproject["project"]["name"]
 
     @property
     def full_title(self):
         try:
             return self._pyproject["tool"]["syllabub"]["project"]["title"]
@@ -124,22 +130,22 @@
 
     @property
     @bad_key_returns_default("Copyright", "MISSING")
     def copyright(self):
         return self._pyproject["tool"]["syllabub"]["project"]["copyright"]
 
     @property
-    @bad_key_returns_default("Bill of materials", "reuse sbom")
-    def sbom_command(self):
-        return self._pyproject["tool"]["syllabub"]["project"]["sbom"]
+    @bad_key_returns_default("Project URL", "MISSING")
+    def url_project(self):
+        return self._pyproject["project"]["urls"]["Project"]
 
     @property
-    @bad_key_returns_default("URL", "https://example.com")
-    def url(self):
-        return self._pyproject["tool"]["syllabub"]["project"]["url"]
+    @bad_key_returns_default("Source URL", "MISSING")
+    def url_source(self):
+        return self._pyproject["project"]["urls"]["Source"]
 
     @property
     @bad_key_returns_default("License", "MISSING")
     def spdx_identifier(self):
         return self._pyproject["project"]["license"]["text"]
 
     @property
```

### Comparing `syllabub-0.0.4/PKG-INFO` & `syllabub-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: syllabub
-Version: 0.0.4
+Version: 0.1.5
 Summary: Keep Python project conventions up-to-date and worry less about trifling matters. 🍰
 Author-Email: David Seaward <david@librem.one>
 License: AGPL-3.0-or-later
+Project-URL: Source, https://gitlab.com/lfdo/syllabub
+Project-URL: Project, https://lofidevops.neocities.org
 Requires-Python: >=3.10
 Requires-Dist: chevron>=0.14.0
 Requires-Dist: tomli>=2.0.1
 Description-Content-Type: text/markdown
 
 # Syllabub project bolt-on
 
 Keep Python project conventions up-to-date and worry less about trifling
 matters. 🍰
 
 ## Status
 
 Unstable prototype. Please wear goggles.
 
-TODO:
-
-- Replace with pdm scripts: https://pdm.fming.dev/latest/usage/scripts/
-- Just use https://pyscaffold.org
-- Add Gherkin, Mermaid, FAQ?
-
 ## Background
 
-High-quality software projects demand more effort to contribute. Syllabub makes
-simplifying assumptions and toolchain/workflow decisions, so that:
+High-quality software projects demand more contribution effort. Syllabub makes
+assumptions so that:
 
 - maintainers make fewer, less frequent project-level decisions
 - contributors require less up-front learning, but can dive into detail when
-  required
-- syllabub can be used as a bolt-on, not a dependency (maintainers can declare
-  it as a dependency if they prefer)
+    required
+- Syllabub is not required as a dependency
+
+## Alternatives
+
+Other Python
+[scaffolding tools](<https://en.wikipedia.org/wiki/Scaffold_(programming)>)
+include:
 
-## Usage (syllabub tool)
+- [Cookiecutter](https://www.cookiecutter.io)
+- [Copier](https://copier.readthedocs.io)
+- [PyScaffold](https://pyscaffold.org)
+
+These tools are general-purpose, allowing a maintainer to define an entire
+project template. Syllabub has fewer options and uses a built-in template.
+
+## Usage
 
 - Set values in `pyproject.toml`.
 - Invoke `syllabub` to overwrite boilerplate files.
-- Review diff.
+- Review and modify diff.
 - Commit changes.
 
-## Usage (syllabub workflow)
-
-See "Development environment" below.
-
 ## Use case scenarios
 
 ```gherkin
 Feature: Syllabub Project Generation
 
   Scenario: Create a new Syllabub-style project
```

