# Comparing `tmp/pdm_conda-0.8.0b0.tar.gz` & `tmp/pdm_conda-0.8.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.8.0b0.tar", last modified: Sun Apr  9 20:06:47 2023, max compression
+gzip compressed data, was "pdm_conda-0.8.1b0.tar", last modified: Fri Apr 14 22:27:37 2023, max compression
```

## Comparing `pdm_conda-0.8.0b0.tar` & `pdm_conda-0.8.1b0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.0b0/LICENSE
--rw-r--r--   0        0        0     4827 2023-04-09 20:05:34.908555 pdm_conda-0.8.0b0/README.md
--rw-r--r--   0        0        0     1927 2023-04-09 20:06:47.733625 pdm_conda-0.8.0b0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-09 20:06:03.212447 pdm_conda-0.8.0b0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.0b0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-09 20:03:17.811169 pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-09 18:24:04.763264 pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 18:47:54.197518 pdm_conda-0.8.0b0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    11001 2023-04-09 20:02:13.031492 pdm_conda-0.8.0b0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.0b0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 19:02:43.417017 pdm_conda-0.8.0b0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2130 2023-04-09 20:03:17.811387 pdm_conda-0.8.0b0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.0b0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.0b0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.0b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6776 2023-04-09 18:57:52.527833 pdm_conda-0.8.0b0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     7145 2023-04-09 20:05:09.458459 pdm_conda-0.8.0b0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3234 2023-04-09 18:57:09.987590 pdm_conda-0.8.0b0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3863 2023-04-09 20:03:17.811832 pdm_conda-0.8.0b0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0     9046 2023-04-09 18:57:52.528315 pdm_conda-0.8.0b0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-04 03:59:08.192367 pdm_conda-0.8.0b0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     7518 2023-04-09 20:03:17.812051 pdm_conda-0.8.0b0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.0b0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.0b0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5740 2023-04-09 20:03:17.812247 pdm_conda-0.8.0b0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.0b0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 pdm_conda-0.8.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b0/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b0/README.md
+-rw-r--r--   0        0        0     1962 2023-04-14 22:27:36.800395 pdm_conda-0.8.1b0/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-10 22:15:32.251560 pdm_conda-0.8.1b0/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b0/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b0/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    10887 2023-04-14 22:23:27.447157 pdm_conda-0.8.1b0/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b0/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b0/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2162 2023-04-14 22:24:14.370967 pdm_conda-0.8.1b0/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b0/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b0/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b0/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1717 2023-04-14 19:31:18.644281 pdm_conda-0.8.1b0/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b0/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3234 2023-04-09 20:29:55.609532 pdm_conda-0.8.1b0/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b0/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0     9046 2023-04-09 20:29:55.611231 pdm_conda-0.8.1b0/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b0/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b0/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b0/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b0/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     5740 2023-04-09 20:29:55.613268 pdm_conda-0.8.1b0/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b0/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b0/PKG-INFO
```

### Comparing `pdm_conda-0.8.0b0/LICENSE` & `pdm_conda-0.8.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/README.md` & `pdm_conda-0.8.1b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Configuration
 
 | Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
 |-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
 | `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
 | `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
 | `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.use-batched`               | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
+| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
 | `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
 | `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
 | `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
 | `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
 | `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
 | `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
 
@@ -23,15 +23,15 @@
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
 excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
-use-batched = true
+batched-commands = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
 [tool.pdm.conda.optional-dependencies]
 extra = ["anaconda:ffmpeg"] # non python dependency, obtained from anaconda channel
```

### Comparing `pdm_conda-0.8.0b0/pyproject.toml` & `pdm_conda-0.8.1b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.8.0b0"
+version = "0.8.1b0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
@@ -58,15 +58,15 @@
     "src",
 ]
 excludes = [
     "tests",
 ]
 
 [tool.pdm.scripts]
-test = "pytest --cov=src/pdm_conda/ tests/"
+test = "pytest --cov=src/pdm_conda/ tests/ --cov-report xml --cov-report term"
 
 [tool.pytest.ini_options]
 addopts = "--random-order"
 
 [tool.mypy]
 python_version = "3.10"
 pretty = true
```

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/__init__.py` & `pdm_conda-0.8.1b0/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.8.0b0"
+__version__ = "0.8.1b0"
```

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.8.1b0/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.8.1b0/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/conda.py` & `pdm_conda-0.8.1b0/src/pdm_conda/conda.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from packaging.version import Version
 from pdm import termui
 from pdm.exceptions import RequirementError
 from pdm.models.setup import Setup
 from pdm.termui import Verbosity
 
 from pdm_conda.models.candidates import CondaCandidate
