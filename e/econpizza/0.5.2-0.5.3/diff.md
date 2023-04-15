# Comparing `tmp/econpizza-0.5.2.tar.gz` & `tmp/econpizza-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.5.2.tar", last modified: Mon Mar 27 09:59:16 2023, max compression
+gzip compressed data, was "econpizza-0.5.3.tar", last modified: Sat Apr 15 12:04:45 2023, max compression
```

## Comparing `econpizza-0.5.2.tar` & `econpizza-0.5.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.884121 econpizza-0.5.2/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.870788 econpizza-0.5.2/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.874121 econpizza-0.5.2/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1506 2023-03-27 00:29:13.000000 econpizza-0.5.2/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.2/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.2/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.2/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-03-27 09:59:16.884121 econpizza-0.5.2/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3339 2023-03-23 23:42:13.000000 econpizza-0.5.2/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.877455 econpizza-0.5.2/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.2/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.874121 econpizza-0.5.2/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.877455 econpizza-0.5.2/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.2/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1539 2023-03-18 08:31:39.000000 econpizza-0.5.2/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.2/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.877455 econpizza-0.5.2/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1278 2023-03-22 08:57:54.000000 econpizza-0.5.2/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.2/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      945 2023-03-22 11:48:25.000000 econpizza-0.5.2/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1489 2023-03-22 11:48:15.000000 econpizza-0.5.2/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13122 2023-03-24 20:13:36.000000 econpizza-0.5.2/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2372 2023-03-22 12:36:34.000000 econpizza-0.5.2/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.2/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.2/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.2/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       52 2023-03-22 13:27:56.000000 econpizza-0.5.2/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.877455 econpizza-0.5.2/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.2/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.2/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.2/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.2/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.2/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.877455 econpizza-0.5.2/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3429 2023-03-27 09:24:35.000000 econpizza-0.5.2/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-03-27 00:29:57.000000 econpizza-0.5.2/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.880788 econpizza-0.5.2/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.2/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.2/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.2/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.2/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.2/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.2/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.2/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.2/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.2/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.2/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.2/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-03-17 21:11:58.000000 econpizza-0.5.2/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.2/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.880788 econpizza-0.5.2/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    11658 2023-03-24 19:51:48.000000 econpizza-0.5.2/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.2/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4348 2023-03-15 15:29:46.000000 econpizza-0.5.2/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.2/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4102 2023-03-24 19:54:58.000000 econpizza-0.5.2/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.880788 econpizza-0.5.2/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.2/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.2/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.2/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5933 2023-03-18 08:06:49.000000 econpizza-0.5.2/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8437 2023-03-17 19:13:59.000000 econpizza-0.5.2/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.884121 econpizza-0.5.2/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.884121 econpizza-0.5.2/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.2/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.2/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.2/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.2/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.2/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.2/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.2/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.2/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.2/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.2/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.884121 econpizza-0.5.2/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.2/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-24 20:21:24.000000 econpizza-0.5.2/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4688 2023-03-25 22:22:00.000000 econpizza-0.5.2/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-18 14:26:12.000000 econpizza-0.5.2/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5313 2023-03-14 09:51:51.000000 econpizza-0.5.2/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-27 09:59:16.880788 econpizza-0.5.2/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-03-27 09:59:16.000000 econpizza-0.5.2/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-03-27 09:59:16.000000 econpizza-0.5.2/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-03-27 09:59:16.000000 econpizza-0.5.2/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       95 2023-03-27 09:59:16.000000 econpizza-0.5.2/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-03-27 09:59:16.000000 econpizza-0.5.2/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      127 2023-03-27 00:31:53.000000 econpizza-0.5.2/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-03-27 09:59:16.884121 econpizza-0.5.2/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1348 2023-03-27 09:25:09.000000 econpizza-0.5.2/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.622183 econpizza-0.5.3/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.605516 econpizza-0.5.3/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.608849 econpizza-0.5.3/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1525 2023-03-28 17:25:45.000000 econpizza-0.5.3/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.3/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.3/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.3/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:04:45.622183 econpizza-0.5.3/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3339 2023-03-23 23:42:13.000000 econpizza-0.5.3/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.605516 econpizza-0.5.3/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1539 2023-03-18 08:31:39.000000 econpizza-0.5.3/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.3/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1278 2023-03-22 08:57:54.000000 econpizza-0.5.3/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.3/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1624 2023-03-30 06:43:39.000000 econpizza-0.5.3/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2117 2023-03-30 06:41:47.000000 econpizza-0.5.3/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13122 2023-03-24 20:13:36.000000 econpizza-0.5.3/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2372 2023-03-22 12:36:34.000000 econpizza-0.5.3/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.3/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.3/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.612182 econpizza-0.5.3/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.3/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.3/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.3/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.3/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.3/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.615516 econpizza-0.5.3/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.3/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-04-15 12:03:43.000000 econpizza-0.5.3/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.3/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.3/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.3/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.3/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.3/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.3/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.3/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.3/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.3/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.3/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.3/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.3/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.3/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12023 2023-03-31 05:55:10.000000 econpizza-0.5.3/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.3/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-03-31 05:57:33.000000 econpizza-0.5.3/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.3/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 18:29:58.000000 econpizza-0.5.3/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.3/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.3/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.3/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5933 2023-03-18 08:06:49.000000 econpizza-0.5.3/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8548 2023-03-28 11:53:45.000000 econpizza-0.5.3/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.3/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.3/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.3/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.3/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.3/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.3/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.618849 econpizza-0.5.3/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.3/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 15:12:39.000000 econpizza-0.5.3/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4688 2023-03-25 22:22:00.000000 econpizza-0.5.3/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.3/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5575 2023-03-28 17:26:05.000000 econpizza-0.5.3/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:04:45.615516 econpizza-0.5.3/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       65 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-04-15 12:04:45.000000 econpizza-0.5.3/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      113 2023-03-30 19:12:29.000000 econpizza-0.5.3/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-15 12:04:45.622183 econpizza-0.5.3/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1318 2023-03-30 19:13:52.000000 econpizza-0.5.3/setup.py
```

### Comparing `econpizza-0.5.2/.github/workflows/continuous-integration.yml` & `econpizza-0.5.3/.github/workflows/continuous-integration.yml`

 * *Files 6% similar despite different names*

```diff
@@ -37,13 +37,13 @@
         python -m pip install --upgrade pip
         python -m pip install .
         # testing deps
         python -m pip install pytest
         python -m pip install testbook
         python -m pip install ipykernel
         python -m pip install grgrlib
