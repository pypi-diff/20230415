# Comparing `tmp/importlib_metadata-6.3.0.tar.gz` & `tmp/importlib_metadata-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.3.0.tar", last modified: Mon Apr 10 02:27:32 2023, max compression
+gzip compressed data, was "importlib_metadata-6.4.0.tar", last modified: Sat Apr 15 13:55:48 2023, max compression
```

## Comparing `importlib_metadata-6.3.0.tar` & `importlib_metadata-6.4.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    28576 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.088812 importlib_metadata-6.3.0/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.892020 importlib_metadata-6.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.892020 importlib_metadata-6.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.892020 importlib_metadata-6.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 13:55:48.000000 importlib_metadata-6.4.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.888020 importlib_metadata-6.4.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:48.896020 importlib_metadata-6.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-15 13:55:25.000000 importlib_metadata-6.4.0/tox.ini
```

### Comparing `importlib_metadata-6.3.0/.github/workflows/main.yml` & `importlib_metadata-6.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/CHANGES.rst` & `importlib_metadata-6.4.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v6.4.0
+======
+
+* Consolidated some behaviors in tests around ``_path``.
+* Added type annotation for ``Distribution.read_text``.
+
 v6.3.0
 ======
 
 * #115: Support ``installed-files.txt`` for ``Distribution.files``
   when present.
 
 v6.2.1
```

### Comparing `importlib_metadata-6.3.0/LICENSE` & `importlib_metadata-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/PKG-INFO` & `importlib_metadata-6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.3.0
+Version: 6.4.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.3.0/README.rst` & `importlib_metadata-6.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/conftest.py` & `importlib_metadata-6.4.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/docs/conf.py` & `importlib_metadata-6.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/docs/index.rst` & `importlib_metadata-6.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/docs/migration.rst` & `importlib_metadata-6.4.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/docs/using.rst` & `importlib_metadata-6.4.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/exercises.py` & `importlib_metadata-6.4.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/__init__.py` & `importlib_metadata-6.4.0/importlib_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from ._itertools import always_iterable, unique_everseen
 from ._meta import PackageMetadata, SimplePath
 
 from contextlib import suppress
 from importlib import import_module
 from importlib.abc import MetaPathFinder
 from itertools import starmap
