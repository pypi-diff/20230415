# Comparing `tmp/econpizza-0.5.3.tar.gz` & `tmp/econpizza-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.5.3.tar", last modified: Sat Apr 15 12:04:45 2023, max compression
+gzip compressed data, was "econpizza-0.5.4.tar", last modified: Sat Apr 15 12:47:11 2023, max compression
```

## Comparing `econpizza-0.5.3.tar` & `econpizza-0.5.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.622183 econpizza-0.5.3/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.605516 econpizza-0.5.3/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.608849 econpizza-0.5.3/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1525 2023-03-28 17:25:45.000000 econpizza-0.5.3/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.3/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.3/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.3/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:04:45.622183 econpizza-0.5.3/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3339 2023-03-23 23:42:13.000000 econpizza-0.5.3/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.605516 econpizza-0.5.3/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1539 2023-03-18 08:31:39.000000 econpizza-0.5.3/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.3/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1278 2023-03-22 08:57:54.000000 econpizza-0.5.3/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.3/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1624 2023-03-30 06:43:39.000000 econpizza-0.5.3/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2117 2023-03-30 06:41:47.000000 econpizza-0.5.3/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13122 2023-03-24 20:13:36.000000 econpizza-0.5.3/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2372 2023-03-22 12:36:34.000000 econpizza-0.5.3/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.3/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.3/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.3/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.3/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.3/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.3/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.615516 econpizza-0.5.3/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.3/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-04-15 12:03:43.000000 econpizza-0.5.3/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.3/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.3/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.3/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.3/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.3/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.3/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.3/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.3/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.3/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.3/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.3/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.3/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.3/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12023 2023-03-31 05:55:10.000000 econpizza-0.5.3/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.3/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-03-31 05:57:33.000000 econpizza-0.5.3/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.3/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 18:29:58.000000 econpizza-0.5.3/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.3/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.3/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.3/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5933 2023-03-18 08:06:49.000000 econpizza-0.5.3/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8548 2023-03-28 11:53:45.000000 econpizza-0.5.3/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.3/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.3/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.3/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.3/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.3/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.3/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 15:12:39.000000 econpizza-0.5.3/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4688 2023-03-25 22:22:00.000000 econpizza-0.5.3/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.3/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5575 2023-03-28 17:26:05.000000 econpizza-0.5.3/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.615516 econpizza-0.5.3/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       65 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      113 2023-03-30 19:12:29.000000 econpizza-0.5.3/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-15 12:04:45.622183 econpizza-0.5.3/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1318 2023-03-30 19:13:52.000000 econpizza-0.5.3/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.098390 econpizza-0.5.4/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.085056 econpizza-0.5.4/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.085056 econpizza-0.5.4/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1527 2023-04-15 12:29:25.000000 econpizza-0.5.4/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.4/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.4/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.4/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:47:11.098390 econpizza-0.5.4/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3339 2023-03-23 23:42:13.000000 econpizza-0.5.4/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.088390 econpizza-0.5.4/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.085056 econpizza-0.5.4/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.088390 econpizza-0.5.4/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1539 2023-03-18 08:31:39.000000 econpizza-0.5.4/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.4/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.088390 econpizza-0.5.4/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1278 2023-03-22 08:57:54.000000 econpizza-0.5.4/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.4/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1624 2023-03-30 06:43:39.000000 econpizza-0.5.4/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2117 2023-03-30 06:41:47.000000 econpizza-0.5.4/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13122 2023-03-24 20:13:36.000000 econpizza-0.5.4/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2372 2023-03-22 12:36:34.000000 econpizza-0.5.4/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.4/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.091723 econpizza-0.5.4/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.4/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.4/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.4/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.4/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.4/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.091723 econpizza-0.5.4/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.4/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-04-15 12:23:21.000000 econpizza-0.5.4/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.4/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.4/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.4/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.4/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.4/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.4/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.4/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.4/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.4/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.4/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.4/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.4/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.4/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12023 2023-03-31 05:55:10.000000 econpizza-0.5.4/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.4/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-03-31 05:57:33.000000 econpizza-0.5.4/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.4/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 18:29:58.000000 econpizza-0.5.4/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.4/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.4/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.4/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5933 2023-03-18 08:06:49.000000 econpizza-0.5.4/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8548 2023-03-28 11:53:45.000000 econpizza-0.5.4/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.098390 econpizza-0.5.4/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.4/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.4/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.4/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.4/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.4/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.098390 econpizza-0.5.4/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.4/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 15:12:39.000000 econpizza-0.5.4/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4688 2023-03-25 22:22:00.000000 econpizza-0.5.4/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.4/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5575 2023-03-28 17:26:05.000000 econpizza-0.5.4/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.091723 econpizza-0.5.4/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-04-15 12:47:11.000000 econpizza-0.5.4/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       77 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      113 2023-04-15 12:24:38.000000 econpizza-0.5.4/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-15 12:47:11.098390 econpizza-0.5.4/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1330 2023-04-15 12:24:22.000000 econpizza-0.5.4/setup.py
```

### Comparing `econpizza-0.5.3/.github/workflows/continuous-integration.yml` & `econpizza-0.5.4/.github/workflows/continuous-integration.yml`

 * *Files 0% similar despite different names*

```diff
@@ -38,12 +38,12 @@
         python -m pip install .
         # testing deps
         python -m pip install pytest
         python -m pip install testbook
         python -m pip install ipykernel
         python -m pip install grgrlib
         # for development versions of grgrjax