-        # to be removed:
-        #python -m pip uninstall -y grgrjax
-        #python -m pip install git+https://github.com/gboehl/grgrjax
+        # for development versions of grgrjax
+        python -m pip uninstall -y grgrjax
+        python -m pip install git+https://github.com/gboehl/grgrjax
     - name: Test with pytest
       run: |
         pytest -x
```

### Comparing `econpizza-0.5.2/.readthedocs.yaml` & `econpizza-0.5.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/LICENSE` & `econpizza-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/PKG-INFO` & `econpizza-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.2
+Version: 0.5.3
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.5.2/README.rst` & `econpizza-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/Makefile` & `econpizza-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/conf.py` & `econpizza-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/guide/installation.rst` & `econpizza-0.5.3/docs/guide/installation.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/guide/method.ipynb` & `econpizza-0.5.3/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/guide/steady_state.rst` & `econpizza-0.5.3/docs/guide/steady_state.rst`

 * *Files 17% similar despite different names*

```diff
@@ -5,13 +5,20 @@
 
 Upon failure, the function tries to be as informative as possible. If the search is not successful, a possible path to find the error is to set the function's keyword argument ``raise_errors`` to ``False``. The function then raises a warning instead of failing with an exception, and returns a dictionary containing the results from the root finding routine, such as, e.g. the last Jacobian matrix.
 
 .. note::
 
    A classic complaint is "**The Jacobian contains NaNs**". This is usually due to numerical errors somewhere along the way. While the package tries to provide more information about where the error occurred, a good idea is to follow JAX's hints on `how to debug NaNs <https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#debugging-nans>`_.
 
