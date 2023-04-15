# Comparing `tmp/fclogr-0.2.0.tar.gz` & `tmp/fclogr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fclogr-0.2.0.tar", last modified: Sat Mar 18 18:23:53 2023, max compression
+gzip compressed data, was "fclogr-0.3.0.tar", last modified: Sat Apr 15 21:19:17 2023, max compression
```

## Comparing `fclogr-0.2.0.tar` & `fclogr-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
--rw-r--r--   0        0        0    17337 2023-01-10 06:28:13.080098 fclogr-0.2.0/LICENSE
-lrwxr-xr-x   0        0        0        0 2023-01-13 06:12:58.354306 fclogr-0.2.0/LICENSES/GPL-2.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     7877 2023-01-14 02:45:59.531460 fclogr-0.2.0/README.md
--rw-r--r--   0        0        0     1588 2023-03-18 18:23:22.220681 fclogr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      104 2023-01-13 06:17:16.597082 fclogr-0.2.0/src/fclogr/__init__.py
--rw-r--r--   0        0        0      209 2023-01-13 23:30:50.869984 fclogr-0.2.0/src/fclogr/__main__.py
--rw-r--r--   0        0        0     1753 2023-03-03 18:30:44.172387 fclogr-0.2.0/src/fclogr/cli/__init__.py
--rw-r--r--   0        0        0      951 2023-03-03 17:58:05.708506 fclogr-0.2.0/src/fclogr/cli/base.py
--rw-r--r--   0        0        0    10293 2023-02-12 19:29:45.752726 fclogr-0.2.0/src/fclogr/cli/dev_entries.py
--rw-r--r--   0        0        0     2219 2023-03-03 21:24:41.285789 fclogr-0.2.0/src/fclogr/cli/sync.py
--rw-r--r--   0        0        0        0 2023-01-07 08:21:55.207097 fclogr-0.2.0/src/fclogr/py.typed
--rw-r--r--   0        0        0        0 2023-03-03 18:54:38.037265 fclogr-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      255 2023-03-03 20:09:51.312624 fclogr-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      418 2023-03-03 20:38:43.523172 fclogr-0.2.0/tests/test_data/package.2.spec
--rw-r--r--   0        0        0      442 2023-03-03 22:00:05.714861 fclogr-0.2.0/tests/test_data/package.3.spec
--rw-r--r--   0        0        0      376 2023-03-03 20:18:25.858606 fclogr-0.2.0/tests/test_data/package.spec
--rw-r--r--   0        0        0      925 2023-03-06 03:38:07.737434 fclogr-0.2.0/tests/test_syncer.py
--rw-r--r--   0        0        0     1508 2023-03-18 18:16:21.500356 fclogr-0.2.0/tox.ini
--rw-r--r--   0        0        0     8925 1970-01-01 00:00:00.000000 fclogr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-15 20:35:53.456294 fclogr-0.3.0/.copr/Makefile
+lrwxr-xr-x   0        0        0        0 2023-04-15 20:35:53.456294 fclogr-0.3.0/LICENSE -> LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0    17337 2023-04-15 20:35:53.456294 fclogr-0.3.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-04-15 16:21:50.774739 fclogr-0.3.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      202 2023-04-15 21:18:22.282312 fclogr-0.3.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-04-15 20:35:53.457294 fclogr-0.3.0/NEWS.md.license
+-rw-r--r--   0        0        0     8143 2023-04-15 16:27:46.566165 fclogr-0.3.0/README.md
+-rwxr-xr-x   0        0        0      932 2023-04-15 16:49:14.180578 fclogr-0.3.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     1267 2023-04-15 21:18:22.283312 fclogr-0.3.0/fclogr.spec
+-rw-r--r--   0        0        0    10554 2023-04-15 21:18:26.214290 fclogr-0.3.0/noxfile.py
+-rw-r--r--   0        0        0     1973 2023-04-15 21:19:16.844004 fclogr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-01-13 06:17:16.597082 fclogr-0.3.0/src/fclogr/__init__.py
+-rw-r--r--   0        0        0      209 2023-01-13 23:30:50.869984 fclogr-0.3.0/src/fclogr/__main__.py
+-rw-r--r--   0        0        0     2047 2023-04-14 04:40:12.125463 fclogr-0.3.0/src/fclogr/cli/__init__.py
+-rw-r--r--   0        0        0     1331 2023-04-14 04:14:48.656998 fclogr-0.3.0/src/fclogr/cli/base.py
+-rw-r--r--   0        0        0     6512 2023-04-15 20:35:53.457294 fclogr-0.3.0/src/fclogr/cli/bump.py
+-rw-r--r--   0        0        0     9971 2023-04-14 04:14:48.657998 fclogr-0.3.0/src/fclogr/cli/dev_entries.py
+-rw-r--r--   0        0        0     2256 2023-04-01 04:25:07.641592 fclogr-0.3.0/src/fclogr/cli/sync.py
+-rw-r--r--   0        0        0        0 2023-01-07 08:21:55.207097 fclogr-0.3.0/src/fclogr/py.typed
+-rw-r--r--   0        0        0        0 2023-03-03 18:54:38.037265 fclogr-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-15 20:35:53.457294 fclogr-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     4369 2023-04-15 20:35:53.457294 fclogr-0.3.0/tests/test_bumper.py
+-rw-r--r--   0        0        0      418 2023-04-01 04:25:07.638592 fclogr-0.3.0/tests/test_data/package.2.spec
+-rw-r--r--   0        0        0      442 2023-03-03 22:00:05.714861 fclogr-0.3.0/tests/test_data/package.3.spec
+-rw-r--r--   0        0        0      376 2023-03-03 20:18:25.858606 fclogr-0.3.0/tests/test_data/package.spec
+-rw-r--r--   0        0        0      961 2023-04-15 20:35:53.457294 fclogr-0.3.0/tests/test_syncer.py
+-rw-r--r--   0        0        0     9638 1970-01-01 00:00:00.000000 fclogr-0.3.0/PKG-INFO
```

### Comparing `fclogr-0.2.0/LICENSE` & `fclogr-0.3.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fclogr-0.2.0/README.md` & `fclogr-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 SPDX-License-Identifier: GPL-2.0-or-later
 -->
 
 # fclogr
 
 fclogr is a tool for managing RPM changelogs and updates.
