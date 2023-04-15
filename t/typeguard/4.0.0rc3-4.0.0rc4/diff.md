# Comparing `tmp/typeguard-4.0.0rc3.tar.gz` & `tmp/typeguard-4.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.0.0rc3.tar", last modified: Mon Apr 10 16:23:40 2023, max compression
+gzip compressed data, was "typeguard-4.0.0rc4.tar", last modified: Sat Apr 15 15:57:00 2023, max compression
```

## Comparing `typeguard-4.0.0rc3.tar` & `typeguard-4.0.0rc4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.572764 typeguard-4.0.0rc3/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    38460 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.572764 typeguard-4.0.0rc3/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.572764 typeguard-4.0.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    30979 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    36886 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.720680 typeguard-4.0.0rc4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.724680 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.724680 typeguard-4.0.0rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.724680 typeguard-4.0.0rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.720680 typeguard-4.0.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.728680 typeguard-4.0.0rc4/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40656 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.728680 typeguard-4.0.0rc4/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31486 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/.github/workflows/publish.yml` & `typeguard-4.0.0rc4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/.github/workflows/test.yml` & `typeguard-4.0.0rc4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/.pre-commit-config.yaml` & `typeguard-4.0.0rc4/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,25 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-      - id: black
-        exclude: "^tests/mypy/negative.py"
-
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: v0.0.261
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+      - id: black
+        exclude: "^tests/mypy/negative.py"
+
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies: [ "typing_extensions" ]
         exclude: "^tests/"
```

### Comparing `typeguard-4.0.0rc3/LICENSE` & `typeguard-4.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/PKG-INFO` & `typeguard-4.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc3
+Version: 4.0.0rc4
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc3/README.rst` & `typeguard-4.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/docs/api.rst` & `typeguard-4.0.0rc4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/docs/conf.py` & `typeguard-4.0.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/docs/extending.rst` & `typeguard-4.0.0rc4/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/docs/features.rst` & `typeguard-4.0.0rc4/docs/features.rst`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 The following type checks are not yet supported in Typeguard:
 
 * Types of values assigned to class or instance variables
 * Types of values assigned to global or nonlocal variables
 * Stubs defined with :func:`@overload <typing.overload>` (the implementation is checked
   if instrumented)
 * ``yield_from`` statements in generator functions
-* ``ParamSpec`` is currently ignored
+* ``ParamSpec`` and ``Concatenate`` are currently ignored
+* Types where they are shadowed by arguments with the same name (e.g.
+  ``def foo(x: type, type: str): ...``)
 
 Other limitations
 -----------------
 
 Local references to nested classes
 ++++++++++++++++++++++++++++++++++
```

### Comparing `typeguard-4.0.0rc3/docs/userguide.rst` & `typeguard-4.0.0rc4/docs/userguide.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/docs/versionhistory.rst` & `typeguard-4.0.0rc4/docs/versionhistory.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.0.0rc4** (2023-04-15)
+
+- Fixed imports guarded by ``if TYPE_CHECKING:`` when used with subscripts
+  (``SomeType[...]``) being replaced with ``Any[...]`` instead of just ``Any``
+- Fixed instrumentation inadvertently mutating a function's annotations on Python 3.7
+  and 3.8
+- Fixed ``Concatenate[...]`` in ``Callable`` parameters causing ``TypeError`` to be
+  raised
+- Fixed type checks for ``*args`` or ``**kwargs`` not being suppressed when their types
+  are unusable (guarded by ``if TYPE_CHECKING:`` or otherwise)
+- Fixed ``TypeError`` when checking against a generic ``NewType``
+- Don't try to check types shadowed by argument names (e.g.
+  ``def foo(x: type, type: str): ...``)
+- Don't check against unions where one of the elements is ``Any``
+
 **4.0.0rc3** (2023-04-10)
 
 - Fixed ``typing.Literal`` subscript contents being evaluated as forward references
 - Fixed resolution of forward references in type aliases
 
 **4.0.0rc2** (2023-04-08)
