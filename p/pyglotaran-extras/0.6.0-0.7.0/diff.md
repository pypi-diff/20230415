# Comparing `tmp/pyglotaran_extras-0.6.0.tar.gz` & `tmp/pyglotaran_extras-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglotaran_extras-0.6.0.tar", last modified: Tue Jun  7 20:16:18 2022, max compression
+gzip compressed data, was "pyglotaran_extras-0.7.0.tar", last modified: Sat Apr 15 19:53:14 2023, max compression
```

## Comparing `pyglotaran_extras-0.6.0.tar` & `pyglotaran_extras-0.7.0.tar`

### file list

```diff
@@ -1,74 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.624223 pyglotaran_extras-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.620223 pyglotaran_extras-0.6.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.624223 pyglotaran_extras-0.6.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/api_docs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.624223 pyglotaran_extras-0.6.0/pyglotaran_extras/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.624223 pyglotaran_extras-0.6.0/pyglotaran_extras/deprecation/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/deprecation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4767 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/deprecation/deprecation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.624223 pyglotaran_extras-0.6.0/pyglotaran_extras/io/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/io/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/io/load_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/io/setup_case_study.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_concentrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_doas.py
--rw-r--r--   0 runner    (1001) docker     (121)     8009 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_overview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_residual.py
--rw-r--r--   0 runner    (1001) docker     (121)     4256 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_spectra.py
--rw-r--r--   0 runner    (1001) docker     (121)    10131 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_svd.py
--rw-r--r--   0 runner    (1001) docker     (121)     7383 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_traces.py
--rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/style.py
--rw-r--r--   0 runner    (1001) docker     (121)     8553 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyglotaran_extras/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.624223 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-06-07 20:16:18.000000 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-06-07 20:16:18.000000 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 20:16:18.000000 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-07 20:16:18.000000 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-07 20:16:18.000000 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 20:16:18.000000 pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/tests/deprecation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/deprecation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/tests/deprecation/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/deprecation/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/deprecation/modules/test_io_boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/deprecation/modules/test_plotting_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5214 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/deprecation/test_deprecation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/tests/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/io/test_get_script_dir.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/io/test_setup_case_study.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 20:16:18.628223 pyglotaran_extras-0.6.0/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-06-07 20:16:13.000000 pyglotaran_extras-0.6.0/tests/plotting/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.204531 pyglotaran_extras-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.200531 pyglotaran_extras-0.7.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/pyglotaran_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/deprecation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.212531 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/a_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.212531 pyglotaran_extras-0.7.0/pyglotaran_extras/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/setup_case_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.212531 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_coherent_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_concentrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_doas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_irf_dispersion_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-15 19:53:14.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.204531 pyglotaran_extras-0.7.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/data/a_matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_decimal_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_default.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_normalized.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_decimal_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_default.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_expanded_dataset_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_heading_offset_0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_min_size_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_multiple_a_matrixes_in_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_normalized.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/deprecation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/deprecation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/deprecation/test_deprecation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/inspect/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/inspect/test_a_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/inspect/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/test_get_script_dir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/test_setup_case_study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/plotting/test_utils.py
```

### Comparing `pyglotaran_extras-0.6.0/CONTRIBUTING.rst` & `pyglotaran_extras-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/LICENSE` & `pyglotaran_extras-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/PKG-INFO` & `pyglotaran_extras-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglotaran_extras
-Version: 0.6.0
+Version: 0.7.0
 Summary: Supplementary package for pyglotaran with (example) plotting code.
 Home-page: https://github.com/glotaran/pyglotaran-extras
 Author: Joris Snellenburg
 Author-email: j.snellenburg@gmail.com
 License: MIT
 Project-URL: GloTarAn Ecosystem, https://glotaran.org
 Project-URL: Documentation, https://pyglotaran-extras.readthedocs.io
@@ -41,15 +41,15 @@
         ```console
         pip install pyglotaran-extras
         ```
         
         If you want to install it via conda, you can run the following command:
         
         ```console
-        conda install pyglotaran-extras
+        conda install -c conda-forge pyglotaran-extras
         ```
         
         ### From Source
         
         To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
         
         ```console
```

### Comparing `pyglotaran_extras-0.6.0/README.md` & `pyglotaran_extras-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```console
 pip install pyglotaran-extras
 ```
 
 If you want to install it via conda, you can run the following command:
 
 ```console
-conda install pyglotaran-extras
+conda install -c conda-forge pyglotaran-extras
 ```
 
 ### From Source
 
 To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
 
 ```console
```

### Comparing `pyglotaran_extras-0.6.0/docs/Makefile` & `pyglotaran_extras-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/docs/_templates/autosummary/class.rst` & `pyglotaran_extras-0.7.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/docs/_templates/autosummary/module.rst` & `pyglotaran_extras-0.7.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/docs/conf.py` & `pyglotaran_extras-0.7.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
     "myst_parser",
+    "sphinx_rtd_theme",
 ]
 
 
 autoclass_content = "both"
 autosummary_generate = True
 add_module_names = False
 autodoc_member_order = "bysource"
```

### Comparing `pyglotaran_extras-0.6.0/docs/installation.rst` & `pyglotaran_extras-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/docs/make.bat` & `pyglotaran_extras-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/__init__.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 """Pyglotaran extension package with convenience functionality such as plotting."""
 from pyglotaran_extras.io.load_data import load_data
 from pyglotaran_extras.io.setup_case_study import setup_case_study
+from pyglotaran_extras.plotting.plot_coherent_artifact import plot_coherent_artifact
 from pyglotaran_extras.plotting.plot_data import plot_data_overview