-Currently an undocumented WIP.
 
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/fclogr/commits/main.svg)](https://builds.sr.ht/~gotmax23/fclogr/commits/main?)
 
 [![fclogr on sr.ht][badge-hub]][link-hub]
 
 [![fclogr on git.sr.ht][badge-repo]][link-repo]
@@ -26,24 +25,30 @@
 GPL-2.0-or-later
 ```
 
 ## Patches
 
 Patches can be sent to ~gotmax23/fclogr@lists.sr.ht ([archives]) with
 [`git-send-email`](https://git-send-email.io).
+Make sure to run tests and linters with `nox` prior to submitting changes
+upstream.
 
 [archives]: https://lists.sr.ht/~gotmax23/fclogr
 
 ```
 git config sendemail.to "~gotmax23/fclogr@lists.sr.ht"
 git config format.subjectprefix "PATCH fclogr"
 git send-email origin/main
 ```
 
+If you prefer, git.sr.ht [has a webui][webui-email] to help you submit patches
+to a mailing list that can be used in place of git send-email.
 
+
+[webui-email]: https://man.sr.ht/git.sr.ht/#sending-patches-upstream)
 [link-hub]: https://sr.ht/~gotmax23/fclogr
 [badge-hub]: https://img.shields.io/badge/Project%20Hub-fclogr-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K&style=for-the-badge
 [link-repo]: https://git.sr.ht/~gotmax23/fclogr
 [badge-repo]: https://img.shields.io/badge/git.sr.ht-fclogr-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K&style=for-the-badge
 [archives]: https://lists.sr.ht/~gotmax23/fclogr
 [badge-list]: https://img.shields.io/badge/lists.sr.ht-fclogr-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K&style=for-the-badge
 [link-todo]: https://todo.sr.ht/~gotmax23/fclogr
```

### Comparing `fclogr-0.2.0/pyproject.toml` & `fclogr-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fclogr"
 description = "fclogr is a tool for managing RPM changelogs and updates"
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPL-2.0-or-later"}
 # license-files.paths = ["LICENSES/GPL-2.0-or-later.txt"]
 keywords = []
 authors = [
     { name = "Maxwell G", email = "gotmax@e.email" },
@@ -36,34 +36,51 @@
 [project.urls]
 Homepage = "https://git.sr.ht/~gotmax23/fclogr"
 
 [project.scripts]
 fclogr = "fclogr.cli:main"
 
 [project.optional-dependencies]
-test = [
-    "pytest",
+# Development
+codeqa = [
+    "ruff",
+    "reuse",
 ]
-lint = [
+formatters = [
     "black",
     "isort",
+]
+typing = [
     "mypy",
-    "reuse",
-    "ruff",
+]
+test = [
+    "pytest",
+    "pytest-mock",
+]
+dev = [
+    "fclogr[codeqa]",
+    "fclogr[formatters]",
+    "fclogr[test]",
+    "nox>=2022.11.21",
+]
+lint = [
+    "fclogr[formatters]",
+    "fclogr[typing]",
 ]
 
 [tool.flit.sdist]
 exclude = [
     ".builds/*",
     ".gitignore",
 ]
 
 
 [tool.isort]
 profile = "black"
+add_imports = ["from __future__ import annotations"]
 
 [[tool.mypy.overrides]]
 module = ["pygit2"]
 ignore_missing_imports = true
 
 [tool.ruff]
 select = [
@@ -74,8 +91,14 @@
     # pycodestyle
     "E",
     "W",
     # pyflakes
     "F",
     # flake8-simplify
     "SIM",
+    # unused-arguments
+    "ARG",
 ]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["ARG"]
+"noxfile.py" = ["ARG"]
```

### Comparing `fclogr-0.2.0/src/fclogr/cli/__init__.py` & `fclogr-0.3.0/src/fclogr/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import argparse
 import logging
+import sys
 from collections.abc import Sequence
+from subprocess import CalledProcessError
 
 from fclogr.cli.sync import Syncer
 
 from .base import LOG, Command, InvalidArgumentError
+from .bump import Bumper
 from .dev_entries import DevEntries, DevSRPM
 
 
 def get_command(argv: Sequence[str] | None = None, **kwargs) -> Command:
     parser = argparse.ArgumentParser(
         description="fclogr is a tool for managing RPM changelogs and updates", **kwargs
     )
@@ -46,18 +49,26 @@
 
 def main(argv: Sequence[str] | None = None) -> int | str:
     try:
         command = get_command(argv)
     except InvalidArgumentError as err:
         # sys.exit() in the console_script handles this
         return str(err)
-    r = command.run()
+    try:
+        r = command.run()
+    except CalledProcessError as err:
+        print(err, file=sys.stderr)
+        r = err.returncode
+    except Exception:
+        LOG.exception("Unexpected Exception")
+        r = 1
     for func in command.cleanup:
         func()
     return r
 
 
 COMMANDS: dict[str, type[Command]] = {
-    "sync": Syncer,
+    "bump": Bumper,
     "dev-entries": DevEntries,
     "dev-srpm": DevSRPM,
+    "sync": Syncer,
 }
```

### Comparing `fclogr-0.2.0/src/fclogr/cli/dev_entries.py` & `fclogr-0.3.0/src/fclogr/cli/dev_entries.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,22 +138,14 @@
         parser.add_argument("-r", "--last-ref", dest="baseversion", metavar="LAST_REF")
         parser.add_argument("--pre")
         parser.add_argument("-o", "--outdir", default=Path.cwd(), type=Path)
         parser.add_argument("--stdout", action="store_true")
         parser.add_argument("-A", "--archive", action="store_true")
         return parser
 
-    def _v_specpath(self, path: Path | None = None) -> Path:
-        if not path:
-            pwd = Path.cwd()
-            path = pwd.joinpath(pwd.name + ".spec")
-        if not path.is_file() or path.suffix != ".spec":
-            raise InvalidArgumentError(f"{path} must exist an end with '.spec'")
-        return path
-
     def _guess_last_ref(self, baseversion: str | None, pre: str | None) -> None:
         self.pre = bool(pre)
         if not baseversion:
             try:
                 baseversion = self.repository.describe(
                     self.repository.head, abbreviated_size=0
                 )
```

### Comparing `fclogr-0.2.0/src/fclogr/cli/sync.py` & `fclogr-0.3.0/src/fclogr/cli/sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,13 +60,14 @@
         return release, lines
 
     def run(self) -> int:
         release, clog = self._get_out_changelog()
         for line in self.inp:
             if release and line.startswith("Release:"):
                 self.out.write(release)
-            elif line.strip() == "%changelog":
+            elif clog and line.strip() == "%changelog":
                 self.out.writelines(clog)
                 break
             else:
                 self.out.write(line)
+        self.out.truncate()
         return 0
```

### Comparing `fclogr-0.2.0/tests/test_syncer.py` & `fclogr-0.3.0/tests/test_syncer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright (c) 2023 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import shutil
 
 import pytest
 
 from fclogr.cli import main
 from fclogr.cli.base import InvalidArgumentError
 from fclogr.cli.sync import Syncer
```

### Comparing `fclogr-0.2.0/PKG-INFO` & `fclogr-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fclogr
-Version: 0.2.0
+Version: 0.3.0
 Summary: fclogr is a tool for managing RPM changelogs and updates
 Keywords: 
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -13,34 +13,44 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: pygit2
 Requires-Dist: specfile
-Requires-Dist: black ; extra == "lint"
-Requires-Dist: isort ; extra == "lint"
-Requires-Dist: mypy ; extra == "lint"
-Requires-Dist: reuse ; extra == "lint"
-Requires-Dist: ruff ; extra == "lint"
+Requires-Dist: ruff ; extra == "codeqa"
+Requires-Dist: reuse ; extra == "codeqa"
+Requires-Dist: fclogr[codeqa] ; extra == "dev"
+Requires-Dist: fclogr[formatters] ; extra == "dev"
+Requires-Dist: fclogr[test] ; extra == "dev"
+Requires-Dist: nox>=2022.11.21 ; extra == "dev"
+Requires-Dist: black ; extra == "formatters"
+Requires-Dist: isort ; extra == "formatters"
+Requires-Dist: fclogr[formatters] ; extra == "lint"
+Requires-Dist: fclogr[typing] ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-mock ; extra == "test"
+Requires-Dist: mypy ; extra == "typing"
 Project-URL: Homepage, https://git.sr.ht/~gotmax23/fclogr
+Provides-Extra: codeqa
+Provides-Extra: dev
+Provides-Extra: formatters
 Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: typing
 
 <!--
 SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
 
 SPDX-License-Identifier: GPL-2.0-or-later
 -->
 
 # fclogr
 
 fclogr is a tool for managing RPM changelogs and updates.
-Currently an undocumented WIP.
 
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/fclogr/commits/main.svg)](https://builds.sr.ht/~gotmax23/fclogr/commits/main?)
 
 [![fclogr on sr.ht][badge-hub]][link-hub]
 
 [![fclogr on git.sr.ht][badge-repo]][link-repo]
@@ -55,24 +65,30 @@
 GPL-2.0-or-later
 ```
 
 ## Patches
 
 Patches can be sent to ~gotmax23/fclogr@lists.sr.ht ([archives]) with
 [`git-send-email`](https://git-send-email.io).
+Make sure to run tests and linters with `nox` prior to submitting changes
+upstream.
 
 [archives]: https://lists.sr.ht/~gotmax23/fclogr
 
 ```
 git config sendemail.to "~gotmax23/fclogr@lists.sr.ht"
 git config format.subjectprefix "PATCH fclogr"
 git send-email origin/main
 ```
 
+If you prefer, git.sr.ht [has a webui][webui-email] to help you submit patches
+to a mailing list that can be used in place of git send-email.
 
+
+[webui-email]: https://man.sr.ht/git.sr.ht/#sending-patches-upstream)
 [link-hub]: https://sr.ht/~gotmax23/fclogr
 [badge-hub]: https://img.shields.io/badge/Project%20Hub-fclogr-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K&style=for-the-badge
 [link-repo]: https://git.sr.ht/~gotmax23/fclogr
 [badge-repo]: https://img.shields.io/badge/git.sr.ht-fclogr-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K&style=for-the-badge
 [archives]: https://lists.sr.ht/~gotmax23/fclogr
 [badge-list]: https://img.shields.io/badge/lists.sr.ht-fclogr-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K&style=for-the-badge
 [link-todo]: https://todo.sr.ht/~gotmax23/fclogr
```

