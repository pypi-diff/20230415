# Comparing `tmp/drclient-0.0.6.tar.gz` & `tmp/drclient-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drclient-0.0.6.tar", last modified: Wed Apr 12 20:28:45 2023, max compression
+gzip compressed data, was "drclient-0.0.7.tar", last modified: Sat Apr 15 17:37:50 2023, max compression
```

## Comparing `drclient-0.0.6.tar` & `drclient-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.167979 drclient-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.159979 drclient-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 20:28:36.000000 drclient-0.0.6/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 20:28:36.000000 drclient-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-12 20:28:36.000000 drclient-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 20:28:36.000000 drclient-0.0.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 20:28:36.000000 drclient-0.0.6/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-12 20:28:36.000000 drclient-0.0.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 20:28:36.000000 drclient-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 20:28:36.000000 drclient-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 20:28:45.167979 drclient-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-12 20:28:36.000000 drclient-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/cli/cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/threaded_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 20:28:44.000000 drclient-0.0.6/drclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.167979 drclient-0.0.6/drclient/view/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/view/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/view/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/view/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 20:28:36.000000 drclient-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 20:28:36.000000 drclient-0.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 20:28:36.000000 drclient-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 20:28:45.167979 drclient-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 20:28:36.000000 drclient-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 20:28:36.000000 drclient-0.0.6/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.167979 drclient-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 20:28:36.000000 drclient-0.0.6/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 20:28:36.000000 drclient-0.0.6/tests/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 20:28:36.000000 drclient-0.0.6/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-12 20:28:36.000000 drclient-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.316156 drclient-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.304155 drclient-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.308155 drclient-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-15 17:37:38.000000 drclient-0.0.7/.github/workflows/gh-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-15 17:37:38.000000 drclient-0.0.7/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-15 17:37:38.000000 drclient-0.0.7/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-15 17:37:38.000000 drclient-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-15 17:37:38.000000 drclient-0.0.7/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.308155 drclient-0.0.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-15 17:37:38.000000 drclient-0.0.7/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-15 17:37:38.000000 drclient-0.0.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-15 17:37:38.000000 drclient-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-15 17:37:38.000000 drclient-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 17:37:38.000000 drclient-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 17:37:50.316156 drclient-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-15 17:37:38.000000 drclient-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.312155 drclient-0.0.7/drclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.312155 drclient-0.0.7/drclient/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/cli/cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.316156 drclient-0.0.7/drclient/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/registry/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/registry/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/threaded_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.316156 drclient-0.0.7/drclient/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/view/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/view/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-15 17:37:38.000000 drclient-0.0.7/drclient/view/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.312155 drclient-0.0.7/drclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 17:37:50.000000 drclient-0.0.7/drclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-15 17:37:38.000000 drclient-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 17:37:38.000000 drclient-0.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 17:37:38.000000 drclient-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-15 17:37:50.316156 drclient-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-15 17:37:38.000000 drclient-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:50.316156 drclient-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 17:37:38.000000 drclient-0.0.7/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 17:37:38.000000 drclient-0.0.7/tests/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 17:37:38.000000 drclient-0.0.7/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-15 17:37:38.000000 drclient-0.0.7/tox.ini
```

### Comparing `drclient-0.0.6/.github/workflows/multi-test.yaml` & `drclient-0.0.7/.github/workflows/multi-test.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 jobs:
   build:
     name: Tox test
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
+        os: [ubuntu-latest]
         python-version: ['3.8', '3.9', '3.10', '3.11']
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
```

### Comparing `drclient-0.0.6/.github/workflows/release.yaml` & `drclient-0.0.7/.github/workflows/pypi-release.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -25,17 +25,7 @@
         run: python setup.py sdist bdist_wheel
 
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-
-  create-release:
-    runs-on: ubuntu-latest
-    permissions:
-      contents: write
-    steps:
-    - uses: actions/checkout@v3
-    - uses: ncipollo/release-action@v1
-      with:
-        generateReleaseNotes: true
```

### Comparing `drclient-0.0.6/.gitignore` & `drclient-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/.pre-commit-config.yaml` & `drclient-0.0.7/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -35,7 +35,16 @@
     - id: black
 
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
     rev: 'v0.0.259'
     hooks:
     - id: ruff
