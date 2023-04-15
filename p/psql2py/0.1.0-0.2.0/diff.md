# Comparing `tmp/psql2py-0.1.0.tar.gz` & `tmp/psql2py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psql2py-0.1.0.tar", max compression
+gzip compressed data, was "psql2py-0.2.0.tar", max compression
```

## Comparing `psql2py-0.1.0.tar` & `psql2py-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        0 2022-12-04 21:15:59.608965 psql2py-0.1.0/README.md
--rw-r--r--   0        0        0      414 2023-01-13 23:10:24.548709 psql2py-0.1.0/psql2py/__main__.py
--rw-r--r--   0        0        0      679 2023-01-13 23:09:35.561157 psql2py-0.1.0/psql2py/config.py
--rw-r--r--   0        0        0      298 2023-01-13 23:51:44.722663 psql2py-0.1.0/psql2py/core.py
--rw-r--r--   0        0        0     5906 2023-01-13 23:14:00.949406 psql2py-0.1.0/psql2py/generate.py
--rw-r--r--   0        0        0     2402 2023-01-12 23:35:41.463924 psql2py-0.1.0/psql2py/inspect.py
--rw-r--r--   0        0        0     1187 2023-01-13 23:53:09.114696 psql2py-0.1.0/psql2py/templates/module.py.jinja
--rw-r--r--   0        0        0      713 2023-01-13 23:10:48.301304 psql2py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 psql2py-0.1.0/setup.py
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 psql2py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-04 21:15:59.608965 psql2py-0.2.0/README.md
+-rw-r--r--   0        0        0     1981 2023-04-04 18:40:36.358320 psql2py-0.2.0/psql2py/__main__.py
+-rw-r--r--   0        0        0      756 2023-04-04 18:40:36.358396 psql2py-0.2.0/psql2py/common.py
+-rw-r--r--   0        0        0     1996 2023-04-04 18:40:36.358514 psql2py-0.2.0/psql2py/generate.py
+-rw-r--r--   0        0        0     3241 2023-04-15 10:56:49.686329 psql2py-0.2.0/psql2py/inspect.py
+-rw-r--r--   0        0        0     4519 2023-04-04 18:40:36.359125 psql2py-0.2.0/psql2py/load.py
+-rw-r--r--   0        0        0     3595 2023-04-04 18:40:36.359273 psql2py-0.2.0/psql2py/render.py
+-rw-r--r--   0        0        0     1059 2023-04-04 18:40:36.359395 psql2py-0.2.0/psql2py/templates/module.py.jinja
+-rw-r--r--   0        0        0     1911 2023-04-15 10:56:58.341550 psql2py-0.2.0/psql2py/types.py
+-rw-r--r--   0        0        0      663 2023-04-15 10:58:03.534058 psql2py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 psql2py-0.2.0/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 psql2py-0.2.0/PKG-INFO
```

### Comparing `psql2py-0.1.0/pyproject.toml` & `psql2py-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 [tool.poetry]
 name = "psql2py"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
-authors = ["Your Name <you@example.com>"]
+authors = ["Momo Eissenhauer <momo.eissenhauer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlparse = "^0.4.3"
 psycopg2 = "^2.9.5"
 click = "^8.1.3"
-pg-docker = "^0.5.0"
 jinja2 = "^3.1.2"
-docstring-parser = "^0.15"
 watchdog = "^2.2.1"
-pydantic = "^1.10.4"
+types-psycopg2 = "^2.9.21.9"
+psql2py-core = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
-snapshottest = "^0.6.0"
 black = "^22.10.0"
 mypy = "^0.991"
-types-psycopg2 = "^2.9.21.2"
+pg-docker = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = [
-    "snapshottest",
     "sqlparse",
 ]
 ignore_missing_imports = true
```

### Comparing `psql2py-0.1.0/setup.py` & `psql2py-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 ['psql2py']
 
 package_data = \
 {'': ['*'], 'psql2py': ['templates/*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
- 'docstring-parser>=0.15,<0.16',
  'jinja2>=3.1.2,<4.0.0',
- 'pg-docker>=0.5.0,<0.6.0',
+ 'psql2py-core>=0.1.0,<0.2.0',
  'psycopg2>=2.9.5,<3.0.0',
- 'pydantic>=1.10.4,<2.0.0',
  'sqlparse>=0.4.3,<0.5.0',
+ 'types-psycopg2>=2.9.21.9,<3.0.0.0',
  'watchdog>=2.2.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'psql2py',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '',
-    'author': 'Your Name',
-    'author_email': 'you@example.com',
+    'author': 'Momo Eissenhauer',
+    'author_email': 'momo.eissenhauer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.11,<4.0',
```

### Comparing `psql2py-0.1.0/PKG-INFO` & `psql2py-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: psql2py
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
-Author: Your Name
-Author-email: you@example.com
+Author: Momo Eissenhauer
+Author-email: momo.eissenhauer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pg-docker (>=0.5.0,<0.6.0)
+Requires-Dist: psql2py-core (>=0.1.0,<0.2.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.3,<0.5.0)
+Requires-Dist: types-psycopg2 (>=2.9.21.9,<3.0.0.0)
 Requires-Dist: watchdog (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
```