```

### Comparing `typeguard-4.0.0rc3/pyproject.toml` & `typeguard-4.0.0rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 "Change log" = "https://typeguard.readthedocs.io/en/latest/versionhistory.html"
 "Source code" = "https://github.com/agronholm/typeguard"
 "Issue tracker" = "https://github.com/agronholm/typeguard/issues"
 
 [project.optional-dependencies]
 test = [
     "pytest >= 7",
-    'mypy >= 0.991; python_implementation != "PyPy"',
+    'mypy >= 1.2.0; python_implementation != "PyPy"',
 ]
 doc = [
     "packaging",
     "sphinx_rtd_theme",
     "sphinx-autodoc-typehints >= 1.2.0",
 ]
```

### Comparing `typeguard-4.0.0rc3/src/typeguard/__init__.py` & `typeguard-4.0.0rc4/src/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_checkers.py` & `typeguard-4.0.0rc4/src/typeguard/_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,17 @@
     if args:
         try:
             signature = inspect.signature(value)
         except (TypeError, ValueError):
             return
 
         argument_types = args[0]
-        if argument_types is not Ellipsis:
+        if isinstance(argument_types, list) and not any(
+            type(item) is ParamSpec for item in argument_types
+        ):
             # The callable must not have keyword-only arguments without defaults
             unfulfilled_kwonlyargs = [
                 param.name
                 for param in signature.parameters.values()
                 if param.kind == Parameter.KEYWORD_ONLY
                 and param.default == Parameter.empty
             ]
@@ -480,17 +482,15 @@
 
 def check_newtype(
     value: Any,
     origin_type: Any,
     args: tuple[Any, ...],
     memo: TypeCheckMemo,
 ) -> None:
-    supertype = origin_type.__supertype__
-    if not isinstance(value, supertype):
-        raise TypeCheckError(f"is not an instance of {qualified_name(supertype)}")
+    check_type_internal(value, origin_type.__supertype__, memo)
 
 
 def check_instance(
     value: Any,
     origin_type: Any,
     args: tuple[Any, ...],
     memo: TypeCheckMemo,
```

### Comparing `typeguard-4.0.0rc3/src/typeguard/_config.py` & `typeguard-4.0.0rc4/src/typeguard/_config.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_decorators.py` & `typeguard-4.0.0rc4/src/typeguard/_decorators.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_exceptions.py` & `typeguard-4.0.0rc4/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_functions.py` & `typeguard-4.0.0rc4/src/typeguard/_functions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_importhook.py` & `typeguard-4.0.0rc4/src/typeguard/_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_memo.py` & `typeguard-4.0.0rc4/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_pytest_plugin.py` & `typeguard-4.0.0rc4/src/typeguard/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_suppression.py` & `typeguard-4.0.0rc4/src/typeguard/_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_transformer.py` & `typeguard-4.0.0rc4/src/typeguard/_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     fix_missing_locations,
     keyword,
     walk,
 )
 from collections import defaultdict
 from collections.abc import Generator, Sequence
 from contextlib import contextmanager
-from copy import copy
+from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Any, ClassVar, cast, overload
 
 if sys.version_info >= (3, 8):
     from ast import NamedExpr
 
 generator_names = (
@@ -330,66 +330,101 @@
         "builtins.set": ("typing", "Set"),
         "builtins.frozenset": ("typing", "FrozenSet"),
     }
 
     def __init__(self, transformer: TypeguardTransformer):
         self.transformer = transformer
         self._memo = transformer._memo
-        self.level = 0
 
     def visit(self, node: AST) -> Any:
         new_node = super().visit(node)
         if isinstance(new_node, Expression) and not hasattr(new_node, "body"):
             return None
 
+        # Return None if this new node matches a variation of typing.Any
+        if isinstance(new_node, expr) and self._memo.name_matches(
+            new_node, *anytype_names
+        ):
+            return None
+
         return new_node
 
     def visit_BinOp(self, node: BinOp) -> Any:
-        self.level += 1
         self.generic_visit(node)
-        self.level -= 1
 