+
+- repo: local
+  hooks:
+    -   id: run-pytest
+        name: Run tests using pytest
+        entry:
+            python -m pytest
+        language: system
+        pass_filenames: false
```

### Comparing `drclient-0.0.6/LICENSE` & `drclient-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/PKG-INFO` & `drclient-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.6
+Version: 0.0.7
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.6/README.md` & `drclient-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/drclient/cli/cmd_info.py` & `drclient-0.0.7/drclient/cli/cmd_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import json
 from typing import Optional
 
 import typer
 
+from ..image import parse_image_url
 from ..registry import DockerRegistryClient
 from ..view.info import print_image_info
 
 
 def info(
     image_name: str = typer.Argument(..., help="The name of the image"),
     output_format: Optional[str] = typer.Option(
         None, "-o", "--output-format", help="Ouput format [json]"
     ),
 ):
     """
     Show information for an image stored in a docker registry
     """
-    registry, repository, tag = DockerRegistryClient.parse_image_url(image_name)
+    registry, repository, tag = parse_image_url(image_name)
     drc = DockerRegistryClient(registry)
     drc.authenticate()
     manifest = drc.get_manifest(repository, tag, expand_config=True)
     if output_format == "json":
         print(json.dumps(manifest, indent=4))
     else:
         print_image_info(manifest)
```

### Comparing `drclient-0.0.6/drclient/cli/cmd_pull.py` & `drclient-0.0.7/drclient/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,37 +4,29 @@
 import tarfile
 from pathlib import Path
 from subprocess import getstatusoutput
 from tempfile import mkdtemp
 
 import typer
 