-.. note::
+.. hint::
 
    A common gotcha for heterogeneous agent models is that the distribution contains negative values. The routine will be informative about that. This is usually due to too much interpolation outside the grid and can often be fixed by using a grid with larger maximum values.
 
+.. hint::
+
+   The steady state procedure is based on the pseudoinverse of the Jacobian (see the original paper). If the procedure fails, it will tell you the rank of the Jacobian and the number of degrees of freedom. More degrees of freedom than the Jacobian rank normally implies that you should fix more steady state values and vice versa.
+
+.. hint::
+
+   If the desired precision is not reached, the error message will tell you in which equation the maximum error did arise. You can use the ``equations`` key to get the list of equations (as strings), e.g. ``print(model['equations'][17])`` to get the equation with index 17.
 
 .. autofunction:: econpizza.PizzaModel.solve_stst
```

### Comparing `econpizza-0.5.2/docs/guide/the_yaml.rst` & `econpizza-0.5.3/docs/guide/the_yaml.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/index.rst` & `econpizza-0.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/lin_and_nlin.png` & `econpizza-0.5.3/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/make.bat` & `econpizza-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/p_and_n.png` & `econpizza-0.5.3/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/tutorial/boehl_hommes.rst` & `econpizza-0.5.3/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/tutorial/hank1.ipynb` & `econpizza-0.5.3/docs/tutorial/hank1.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/tutorial/hank2.ipynb` & `econpizza-0.5.3/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/tutorial/quickstart.ipynb` & `econpizza-0.5.3/docs/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/docs/tutorial/rank.ipynb` & `econpizza-0.5.3/docs/tutorial/rank.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/__init__.py` & `econpizza-0.5.3/econpizza/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 import jax
 import jax.numpy as jnp
-from copy import deepcopy as copy
+from copy import deepcopy
 
 from . import examples
 from .__version__ import __version__
 from .solvers.steady_state import solve_stst
 from .solvers.stacking import find_path_stacking
 from .solvers.solve_linear import find_path_linear
 from .solvers.solve_linear_state_space import solve_linear_state_space, find_path_linear_state_space
@@ -17,21 +17,26 @@
 
 
 # set number of cores for XLA
 os.environ["XLA_FLAGS"] = f"--xla_force_host_platform_device_count={os.cpu_count()}"
 
 jax.config.update("jax_enable_x64", True)
 
+# create local alias
+copy = deepcopy
+
 
 class PizzaModel(dict):
     """Base class for models. Contains all necessary methods and informations.
     """
 