-        if sys.version_info < (3, 10) and isinstance(node.op, BitOr):
-            union_name = self.transformer._get_import("typing", "Union")
-            return Subscript(
-                value=union_name,
-                slice=Index(
-                    Tuple(elts=[node.left, node.right], ctx=Load()), ctx=Load()
-                ),
-                ctx=Load(),
-            )
+        if isinstance(node.op, BitOr):
+            # If either side of the operation resolved to None, return None
+            if not hasattr(node, "left") or not hasattr(node, "right"):
+                return None
+
+            if sys.version_info < (3, 10):
+                union_name = self.transformer._get_import("typing", "Union")
+                return Subscript(
+                    value=union_name,
+                    slice=Index(
+                        Tuple(elts=[node.left, node.right], ctx=Load()), ctx=Load()
+                    ),
+                    ctx=Load(),
+                )
 
         return node
 
     def visit_Attribute(self, node: Attribute) -> Any:
         if self._memo.is_ignored_name(node):
-            if self.level > 0:
-                return self.transformer._get_import("typing", "Any")
-            else:
-                return None
+            return None
 
         return node
 
     def visit_Subscript(self, node: Subscript) -> Any:
-        self.level += 1
+        if self._memo.is_ignored_name(node.value):
+            return None
 
         # The subscript of typing(_extensions).Literal can be any arbitrary string, so
         # don't try to evaluate it as code
-        if not self._memo.name_matches(node.value, *literal_names):
-            self.generic_visit(node)
+        if not self._memo.name_matches(node.value, *literal_names) and node.slice:
+            if isinstance(node.slice, Index):
+                # Python 3.7 and 3.8
+                slice_value = node.slice.value  # type: ignore[attr-defined]
+            else:
+                slice_value = node.slice
+
+            if isinstance(slice_value, Tuple):
+                items = [self.visit(item) for item in slice_value.elts]
+
+                # If this is a Union and any of the items is None, erase the entire
+                # annotation
+                if self._memo.name_matches(node.value, "typing.Union") and any(
+                    item is None for item in items
+                ):
+                    return None
+
+                # If all items in the subscript were Any, erase the subscript entirely
+                if all(item is None for item in items):
+                    return node.value
+
+                for index, item in enumerate(items):
+                    if item is None:
+                        items[index] = self.transformer._get_import("typing", "Any")
+
+                slice_value.elts = items
+            else:
+                self.generic_visit(node)
+
+                # If the transformer erased the slice entirely, just return the node
+                # value without the subscript
+                if sys.version_info >= (3, 9) and not hasattr(node, "slice"):
+                    return node.value
+                elif sys.version_info < (3, 9) and not hasattr(node.slice, "value"):
+                    return node.value
 
-        self.level -= 1
         return node
 
     def visit_Name(self, node: Name) -> Any:
         if self._memo.is_ignored_name(node):
-            if self.level > 0:
-                return self.transformer._get_import("typing", "Any")
-            else:
-                return None
+            return None
 
         if sys.version_info < (3, 9):
             for typename, substitute in self.type_substitutions.items():
                 if self._memo.name_matches(node, typename):
                     new_node = self.transformer._get_import(*substitute)
                     return copy_location(new_node, node)
 
@@ -438,15 +473,15 @@
             if new_memo.should_instrument:
                 # Check if the function is a generator function
                 detector = GeneratorDetector()
                 detector.visit(node)
 
                 # Extract yield, send and return types where possible from a subscripted
                 # annotation like Generator[int, str, bool]
-                return_annotation = copy(node.returns)
+                return_annotation = deepcopy(node.returns)
                 if detector.contains_yields and new_memo.name_matches(
                     return_annotation, *generator_names
                 ):
                     if isinstance(return_annotation, Subscript):
                         annotation_slice = return_annotation.slice
 
                         # Python < 3.9
@@ -611,60 +646,77 @@
                                 kw.arg: kw.value for kw in decorator.keywords if kw.arg
                             }
 
                 all_args = node.args.args + node.args.kwonlyargs
                 if sys.version_info >= (3, 8):
                     all_args.extend(node.args.posonlyargs)
 
+                # Ensure that any type shadowed by the positional or keyword-only
+                # argument names are ignored in this function
+                for arg in all_args:
+                    self._memo.ignored_names.add(arg.arg)
+
+                # Ensure that any type shadowed by the variable positional argument name
+                # (e.g. "args" in *args) is ignored this function
+                if node.args.vararg:
+                    self._memo.ignored_names.add(node.args.vararg.arg)
+
+                # Ensure that any type shadowed by the variable keywrod argument name
+                # (e.g. "kwargs" in *kwargs) is ignored this function
+                if node.args.kwarg:
+                    self._memo.ignored_names.add(node.args.kwarg.arg)
+
                 for arg in all_args:
-                    annotation = self._convert_annotation(copy(arg.annotation))
-                    if annotation and not self._memo.name_matches(
-                        annotation, *anytype_names
-                    ):
+                    annotation = self._convert_annotation(deepcopy(arg.annotation))
+                    if annotation:
                         arg_annotations[arg.arg] = annotation
 
-                if node.args.vararg and node.args.vararg.annotation:
-                    if sys.version_info >= (3, 9):
-                        container = Name("tuple", ctx=Load())
-                    else:
-                        container = self._get_import("typing", "Tuple")
+                if node.args.vararg:
+                    annotation_ = self._convert_annotation(node.args.vararg.annotation)
+                    if annotation_:
+                        if sys.version_info >= (3, 9):
+                            container = Name("tuple", ctx=Load())
+                        else:
+                            container = self._get_import("typing", "Tuple")
 
-                    subscript_slice: Tuple | Index = Tuple(
-                        [
-                            self._convert_annotation(node.args.vararg.annotation),
-                            Constant(Ellipsis),
-                        ],
-                        ctx=Load(),
-                    )
-                    if sys.version_info < (3, 9):
-                        subscript_slice = Index(subscript_slice, ctx=Load())
+                        subscript_slice: Tuple | Index = Tuple(
+                            [
+                                annotation_,
+                                Constant(Ellipsis),
+                            ],
+                            ctx=Load(),
+                        )
+                        if sys.version_info < (3, 9):
+                            subscript_slice = Index(subscript_slice, ctx=Load())
 
-                    arg_annotations[node.args.vararg.arg] = Subscript(
-                        container, subscript_slice, ctx=Load()
-                    )
+                        arg_annotations[node.args.vararg.arg] = Subscript(
+                            container, subscript_slice, ctx=Load()
+                        )
 
-                if node.args.kwarg and node.args.kwarg.annotation:
-                    if sys.version_info >= (3, 9):
-                        container = Name("dict", ctx=Load())
-                    else:
-                        container = self._get_import("typing", "Dict")
+                if node.args.kwarg:
+                    annotation_ = self._convert_annotation(node.args.kwarg.annotation)
+                    if annotation_:
+                        if sys.version_info >= (3, 9):
+                            container = Name("dict", ctx=Load())
+                        else:
+                            container = self._get_import("typing", "Dict")
 
-                    subscript_slice = Tuple(
-                        [
-                            Name("str", ctx=Load()),
-                            self._convert_annotation(node.args.kwarg.annotation),
-                        ],
-                        ctx=Load(),
-                    )
-                    if sys.version_info < (3, 9):
-                        subscript_slice = Index(subscript_slice, ctx=Load())
+                        subscript_slice = Tuple(
+                            [
+                                Name("str", ctx=Load()),
+                                annotation_,
+                            ],
+                            ctx=Load(),
+                        )
+                        if sys.version_info < (3, 9):
+                            subscript_slice = Index(subscript_slice, ctx=Load())
 
-                    arg_annotations[node.args.kwarg.arg] = Subscript(
-                        container, subscript_slice, ctx=Load()
-                    )
+                        arg_annotations[node.args.kwarg.arg] = Subscript(
+                            container, subscript_slice, ctx=Load()
+                        )
 
                 if arg_annotations:
                     self._memo.variable_annotations.update(arg_annotations)
 
             self.generic_visit(node)
 
             if arg_annotations:
@@ -685,17 +737,14 @@
                 ]
                 node.body.insert(0, Expr(Call(func_name, args, [])))
 
             # Add a checked "return None" to the end if there's no explicit return
             # Skip if the return annotation is None or Any
             if (
                 self._memo.return_annotation
-                and not self._memo.name_matches(
-                    self._memo.return_annotation, *anytype_names
-                )
                 and (not self._memo.is_async or not self._memo.has_yield_expressions)
                 and not isinstance(node.body[-1], Return)
                 and (
                     not isinstance(self._memo.return_annotation, Constant)
                     or self._memo.return_annotation.value is not None
                 )
             ):
