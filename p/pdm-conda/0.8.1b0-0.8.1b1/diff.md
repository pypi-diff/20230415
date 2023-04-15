# Comparing `tmp/pdm_conda-0.8.1b0.tar.gz` & `tmp/pdm_conda-0.8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.8.1b0.tar", last modified: Fri Apr 14 22:27:37 2023, max compression
+gzip compressed data, was "pdm_conda-0.8.1b1.tar", last modified: Sat Apr 15 17:38:01 2023, max compression
```

## Comparing `pdm_conda-0.8.1b0.tar` & `pdm_conda-0.8.1b1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b0/LICENSE
--rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b0/README.md
--rw-r--r--   0        0        0     1962 2023-04-14 22:27:36.800395 pdm_conda-0.8.1b0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-10 22:15:32.251560 pdm_conda-0.8.1b0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    10887 2023-04-14 22:23:27.447157 pdm_conda-0.8.1b0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2162 2023-04-14 22:24:14.370967 pdm_conda-0.8.1b0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1717 2023-04-14 19:31:18.644281 pdm_conda-0.8.1b0/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3234 2023-04-09 20:29:55.609532 pdm_conda-0.8.1b0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0     9046 2023-04-09 20:29:55.611231 pdm_conda-0.8.1b0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5740 2023-04-09 20:29:55.613268 pdm_conda-0.8.1b0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b1/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b1/README.md
+-rw-r--r--   0        0        0     2021 2023-04-15 17:38:01.598644 pdm_conda-0.8.1b1/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-15 17:37:37.531424 pdm_conda-0.8.1b1/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b1/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b1/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    11223 2023-04-15 17:34:37.904070 pdm_conda-0.8.1b1/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b1/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b1/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2162 2023-04-14 22:24:14.370967 pdm_conda-0.8.1b1/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b1/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b1/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b1/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-15 01:10:11.358619 pdm_conda-0.8.1b1/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b1/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3234 2023-04-09 20:29:55.609532 pdm_conda-0.8.1b1/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b1/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    10806 2023-04-15 17:37:15.580889 pdm_conda-0.8.1b1/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b1/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b1/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b1/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b1/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     5455 2023-04-15 17:36:44.693219 pdm_conda-0.8.1b1/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b1/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b1/PKG-INFO
```

### Comparing `pdm_conda-0.8.1b0/LICENSE` & `pdm_conda-0.8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/README.md` & `pdm_conda-0.8.1b1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/pyproject.toml` & `pdm_conda-0.8.1b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,37 +20,43 @@
 dynamic = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "pdm~=2.4.0",
-    "requests>=2.28.1",
+    "prefect",
 ]
-version = "0.8.1b0"
+version = "0.8.1b1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
 
 [project.entry-points.pdm]
 conda = "pdm_conda:main"
 