-    def __init__(self, *args, **kwargs):
-        super(PizzaModel, self).__init__(*args, **kwargs)
+    def __init__(self, mdict, *args, **kwargs):
+        # do not overwrite original input
+        mdict = deepcopy(mdict)
+        super(PizzaModel, self).__init__(mdict, *args, **kwargs)
         self.__dict__ = self
 
     solve_stst = solve_stst
     find_path = find_path_stacking
 
     def get_distributions(model, trajectory, init_dist=None, shock=None, pars=None):
         """Get all disaggregated variables for a given trajectory of aggregate variables.
```

### Comparing `econpizza-0.5.2/econpizza/examples/bh.yml` & `econpizza-0.5.3/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/dsge.yml` & `econpizza-0.5.3/econpizza/examples/dsge.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/ghls.yml` & `econpizza-0.5.3/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank2.yml` & `econpizza-0.5.3/econpizza/examples/hank2.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank2_functions.py` & `econpizza-0.5.3/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.5.3/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank_functions.py` & `econpizza-0.5.3/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank_labor.yml` & `econpizza-0.5.3/econpizza/examples/hank_labor.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank_labor_functions.py` & `econpizza-0.5.3/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/hank_with_comments.yml` & `econpizza-0.5.3/econpizza/examples/hank_with_comments.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/nk.yml` & `econpizza-0.5.3/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/examples/tank.yml` & `econpizza-0.5.3/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/parser/__init__.py` & `econpizza-0.5.3/econpizza/parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     mtxt = mtxt.replace("   ~ ", "   - ")
 
     # get dict
     mdict = yaml.safe_load(mtxt)
     # create nice shortcuts
     mdict['path'] = mfile
     mdict["vars"] = mdict["variables"]
+    # load file with additional functions as module (if it exists)
+    _parse_external_functions_file(mdict)
 
     return mdict
 
 
 def _eval_strs(vdict, context={}):
     """Evaluate a dictionary of strings into a given context
     """
@@ -240,19 +242,23 @@
     # collect initial guesses
     init_guesses = _eval_strs(model["steady_state"].get(
         "init_guesses"), context=context)
     init_vals = _compile_init_values(
         evars, par_names, init_guesses, fixed_evaluated)
 
     # get the initial decision functions
-    if model.get('decisions'):
+    if model.get('distributions'):
         dist_names = list(model['distributions'].keys())
         # for now assume that this must be present
         init_wf = jnp.array([init_guesses[dec_input]
                             for dec_input in model['decisions']['inputs']])
+        # allow `n` in distributions to be a variable from the context (so far only for one distribution)
+        for d in model['distributions'][dist_names[0]].values():
+            if isinstance(d['n'], str):
+                d['n'] = eval(d['n'], context)
         # check if initial decision functions and the distribution have same shapes
         check_shapes(model['distributions'], init_wf, dist_names)
     else:
         init_wf = jnp.array(None)
 
     # define func_pre_stst
     mapping = _get_pre_stst_mapping(
@@ -287,31 +293,29 @@
     from ..__init__ import PizzaModel
 
     # parse if this is a path to yaml file
     if isinstance(model, str):
         full_path = model
         model = parse(model)
         model['path'] = full_path
-    # make it a model
-    model = PizzaModel(model)
-    # load file with additional functions as module (if it exists)
-    _parse_external_functions_file(model)
 
+    # define the model dictionary as key for cached models
     mdict = deepcopy(model)
     stst_subdict = mdict.pop('steady_state') if 'steady_state' in mdict else {}
-
     # check if model is already cached
     if mdict in cached_mdicts:
         model = copy(cached_models[cached_mdicts.index(mdict)])
         # always use the fresh current stst sec from yaml
         model['steady_state'] = stst_subdict
         if verbose:
             print("(load:) Loading cached model.")
         return model
 
+    # make it a model
+    model = PizzaModel(model)
     # initialize objects
     model['context'] = _initialize_context()
     model['cache'] = _initialize_cache()
     _load_external_functions_file(model, model['context'])
 
     # compile definitions
     defs = model.get("definitions")
@@ -322,15 +326,16 @@
     eqns = model["equations"].copy()
 
     # check if there are dublicate variables
     check_dublicates(model["variables"])
     check_dublicates(model.get("parameters"))
     evars = check_determinancy(model["variables"], eqns)
     # check if each variable is defined in time t (only defining xSS does not give a valid root)
-    check_if_defined(evars, eqns, model.get('skip_check_if_defined'))
+    check_if_defined(evars, eqns, model.get('decisions'),
+                     model.get('skip_check_if_defined'))
 
     # create fixed (time invariant) grids
     grids.create_grids(model.get('distributions'), model["context"], verbose)
     shocks = model.get("shocks") or ()
 
     # initialize storages
     _ = _define_subdict_if_absent(model, "func_strings")
```

### Comparing `econpizza-0.5.2/econpizza/parser/build_functions.py` & `econpizza-0.5.3/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/parser/checks.py` & `econpizza-0.5.3/econpizza/parser/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Checking functions for parsing.py.
 """
 
 import sys
 import jax.numpy as jnp
 from .build_functions import func_pre_stst
+import re
 
 
-def check_if_defined(evars, eqns, skipped_vars):
+def _strip_comments(code):
+    code = str(code)
+    return re.sub(r'(?m)^ *#.*\n?', '', code)
+
+
+def check_if_defined(evars, eqns, decisions, skipped_vars):
     """Check if all variables are defined in period t.
     """
     skipped_vars = [] if skipped_vars is None else skipped_vars
