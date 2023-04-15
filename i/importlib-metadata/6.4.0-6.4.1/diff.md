# Comparing `tmp/importlib_metadata-6.4.0.tar.gz` & `tmp/importlib_metadata-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.4.0.tar", last modified: Sat Apr 15 13:55:48 2023, max compression
+gzip compressed data, was "importlib_metadata-6.4.1.tar", last modified: Sat Apr 15 15:24:44 2023, max compression
```

## Comparing `importlib_metadata-6.4.0.tar` & `importlib_metadata-6.4.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.892020 importlib_metadata-6.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.892020 importlib_metadata-6.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.892020 importlib_metadata-6.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.888020 importlib_metadata-6.4.0/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.350520 importlib_metadata-6.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.350520 importlib_metadata-6.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.350520 importlib_metadata-6.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.354520 importlib_metadata-6.4.1/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.342520 importlib_metadata-6.4.1/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tox.ini
```

### Comparing `importlib_metadata-6.4.0/.github/workflows/main.yml` & `importlib_metadata-6.4.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/CHANGES.rst` & `importlib_metadata-6.4.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v6.4.1
+======
+
+* Updated docs with tweaks from upstream CPython.
+
 v6.4.0
 ======
 
 * Consolidated some behaviors in tests around ``_path``.
 * Added type annotation for ``Distribution.read_text``.
 
 v6.3.0
```

### Comparing `importlib_metadata-6.4.0/LICENSE` & `importlib_metadata-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/PKG-INFO` & `importlib_metadata-6.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.4.0
+Version: 6.4.1
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.4.0/README.rst` & `importlib_metadata-6.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/conftest.py` & `importlib_metadata-6.4.1/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/docs/conf.py` & `importlib_metadata-6.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/docs/index.rst` & `importlib_metadata-6.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/docs/migration.rst` & `importlib_metadata-6.4.1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/docs/using.rst` & `importlib_metadata-6.4.1/docs/using.rst`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ========
 
 Let's say you wanted to get the version string for a
 :term:`packaging:Distribution Package` you've installed
 using ``pip``.  We start by creating a virtual environment and installing
 something into it::
 
-    $ python3 -m venv example
+    $ python -m venv example
     $ source example/bin/activate
     (example) $ python -m pip install importlib_metadata
     (example) $ python -m pip install wheel
 
 You can get the version string for ``wheel`` by running the following::
 
     (example) $ python
@@ -339,15 +339,15 @@
 Extending the search algorithm
 ==============================
 
 Because :term:`packaging:Distribution Package` metadata
 is not available through :data:`sys.path` searches, or
 package loaders directly,
 the metadata for a distribution is found through import
-system `finders`_.  To find a distribution package's metadata,
+system :ref:`finders <finders-and-loaders>`.  To find a distribution package's metadata,
 ``importlib.metadata`` queries the list of :term:`meta path finders <meta path finder>` on
 :data:`sys.meta_path`.
 
 By default ``importlib_metadata`` installs a finder for distribution packages
 found on the file system.
 This finder doesn't actually find any *distributions*,
 but it can find their metadata.
@@ -375,8 +375,7 @@
 ``Distribution`` and implement the abstract methods. Then from
 a custom finder, return instances of this derived ``Distribution`` in the
 ``find_distributions()`` method.
 
 
 .. _`entry point API`: https://setuptools.readthedocs.io/en/latest/pkg_resources.html#entry-points
 .. _`metadata API`: https://setuptools.readthedocs.io/en/latest/pkg_resources.html#metadata-api
-.. _`finders`: https://docs.python.org/3/reference/import.html#finders-and-loaders
```

### Comparing `importlib_metadata-6.4.0/exercises.py` & `importlib_metadata-6.4.1/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/__init__.py` & `importlib_metadata-6.4.1/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_adapters.py` & `importlib_metadata-6.4.1/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_collections.py` & `importlib_metadata-6.4.1/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_compat.py` & `importlib_metadata-6.4.1/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_functools.py` & `importlib_metadata-6.4.1/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_itertools.py` & `importlib_metadata-6.4.1/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_meta.py` & `importlib_metadata-6.4.1/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_py39compat.py` & `importlib_metadata-6.4.1/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata/_text.py` & `importlib_metadata-6.4.1/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.4.1/importlib_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.4.0
+Version: 6.4.1
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.4.0/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.4.1/importlib_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/pytest.ini` & `importlib_metadata-6.4.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/setup.cfg` & `importlib_metadata-6.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/_path.py` & `importlib_metadata-6.4.1/tests/_path.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.4.1/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.4.1/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.4.1/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/fixtures.py` & `importlib_metadata-6.4.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/test_api.py` & `importlib_metadata-6.4.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/test_integration.py` & `importlib_metadata-6.4.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/test_main.py` & `importlib_metadata-6.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/test_py39compat.py` & `importlib_metadata-6.4.1/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tests/test_zip.py` & `importlib_metadata-6.4.1/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.0/tox.ini` & `importlib_metadata-6.4.1/tox.ini`

 * *Files identical despite different names*