-[tool.pdm.dev-dependencies]
-dev = [
-    "pytest>=7.2.0",
-    "pytest-mock>=3.10.0",
-    "pytest-cov>=4.0.0",
-    "pytest-random-num>=1.0.13",
-    "responses>=0.22.0",
+[tool.pdm.conda]
+runner = "micromamba"
+channels = [
+    "conda-forge",
 ]
+as-default-manager = true
+excludes = [
+    "streamlink",
+    "moto",
+    "python-telegram-bot-raw",
+    "fastapi-crudrouter",
+    "ormar",
+    "databases",
+]
+batched-commands = true
 
 [tool.pdm.version]
 source = "file"
 path = "src/pdm_conda/__init__.py"
 
 [tool.pdm.build]
 package-dir = "src"
```

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/__init__.py` & `pdm_conda-0.8.1b1/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.8.1b0"
+__version__ = "0.8.1b1"
```

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.8.1b1/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/conda.py` & `pdm_conda-0.8.1b1/src/pdm_conda/conda.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,34 +76,45 @@
             msg += process.stderr
         if environment:
             msg += f"\n{environment}"
         raise RequirementError(msg) from e
     return response
 
 
+@lru_cache(maxsize=None)
+def _get_channel_sorter(platform: str, channels: tuple[str]) -> ChannelSorter:
+    """
+    Get channel sorter
+    :param channels: list of conda channels used to determine priority
+    :param platform: env platform
+    :return: channel sorter
+    """
+    return ChannelSorter(platform, channels)
+
+
 def _sort_packages(packages: list[dict], channels: Iterable[str], platform: str) -> Iterable[dict]:
     """
     Sort packages following mamba specification
     (https://mamba.readthedocs.io/en/latest/advanced_usage/package_resolution.html).
     :param packages: list of conda packages
     :param channels: list of conda channels used to determine priority
     :param platform: env platform
     :return: sorted conda packages
     """
     if len(packages) <= 1:
         return packages
 
-    channels_sorter = ChannelSorter(platform, channels)
+    channels_sorter = _get_channel_sorter(platform, tuple(channels))
 
     def get_preference(package):
         return (
             not package.get("track_feature", ""),
-            -channels_sorter.get_priority(package["channel"]),
             Version(parse_conda_version(package["version"], inverse=package.get("name", "") == "openssl")),
             package.get("build_number", 0),
+            -channels_sorter.get_priority(package["channel"]),
             package.get("timestamp", 0),
         )
 
     return sorted(packages, key=get_preference, reverse=True)
 
 
 @lru_cache(maxsize=None)
```

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.8.1b1/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.8.1b1/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/mapping.py` & `pdm_conda-0.8.1b1/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/conda.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/conda.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,35 +14,35 @@
                 self.add_defaults(root)
 
     def get_root(self, channel: str) -> str:
         return channel.split("/")[0]
 
     def add_defaults(self, root: str):
         for channel in [f"{root}/{self.platform}", rf"{root}/.*", f"{root}/noarch"]:
-            self.add_channel(channel)
+            self.add_channel(channel, allow_fuzzy=not channel.endswith("noarch"))
 
     def get_variants(self, root: str):
         # add parent channel priority
         if root not in self._tree:
             self._priority[root] = 1000 * len(self._tree)
             self._tree[root] = []
 
         return self._tree[root]
 
-    def add_channel(self, channel: str):
+    def add_channel(self, channel: str, allow_fuzzy=True):
         root = self.get_root(channel)
         if channel not in self._priority:
             for c in (variants := self.get_variants(root)):
-                if re.match(c, channel):
+                if c == channel or (allow_fuzzy and re.match(c, channel)):
                     self._priority[channel] = self._priority[c]
                     # then fuzzy match
                     if c != channel:
                         self._priority[c] += 1
                     break
             # couldn't find priority in saved variant
             if channel not in self._priority:
-                self._priority[channel] = self._priority[root] + len(variants)
+                self._priority[channel] = self._priority[root] + len(variants) * 10
                 variants.append(channel)
 
     def get_priority(self, channel: str) -> int:
         self.add_channel(channel)
         return self._priority[channel]
```

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/config.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/environment.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,14 +92,48 @@
             _compatible &= re.match(rf"{self.build_string.replace('*', r'.*')}", build_string) is not None
         return (
             _compatible
             and self.conda_name == requirement.conda_name
             and all(self.specifier.contains(s.version) for s in requirement.specifier)
         )
 
+    def merge(self, requirement: Requirement) -> "CondaRequirement":
+        """
+        Merge with other requirement to get more specific
+        :param requirement: other requirement
+        :return: merged requirement
+        """
+        _req = copy(self)
+        _req.specifier &= requirement.specifier
+        if isinstance(requirement, CondaRequirement):
+            _req.channel = requirement.channel
+            _req.version_mapping.update(requirement.version_mapping)
+            if not _req.build_string:
+                _req.build_string = requirement.build_string
+            elif requirement.build_string and requirement.build_string != _req.build_string:
+                # test compatibility
+                _compatible = dict()
+                build_strings = [requirement.build_string, _req.build_string]
+                for build_string in build_strings:
+                    if build_string not in _compatible:
+                        _compatible[build_string] = all(
+                            re.match(build_string.replace("*", r".*"), bs)
+                            or re.match(bs.replace("*", r".*"), build_string)
+                            for bs in build_strings
+                            if bs != build_string
+                        )
+                # if all incompatibles then keep fake build string to force failing search
+                if not all(_compatible.values()):
+                    build_string = f"{_req.build_string}{requirement.build_string}"
+                else:
+                    # tries to find the most specific build string
+                    build_string = min(build_strings, key=lambda x: (-len(x.replace("*", "")), x.count("*")))
+                _req.build_string = build_string
+        return _req
+
 
 def as_conda_requirement(requirement: NamedRequirement | CondaRequirement) -> Requirement:
     if isinstance(requirement, NamedRequirement) and not isinstance(requirement, CondaRequirement):
         req = copy(requirement)
         req.marker = None
         req.name = req.conda_name
         conda_req = parse_requirement(f"conda:{req.as_line()}")
```

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/models/setup.py` & `pdm_conda-0.8.1b1/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/project.py` & `pdm_conda-0.8.1b1/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.8.1b1/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/resolvers.py` & `pdm_conda-0.8.1b1/src/pdm_conda/resolvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from copy import copy
 from dataclasses import dataclass, field
 
 from packaging.version import Version
-from resolvelib.resolvers import _build_result  # type: ignore
-from resolvelib.resolvers import RequirementInformation, Resolution, Resolver
+from resolvelib.resolvers import (  # type: ignore
+    RequirementInformation,
+    Resolution,
+    Resolver,
+    _build_result,
+)
 
 from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.models.environment import CondaEnvironment
 from pdm_conda.models.requirements import CondaRequirement, as_conda_requirement
 
 
 @dataclass
@@ -41,19 +44,16 @@
         self._states.append(state)
 
     def _add_to_criteria(self, criteria, requirement, parent):
         _req = requirement
         if self._is_conda_environment:
             constrains = self.state.constrains
             if (constrain := constrains.get(requirement.conda_name, None)) is not None:
-                _req = copy(constrain)
-                _req.specifier &= requirement.specifier
-                _req.version_mapping.update(getattr(requirement, "version_mapping", dict()))
-                if isinstance(requirement, CondaRequirement):
-                    _req.channel = requirement.channel
+                _req = constrain.merge(requirement)
+
             identifier = self._p.identify(_req)
             if criterion := criteria.get(identifier):
                 excluded = self._p.repository.environment.project.conda_config.excludes
                 if isinstance(_req, CondaRequirement):
                     # if conda requirement but other not conda requirement and excluded
                     # then transform to named requirement
                     if any(
```

### Comparing `pdm_conda-0.8.1b0/src/pdm_conda/utils.py` & `pdm_conda-0.8.1b1/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b0/PKG-INFO` & `pdm_conda-0.8.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.8.1b0
+Version: 0.8.1b1
 Summary:  A PDM plugin to install project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -27,16 +27,15 @@
         SOFTWARE.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Homepage, https://github.com/macro128/pdm-conda
 Project-URL: Changelog, https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md
 Requires-Python: >=3.10
-Requires-Dist: pdm~=2.4.0
-Requires-Dist: requests>=2.28.1
+Requires-Dist: prefect
 Description-Content-Type: text/markdown
 
 # pdm-conda
 
 A PDM plugin to install project dependencies with Conda.
 
 ## Configuration
```