+from pdm_conda.models.conda import ChannelSorter
 from pdm_conda.models.config import CondaRunner
 from pdm_conda.models.requirements import (
     CondaRequirement,
-    Requirement,
     parse_conda_version,
     parse_requirement,
 )
 from pdm_conda.models.setup import CondaSetupDistribution
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
@@ -76,54 +76,70 @@
             msg += process.stderr
         if environment:
             msg += f"\n{environment}"
         raise RequirementError(msg) from e
     return response
 
 
-def _sort_packages(packages: list[dict]) -> Iterable[dict]:
+def _sort_packages(packages: list[dict], channels: Iterable[str], platform: str) -> Iterable[dict]:
     """
     Sort packages following mamba specification
     (https://mamba.readthedocs.io/en/latest/advanced_usage/package_resolution.html).
     :param packages: list of conda packages
+    :param channels: list of conda channels used to determine priority
+    :param platform: env platform
     :return: sorted conda packages
     """
     if len(packages) <= 1:
         return packages
 
+    channels_sorter = ChannelSorter(platform, channels)
+
     def get_preference(package):
         return (
             not package.get("track_feature", ""),
+            -channels_sorter.get_priority(package["channel"]),
             Version(parse_conda_version(package["version"], inverse=package.get("name", "") == "openssl")),
             package.get("build_number", 0),
             package.get("timestamp", 0),
         )
 
     return sorted(packages, key=get_preference, reverse=True)
 
 
 @lru_cache(maxsize=None)
+def _parse_channel(channel_url: str) -> str:
+    """
+    Parse channel from channel url
+    :param channel_url: channel url from package
+    :return: channel
+    """
+    channel = urlparse(channel_url).path
+    if channel.startswith("/"):
+        channel = channel[1:]
+    return channel
+
+
+@lru_cache(maxsize=None)
 def _conda_search(
     requirement: str,
     project: CondaProject,
     channels: tuple[str],
 ) -> list[CondaCandidate]:
     """
     Search conda candidates for a requirement
     :param requirement: requirement
     :param project: PDM project
     :param channels: requirement channels
     :return: list of conda candidates
     """
     config = project.conda_config
     command = config.command("search")
-    if not project.virtual_packages:
-        project.virtual_packages = conda_virtual_packages(project)
-
     command.append(requirement)
+
     for c in channels:
         command.extend(["-c", c])
     if channels:
         command.append("--override-channels")
     command.append("--json")
     try:
         result = run_conda(command)
@@ -135,32 +151,27 @@
 
     candidates = []
     if config.runner == CondaRunner.CONDA:
         packages = result.get(parse_requirement(f"conda:{requirement}").name, [])
     else:
         packages = result.get("result", dict()).get("pkgs", [])
 
-    for p in _sort_packages(packages):
+    for p in packages:
+        p["channel"] = _parse_channel(p["channel"])
+
+    for p in _sort_packages(packages, channels, project.platform):
         dependencies = p.get("depends", [])
         valid_candidate = True
         for d in dependencies:
             if d.startswith("__"):
                 d = parse_requirement(f"conda:{d}")
                 if not any(d.is_compatible(v) for v in project.virtual_packages):
                     valid_candidate = False
                     break
         if valid_candidate:
-            package_channel = urlparse(p["channel"]).path
-            for c in channels:
-                if c in package_channel:
-                    p["channel"] = c
-                    break
-            if "defaults" in channels and p["channel"].startswith("http"):
-                p["channel"] = "defaults"
-
             candidates.append(CondaCandidate.from_conda_package(p))
 
     return candidates
 
 
 def conda_search(
     requirement: CondaRequirement | str,
@@ -177,37 +188,28 @@
     if isinstance(requirement, CondaRequirement):
         channel = channel or requirement.channel
         requirement = requirement.as_line(with_build_string=True, conda_compatible=True).replace(" ", "=")
     if "::" in requirement:
         channel, requirement = requirement.split("::", maxsplit=1)
     channels = [channel] if channel else project.conda_config.channels
     if not channels:
-        project.core.ui.echo(f"No channel specified for searching [success]{requirement}[/]", verbosity=Verbosity.DEBUG)
-    return _conda_search(requirement, project, tuple(channels))
+        project.core.ui.echo(
+            f"No channel specified for searching [success]{requirement}[/] using defaults if exist.",
+            verbosity=Verbosity.DEBUG,
+        )
+        channels.append("defaults")
 
+    # set defaults if exist
+    try:
+        idx = channels.index("defaults")
+        channels = channels[:idx] + project.default_channels + channels[idx + 1 :]
+    except ValueError:
+        pass
 
-def update_requirements(requirements: list[Requirement], conda_packages: dict[str, CondaCandidate]):
-    """
-    Update requirements list with conda_packages
-    :param requirements: requirements list
-    :param conda_packages: conda packages
-    """
-    repeated_packages: dict[str, int] = dict()
-    for i, requirement in enumerate(requirements):
-        if (name := requirement.conda_name) in conda_packages and not isinstance(requirement, CondaRequirement):
-            requirement.name = requirement.conda_name
-            requirements[i] = parse_requirement(f"conda:{requirement.as_line()}")
-        repeated_packages[name] = repeated_packages.get(name, 0) + 1
-    to_remove = []
-    for r in requirements:
-        if repeated_packages.get(r.name, 1) > 1:
-            to_remove.append(r)
-            repeated_packages.pop(r.name)
-    for r in to_remove:
-        requirements.remove(r)
+    return _conda_search(requirement, project, tuple(channels))
 
 
 def _conda_install(
     project: CondaProject,
     command: list[str],
     packages: str | list[str] | None = None,
     verbose: bool = False,
@@ -287,33 +289,35 @@
 
 def not_initialized_warning(project):
     project.core.ui.echo(
         "[warning]Tried to execute a conda command but no pdm-conda configs were found on pyproject.toml.[/]",
     )
 
 
-def conda_virtual_packages(project: CondaProject) -> set[CondaRequirement]:
+def conda_info(project: CondaProject) -> dict:
     """
-    Get conda virtual packages
+    Get conda info containing virtual packages, default channels and packages
     :param project: PDM project
-    :return: set of virtual packages
+    :return: dict with conda info
     """
     config = project.conda_config
-    virtual_packages = set()
+    res: dict = dict(virtual_packages=set(), platform="", channels=[])
     if config.is_initialized:
         info = run_conda(config.command("info") + ["--json"])
         if config.runner != CondaRunner.MICROMAMBA:
-            _virtual_packages = {"=".join(p) for p in info["virtual_pkgs"]}
+            virtual_packages = {"=".join(p) for p in info["virtual_pkgs"]}
         else:
-            _virtual_packages = set(info["virtual packages"])
+            virtual_packages = set(info["virtual packages"])
 
-        virtual_packages = {parse_requirement(f"conda:{p.replace('=', '==', 1)}") for p in _virtual_packages}
+        res["virtual_packages"] = {parse_requirement(f"conda:{p.replace('=', '==', 1)}") for p in virtual_packages}
+        res["platform"] = info["platform"]
+        res["channels"] = [_parse_channel(channel) for channel in (info["channels"] or [])]
     else:
         not_initialized_warning(project)
-    return virtual_packages
+    return res
 
 
 def conda_list(project: CondaProject) -> dict[str, CondaSetupDistribution]:
     """
     List conda installed packages
     :param project: PDM project
     :return: packages distribution
```

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.8.1b0/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.8.1b0/src/pdm_conda/installers/synchronizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
         to_add, to_update, to_remove = super().compare_with_working_set()
 
         # deactivate parallel execution if uninstall
         self.parallel = self.environment.project.config["install.parallel"]
         if to_remove:
             to_remove = [p for p in to_remove if p not in self.environment.python_dependencies]
 
-        if self.parallel and any(True for d in to_remove + to_update if isinstance(self.candidates[d], CondaCandidate)):
+        if self.parallel and any(
+            True for d in to_remove + to_update if isinstance(self.candidates.get(d, None), CondaCandidate)
+        ):
             self.environment.project.core.ui.echo("Deactivating parallel uninstall.")
             self.parallel = False
 
         if self.environment.project.conda_config.batched_commands:
             self.manager.prepare_batch_operations(
                 *(
                     len([p for p in pkgs if isinstance(self.candidates[p], CondaCandidate)])
```

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/mapping.py` & `pdm_conda-0.8.1b0/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.8.1b0/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/models/config.py` & `pdm_conda-0.8.1b0/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/models/environment.py` & `pdm_conda-0.8.1b0/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.8.1b0/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.8.1b0/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/models/setup.py` & `pdm_conda-0.8.1b0/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/project.py` & `pdm_conda-0.8.1b0/src/pdm_conda/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,19 +40,61 @@
         super().__init__(core, root_path, is_global, global_config)
         self.core.repository_class = PyPICondaRepository
         self.core.install_manager_class = CondaInstallManager
         self.core.synchronizer_class = CondaSynchronizer
         self.core.resolver_class = CondaResolver
         self.locked_repository_class = LockedCondaRepository
         self.environment_class = CondaEnvironment
-        self.virtual_packages: set[CondaRequirement] = set()
+        self._virtual_packages: set[CondaRequirement] | None = None
+        self._platform: str | None = None
+        self._default_channels: list[str] | None = None
         self._conda_mapping: dict[str, str] = dict()
         self._pypi_mapping: dict[str, str] = dict()
         self.conda_config = PluginConfig.load_config(self)
 
+    def _check_update_info(self, prop):
+        if prop is None:
+            self._get_conda_info()
+        return prop
+
+    @property
+    def virtual_packages(self) -> set[CondaRequirement]:
+        return self._check_update_info(self._virtual_packages)  # type: ignore
+
+    @property
+    def platform(self) -> str:
+        return self._check_update_info(self._platform)  # type: ignore
+
+    @property
+    def default_channels(self) -> list[str]:
+        return self._check_update_info(self._default_channels)  # type: ignore
+
+    @property
+    def locked_repository(self) -> LockedRepository:
+        try:
+            lockfile = self.lockfile._data.unwrap()
+        except ProjectError:
+            lockfile = {}
+
+        return self.locked_repository_class(lockfile, self.sources, self.environment)
+
+    @property
+    def python_requires(self) -> PySpecSet:
+        if not self._python:
+            return super().python_requires
+        return PySpecSet(f"=={self.python.version}")
+
+    def _get_conda_info(self):
+        from pdm_conda.conda import conda_info
+
+        info = conda_info(self)
+        self._virtual_packages = info["virtual_packages"]
+        self._platform = info["platform"]
+        self._default_channels = info["channels"]
+
     def get_conda_pyproject_dependencies(self, group: str, dev: bool = False, set_defaults=False) -> list[str]:
         """
         Get the conda dependencies array in the pyproject.toml
         """
 
         def _getter(conf, name, default, set_defaults=False):
             return (conf.setdefault if set_defaults else conf.get)(name, default)
@@ -106,23 +148,14 @@
             for k in list(result):
                 req = result[k]
                 if req.name not in self.conda_config.excludes and not isinstance(req, CondaRequirement):
                     result[k] = as_conda_requirement(req)
 
         return result
 
-    @property
-    def locked_repository(self) -> LockedRepository:
-        try:
-            lockfile = self.lockfile._data.unwrap()
-        except ProjectError:
-            lockfile = {}
-
-        return self.locked_repository_class(lockfile, self.sources, self.environment)
-
     def add_dependencies(
         self,
         requirements: dict[str, Requirement],
         to_group: str = "default",
         dev: bool = False,
         show_message: bool = True,
     ) -> None:
@@ -141,20 +174,14 @@
                 if matched_index is None:
                     deps.append(req)
                 else:
                     deps[matched_index] = req
 
         super().add_dependencies(requirements, to_group, dev, show_message)
 
-    @property
-    def python_requires(self) -> PySpecSet:
-        if not self._python:
-            return super().python_requires
-        return PySpecSet(f"=={self.python.version}")
-
     def get_environment(self) -> Environment:
         if not self.config["python.use_venv"]:
             raise ProjectError("python.use_venv is required to use Conda.")
         if get_venv_like_prefix(self.python.executable) is None:
             raise ProjectError("Conda environment not detected.")
 
         return self.environment_class(self)
```

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.8.1b0/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/resolvers.py` & `pdm_conda-0.8.1b0/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/src/pdm_conda/utils.py` & `pdm_conda-0.8.1b0/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0b0/PKG-INFO` & `pdm_conda-0.8.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.8.0b0
+Version: 0.8.1b0
 Summary:  A PDM plugin to install project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -42,15 +42,15 @@
 ## Configuration
 
 | Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
 |-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
 | `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
 | `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
 | `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.use-batched`               | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
+| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
 | `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
 | `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
 | `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
 | `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
 | `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
 | `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
 
@@ -60,15 +60,15 @@
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
 excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
-use-batched = true
+batched-commands = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
 [tool.pdm.conda.optional-dependencies]
 extra = ["anaconda:ffmpeg"] # non python dependency, obtained from anaconda channel
```

