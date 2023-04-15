# Comparing `tmp/netcheck-0.1.7.tar.gz` & `tmp/netcheck-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.1.7.tar", max compression
+gzip compressed data, was "netcheck-0.2.0a1.tar", max compression
```

## Comparing `netcheck-0.1.7.tar` & `netcheck-0.2.0a1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0    11357 2022-11-09 03:08:13.772884 netcheck-0.1.7/LICENSE
--rw-r--r--   0        0        0     3872 2022-12-01 08:16:37.901661 netcheck-0.1.7/README.md
--rw-r--r--   0        0        0        0 2022-11-09 01:38:21.119629 netcheck-0.1.7/netcheck/__init__.py
--rw-r--r--   0        0        0     7606 2022-12-01 09:37:58.880630 netcheck-0.1.7/netcheck/cli.py
--rw-r--r--   0        0        0      389 2022-11-10 08:03:11.929678 netcheck-0.1.7/netcheck/dns.py
--rw-r--r--   0        0        0      573 2022-12-01 09:38:23.389849 netcheck-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 netcheck-0.1.7/setup.py
--rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 netcheck-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 04:20:27.771741 netcheck-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     7020 2023-04-15 04:20:27.771741 netcheck-0.2.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/__init__.py
+-rw-r--r--   0        0        0     5896 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/cli.py
+-rw-r--r--   0        0        0     2418 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/dns.py
+-rw-r--r--   0        0        0     2192 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/http.py
+-rw-r--r--   0        0        0     3406 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/runner.py
+-rw-r--r--   0        0        0     1146 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/validation.py
+-rw-r--r--   0        0        0      229 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/version.py
+-rw-r--r--   0        0        0      634 2023-04-15 04:20:27.791741 netcheck-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 netcheck-0.2.0a1/PKG-INFO
```

### Comparing `netcheck-0.1.7/LICENSE` & `netcheck-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.1.7/pyproject.toml` & `netcheck-0.2.0a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 [tool.poetry]
 name = "netcheck"
-version = "0.1.7"
+version = "0.2.0-alpha.1"
 description = ""
-authors = ["Brian Thorne <brian@thorne.link>"]
+authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "netcheck"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 dnspython = "^2.2"
 requests = "^2.28"
-typer = {extras = ["all"], version = "^0.7"}
+typer = "^0.7"
 pydantic = "^1.10"
-rich = "^12.6.0"
+rich = ">=10.11.0,<14.0.0"
+cel-python = "^0.1.5"
 
 
 [tool.poetry.scripts]
 netcheck = "netcheck.cli:app"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coveralls = "^3.3.1"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.241"
+
+[tool.ruff]
+line-length = 120
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