+from pyglotaran_extras.plotting.plot_doas import plot_doas
+from pyglotaran_extras.plotting.plot_guidance import plot_guidance
+from pyglotaran_extras.plotting.plot_irf_dispersion_center import plot_irf_dispersion_center
 from pyglotaran_extras.plotting.plot_overview import plot_overview
 from pyglotaran_extras.plotting.plot_overview import plot_simple_overview
 from pyglotaran_extras.plotting.plot_traces import plot_fitted_traces
 from pyglotaran_extras.plotting.plot_traces import select_plot_wavelengths
 
 __all__ = [
     "load_data",
     "setup_case_study",
+    "plot_coherent_artifact",
     "plot_data_overview",
+    "plot_doas",
+    "plot_guidance",
+    "plot_irf_dispersion_center",
     "plot_overview",
     "plot_simple_overview",
     "plot_fitted_traces",
     "select_plot_wavelengths",
 ]
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/deprecation/deprecation_utils.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/deprecation_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Module containing deprecation functionality."""
 from __future__ import annotations
 
 from importlib.metadata import distribution
 from warnings import warn
 
 FIG_ONLY_WARNING = (
-    "In the future plot functions which create figures, will return a tuple "
-    "of Figure AND the Axes. Please set ``figure_only=False`` and adjust your code.\n"
-    "This usage will be an error in version: 0.7.0."
+    "The ``figure_only`` argument was deprecated please remove it from the function call.\n"
+    "This usage will be an error in version: 0.8.0."
 )
 
 
 class OverDueDeprecation(Exception):
     """Error thrown when a deprecation should have been removed.
 
     See Also
@@ -36,15 +35,15 @@
 def pyglotaran_extras_version() -> str:
     """Version of the distribution.
 
     This is basically the same as ``pyglotaran_extras.__version__`` but independent
     from pyglotaran_extras.
     This way all of the deprecation functionality can be used even in
     ``pyglotaran_extras.__init__.py`` without moving the import below the definition of
-    ``__version__`` or causeing a circular import issue.
+    ``__version__`` or causing a circular import issue.
 
     Returns
     -------
     str
         The version string.
     """
     return distribution("pyglotaran-extras").version
@@ -77,16 +76,16 @@
     split_version = version_str.partition("-")[0].split(".")
     if len(split_version) < 3:
         raise ValueError(error_message)
     try:
         return tuple(
             map(int, (*split_version[:2], split_version[2].partition("rc")[0]))
         )  # type:ignore[return-value]
-    except ValueError:
-        raise ValueError(error_message)
+    except ValueError as error:
+        raise ValueError(error_message) from error
 
 
 def check_overdue(deprecated_qual_name_usage: str, to_be_removed_in_version: str) -> None:
     """Check if a deprecation is overdue for removal.
 
     Parameters
     ----------
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/io/load_data.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/io/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-"""Data loading utility module."""
+"""Io utility module."""
 from __future__ import annotations
 
+from collections.abc import Mapping
+from collections.abc import Sequence
 from pathlib import Path
 
 import xarray as xr
-from glotaran.io import load_dataset
 from glotaran.project.result import Result
 
-from pyglotaran_extras.types import DatasetConvertible
+from pyglotaran_extras.io.load_data import load_data
+from pyglotaran_extras.types import ResultLike
 
 
-def load_data(result: DatasetConvertible, dataset_name: str | None = None) -> xr.Dataset:
-    """Extract a single dataset from a :class:`DatasetConvertible` object.
+def result_dataset_mapping(result: ResultLike) -> Mapping[str, xr.Dataset]:
+    """Convert a ``ResultLike`` object to a per dataset mapping of result like data.
 
     Parameters
     ----------
-    result : DatasetConvertible
-        Result class instance, xarray Dataset or path to a dataset file.
-    dataset_name : str, optional
-        Name of a specific dataset contained in ``result``, if not provided
-        the first dataset will be extracted. Defaults to None.
+    result : ResultLike
+        Data structure which can be converted to a mapping.
 
     Returns
     -------
-    xr.Dataset
-        Extracted dataset.
+    Mapping[str, Dataset]
+        Per dataset mapping of result like data.
 
     Raises
     ------
     TypeError
-        If ``result`` isn't a :class:`DatasetConvertible` object.
+        If any value of a ``result`` isn't of :class:`DatasetConvertible`.
+    TypeError
+        If ``result`` isn't a :class:`ResultLike` object.
     """
-    if isinstance(result, xr.Dataset):
-        return result
-    if isinstance(result, xr.DataArray):
-        return result.to_dataset(name="data")
+    result_mapping = {}
     if isinstance(result, Result):
-        if dataset_name is not None:
-            return result.data[dataset_name]
-        keys = list(result.data)
-        return result.data[keys[0]]
-    if isinstance(result, (str, Path)):
-        return load_data(load_dataset(result))
-    raise TypeError(f"Result needs to be of type {DatasetConvertible!r}, but was {result!r}.")
+        return result.data
+    if isinstance(result, (xr.Dataset, xr.DataArray, Path, str)):
+        return {"dataset": load_data(result)}
+    if isinstance(result, Sequence):
+        for index, value in enumerate(result):
+            result_mapping[f"dataset{index}"] = load_data(value)
+        return result_mapping
+    if isinstance(result, Mapping):
+        for key, value in result.items():
+            result_mapping[key] = load_data(value)
+        return result_mapping
+    raise TypeError(f"Result needs to be of type {ResultLike!r}, but was {result!r}.")
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/io/setup_case_study.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/io/setup_case_study.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_concentrations.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_overview.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_traces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,217 +1,207 @@
-"""Module containing overview plotting functionality."""
+"""Module containing functionality to plot fitted traces."""
 from __future__ import annotations
 
-from pathlib import Path
 from typing import TYPE_CHECKING
 from warnings import warn
 
 import matplotlib.pyplot as plt
 