@@ -802,17 +851,15 @@
 
     def visit_Return(self, node: Return) -> Return:
         """This injects type checks into "return" statements."""
         self.generic_visit(node)
         if (
             self._memo.return_annotation
             and self._memo.should_instrument
-            and not self._memo.name_matches(
-                self._memo.return_annotation, *anytype_names
-            )
+            and not self._memo.is_ignored_name(self._memo.return_annotation)
         ):
             func_name = self._get_import("typeguard._functions", "check_return_type")
             old_node = node
             retval = old_node.value or Constant(None)
             node = Return(
                 Call(
                     func_name,
@@ -838,15 +885,15 @@
         self._memo.has_yield_expressions = True
         self.generic_visit(node)
 
         self.generic_visit(node)
         if (
             self._memo.yield_annotation
             and self._memo.should_instrument
-            and not self._memo.name_matches(self._memo.yield_annotation, *anytype_names)
+            and not self._memo.is_ignored_name(self._memo.yield_annotation)
         ):
             func_name = self._get_import("typeguard._functions", "check_yield_type")
             yieldval = node.value or Constant(None)
             node.value = Call(
                 func_name,
                 [
                     self._memo.joined_path,
@@ -856,15 +903,15 @@
                 ],
                 [],
             )
 
         if (
             self._memo.send_annotation
             and self._memo.should_instrument
-            and not self._memo.name_matches(self._memo.send_annotation, *anytype_names)
+            and not self._memo.is_ignored_name(self._memo.send_annotation)
         ):
             func_name = self._get_import("typeguard._functions", "check_send_type")
             old_node = node
             call_node = Call(
                 func_name,
                 [
                     self._memo.joined_path,
@@ -888,20 +935,18 @@
         self.generic_visit(node)
 
         if (
             isinstance(self._memo.node, (FunctionDef, AsyncFunctionDef))
             and node.annotation
             and isinstance(node.target, Name)
         ):
-            annotation = self._convert_annotation(copy(node.annotation))
+            annotation = self._convert_annotation(deepcopy(node.annotation))
             if annotation:
                 self._memo.variable_annotations[node.target.id] = annotation
-                if node.value and not self._memo.name_matches(
-                    annotation, *anytype_names
-                ):
+                if node.value:
                     func_name = self._get_import(
                         "typeguard._functions", "check_variable_assignment"
                     )
                     node.value = Call(
                         func_name,
                         [
                             node.value,
```

### Comparing `typeguard-4.0.0rc3/src/typeguard/_union_transformer.py` & `typeguard-4.0.0rc4/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard/_utils.py` & `typeguard-4.0.0rc4/src/typeguard/_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.0.0rc4/src/typeguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc3
+Version: 4.0.0rc4
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc3/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.0.0rc4/src/typeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/__init__.py` & `typeguard-4.0.0rc4/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 class Employee(NamedTuple):
     name: str
     id: int
 
 
 JSONType = Union[str, float, bool, None, List["JSONType"], Dict[str, "JSONType"]]
 myint = NewType("myint", int)
+mylist = NewType("mylist", List[int])
 
 
 class FooGeneric(Generic[T_Foo]):
     pass
 
 
 class Parent:
```

### Comparing `typeguard-4.0.0rc3/tests/conftest.py` & `typeguard-4.0.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/dummymodule.py` & `typeguard-4.0.0rc4/tests/dummymodule.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,22 +66,14 @@
 
 
 @typeguard_ignore
 def non_typeguard_checked_func(x: int, y: str) -> 6:
     return "foo"
 
 
-def dynamic_type_checking_func(arg, argtype, return_annotation):
-    @typechecked
-    def inner(x: argtype) -> return_annotation:
-        return str(x)
-
-    return inner(arg)
-
-
 class Metaclass(type):
     pass
 
 
 @typechecked
 class DummyClass(metaclass=Metaclass):
     def type_checked_method(self, x: int, y: int) -> int:
@@ -312,21 +304,40 @@
 def typed_variable_args(
     *args: str, **kwargs: int
 ) -> Tuple[Tuple[str, ...], Dict[str, int]]:
     return args, kwargs
 
 
 @typechecked
-def guarded_type_hint(x: "Imaginary") -> "Imaginary":
+def guarded_type_hint_plain(x: "Imaginary") -> "Imaginary":
     y: Imaginary = x
     return y
 
 
 @typechecked
+def guarded_type_hint_subscript_toplevel(x: "Imaginary[int]") -> "Imaginary[int]":
+    y: Imaginary[int] = x
+    return y
+
+
+@typechecked
+def guarded_type_hint_subscript_nested(
+    x: List["Imaginary[int]"],
+) -> List["Imaginary[int]"]:
+    y: List[Imaginary[int]] = x
+    return y
+
+
+@typechecked
 def literal(x: Literal["foo"]) -> Literal["foo"]:
     y: Literal["foo"] = x
     return y
 
 
 @typechecked
 def typevar_forwardref(x: Type[T]) -> T:
     return x()
+
+
+def never_called(x: List["NonExistentType"]) -> List["NonExistentType"]:  # noqa: F821
+    """Regression test for #335."""
+    return x
```

### Comparing `typeguard-4.0.0rc3/tests/mypy/negative.py` & `typeguard-4.0.0rc4/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/mypy/positive.py` & `typeguard-4.0.0rc4/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/mypy/test_type_annotations.py` & `typeguard-4.0.0rc4/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_checkers.py` & `typeguard-4.0.0rc4/tests/test_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,39 +49,42 @@
     RuntimeProtocol,
     StaticProtocol,
     TChild,
     TIntStr,
     TParent,
     TTypingConstrained,
     myint,
+    mylist,
 )
 
 if sys.version_info >= (3, 11):
     from typing import LiteralString
 
     SubclassableAny = Any
 else:
     from typing_extensions import Any as SubclassableAny
     from typing_extensions import LiteralString
 
 if sys.version_info >= (3, 10):
-    from typing import TypeGuard
+    from typing import Concatenate, ParamSpec, TypeGuard
 else:
-    from typing_extensions import TypeGuard
+    from typing_extensions import Concatenate, ParamSpec, TypeGuard
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 if sys.version_info >= (3, 8):
     from typing import Literal, TypedDict
 else:
     from typing_extensions import Literal, TypedDict
 
+P = ParamSpec("P")
+
 
 class TestAnyStr:
     @pytest.mark.parametrize(
         "value", [pytest.param("bar", id="str"), pytest.param(b"bar", id="bytes")]
     )
     def test_valid(self, value):
         check_type(value, AnyStr)
@@ -253,14 +256,18 @@
         """
         Test that checking a Callable annotation against a builtin callable does not
         raise an error.
 
         """
         check_type([].append, Callable[[int], Any])
 
+    def test_concatenate(self):
+        """Test that ``Concatenate`` in the arglist is ignored."""
+        check_type([].append, Callable[Concatenate[object, P], Any])
+
 
 class TestLiteral:
     def test_literal_union(self):
         annotation = Union[str, Literal[1, 6, 8]]
         check_type(6, annotation)
         pytest.raises(TypeCheckError, check_type, 4, annotation).match(
             r"int did not match any element in the union:\n"
@@ -747,22 +754,30 @@
     def test_constraints_fail(self):
         pytest.raises(TypeCheckError, check_type, 2.5, TIntStr).match(
             r"float does not match any of the constraints \(int, str\)"
         )
 
 
 class TestNewType:
-    def test_valid(self):
+    def test_simple_valid(self):
         check_type(1, myint)
 
-    def test_bad_value(self):
+    def test_simple_bad_value(self):
         pytest.raises(TypeCheckError, check_type, "a", myint).match(
             r"str is not an instance of int"
         )
 
+    def test_generic_valid(self):
+        check_type([1], mylist)
+
+    def test_generic_bad_value(self):
+        pytest.raises(TypeCheckError, check_type, ["a"], mylist).match(
+            r"item 0 of list is not an instance of int"
+        )
+
 
 class TestType:
     @pytest.mark.parametrize("annotation", [pytest.param(Type), pytest.param(type)])
     def test_unparametrized(self, annotation: Any):
         check_type(TestNewType, annotation)
 
     @pytest.mark.parametrize("annotation", [pytest.param(Type), pytest.param(type)])
```

### Comparing `typeguard-4.0.0rc3/tests/test_importhook.py` & `typeguard-4.0.0rc4/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_instrumentation.py` & `typeguard-4.0.0rc4/tests/test_instrumentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 
 @pytest.fixture(scope="module")
 def dummymodule(method: str):
     config.debug_instrumentation = True
     sys.path.insert(0, str(this_dir))
     try:
+        sys.modules.pop("dummymodule", None)
         if cached_module_path.exists():
             cached_module_path.unlink()
-            sys.modules.pop("dummymodule", None)
 
         if method == "typechecked":
             return import_module("dummymodule")
 
         with install_import_hook(["dummymodule"]):
             with warnings.catch_warnings():
                 warnings.filterwarnings("error", module="typeguard")
@@ -93,37 +93,14 @@
 
 def test_type_checked_staticmethod(dummymodule):
     pytest.raises(
         TypeCheckError, dummymodule.DummyClass.type_checked_staticmethod, "bah", 9
     ).match(r'argument "x" \(str\) is not an instance of int')
 
 
-@pytest.mark.parametrize(
-    "argtype, returntype, error",
-    [
-        (int, str, None),
-        (str, str, r'argument "x" \(int\) is not an instance of str'),
-        (int, int, r"the return value \(str\) is not an instance of int"),
-    ],
-    ids=["correct", "bad_argtype", "bad_returntype"],
-)
-def test_dynamic_type_checking_func(dummymodule, argtype, returntype, error):
-    if error:
-        exc = pytest.raises(
-            TypeCheckError,
-            dummymodule.dynamic_type_checking_func,
-            4,
-            argtype,
-            returntype,
-        )
-        exc.match(error)
-    else:
-        assert dummymodule.dynamic_type_checking_func(4, argtype, returntype) == "4"
-
-
 @pytest.mark.xfail(reason="No workaround for this has been implemented yet")
 def test_inner_class_method(dummymodule):
     retval = dummymodule.Outer().create_inner()
     assert retval.__class__.__qualname__ == "Outer.Inner"
 
 
 @pytest.mark.xfail(reason="No workaround for this has been implemented yet")
@@ -328,16 +305,23 @@
             TypeCheckError,
             match=r'value of key \'a\' of argument "kwargs" \(dict\) is not an '
             r"instance of int",
         ):
             dummymodule.typed_variable_args("foo", "bar", a="baz")
 
 
-def test_guarded_type(dummymodule):
-    assert dummymodule.guarded_type_hint("foo") == "foo"
+class TestGuardedType:
+    def test_plain(self, dummymodule):
+        assert dummymodule.guarded_type_hint_plain("foo") == "foo"
+
+    def test_subscript_toplevel(self, dummymodule):
+        assert dummymodule.guarded_type_hint_subscript_toplevel("foo") == "foo"
+
+    def test_subscript_nested(self, dummymodule):
+        assert dummymodule.guarded_type_hint_subscript_nested(["foo"]) == ["foo"]
 
 
 def test_literal(dummymodule):
     assert dummymodule.literal("foo") == "foo"
 
 
 def test_typevar_forwardref(dummymodule):
```

### Comparing `typeguard-4.0.0rc3/tests/test_plugins.py` & `typeguard-4.0.0rc4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_suppression.py` & `typeguard-4.0.0rc4/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_transformer.py` & `typeguard-4.0.0rc4/tests/test_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,14 +344,64 @@
             def foo(x, y: {annotation}) -> {annotation}:
                 return 1
             """
         ).strip()
     )
 
 
+def test_any_in_union() -> None:
+    node = parse(
+        dedent(
+            """
+            from typing import Any, Union
+
+            def foo(x, y: Union[Any, None]) -> Union[Any, None]:
+                return 1
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from typing import Any, Union
+
+            def foo(x, y: Union[Any, None]) -> Union[Any, None]:
+                return 1
+            """
+        ).strip()
+    )
+
+
+def test_any_in_pep_604_union() -> None:
+    node = parse(
+        dedent(
+            """
+            from typing import Any
+
+            def foo(x, y: Any | None) -> Any | None:
+                return 1
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from typing import Any
+
+            def foo(x, y: Any | None) -> Any | None:
+                return 1
+            """
+        ).strip()
+    )
+
+
 def test_avoid_global_names() -> None:
     node = parse(
         dedent(
             """
             memo = TypeCheckMemo = check_argument_types = check_return_type = None
 
             def func1(x: int) -> int:
@@ -738,15 +788,16 @@
             dedent(
                 """
                 from typing import TYPE_CHECKING
                 if TYPE_CHECKING:
                     import typing
                     from typing import Hashable, Sequence
 
-                def foo(x: Hashable, y: typing.Collection) -> Sequence:
+                def foo(x: Hashable, y: typing.Collection, *args: Hashable, \
+**kwargs: typing.Collection) -> Sequence:
                     bar: typing.Collection
                     baz: Hashable = 1
                     return (1, 2)
                 """
             )
         )
         TypeguardTransformer().visit(node)
@@ -755,15 +806,16 @@
             == dedent(
                 """
                 from typing import TYPE_CHECKING
                 if TYPE_CHECKING:
                     import typing
                     from typing import Hashable, Sequence
 
-                def foo(x: Hashable, y: typing.Collection) -> Sequence:
+                def foo(x: Hashable, y: typing.Collection, *args: Hashable, \
+**kwargs: typing.Collection) -> Sequence:
                     bar: typing.Collection
                     baz: Hashable = 1
                     return (1, 2)
                 """
             ).strip()
         )
 
@@ -783,23 +835,22 @@
         TypeguardTransformer().visit(node)
         assert (
             unparse(node)
             == dedent(
                 """
                 from typeguard import TypeCheckMemo
                 from typeguard._functions import check_argument_types, check_return_type
-                from typing import Any
                 from typing import TYPE_CHECKING
                 if TYPE_CHECKING:
                     from nonexistent import FooBar
 
                 def foo(x: list[FooBar]) -> list[FooBar]:
                     memo = TypeCheckMemo(globals(), locals())
-                    check_argument_types('foo', {'x': (x, list[Any])}, memo)
-                    return check_return_type('foo', x, list[Any], memo)
+                    check_argument_types('foo', {'x': (x, list)}, memo)
+                    return check_return_type('foo', x, list, memo)
                 """
             ).strip()
         )
 
     def test_variable_annotations(self) -> None:
         node = parse(
             dedent(
@@ -824,15 +875,15 @@
                 from typing import Any, TYPE_CHECKING
                 if TYPE_CHECKING:
                     from nonexistent import FooBar
 
                 def foo(x: Any) -> None:
                     memo = TypeCheckMemo(globals(), locals())
                     y: FooBar = x
-                    z: list[FooBar] = check_variable_assignment([y], 'z', list[Any], \
+                    z: list[FooBar] = check_variable_assignment([y], 'z', list, \
 memo)
                 """
             ).strip()
         )
 
     def test_generator_function(self) -> None:
         node = parse(
@@ -1231,7 +1282,36 @@
                 def foo(x: int) -> None:
                     memo = TypeCheckMemo(globals(), locals())
                     check_argument_types('foo', {'x': (x, int)}, memo)
                     x = check_variable_assignment(iadd(x, 6), 'x', int, memo)
                 """
             ).strip()
         )
+
+
+def test_argname_typename_conflicts() -> None:
+    node = parse(
+        dedent(
+            """
+            from collections.abc import Generator
+
+            def foo(x: kwargs, /, y: args, *args: x, baz: x, **kwargs: y) -> \
+Generator[args, x, kwargs]:
+                yield y
+                return x
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from collections.abc import Generator
+
+            def foo(x: kwargs, /, y: args, *args: x, baz: x, **kwargs: y) -> \
+Generator[args, x, kwargs]:
+                yield y
+                return x
+            """
+        ).strip()
+    )
```

### Comparing `typeguard-4.0.0rc3/tests/test_typechecked.py` & `typeguard-4.0.0rc4/tests/test_typechecked.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_union_transformer.py` & `typeguard-4.0.0rc4/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_utils.py` & `typeguard-4.0.0rc4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc3/tests/test_warn_on_error.py` & `typeguard-4.0.0rc4/tests/test_warn_on_error.py`

 * *Files identical despite different names*