+    calls = _strip_comments(
+        decisions['calls']) if decisions is not None else ''
 
     for v in evars:
         v_in_eqns = [
             v in e.replace(v + "SS", "").replace(v + "Lag",
                                                  "").replace(v + "Prime", "")
             for e in eqns
         ]
-        if not any(v_in_eqns) and not v in skipped_vars:
+        v_in_calls = v in calls.replace(
+            v + "SS", "").replace(v + "Lag", "").replace(v + "Prime", "")
+        if not any(v_in_eqns) and not v_in_calls and not v in skipped_vars:
             raise Exception(f"Variable `{v}` is not defined for time t.")
     return
 
 
 def check_dublicates(evars):
     """Check if there are dublicates
     """
@@ -101,14 +111,15 @@
     if mess:
         raise Exception(mess + ' for initial values.')
     return
 
 
 def check_shapes(distributions, init_decisions, dist_names):
     decisions_shape = init_decisions.shape
+    # so far only for one distribution
     dist_shape = tuple([d.get('n')
                        for d in distributions[dist_names[0]].values()])
     check = [(ds == decisions_shape[-len(dist_shape):][i] or ds is None)
              for i, ds in enumerate(dist_shape)]
     if not all(check):
         raise Exception(
             f"Initial decisions and the distribution have different shapes in last dimensions: {decisions_shape}, {dist_shape}")
```

### Comparing `econpizza-0.5.2/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.5.3/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.5.3/econpizza/parser/write_dynamic_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,18 @@
             'More than one distribution is not yet implemented.')
 
     # already prepare for more than one distributions
     for dist_name in distributions:
 
         dist = distributions[dist_name]
 