-from pyglotaran_extras.deprecation.deprecation_utils import FIG_ONLY_WARNING
-from pyglotaran_extras.deprecation.deprecation_utils import PyglotaranExtrasApiDeprecationWarning
-from pyglotaran_extras.io.load_data import load_data
-from pyglotaran_extras.plotting.plot_concentrations import plot_concentrations
-from pyglotaran_extras.plotting.plot_residual import plot_residual
-from pyglotaran_extras.plotting.plot_spectra import plot_spectra
-from pyglotaran_extras.plotting.plot_svd import plot_svd
+from pyglotaran_extras.io.utils import result_dataset_mapping
 from pyglotaran_extras.plotting.style import PlotStyle
+from pyglotaran_extras.plotting.utils import PlotDuplicationWarning
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
+from pyglotaran_extras.plotting.utils import add_unique_figure_legend
+from pyglotaran_extras.plotting.utils import extract_dataset_scale
+from pyglotaran_extras.plotting.utils import extract_irf_location
+from pyglotaran_extras.plotting.utils import select_plot_wavelengths
+
+__all__ = ["select_plot_wavelengths", "plot_fitted_traces"]
 
 if TYPE_CHECKING:
+    from typing import Iterable
+
     from cycler import Cycler
+    from matplotlib.axis import Axis
     from matplotlib.figure import Figure
     from matplotlib.pyplot import Axes
 