-from typing import List, Mapping, Optional
+from typing import List, Mapping, Optional, cast
 
 
 __all__ = [
     'Distribution',
     'DistributionFinder',
     'PackageMetadata',
     'PackageNotFoundError',
@@ -348,15 +348,15 @@
         return f'<FileHash mode: {self.mode} value: {self.value}>'
 
 
 class Distribution(metaclass=abc.ABCMeta):
     """A Python distribution package."""
 
     @abc.abstractmethod
-    def read_text(self, filename):
+    def read_text(self, filename) -> Optional[str]:
         """Attempt to load metadata file given by the name.
 
         :param filename: The name of the file in the distribution info.
         :return: The text if found, otherwise None.
         """
 
     @abc.abstractmethod
@@ -422,22 +422,23 @@
     @property
     def metadata(self) -> _meta.PackageMetadata:
         """Return the parsed metadata for this Distribution.
 
         The returned object will have keys that name the various bits of
         metadata.  See PEP 566 for details.
         """
-        text = (
+        opt_text = (
             self.read_text('METADATA')
             or self.read_text('PKG-INFO')
             # This last clause is here to support old egg-info files.  Its
             # effect is to just end up using the PathDistribution's self._path
             # (which points to the egg-info file) attribute unchanged.
             or self.read_text('')
         )
+        text = cast(str, opt_text)
         return _adapters.Message(email.message_from_string(text))
 
     @property
     def name(self):
         """Return the 'Name' metadata for the distribution package."""
         return self.metadata['Name']
```

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_adapters.py` & `importlib_metadata-6.4.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_collections.py` & `importlib_metadata-6.4.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_compat.py` & `importlib_metadata-6.4.0/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_functools.py` & `importlib_metadata-6.4.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_itertools.py` & `importlib_metadata-6.4.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_meta.py` & `importlib_metadata-6.4.0/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_py39compat.py` & `importlib_metadata-6.4.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata/_text.py` & `importlib_metadata-6.4.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.4.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.3.0
+Version: 6.4.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.3.0/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.4.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/pytest.ini` & `importlib_metadata-6.4.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/setup.cfg` & `importlib_metadata-6.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/_path.py` & `importlib_metadata-6.4.0/tests/_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,19 @@
 
 
 @create.register
 def _(content: str, path):
     path.write_text(content, encoding='utf-8')
 
 
+@create.register
+def _(content: str, path):
+    path.write_text(content, encoding='utf-8')
+
+
 class Recording:
     """
     A TreeMaker object that records everything that would be written.
 
     >>> r = Recording()
     >>> build({'foo': {'foo1.txt': 'yes'}, 'bar.txt': 'abc'}, r)
     >>> r.record
```

### Comparing `importlib_metadata-6.3.0/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.4.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.4.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.4.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/fixtures.py` & `importlib_metadata-6.4.0/tests/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import pathlib
 import tempfile
 import textwrap
 import functools
 import contextlib
 
 from .py39compat import FS_NONASCII
-from typing import Dict, Union
 
 from . import _path
+from ._path import FilesSpec
 
 
 try:
     from importlib import resources  # type: ignore
 
     getattr(resources, 'files')
     getattr(resources, 'as_file')
@@ -81,23 +81,16 @@
             sys.path.remove(str(dir))
 
     def setUp(self):
         super().setUp()
         self.fixtures.enter_context(self.add_sys_path(self.site_dir))
 
 
-# Except for python/mypy#731, prefer to define
-# FilesDef = Dict[str, Union['FilesDef', str, bytes]]
-FilesDef = Dict[
-    str, Union[Dict[str, Union[Dict[str, Union[str, bytes]], str, bytes]], str, bytes]
-]
-
-
 class DistInfoPkg(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "distinfo_pkg-1.0.0.dist-info": {
             "METADATA": """
                 Name: distinfo-pkg
                 Author: Steven Ma
                 Version: 1.0.0
                 Requires-Dist: wheel >= 1.0
                 Requires-Dist: pytest; extra == 'test'
@@ -131,30 +124,30 @@
         files = copy.deepcopy(DistInfoPkg.files)
         info = files["distinfo_pkg-1.0.0.dist-info"]
         info["METADATA"] = info["METADATA"].upper()
         build_files(files, self.site_dir)
 
 
 class DistInfoPkgWithDot(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "pkg_dot-1.0.0.dist-info": {
             "METADATA": """
                 Name: pkg.dot
                 Version: 1.0.0
                 """,
         },
     }
 
     def setUp(self):
         super().setUp()
         build_files(DistInfoPkgWithDot.files, self.site_dir)
 
 
 class DistInfoPkgWithDotLegacy(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "pkg.dot-1.0.0.dist-info": {
             "METADATA": """
                 Name: pkg.dot
                 Version: 1.0.0
                 """,
         },
         "pkg.lot.egg-info": {
@@ -173,15 +166,15 @@
 class DistInfoPkgOffPath(SiteDir):
     def setUp(self):
         super().setUp()
         build_files(DistInfoPkg.files, self.site_dir)
 
 
 class EggInfoPkg(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "egginfo_pkg.egg-info": {
             "PKG-INFO": """
                 Name: egginfo-pkg
                 Author: Steven Ma
                 License: Unknown
                 Version: 1.0.0
                 Classifier: Intended Audience :: Developers
@@ -213,15 +206,15 @@
 
     def setUp(self):
         super().setUp()
         build_files(EggInfoPkg.files, prefix=self.site_dir)
 
 
 class EggInfoPkgPipInstalledNoToplevel(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "egg_with_module_pkg.egg-info": {
             "PKG-INFO": "Name: egg_with_module-pkg",
             # SOURCES.txt is made from the source archive, and contains files
             # (setup.py) that are not present after installation.
             "SOURCES.txt": """
                 egg_with_module.py
                 setup.py
@@ -248,15 +241,15 @@
 
     def setUp(self):
         super().setUp()
         build_files(EggInfoPkgPipInstalledNoToplevel.files, prefix=self.site_dir)
 
 
 class EggInfoPkgPipInstalledNoModules(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "egg_with_no_modules_pkg.egg-info": {
             "PKG-INFO": "Name: egg_with_no_modules-pkg",
             # SOURCES.txt is made from the source archive, and contains files
             # (setup.py) that are not present after installation.
             "SOURCES.txt": """
                 setup.py
                 egg_with_no_modules_pkg.egg-info/PKG-INFO
@@ -278,15 +271,15 @@
 
     def setUp(self):
         super().setUp()
         build_files(EggInfoPkgPipInstalledNoModules.files, prefix=self.site_dir)
 
 
 class EggInfoPkgSourcesFallback(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "sources_fallback_pkg.egg-info": {
             "PKG-INFO": "Name: sources_fallback-pkg",
             # SOURCES.txt is made from the source archive, and contains files
             # (setup.py) that are not present after installation.
             "SOURCES.txt": """
                 sources_fallback.py
                 setup.py
@@ -304,15 +297,15 @@
 
     def setUp(self):
         super().setUp()
         build_files(EggInfoPkgSourcesFallback.files, prefix=self.site_dir)
 
 
 class EggInfoFile(OnSysPath, SiteDir):
-    files: FilesDef = {
+    files: FilesSpec = {
         "egginfo_file.egg-info": """
             Metadata-Version: 1.0
             Name: egginfo_file
             Version: 0.1
             Summary: An example package
             Home-page: www.example.com
             Author: Eric Haffa-Vee
@@ -324,46 +317,20 @@
     }
 
     def setUp(self):
         super().setUp()
         build_files(EggInfoFile.files, prefix=self.site_dir)
 
 
-def build_files(file_defs, prefix=pathlib.Path()):
-    """Build a set of files/directories, as described by the
+# dedent all text strings before writing
+orig = _path.create.registry[str]
+_path.create.register(str, lambda content, path: orig(DALS(content), path))
 
-    file_defs dictionary.  Each key/value pair in the dictionary is
-    interpreted as a filename/contents pair.  If the contents value is a
-    dictionary, a directory is created, and the dictionary interpreted
-    as the files within it, recursively.
-
-    For example:
-
-    {"README.txt": "A README file",
-     "foo": {
-        "__init__.py": "",
-        "bar": {
-            "__init__.py": "",
-        },
-        "baz.py": "# Some code",
-     }
-    }
-    """
-    for name, contents in file_defs.items():
-        full_name = prefix / name
-        if isinstance(contents, dict):
-            full_name.mkdir()
-            build_files(contents, prefix=full_name)
-        else:
-            if isinstance(contents, bytes):
-                with full_name.open('wb') as f:
-                    f.write(contents)
-            else:
-                with full_name.open('w', encoding='utf-8') as f:
-                    f.write(DALS(contents))
+
+build_files = _path.build
 
 
 def build_record(file_defs):
     return ''.join(f'{name},,\n' for name in record_names(file_defs))
 
 
 def record_names(file_defs):
```

### Comparing `importlib_metadata-6.3.0/tests/test_api.py` & `importlib_metadata-6.4.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/test_integration.py` & `importlib_metadata-6.4.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/test_main.py` & `importlib_metadata-6.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/test_py39compat.py` & `importlib_metadata-6.4.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tests/test_zip.py` & `importlib_metadata-6.4.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.3.0/tox.ini` & `importlib_metadata-6.4.0/tox.ini`

 * *Files identical despite different names*