-        implemented_endo = ('exogenous', 'exogenous_rouwenhorst')
-        implemented_exo = ('endogenous', 'endogenous_log')
+        implemented_endo = (
+            'exogenous', 'exogenous_rouwenhorst', 'exogenous_generic')
+        implemented_exo = ('endogenous', 'endogenous_log',
+                           'endogenous_generic')
         exog = [v for v in dist if dist[v]['type'] in implemented_endo]
         endo = [v for v in dist if dist[v]['type'] in implemented_exo]
         other = [dist[v]['type'] for v in dist if dist[v]
                  ['type'] not in implemented_endo + implemented_exo]
 
         if len(exog) > 1:
             raise NotImplementedError(
```

### Comparing `econpizza-0.5.2/econpizza/solvers/shooting.py` & `econpizza-0.5.3/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/solvers/solve_linear.py` & `econpizza-0.5.3/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.5.3/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/solvers/stacking.py` & `econpizza-0.5.3/econpizza/solvers/stacking.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/solvers/steady_state.py` & `econpizza-0.5.3/econpizza/solvers/steady_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     wfSS, decisions_output, cnt_backwards = res_backw
     distSS, cnt_forwards = res_forw
     decisions_output_names = model['decisions']['outputs']
 
     # compile informative message
     mess = ''
     if jnp.isnan(jnp.array(wfSS)).any() or jnp.isnan(jnp.array(decisions_output)).any():
-        mess += f"Backward iteration returns 'NaN's. "
+        mess += f"Backward iteration returns NaNs. "
     elif jnp.isnan(distSS).any():
-        mess += f"Forward iteration returns 'NaN's. "
+        mess += f"Forward iteration returns NaNs. "
     elif distSS.min() < 0:
         mess += f"Distribution contains negative values ({distSS.min():0.1e}). "
     if cnt_backwards == maxit_backwards:
         mess += f'Maximum of {maxit_backwards} backwards calls reached. '
     if cnt_forwards == maxit_forwards:
         mess += f'Maximum of {maxit_forwards} forwards calls reached. '
 
@@ -50,33 +50,33 @@
     """Solves for the steady state.
 
     Parameters
     ----------
     model : PizzaModel
         PizzaModel instance
     tol : float, optional
-        tolerance of the Newton method, defaults to 1e-8
+        tolerance of the Newton method, defaults to ``1e-8``
     maxit : int, optional
         maximum of iterations for the Newton method, defaults to 15
     tol_backwards : float, optional
-        tolerance required for backward iteration. Defaults to tol
+        tolerance required for backward iteration. Defaults to ``tol``
     maxit_backwards : int, optional
         maximum of iterations for the backward iteration. Defaults to 2000
     tol_forwards : float, optional
-        tolerance required for forward iteration. Defaults to tol
+        tolerance required for forward iteration. Defaults to ``tol*1e-2``
     maxit_forwards : int, optional
         maximum of iterations for the forward iteration. Defaults to 5000
     force : bool, optional
-        force recalculation of steady state, even if it is already evaluated. Defaults to False
+        force recalculation of steady state, even if it is already evaluated. Defaults to ``False``
     raise_errors : bool, optional
-        raise an error if Newton method does not converge. Useful for debuggin models. Defaults to True
+        raise an error if Newton method does not converge. Useful for debuggin models. Defaults to ``True``
     check_rank : bool, optional
-        force checking the rank of the Jacobian, even if the Newton method was successful. Defualts to False
+        force checking the rank of the Jacobian, even if the Newton method was successful. Defualts to ``False``
     verbose : bool, optional
-        level of verbosity. Defaults to True
+        level of verbosity. Defaults to ``True``
     newton_kwargs : keyword arguments
         keyword arguments passed on to the Newton method
 
     Returns
     -------
     rdict : dict
         a dictionary containing information about the root finding result. Note that the results are added to the model (PizzaModel instance) automatically, `rdict` is hence only useful for model debugging.
@@ -84,16 +84,16 @@
 
     st = time.time()
     evars = model["variables"]
     par_names = model["parameters"]
     shocks = model.get("shocks") or ()
 
     # default setup
-    tol_backwards = 1e-8 if tol_backwards is None else tol_backwards
-    tol_forwards = 1e-10 if tol_forwards is None else tol_forwards
+    tol_backwards = tol if tol_backwards is None else tol_backwards
+    tol_forwards = tol*1e-2 if tol_forwards is None else tol_forwards
     setup = tol, maxit, tol_backwards, maxit_backwards, tol_forwards, maxit_forwards
 
     # parse and compile steady_state section from yaml
     init_vals, fixed_vals, init_wf, pre_stst_mapping = compile_stst_inputs(
         model)
 
     # check if model is already cached
@@ -170,15 +170,17 @@
     if mess:
         not_var_nor_par = list(
             set(model['steady_state']['fixed_values']) - set(evars) - set(par_names))
         mess += f"Fixed value(s) ``{'``, ``'.join(not_var_nor_par)}`` not defined. " if not_var_nor_par else ''
 
     if err > tol or not res['success']:
         if not res["success"] or raise_errors:
-            mess = f"Steady state FAILED (max. error is {err:1.2e} in eqn. {errarg}). {res['message']} {mess}"
+            location = '' if jnp.isnan(
+                err) else f" (max. error is {err:1.2e} in eqn. {errarg})"
+            mess = f"Steady state FAILED{location}. {res['message']} {mess}"
         else:
             mess = f"{res['message']} WARNING: Steady state error is {err:1.2e} in eqn. {errarg}. {mess}"
         if raise_errors:
             raise Exception(mess)
     elif verbose:
         duration = time.time() - st
         mess = f"Steady state found ({duration:1.5g}s). {res['message']}" + (
```

### Comparing `econpizza-0.5.2/econpizza/testing/cache/bh.npy` & `econpizza-0.5.3/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.5.3/econpizza/testing/cache/hank_labor.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/testing/cache/hank_solid.npy` & `econpizza-0.5.3/econpizza/testing/cache/hank_solid.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/testing/test_rest.py` & `econpizza-0.5.3/econpizza/testing/test_rest.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/tools.py` & `econpizza-0.5.3/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/utilities/dists.py` & `econpizza-0.5.3/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/utilities/grids.py` & `econpizza-0.5.3/econpizza/utilities/grids.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     if not distributions:
         return
 
     grid_strings = ()
 
     if verbose:
-        print("Creating grid variables...")
+        print("Creating grid variables:")
 
     # create strings of the function that define the grids
     for dist_name, dist in distributions.items():
         for grid_name, g in dist.items():
 
             # shortcuts
             g['type'] = 'endogenous_log' if g['type'] == 'endogenous' else g['type']
@@ -80,19 +80,19 @@
 
             g['grid_name'] = grid_name + '_grid'
             # generic grid added by the user
             if g['type'] == 'exogenous_generic':
                 g['transition_name'] = grid_name + '_transition'
                 if verbose:
                     print(
-                        f"    ...expecting the objects '{g['transition_name']}' and '{g['grid_name']}' for the exogenous grid of '{grid_name}'")
+                        f"    ...expecting the objects '{g['transition_name']}' and '{g['grid_name']}' for the exogenous grid of '{grid_name}'.")
             if g['type'] == 'endogenous_generic':
                 if verbose:
                     print(
-                        f"    ...dxpecting the object '{g['grid_name']}' for the endogenous grid of '{grid_name}'")
+                        f"    ...expecting the object '{g['grid_name']}' for the endogenous grid of '{grid_name}'.")
 
             # predefined grids
             if g['type'] == 'exogenous_rouwenhorst':
                 grid_strings += f"{grid_name}_grid, {grid_name}_stationary, {grid_name}_transition = grids.markov_rouwenhorst(rho={g['rho']}, sigma={g['sigma']}, N={g['n']})",
                 g['transition_name'] = grid_name + '_transition'
                 if verbose:
                     print(
```

### Comparing `econpizza-0.5.2/econpizza/utilities/interp.py` & `econpizza-0.5.3/econpizza/utilities/interp.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/utilities/jacobian.py` & `econpizza-0.5.3/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/econpizza/utilities/newton.py` & `econpizza-0.5.3/econpizza/utilities/newton.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Newton heavy lifting functions and helpers
 """
 
+from grgrjax import jax_print
 import jax
 import time
 import jax.numpy as jnp
 from functools import partial
 from jax._src.lax.linalg import lu_solve
 from grgrjax import callback_func, amax, newton_jax_jit
 
 
-def callback_with_damp(cnt, err, fev, dampening, ltime, verbose): return callback_func(
-    cnt, err, fev=fev, misc=('dampening', dampening), ltime=ltime, verbose=verbose)
+def callback_with_damp(cnt, err, fev, err_inner, dampening, ltime, verbose):
+    inner = f' | inner {err_inner:.2e}'
+    damp = f' | dampening {dampening:1.3f}'
+    return callback_func(cnt, err, inner, damp, fev=fev, ltime=ltime, verbose=verbose)
 
 
 def iteration_step(carry):
     (y, dampening, fev), (x, f, jvp_func, jacobian, factor), (_, tol, maxit) = carry
     _, v = jvp_func(x, y)
     v = lu_solve(*jacobian[0], v, 0)[jacobian[1]]
     dampening = jnp.minimum(dampening, factor*jnp.abs((y.T@y)/(v.T@y)))
@@ -26,35 +29,36 @@
 
 def iteration_cond(carry):
     (_, _, fev), _, (eps, tol, maxit) = carry
     return jnp.logical_and(fev <= maxit, eps > tol)
 
 
 def jvp_while_body(carry):
-    (x, _, _, cnt, fev), (jvp_func, jacobian, maxit,
-                          nsteps, tol, factor, verbose) = carry
+    (x, _, _, cnt, fev, _), (jvp_func, jacobian, maxit,
+                             nsteps, tol, factor, verbose) = carry
     # first iteration
     f, _ = jvp_func(x, jnp.zeros_like(x))
     f = lu_solve(*jacobian[0], f, 0)[jacobian[1]]
     # other iterations
     iteration_tol = jnp.minimum(1e-5, 1e-1*amax(f))
     init = ((f, 1., 0), (x, f, jvp_func, jacobian, factor),
             (1e8, iteration_tol, nsteps))
-    (y, dampening, fev_inner), _, _ = jax.lax.while_loop(
+    (y, dampening, fev_inner), _, (err_inner, _, _) = jax.lax.while_loop(
         iteration_cond, iteration_step, init)
-    return (x-y, amax(f), dampening, cnt+1, fev+fev_inner), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)
+    return (x-y, amax(f), dampening, cnt+1, fev+fev_inner, err_inner), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)
 
 
 def jvp_while_cond(carry):