-    from pyglotaran_extras.types import DatasetConvertible
+    from pyglotaran_extras.types import ResultLike
 
 
-def plot_overview(
-    result: DatasetConvertible,
+def plot_data_and_fits(
+    result: ResultLike,
+    wavelength: float,
+    axis: Axis,
     center_λ: float | None = None,
-    linlog: bool = True,
-    linthresh: float = 1,
-    linscale: float = 1,
-    show_data: bool = False,
     main_irf_nr: int = 0,
-    figsize: tuple[int, int] = (18, 16),
-    cycler: Cycler | None = PlotStyle().cycler,
-    figure_only: bool = True,
-    nr_of_data_svd_vectors: int = 4,
-    nr_of_residual_svd_vectors: int = 2,
-    show_data_svd_legend: bool = True,
-    show_residual_svd_legend: bool = True,
-) -> Figure | tuple[Figure, Axes]:
-    """Plot overview of the optimization result.
+    linlog: bool = False,
+    linthresh: float = 1,
+    divide_by_scale: bool = True,
+    per_axis_legend: bool = False,
+    y_label: str = "a.u.",
+    cycler: Cycler | None = PlotStyle().data_cycler_solid,
+    show_zero_line: bool = True,
+) -> None:
+    """Plot data and fits for a given ``wavelength`` on a given ``axis``.
+
+    If the wavelength isn't part of a dataset, that dataset will be skipped.
 
     Parameters
     ----------
-    result: DatasetConvertible
-        Result from a pyglotaran optimization as dataset, Path or Result object.
+    result : ResultLike
+        Data structure which can be converted to a mapping.
+    wavelength : float
+        Wavelength to plot data and fits for.
+    axis: Axis
+        Axis to plot the data and fits on.
     center_λ: float | None
         Center wavelength (λ in nm)
-    linlog: bool
+    main_irf_nr : int
+        Index of the main ``irf`` component when using an ``irf``
+        parametrized with multiple peaks. Defaults to 0.
+    linlog : bool
         Whether to use 'symlog' scale or not. Defaults to False.
-    linthresh: float
+    linthresh : float
         A single float which defines the range (-x, x), within which the plot is linear.
         This avoids having the plot go to infinity around zero. Defaults to 1.
-    linscale: float
-        This allows the linear range (-linthresh to linthresh) to be stretched
-        relative to the logarithmic range.
-        Its value is the number of decades to use for each half of the linear range.
-        For example, when linscale == 1.0 (the default), the space used for the
-        positive and negative halves of the linear range will be equal to one
-        decade in the logarithmic range. Defaults to 1.
-    show_data: bool
-        Whether to show the input data or residual. Defaults to False.
-    main_irf_nr: int
-        Index of the main ``irf`` component when using an ``irf``
-        parametrized with multiple peaks. Defaults to 0.
-    figsize : tuple[int, int]
-        Size of the figure (N, M) in inches. Defaults to (18, 16).
+    divide_by_scale : bool
+        Whether or not to divide the data by the dataset scale used for optimization.
+        Defaults to True.
+    per_axis_legend: bool
+        Whether to use a legend per plot or for the whole figure. Defaults to False.
+    y_label: str
+        Label used for the y-axis of each subplot.
     cycler : Cycler | None
-        Plot style cycler to use. Defaults to PlotStyle().cycler.
-    figure_only: bool
-        Whether or not to only return the figure.
-        This is a deprecation helper argument to transition to a consistent return value
-        consisting of the :class:`Figure` and the :class:`Axes`. Defaults to True.
-    nr_of_data_svd_vectors: int
-        Number of data SVD vector to plot. Defaults to 4.
-    nr_of_residual_svd_vectors: int
-        Number of residual SVD vector to plot. Defaults to 2.
-    show_data_svd_legend: bool
-        Whether or not to show the data SVD legend. Defaults to True.
-    show_residual_svd_legend: bool
-        Whether or not to show the residual SVD legend. Defaults to True.
-
-    Returns
-    -------
-    Figure|tuple[Figure, Axes]
-        If ``figure_only`` is True, Figure object which contains the plots (deprecated).
-        If ``figure_only`` is False, Figure object which contains the plots and the Axes.
+        Plot style cycler to use. Defaults to PlotStyle().data_cycler_solid.
+    show_zero_line: bool
+        Whether or not to add a horizontal line at zero. Defaults to True.
+
+    See Also
+    --------
+    plot_fit_overview
     """
-    res = load_data(result)
-
-    # Plot dimensions
-    M = 4
-    N = 3
-    fig, axes = plt.subplots(M, N, figsize=figsize, constrained_layout=True)
-
-    if center_λ is None:  # center wavelength (λ in nm)
-        center_λ = min(res.dims["spectral"], round(res.dims["spectral"] / 2))
-
-    # First and second row: concentrations - SAS/EAS - DAS
-    plot_concentrations(
-        res,
-        axes[0, 0],
-        center_λ,
-        linlog=linlog,
-        linthresh=linthresh,
-        linscale=linscale,
-        main_irf_nr=main_irf_nr,
-        cycler=cycler,
-    )
-    plot_spectra(res, axes[0:2, 1:3], cycler=cycler)
-    plot_svd(
-        res,
-        axes[2:4, 0:3],
-        linlog=linlog,
-        linthresh=linthresh,
-        cycler=cycler,
-        nr_of_data_svd_vectors=nr_of_data_svd_vectors,
-        nr_of_residual_svd_vectors=nr_of_residual_svd_vectors,
-        show_data_svd_legend=show_data_svd_legend,
-        show_residual_svd_legend=show_residual_svd_legend,
-    )
-    plot_residual(
-        res, axes[1, 0], linlog=linlog, linthresh=linthresh, show_data=show_data, cycler=cycler
-    )
-    # plt.tight_layout(pad=3, w_pad=4.0, h_pad=4.0)
-    if figure_only is True:
-        warn(PyglotaranExtrasApiDeprecationWarning(FIG_ONLY_WARNING), stacklevel=2)
-        return fig
-    else:
-        return fig, axes
-
-
-def plot_simple_overview(
-    result: DatasetConvertible,
-    title: str | None = None,
-    figsize: tuple[int, int] = (12, 6),
-    cycler: Cycler | None = PlotStyle().cycler,
-    figure_only: bool = True,
-) -> Figure | tuple[Figure, Axes]:
-    """Plot simple overview.
+    result_map = result_dataset_mapping(result)
+    add_cycler_if_not_none(axis, cycler)
+    for dataset_name in result_map.keys():
+        if result_map[dataset_name].coords["time"].values.size == 1:
+            continue
+        spectral_coords = result_map[dataset_name].coords["spectral"].values
+        if spectral_coords.min() <= wavelength <= spectral_coords.max():
+            result_data = result_map[dataset_name].sel(spectral=[wavelength], method="nearest")
+            scale = extract_dataset_scale(result_data, divide_by_scale)
+            irf_loc = extract_irf_location(result_data, center_λ, main_irf_nr)
+            result_data = result_data.assign_coords(time=result_data.coords["time"] - irf_loc)
+            (result_data.data / scale).plot(x="time", ax=axis, label=f"{dataset_name}_data")
+            (result_data.fitted_data / scale).plot(x="time", ax=axis, label=f"{dataset_name}_fit")
+        else:
+            [next(axis._get_lines.prop_cycler) for _ in range(2)]
+    if linlog:
+        axis.set_xscale("symlog", linthresh=linthresh)
+    if show_zero_line is True:
+        axis.axhline(0, color="k", linewidth=1)
+    axis.set_ylabel(y_label)
+    if per_axis_legend is True:
+        axis.legend()
+
+
+def plot_fitted_traces(
+    result: ResultLike,
+    wavelengths: Iterable[float],
+    axes_shape: tuple[int, int] = (4, 4),
+    center_λ: float | None = None,
+    main_irf_nr: int = 0,
+    linlog: bool = False,
+    linthresh: float = 1,
+    divide_by_scale: bool = True,
+    per_axis_legend: bool = False,
+    figsize: tuple[float, float] = (30, 15),
+    title: str = "Fit overview",
+    y_label: str = "a.u.",
+    cycler: Cycler | None = PlotStyle().data_cycler_solid,
+    show_zero_line: bool = True,
+) -> tuple[Figure, Axes]:
+    """Plot data and their fit in per wavelength plot grid.
 
     Parameters
     ----------
-    result: DatasetConvertible
-        Result from a pyglotaran optimization as dataset, Path or Result object.
-    title: str | None
-        Title of the figure. Defaults to None.
+    result : ResultLike
+        Data structure which can be converted to a mapping of datasets.
+    axes_shape : tuple[int, int]
+        Shape of the plot grid (N, M). Defaults to (4, 4).
+    wavelengths: Iterable[float]
+        Wavelength which should be used for each subplot, should to be of length N*M
+        with ``axes_shape`` being of shape (N, M), else it will result in missing plots.
+    center_λ: float | None
+        Center wavelength of the IRF (λ in nm).
+    main_irf_nr : int
+        Index of the main ``irf`` component when using an ``irf``
+        parametrized with multiple peaks. Defaults to 0.
+    linlog : bool
+        Whether to use 'symlog' scale or not. Defaults to False.
+    linthresh : float
+        A single float which defines the range (-x, x), within which the plot is linear.
+        This avoids having the plot go to infinity around zero. Defaults to 1.
+    divide_by_scale : bool
+        Whether or not to divide the data by the dataset scale used for optimization.
+        Defaults to True.
+    per_axis_legend : bool
+        Whether to use a legend per plot or for the whole figure. Defaults to False.
     figsize : tuple[int, int]
-        Size of the figure (N, M) in inches. Defaults to (18, 16).
+        Size of the figure (N, M) in inches. Defaults to (30, 15).
+    title : str
+        Title to add to the figure. Defaults to "Fit overview".
+    y_label: str
+        Label used for the y-axis of each subplot.
     cycler : Cycler | None
-        Plot style cycler to use. Defaults to PlotStyle().cycler.
-    figure_only: bool
-        Whether or not to only return the figure.
-        This is a deprecation helper argument to transition to a consistent return value
-        consisting of the :class:`Figure` and the :class:`Axes`. Defaults to True.
+        Plot style cycler to use. Defaults to PlotStyle().data_cycler_solid.
+    show_zero_line: bool
+        Whether or not to add a horizontal line at zero. Defaults to True.
+
 
     Returns
     -------
-    Figure|tuple[Figure, Axes]
-        If ``figure_only`` is True, Figure object which contains the plots (deprecated).
-        If ``figure_only`` is False, Figure object which contains the plots and the Axes.
-    """
-    res = load_data(result)
-
-    fig, axes = plt.subplots(2, 3, figsize=figsize, constrained_layout=True)
-    for ax in axes.flatten():
-        add_cycler_if_not_none(ax, cycler)
-    if title:
-        fig.suptitle(title, fontsize=16)
-    sas = res.species_associated_spectra
-    traces = res.species_concentration
-    if "spectral" in traces.coords:
-        traces.sel(spectral=res.spectral.values[0], method="nearest").plot.line(
-            x="time", ax=axes[0, 0]
-        )
-    else:
-        traces.plot.line(x="time", ax=axes[0, 0])
-    sas.plot.line(x="spectral", ax=axes[0, 1])
-    rLSV = res.residual_left_singular_vectors
-    rLSV.isel(left_singular_value_index=range(min(2, len(rLSV)))).plot.line(
-        x="time", ax=axes[1, 0]
-    )
+    tuple[Figure, Axes]
+        Figure and axes which can then be refined by the user.
 
-    axes[1, 0].set_title("res. LSV")
-    rRSV = res.residual_right_singular_vectors
-    rRSV.isel(right_singular_value_index=range(min(2, len(rRSV)))).plot.line(
-        x="spectral", ax=axes[1, 1]
+    See Also
+    --------
+    maximum_coordinate_range
+    add_unique_figure_legend
+    plot_data_and_fits
+    calculate_wavelengths
+    """
+    result_map = result_dataset_mapping(result)
+    fig, axes = plt.subplots(*axes_shape, figsize=figsize)
+    nr_of_plots = len(axes.flatten())
+    max_spectral_values = max(
+        len(result_map[dataset_name].coords["spectral"]) for dataset_name in result_map.keys()
     )
-
-    axes[1, 1].set_title("res. RSV")
-    res.data.plot(x="time", ax=axes[0, 2])
-    axes[0, 2].set_title("data")
-    res.residual.plot(x="time", ax=axes[1, 2])
-    axes[1, 2].set_title("residual")
-    if figure_only is not True:
-        return fig, axes
-    warn(PyglotaranExtrasApiDeprecationWarning(FIG_ONLY_WARNING), stacklevel=2)
-    return fig
-
-
-if __name__ == "__main__":
-    import sys
-
-    result_path = Path(sys.argv[1])
-    res = load_data(result_path)
-    print(res)
-
-    fig, plt.axes = plot_overview(res, figure_only=False)
-    if len(sys.argv) > 2:
-        fig.savefig(sys.argv[2], bbox_inches="tight")
-        print(f"Saved figure to: {sys.argv[2]}")
-    else:
-        plt.show(block=False)
-        input("press <ENTER> to continue")
+    if nr_of_plots > max_spectral_values:
+        warn(
+            PlotDuplicationWarning(
+                f"The number of plots ({nr_of_plots}) exceeds the maximum number of "
+                f"spectral data points ({max_spectral_values}), "
+                "which will lead in duplicated plots."
+            ),
+            stacklevel=2,
+        )
+    for wavelength, axis in zip(wavelengths, axes.flatten()):
+        plot_data_and_fits(
+            result=result_map,
+            wavelength=wavelength,
+            axis=axis,
+            center_λ=center_λ,
+            main_irf_nr=main_irf_nr,
+            linlog=linlog,
+            linthresh=linthresh,
+            divide_by_scale=divide_by_scale,
+            per_axis_legend=per_axis_legend,
+            y_label=y_label,
+            cycler=cycler,
+            show_zero_line=show_zero_line,
+        )
+    if per_axis_legend is False:
+        add_unique_figure_legend(fig, axes)
+    fig.suptitle(title, fontsize=28)
+    fig.tight_layout()
+    return fig, axes
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_residual.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_residual.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,86 @@
 """Module containing residual plot functionality."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 
+from pyglotaran_extras.plotting.plot_irf_dispersion_center import _plot_irf_dispersion_center
 from pyglotaran_extras.plotting.style import PlotStyle
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
+from pyglotaran_extras.plotting.utils import shift_time_axis_by_irf_location
 
 if TYPE_CHECKING:
     import xarray as xr
     from cycler import Cycler
     from matplotlib.axis import Axis
 
 
 def plot_residual(
     res: xr.Dataset,
     ax: Axis,
     linlog: bool = False,
     linthresh: float = 1,
-    show_data: bool = False,
+    show_data: bool | None = False,
     cycler: Cycler | None = PlotStyle().cycler,
+    show_irf_dispersion_center: bool = True,
+    irf_location: float | None = None,
 ) -> None:
     """Plot data or residual on a 2D contour plot.
 
     Parameters
     ----------
     res : xr.Dataset
         Result dataset
     ax : Axis
         Axis to plot on.
     linlog : bool
         Whether to use 'symlog' scale or not. Defaults to False.
     linthresh : float
         A single float which defines the range (-x, x), within which the plot is linear.
         This avoids having the plot go to infinity around zero. Defaults to 1.
-    show_data : bool
-        Whether to show the data or the residual. Defaults to False.
+    show_data: bool | None
+        Whether to show the input data or residual. If set to ``None`` the plot is skipped
+        which improves plotting performance for big datasets. Defaults to False.
     cycler : Cycler | None
         Plot style cycler to use. Defaults to PlotStyle().cycler.
+    show_irf_dispersion_center: bool
+        Whether to show the the IRF dispersion center as overlay on the residual/data plot.
+        Defaults to True.
+    irf_location:  float | None
+        Location of the ``irf`` by which the time axis will get shifted. If it is None the time
+        axis will not be shifted. Defaults to None.
     """
+    if show_data is None:
+        ax.text(
+            0.5,
+            0.5,
+            "Skipped",
+            horizontalalignment="center",
+            verticalalignment="center",
+            fontsize=24,
+        )
+        return
+
     add_cycler_if_not_none(ax, cycler)
     data = res.data if show_data else res.residual
+    data = shift_time_axis_by_irf_location(data, irf_location)
     title = "dataset" if show_data else "residual"
     shape = np.array(data.shape)
-    dims = data.coords.dims
     # Handle different dimensionality of data
     if min(shape) == 1:
+        dims = data.coords.dims
         data.plot.line(x=dims[shape.argmax()], ax=ax)
     elif min(shape) < 5:
         data.plot(x="time", ax=ax)
     else:
         data.plot(x="time", ax=ax, add_colorbar=False)
+    if show_irf_dispersion_center is True:
+        _plot_irf_dispersion_center(
+            res, ax=ax, spectral_axis="y", cycler=cycler, irf_location=irf_location
+        )
+        ax.set_xlabel("time")
+        ax.legend()
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
     ax.set_title(title)
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/plot_svd.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_svd.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from typing import TYPE_CHECKING
 
 from glotaran.io.prepare_dataset import add_svd_to_dataset
 
 from pyglotaran_extras.plotting.style import PlotStyle
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
+from pyglotaran_extras.plotting.utils import shift_time_axis_by_irf_location
 
 if TYPE_CHECKING:
     from typing import Sequence
 
     import xarray as xr
     from cycler import Cycler
     from matplotlib.axis import Axis
@@ -23,14 +24,15 @@
     linlog: bool = False,
     linthresh: float = 1,
     cycler: Cycler | None = PlotStyle().cycler,
     nr_of_data_svd_vectors: int = 4,
     nr_of_residual_svd_vectors: int = 2,
     show_data_svd_legend: bool = True,
     show_residual_svd_legend: bool = True,
+    irf_location: float | None = None,
 ) -> None:
     """Plot SVD (Singular Value Decomposition) of data and residual.
 
     Parameters
     ----------
     res : xr.Dataset
         Result dataset
@@ -47,27 +49,31 @@
         Number of data SVD vector to plot. Defaults to 4.
     nr_of_residual_svd_vectors: int
         Number of residual SVD vector to plot. Defaults to 2.
     show_data_svd_legend: bool
         Whether or not to show the data SVD legend. Defaults to True.
     show_residual_svd_legend: bool
         Whether or not to show the residual SVD legend. Defaults to True.
+    irf_location:  float | None
+        Location of the ``irf`` by which the time axis will get shifted. If it is None the time
+        axis will not be shifted. Defaults to None.
     """
     if "weighted_residual" in res:
         add_svd_to_dataset(dataset=res, name="weighted_residual")
     else:
         add_svd_to_dataset(dataset=res, name="residual")
     plot_lsv_residual(
         res,
         axes[0, 0],
         linlog=linlog,
         linthresh=linthresh,
         cycler=cycler,
         indices=range(nr_of_residual_svd_vectors),
         show_legend=show_residual_svd_legend,
+        irf_location=irf_location,
     )
     plot_rsv_residual(
         res,
         axes[0, 1],
         cycler=cycler,
         indices=range(nr_of_residual_svd_vectors),
         show_legend=show_residual_svd_legend,
@@ -78,14 +84,15 @@
         res,
         axes[1, 0],
         linlog=linlog,
         linthresh=linthresh,
         cycler=cycler,
         indices=range(nr_of_data_svd_vectors),
         show_legend=show_data_svd_legend,
+        irf_location=irf_location,
     )
     plot_rsv_data(
         res,
         axes[1, 1],
         cycler=cycler,
         indices=range(nr_of_data_svd_vectors),
         show_legend=show_data_svd_legend,
@@ -97,14 +104,15 @@
     res: xr.Dataset,
     ax: Axis,
     indices: Sequence[int] = range(4),
     linlog: bool = False,
     linthresh: float = 1,
     cycler: Cycler | None = PlotStyle().cycler,
     show_legend: bool = True,
+    irf_location: float | None = None,
 ) -> None:
     """Plot left singular vectors (time) of the data matrix.
 
     Parameters
     ----------
     res : xr.Dataset
         Result dataset
@@ -117,18 +125,22 @@
     linthresh : float
         A single float which defines the range (-x, x), within which the plot is linear.
         This avoids having the plot go to infinity around zero. Defaults to 1.
     cycler : Cycler | None
         Plot style cycler to use. Defaults to PlotStyle().cycler.
     show_legend: bool
         Whether or not to show the legend. Defaults to True.
+    irf_location:  float | None
+        Location of the ``irf`` by which the time axis will get shifted. If it is None the time
+        axis will not be shifted. Defaults to None.
     """
     add_cycler_if_not_none(ax, cycler)
     dLSV = res.data_left_singular_vectors
-    _plot_svd_vetors(dLSV, indices, "left_singular_value_index", ax, show_legend)
+    dLSV = shift_time_axis_by_irf_location(dLSV, irf_location)
+    _plot_svd_vectors(dLSV, indices, "left_singular_value_index", ax, show_legend)
     ax.set_title("data. LSV")
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
 
 
 def plot_rsv_data(
     res: xr.Dataset,
@@ -150,15 +162,15 @@
     cycler : Cycler | None
         Plot style cycler to use. Defaults to PlotStyle().cycler.
     show_legend: bool
         Whether or not to show the legend. Defaults to True.
     """
     add_cycler_if_not_none(ax, cycler)
     dRSV = res.data_right_singular_vectors
-    _plot_svd_vetors(dRSV, indices, "right_singular_value_index", ax, show_legend)
+    _plot_svd_vectors(dRSV, indices, "right_singular_value_index", ax, show_legend)
     ax.set_title("data. RSV")
 
 
 def plot_sv_data(
     res: xr.Dataset,
     ax: Axis,
     indices: Sequence[int] = range(10),
@@ -189,14 +201,15 @@
     res: xr.Dataset,
     ax: Axis,
     indices: Sequence[int] = range(2),
     linlog: bool = False,
     linthresh: float = 1,
     cycler: Cycler | None = PlotStyle().cycler,
     show_legend: bool = True,
+    irf_location: float | None = None,
 ) -> None:
     """Plot left singular vectors (time) of the residual matrix.
 
     Parameters
     ----------
     res : xr.Dataset
         Result dataset
@@ -209,21 +222,25 @@
     linthresh : float
         A single float which defines the range (-x, x), within which the plot is linear.
         This avoids having the plot go to infinity around zero. Defaults to 1.
     cycler : Cycler | None
         Plot style cycler to use. Defaults to PlotStyle().cycler.
     show_legend: bool
         Whether or not to show the legend. Defaults to True.
+    irf_location:  float | None
+        Location of the ``irf`` by which the time axis will get shifted. If it is None the time
+        axis will not be shifted. Defaults to None.
     """
     add_cycler_if_not_none(ax, cycler)
     if "weighted_residual_left_singular_vectors" in res:
         rLSV = res.weighted_residual_left_singular_vectors
     else:
         rLSV = res.residual_left_singular_vectors
-    _plot_svd_vetors(rLSV, indices, "left_singular_value_index", ax, show_legend)
+    rLSV = shift_time_axis_by_irf_location(rLSV, irf_location)
+    _plot_svd_vectors(rLSV, indices, "left_singular_value_index", ax, show_legend)
     ax.set_title("res. LSV")
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
 
 
 def plot_rsv_residual(
     res: xr.Dataset,
@@ -248,15 +265,15 @@
         Whether or not to show the legend. Defaults to True.
     """
     add_cycler_if_not_none(ax, cycler)
     if "weighted_residual_right_singular_vectors" in res:
         rRSV = res.weighted_residual_right_singular_vectors
     else:
         rRSV = res.residual_right_singular_vectors
-    _plot_svd_vetors(rRSV, indices, "right_singular_value_index", ax, show_legend)
+    _plot_svd_vectors(rRSV, indices, "right_singular_value_index", ax, show_legend)
     ax.set_title("res. RSV")
 
 
 def plot_sv_residual(
     res: xr.Dataset,
     ax: Axis,
     indices: Sequence[int] = range(10),
@@ -282,15 +299,15 @@
         rSV = res.residual_singular_values
     rSV.sel(singular_value_index=indices[: len(rSV.singular_value_index)]).plot.line(
         "ro-", yscale="log", ax=ax
     )
     ax.set_title("res. log(SV)")
 
 
-def _plot_svd_vetors(
+def _plot_svd_vectors(
     vector_data: xr.DataArray,
     indices: Sequence[int],
     sv_index_dim: str,
     ax: Axis,
     show_legend: bool,
 ) -> None:
     """Plot SVD vectors with decreasing zorder on axis ``ax``.
@@ -317,11 +334,11 @@
     """
     max_index = len(getattr(vector_data, sv_index_dim))
     values = vector_data.isel(**{sv_index_dim: indices[:max_index]})
     x_dim = vector_data.dims[1]
     if x_dim == sv_index_dim:
         values = values.T
         x_dim = vector_data.dims[0]
-    for index, (zorder, value) in enumerate(zip(range(100)[::-1], values)):
-        value.plot.line(x=x_dim, ax=ax, zorder=zorder, label=index)
+    for zorder, label, value in zip(range(100)[::-1], indices[:max_index], values):
+        value.plot.line(x=x_dim, ax=ax, zorder=zorder, label=label)
     if show_legend is True:
         ax.legend(title=sv_index_dim)
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/plotting/style.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/style.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import matplotlib.pyplot as plt
 from cycler import cycler
 
 if TYPE_CHECKING:
     from cycler import Cycler
 
 
-class ColorCode(Enum):
+class ColorCode(str, Enum):
     """Color definitions from legacy glotaran.
 
     See: https://glotaran.github.io/legacy/plot_styles
     """
 
     # Name	#Hex
     black = "#000000"
@@ -68,24 +68,24 @@
         -------
         str
             Hex code representing the same color as ``rgb_tuple``.
         """
         return colors.rgb2hex([1.0 * x / 255 for x in rgb_tuple])
 
 
-class LineStyle(Enum):
+class LineStyle(str, Enum):
     """Subset of line styles supported by matplotlib."""
 
     solid = "-"
     dashed = "--"
     dotted = ".."
     dashdot = "-."
 
 
-class DataColorCode(Enum):
+class DataColorCode(str, Enum):
     """Colors used to plot data and fits.
 
     Pairs of visually similar looking colors whereby the
     first (lighter) color is used to plot the data,
     and the second (darker) color is used to represent
     the fitted trace (that goes 'through' the data).
     """
@@ -105,15 +105,15 @@
     maroon = "#800000"
     yellow = "#ffff00"
     # Needs to be added manually to the list in PlotStyle
     # since Enum doesn't allow duplicates
     # orange = "#ff8c00"
 
 
-class DataLineStyle(Enum):
+class DataLineStyle(str, Enum):
     """Data plots can alternate between solid lines for data and dashed lines for fits.
 
     This is mostly useful for data with very low noise (e.g. simulated data),
     since data and fir often overlap
     """
 
     solid = "-"
@@ -121,22 +121,20 @@
 
 
 class PlotStyle:
     """Wrapper class to hold predefined Plot styles."""
 
     def __init__(self) -> None:
         """Initialize Stiles from Enums."""
-        self._line_style = [e.value for e in LineStyle]
-        self._color_codes = [e.value for e in ColorCode]
+        self._line_style = list(LineStyle)
+        self._color_codes = list(ColorCode)
         # Since Enum only supports unique values we need to manually add the last one
-        self._data_color_codes = [e.value for e in DataColorCode] + [DataColorCode.orange.value]
+        self._data_color_codes = list(DataColorCode) + [DataColorCode.orange]
         # Extend linecycler to same size as colorcycler
-        self._data_line_style = [e.value for e in DataLineStyle] * (
-            len(self._data_color_codes) // 2
-        )
+        self._data_line_style = list(DataLineStyle) * (len(self._data_color_codes) // 2)
         self.SMALL_SIZE = 12
         self.MEDIUM_SIZE = 14
         self.BIGGER_SIZE = 18
 
     def set_default_fontsize(self) -> None:
         """Set global plot settings for matplotlib."""
         plt.rc("font", size=self.SMALL_SIZE)  # controls default text sizes
```

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras/types.py` & `pyglotaran_extras-0.7.0/pyglotaran_extras/types.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/pyglotaran_extras.egg-info/PKG-INFO` & `pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglotaran-extras
-Version: 0.6.0
+Version: 0.7.0
 Summary: Supplementary package for pyglotaran with (example) plotting code.
 Home-page: https://github.com/glotaran/pyglotaran-extras
 Author: Joris Snellenburg
 Author-email: j.snellenburg@gmail.com
 License: MIT
 Project-URL: GloTarAn Ecosystem, https://glotaran.org
 Project-URL: Documentation, https://pyglotaran-extras.readthedocs.io
@@ -41,15 +41,15 @@
         ```console
         pip install pyglotaran-extras
         ```
         
         If you want to install it via conda, you can run the following command:
         
         ```console
-        conda install pyglotaran-extras
+        conda install -c conda-forge pyglotaran-extras
         ```
         
         ### From Source
         
         To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
         
         ```console
```

### Comparing `pyglotaran_extras-0.6.0/setup.cfg` & `pyglotaran_extras-0.7.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -28,48 +28,35 @@
 	Changelog=https://pyglotaran-extras.readthedocs.io/en/latest/changelog.html
 	Source=https://github.com/glotaran/pyglotaran-extras
 	Tracker=https://github.com/glotaran/pyglotaran-extras/issues
 
 [options]
 packages = find:
 install_requires = 
+	cycler>=0.10
 	matplotlib>=3.3.0
-	pyglotaran>=0.5.1
+	numpy>=1.21.2,<1.24
+	pyglotaran>=0.6
+	tabulate>=0.8.9
 	xarray>=2022.3.0
 python_requires = >=3.8,<3.11
 zip_safe = True
 
 [options.packages.find]
 include = 
 	pyglotaran_extras
 	pyglotaran_extras.*
 
 [rstcheck]
-ignore_directives = autoattribute,autoclass,autoexception,autofunction,automethod,automodule,highlight
+ignore_directives = autosummary
 
 [darglint]
 docstring_style = numpy
 ignore_regex = test_.+|.*dummy.*
 
 [pydocstyle]
 convention = numpy
 
-[mypy]
-ignore_missing_imports = True
-scripts_are_modules = True
-show_error_codes = True
-warn_unused_ignores = True
-no_implicit_optional = True
-disallow_incomplete_defs = True
-disallow_untyped_defs = True
-disallow_untyped_calls = True
-no_implicit_reexport = True
-warn_unused_configs = True
-
-[mypy-tests.*]
-disallow_incomplete_defs = False
-disallow_untyped_defs = False
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyglotaran_extras-0.6.0/tests/deprecation/test_deprecation_utils.py` & `pyglotaran_extras-0.7.0/tests/deprecation/test_deprecation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from pyglotaran_extras.deprecation.deprecation_utils import PyglotaranExtrasApiDeprecationWarning
 from pyglotaran_extras.deprecation.deprecation_utils import check_overdue
 from pyglotaran_extras.deprecation.deprecation_utils import parse_version
 from pyglotaran_extras.deprecation.deprecation_utils import pyglotaran_extras_version
 from pyglotaran_extras.deprecation.deprecation_utils import warn_deprecated
 
 if TYPE_CHECKING:
-
     from _pytest.monkeypatch import MonkeyPatch
 
 OVERDUE_ERROR_MESSAGE = (
     "Support for 'pyglotaran_extras.deprecation.deprecation_utils.parse_version' "
     "was supposed to be dropped in version: '0.6.0'.\n"
     "Current version is: '1.0.0'"
 )
```

### Comparing `pyglotaran_extras-0.6.0/tests/io/test_get_script_dir.ipynb` & `pyglotaran_extras-0.7.0/tests/io/test_get_script_dir.ipynb`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.6.0/tests/io/test_setup_case_study.py` & `pyglotaran_extras-0.7.0/tests/io/test_setup_case_study.py`

 * *Files identical despite different names*