-        python -m pip uninstall -y grgrjax
-        python -m pip install git+https://github.com/gboehl/grgrjax
+        #python -m pip uninstall -y grgrjax
+        #python -m pip install git+https://github.com/gboehl/grgrjax
     - name: Test with pytest
       run: |
         pytest -x
```

### Comparing `econpizza-0.5.3/.readthedocs.yaml` & `econpizza-0.5.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/LICENSE` & `econpizza-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/PKG-INFO` & `econpizza-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.3
+Version: 0.5.4
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.5.3/README.rst` & `econpizza-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/Makefile` & `econpizza-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/conf.py` & `econpizza-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/guide/installation.rst` & `econpizza-0.5.4/docs/guide/installation.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/guide/method.ipynb` & `econpizza-0.5.4/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/guide/solution.rst` & `econpizza-0.5.4/docs/guide/solution.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/guide/steady_state.rst` & `econpizza-0.5.4/docs/guide/steady_state.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/guide/the_yaml.rst` & `econpizza-0.5.4/docs/guide/the_yaml.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/index.rst` & `econpizza-0.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/lin_and_nlin.png` & `econpizza-0.5.4/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/make.bat` & `econpizza-0.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/p_and_n.png` & `econpizza-0.5.4/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/tutorial/boehl_hommes.rst` & `econpizza-0.5.4/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/tutorial/hank1.ipynb` & `econpizza-0.5.4/docs/tutorial/hank1.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/tutorial/hank2.ipynb` & `econpizza-0.5.4/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/tutorial/quickstart.ipynb` & `econpizza-0.5.4/docs/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/docs/tutorial/rank.ipynb` & `econpizza-0.5.4/docs/tutorial/rank.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/__init__.py` & `econpizza-0.5.4/econpizza/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/bh.yml` & `econpizza-0.5.4/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/dsge.yml` & `econpizza-0.5.4/econpizza/examples/dsge.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/ghls.yml` & `econpizza-0.5.4/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank2.yml` & `econpizza-0.5.4/econpizza/examples/hank2.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank2_functions.py` & `econpizza-0.5.4/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.5.4/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank_functions.py` & `econpizza-0.5.4/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank_labor.yml` & `econpizza-0.5.4/econpizza/examples/hank_labor.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank_labor_functions.py` & `econpizza-0.5.4/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/hank_with_comments.yml` & `econpizza-0.5.4/econpizza/examples/hank_with_comments.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/nk.yml` & `econpizza-0.5.4/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/examples/tank.yml` & `econpizza-0.5.4/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/parser/__init__.py` & `econpizza-0.5.4/econpizza/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/parser/build_functions.py` & `econpizza-0.5.4/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/parser/checks.py` & `econpizza-0.5.4/econpizza/parser/checks.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.5.4/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.5.4/econpizza/parser/write_dynamic_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/solvers/shooting.py` & `econpizza-0.5.4/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/solvers/solve_linear.py` & `econpizza-0.5.4/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.5.4/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/solvers/stacking.py` & `econpizza-0.5.4/econpizza/solvers/stacking.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/solvers/steady_state.py` & `econpizza-0.5.4/econpizza/solvers/steady_state.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/testing/cache/bh.npy` & `econpizza-0.5.4/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.5.4/econpizza/testing/cache/hank_labor.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/testing/cache/hank_solid.npy` & `econpizza-0.5.4/econpizza/testing/cache/hank_solid.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/testing/test_rest.py` & `econpizza-0.5.4/econpizza/testing/test_rest.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/tools.py` & `econpizza-0.5.4/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/utilities/dists.py` & `econpizza-0.5.4/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/utilities/grids.py` & `econpizza-0.5.4/econpizza/utilities/grids.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/utilities/interp.py` & `econpizza-0.5.4/econpizza/utilities/interp.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/utilities/jacobian.py` & `econpizza-0.5.4/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza/utilities/newton.py` & `econpizza-0.5.4/econpizza/utilities/newton.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/econpizza.egg-info/PKG-INFO` & `econpizza-0.5.4/econpizza.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.3
+Version: 0.5.4
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.5.3/econpizza.egg-info/SOURCES.txt` & `econpizza-0.5.4/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.3/setup.py` & `econpizza-0.5.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     packages=['econpizza', 'econpizza.parser',
               'econpizza.utilities', 'econpizza.solvers'],
     package_data={"econpizza": ["examples/*"]},
     extras_require={
         'linear': ['grgrlib>=0.1.22'],
     },
     install_requires=[
-        "jax",
-        "jaxlib",
-        "grgrjax>=0.4.1",
+        "jax<0.4.6",
+        "jaxlib<0.4.6",
+        "grgrjax>=0.4.3",
         "pyyaml",
         "scipy",
     ],
 )
```