-from ..extract import extract_layers
-from ..registry import DockerRegistryClient
-from ..threaded_pull import pull_layers_in_threads
-from ..view.info import sizeof_fmt
-
-
-def pull(
-    image_name: str = typer.Argument(..., help="The name of the image"),
-    tar_file: Path = typer.Option(
-        None, "-t", "--tar-file", help="Output to a tar.gz file"
-    ),
-    squafshfs_file: Path = typer.Option(
-        None, "-s", "--squashfs-file", help="Output to a .sqfs file"
-    ),
-    output_directory: Path = typer.Option(
-        None, "-d", "--output-directory", help="Output to a directory"
-    ),
+from .registry import DockerRegistryClient
+from .threaded_pull import pull_layers_in_threads
+from .view.info import sizeof_fmt
+
+DEFAULT_REGISTRY = os.environ.get("DOCKER_REGISTRY", "registry-1.docker.io")
+
+
+def pull_image(
+    image_url: str, output_directory=None, tar_file=None, squashfs_file=None
 ):
     """
     Pull image from a docker registry
     """
     is_tmp_output_directory = False
-    registry, repository, tag = DockerRegistryClient.parse_image_url(image_name)
+    registry, repository, tag = parse_image_url(image_url)
     source_reference = f"{registry}/{repository}:{tag}"
 
     drc = DockerRegistryClient(registry)
     drc.authenticate()
     manifest = drc.get_manifest(repository, tag)
     layers = manifest["layers"]
     local_image_name = f"{repository}:{tag}"
@@ -42,15 +34,15 @@
     print(
         f"Pulling {len(layers)} layer(s) [{sizeof_fmt(total_size)}] "
         f"for image {source_reference} to local image {local_image_name}"
     )
 
     if output_directory is None:
         output_directory = mkdtemp()
-        if tar_file or squafshfs_file:
+        if tar_file or squashfs_file:
             is_tmp_output_directory = True
             atexit.register(shutil.rmtree, output_directory)
     else:
         print(output_directory)
         if not output_directory.exists():
             output_directory.mkdir(parents=True)
         else:
@@ -61,31 +53,44 @@
             os.scandir(output_directory)
             if any(os.scandir(output_directory)):
                 raise typer.BadParameter(
                     f"Output directory {output_directory} is not empty"
                 )
 
     pull_layers_in_threads(drc, layers, output_directory)
-    print("Extracting layers...", end="", flush=True)
-    extract_layers(layers, Path(output_directory))
-    print("Done")
+
     if tar_file:
         cwd = os.getcwd()
         os.chdir(output_directory)
         with tarfile.open(tar_file, "w:gz") as tar:
             tar.add(".", arcname="", recursive=True)
         os.chdir(cwd)
 
-    if squafshfs_file:
-        squafshfs_file = Path(squafshfs_file)
+    if squashfs_file:
+        squafshfs_file = Path(squashfs_file)
         if squafshfs_file.exists():
             squafshfs_file.unlink()
         print("Creating squashfs file...", end="", flush=True)
         exit_code, output = getstatusoutput(
             f"mksquashfs {output_directory} {squafshfs_file}"
         )
         if exit_code != 0:
             raise typer.Exit(f"Failed to create squashfs file: {output}")
         print("Done")
 
     if not is_tmp_output_directory:
         print(f"Contents of {source_reference} extracted to {output_directory}")
+
+
+def parse_image_url(image_name: str) -> tuple:
+    registry = DEFAULT_REGISTRY
+    tag = "latest"
+    if "/" in image_name:
+        first_part, other_parts = image_name.split("/", 1)
+        if "." in first_part:
+            image_name = other_parts
+            registry = f"{first_part}"
+    else:
+        image_name = f"library/{image_name}"
+    if ":" in image_name:
+        image_name, tag = image_name.split(":")
+    return registry, image_name, tag
```

### Comparing `drclient-0.0.6/drclient/extract.py` & `drclient-0.0.7/drclient/extract.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/drclient/registry/registry.py` & `drclient-0.0.7/drclient/registry/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import os
 import re
 from pathlib import Path
 
 import requests
 
 from .manifest import DockerManifest
 from .specs import Manifests
 
-DEFAULT_REGISTRY = os.environ.get("DOCKER_REGISTRY", "registry-1.docker.io")
 API_URL = "/v2/"
 
 
 class DockerRegistryClient(object):
     def __init__(
         self, registry, verify=True, username=None, password=None, timeout=5.0
     ):
@@ -134,26 +132,7 @@
                 with open(out_filename, "wb+") as output_file:
                     for data in r.iter_content(chunk_size=512 * 1024):
                         output_file.write(data)
                         if update_hook:
                             update_hook(len(data))
         else:
             return self._http_get(url, allow_redirects=True)
-
-    def parse_image_url(image_name: str) -> tuple:
-        registry = DEFAULT_REGISTRY
-        tag = "latest"
-        protocol_prefix = "https://"
-        protocol_mark = image_name.find("://")
-        if protocol_mark > -1:
-            protocol_prefix = image_name[: protocol_mark + 3]
-            image_name = image_name[protocol_mark + 3 :]
-        if "/" in image_name:
-            first_part, other_parts = image_name.split("/", 1)
-            if "." in first_part:
-                image_name = other_parts
-                registry = f"{protocol_prefix}{first_part}"
-        else:
-            image_name = f"library/{image_name}"
-        if ":" in image_name:
-            image_name, tag = image_name.split(":")
-        return registry, image_name, tag
```

### Comparing `drclient-0.0.6/drclient/threaded_pull.py` & `drclient-0.0.7/drclient/threaded_pull.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/drclient/view/history.py` & `drclient-0.0.7/drclient/view/history.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/drclient/view/info.py` & `drclient-0.0.7/drclient/view/info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.6/drclient.egg-info/PKG-INFO` & `drclient-0.0.7/drclient.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.6
+Version: 0.0.7
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.6/drclient.egg-info/SOURCES.txt` & `drclient-0.0.7/drclient.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 .gitignore
 .pre-commit-config.yaml
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
-test.py
 tox.ini
+.github/workflows/gh-release.yaml
 .github/workflows/multi-test.yaml
-.github/workflows/release.yaml
+.github/workflows/pypi-release.yaml
 .vscode/launch.json
 .vscode/settings.json
 drclient/__main__.py
 drclient/extract.py
+drclient/image.py
 drclient/threaded_pull.py
 drclient/version.py
 drclient.egg-info/PKG-INFO
 drclient.egg-info/SOURCES.txt
 drclient.egg-info/dependency_links.txt
 drclient.egg-info/entry_points.txt
 drclient.egg-info/requires.txt
```

### Comparing `drclient-0.0.6/setup.py` & `drclient-0.0.7/setup.py`

 * *Files identical despite different names*