-    (_, err, dampening, cnt, fev), (_, _, maxit, nsteps, tol, _, verbose) = carry
-    cond = jnp.logical_and(err > tol, fev < maxit)
+    (_, err, dampening, cnt, fev, err_inner), (_,
+                                               _, maxit, nsteps, tol, _, verbose) = carry
+    cond = jnp.logical_and(err > tol, cnt < maxit)
     verbose = jnp.logical_and(cond, verbose)
     verbose = jnp.logical_and(fev, verbose)
     jax.debug.callback(callback_with_damp, cnt, err, fev=fev,
-                       dampening=dampening, ltime=None, verbose=verbose)
+                       err_inner=err_inner, dampening=dampening, ltime=None, verbose=verbose)
     return cond
 
 
 def sweep_banded_down(val, i):
     jav_func, fmod, forward_mat, X, shocks = val
     # calculate value and jacobians
     fval, (jac_f2xLag, jac_f2x, jac_f2xPrime) = jav_func(
@@ -74,31 +78,31 @@
 
 def check_status(err, cnt, maxit, tol):
     """Check whether to exit iteration and compile error message"""
     # exit causes
     if err < tol:
         return True, (True, "The solution converged.")
     elif jnp.isnan(err):
-        return True, (False, "Function returns 'NaN's.")
-    elif cnt > maxit:
+        return True, (False, "Function returns NaNs.")
+    elif cnt >= maxit:
         return True, (False, f"Maximum number of {maxit} iterations reached.")
     else:
         return False, (False, "")
 
 
 def newton_for_jvp(jvp_func, jacobian, x_init, verbose, tol=1e-8, maxit=500, nsteps=30, factor=1.5):
 
     start_time = time.time()
     x = x_init[1:-1].flatten()
 
-    (x, err, dampening, cnt, fev), _ = jax.lax.while_loop(jvp_while_cond, jvp_while_body,
-                                                          ((x, 1., 0., 0, 0), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)))
+    (x, err, dampening, cnt, fev, err_inner), _ = jax.lax.while_loop(jvp_while_cond, jvp_while_body,
+                                                                     ((x, 1., 0., 0, 0, 0), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)))
     ltime = time.time() - start_time
-    callback_with_damp(cnt, err, fev=fev, dampening=dampening,
-                       ltime=ltime, verbose=verbose)
+    callback_with_damp(cnt, err, fev=fev, err_inner=err_inner,
+                       dampening=dampening, ltime=ltime, verbose=verbose)
     _, (success, mess) = check_status(err, cnt, maxit, tol)
     # compile error/report message
     if not success and not jnp.isnan(err):
         mess += f" Max. error is {err:1.2e}."
 
     return x, not success, mess
 
@@ -126,15 +130,15 @@
             print(info_str)
 
         do_break, (success, mess) = check_status(err, cnt, maxit, tol)
         if do_break:
             break
 
     if not success:
-        mess += f" Max. error is {err:1.2e}."
+        mess += f"Max. error is {err:1.2e}."
 
     return X, False, ''
 
 
 def newton_jax_jit_wrapper(func, init, **args):
     """Wrapper around grgrjax.newton.newton_jax_jit to return flag and message
     """
```

### Comparing `econpizza-0.5.2/econpizza.egg-info/PKG-INFO` & `econpizza-0.5.3/econpizza.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.2
+Version: 0.5.3
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.5.2/econpizza.egg-info/SOURCES.txt` & `econpizza-0.5.3/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.2/setup.py` & `econpizza-0.5.3/setup.py`

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
-        "jax>=0.3.20,<0.4.6",
-        "jaxlib>=0.3.20,<0.4.6",
+        "jax",
+        "jaxlib",
         "grgrjax>=0.4.1",
         "pyyaml",
         "scipy",
     ],
 )
```

