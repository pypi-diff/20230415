# Comparing `tmp/mizani-0.8.1.tar.gz` & `tmp/mizani-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizani-0.8.1.tar", last modified: Wed Sep 28 13:42:35 2022, max compression
+gzip compressed data, was "mizani-0.9.0.tar", last modified: Sat Apr 15 15:00:08 2023, max compression
```

## Comparing `mizani-0.8.1.tar` & `mizani-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,106 @@
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.299377 mizani-0.8.1/
--rw-r--r--   0 hassan     (503) staff       (20)       32 2016-06-28 12:36:41.000000 mizani-0.8.1/.gitattributes
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.241001 mizani-0.8.1/.github/
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.250509 mizani-0.8.1/.github/workflows/
--rw-r--r--   0 hassan     (503) staff       (20)     2814 2022-09-01 13:59:24.000000 mizani-0.8.1/.github/workflows/testing.yml
--rw-r--r--   0 hassan     (503) staff       (20)      751 2022-07-06 06:38:46.000000 mizani-0.8.1/.gitignore
--rw-r--r--   0 hassan     (503) staff       (20)      660 2022-06-23 11:43:31.000000 mizani-0.8.1/.readthedocs.yml
--rw-r--r--   0 hassan     (503) staff       (20)     1478 2016-06-28 12:36:41.000000 mizani-0.8.1/LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)       27 2022-06-23 11:43:31.000000 mizani-0.8.1/MANIFEST.in
--rw-r--r--   0 hassan     (503) staff       (20)     1549 2022-06-23 11:43:31.000000 mizani-0.8.1/Makefile
--rw-r--r--   0 hassan     (503) staff       (20)     2395 2022-09-28 13:42:35.299723 mizani-0.8.1/PKG-INFO
--rw-r--r--   0 hassan     (503) staff       (20)     1433 2022-06-23 11:43:31.000000 mizani-0.8.1/README.rst
--rw-r--r--   0 hassan     (503) staff       (20)      329 2022-06-23 11:43:31.000000 mizani-0.8.1/codecov.yml
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.256474 mizani-0.8.1/doc/
--rw-r--r--   0 hassan     (503) staff       (20)     7238 2022-09-26 09:54:13.000000 mizani-0.8.1/doc/Makefile
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.257638 mizani-0.8.1/doc/_static/
--rw-r--r--   0 hassan     (503) staff       (20)     3143 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/_static/copybutton.js
--rw-r--r--   0 hassan     (503) staff       (20)     2494 2022-06-23 11:43:31.000000 mizani-0.8.1/doc/_static/custom.css
--rw-r--r--   0 hassan     (503) staff       (20)      148 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/bounds.rst
--rw-r--r--   0 hassan     (503) staff       (20)      182 2022-04-01 15:37:12.000000 mizani-0.8.1/doc/breaks.rst
--rw-r--r--   0 hassan     (503) staff       (20)    11879 2022-09-28 12:25:15.000000 mizani-0.8.1/doc/changelog.rst
--rw-r--r--   0 hassan     (503) staff       (20)    11582 2022-06-23 11:43:31.000000 mizani-0.8.1/doc/conf.py
--rw-r--r--   0 hassan     (503) staff       (20)      118 2022-06-23 11:43:31.000000 mizani-0.8.1/doc/docutils.conf
--rw-r--r--   0 hassan     (503) staff       (20)      158 2020-06-03 18:30:42.000000 mizani-0.8.1/doc/formatters.rst
--rw-r--r--   0 hassan     (503) staff       (20)      362 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/index.rst
--rw-r--r--   0 hassan     (503) staff       (20)      967 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/installation.rst
--rw-r--r--   0 hassan     (503) staff       (20)      170 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/palettes.rst
--rw-r--r--   0 hassan     (503) staff       (20)      116 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/scale.rst
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.258814 mizani-0.8.1/doc/sphinxext/
--rw-r--r--   0 hassan     (503) staff       (20)        0 2016-06-28 12:36:41.000000 mizani-0.8.1/doc/sphinxext/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)      416 2022-06-23 11:43:31.000000 mizani-0.8.1/doc/sphinxext/inline_code_highlight.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.268131 mizani-0.8.1/doc/theme/
--rw-r--r--   0 hassan     (503) staff       (20)      455 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/globaltoc.html
--rw-r--r--   0 hassan     (503) staff       (20)     3664 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/layout.html
--rw-r--r--   0 hassan     (503) staff       (20)       10 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/localtoc.html
--rw-r--r--   0 hassan     (503) staff       (20)     2002 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/navbar-2.html
--rw-r--r--   0 hassan     (503) staff       (20)     2072 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/navbar.html
--rw-r--r--   0 hassan     (503) staff       (20)      360 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/navbarsearchbox.html
--rw-r--r--   0 hassan     (503) staff       (20)      305 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/navbartoc.html
--rw-r--r--   0 hassan     (503) staff       (20)     1111 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/relations.html
--rw-r--r--   0 hassan     (503) staff       (20)     2614 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/search.html
--rw-r--r--   0 hassan     (503) staff       (20)      327 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/searchbox.html
--rw-r--r--   0 hassan     (503) staff       (20)     1120 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/searchresults.html
--rw-r--r--   0 hassan     (503) staff       (20)      195 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/sourcelink.html
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.269753 mizani-0.8.1/doc/theme/static/
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.241921 mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.270644 mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/css/
--rw-r--r--   0 hassan     (503) staff       (20)   124541 2022-09-26 09:54:13.000000 mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.272741 mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/js/
--rw-r--r--   0 hassan     (503) staff       (20)    40021 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
--rw-r--r--   0 hassan     (503) staff       (20)     5924 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/static/bootstrap-sphinx.css_t
--rw-r--r--   0 hassan     (503) staff       (20)     5162 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/static/bootstrap-sphinx.js_t
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.275932 mizani-0.8.1/doc/theme/static/js/
--rw-r--r--   0 hassan     (503) staff       (20)    97163 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/static/js/jquery-1.12.4.min.js
--rw-r--r--   0 hassan     (503) staff       (20)       90 2022-09-25 14:26:17.000000 mizani-0.8.1/doc/theme/static/js/jquery-fix.js
--rw-r--r--   0 hassan     (503) staff       (20)     1860 2022-09-26 09:54:13.000000 mizani-0.8.1/doc/theme/theme.conf
--rw-r--r--   0 hassan     (503) staff       (20)      188 2018-10-03 08:09:15.000000 mizani-0.8.1/doc/transforms.rst
--rw-r--r--   0 hassan     (503) staff       (20)     1344 2022-06-23 11:43:31.000000 mizani-0.8.1/how-to-release.rst
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.280124 mizani-0.8.1/licences/
--rw-r--r--   0 hassan     (503) staff       (20)     1059 2016-06-28 12:36:41.000000 mizani-0.8.1/licences/HUSL_LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)       77 2016-06-28 12:36:41.000000 mizani-0.8.1/licences/SCALES_LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)     1498 2016-06-28 12:36:41.000000 mizani-0.8.1/licences/SEABORN_LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)     1066 2016-06-28 12:36:41.000000 mizani-0.8.1/licences/SIX_LICENSE
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.285151 mizani-0.8.1/mizani/
--rw-r--r--   0 hassan     (503) staff       (20)      173 2022-07-31 19:48:52.000000 mizani-0.8.1/mizani/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)    14985 2022-09-26 09:54:13.000000 mizani-0.8.1/mizani/bounds.py
--rw-r--r--   0 hassan     (503) staff       (20)    26214 2022-09-01 14:01:36.000000 mizani-0.8.1/mizani/breaks.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.290583 mizani-0.8.1/mizani/external/
--rw-r--r--   0 hassan     (503) staff       (20)      104 2018-10-03 08:09:15.000000 mizani-0.8.1/mizani/external/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)     5055 2018-10-03 08:09:15.000000 mizani-0.8.1/mizani/external/crayon_rgb.py
--rw-r--r--   0 hassan     (503) staff       (20)     6488 2017-01-28 08:50:04.000000 mizani-0.8.1/mizani/external/husl.py
--rw-r--r--   0 hassan     (503) staff       (20)    28029 2018-10-03 08:09:15.000000 mizani-0.8.1/mizani/external/xkcd_rgb.py
--rw-r--r--   0 hassan     (503) staff       (20)    23009 2022-09-28 12:35:01.000000 mizani-0.8.1/mizani/formatters.py
--rw-r--r--   0 hassan     (503) staff       (20)    24027 2022-09-26 09:54:13.000000 mizani-0.8.1/mizani/palettes.py
--rw-r--r--   0 hassan     (503) staff       (20)     7504 2022-06-23 11:43:31.000000 mizani-0.8.1/mizani/scale.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.295595 mizani-0.8.1/mizani/tests/
--rw-r--r--   0 hassan     (503) staff       (20)        0 2022-06-23 11:43:31.000000 mizani-0.8.1/mizani/tests/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)    14012 2022-09-26 09:54:13.000000 mizani-0.8.1/mizani/tests/test_bounds.py
--rw-r--r--   0 hassan     (503) staff       (20)     8231 2022-06-23 11:43:31.000000 mizani-0.8.1/mizani/tests/test_breaks.py
--rw-r--r--   0 hassan     (503) staff       (20)     7644 2022-09-28 12:36:34.000000 mizani-0.8.1/mizani/tests/test_formatters.py
--rw-r--r--   0 hassan     (503) staff       (20)     5684 2022-09-26 09:54:13.000000 mizani-0.8.1/mizani/tests/test_palettes.py
--rw-r--r--   0 hassan     (503) staff       (20)     3749 2022-06-23 11:43:31.000000 mizani-0.8.1/mizani/tests/test_scale.py
--rw-r--r--   0 hassan     (503) staff       (20)     7041 2022-09-02 13:13:02.000000 mizani-0.8.1/mizani/tests/test_transforms.py
--rw-r--r--   0 hassan     (503) staff       (20)     4265 2022-06-23 11:43:31.000000 mizani-0.8.1/mizani/tests/test_utils.py
--rw-r--r--   0 hassan     (503) staff       (20)    21762 2022-09-01 14:01:36.000000 mizani-0.8.1/mizani/transforms.py
--rw-r--r--   0 hassan     (503) staff       (20)     6243 2022-09-02 13:12:01.000000 mizani-0.8.1/mizani/utils.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.288340 mizani-0.8.1/mizani.egg-info/
--rw-r--r--   0 hassan     (503) staff       (20)     2395 2022-09-28 13:42:35.000000 mizani-0.8.1/mizani.egg-info/PKG-INFO
--rw-r--r--   0 hassan     (503) staff       (20)     1915 2022-09-28 13:42:35.000000 mizani-0.8.1/mizani.egg-info/SOURCES.txt
--rw-r--r--   0 hassan     (503) staff       (20)        1 2022-09-28 13:42:35.000000 mizani-0.8.1/mizani.egg-info/dependency_links.txt
--rw-r--r--   0 hassan     (503) staff       (20)        1 2022-09-28 13:42:35.000000 mizani-0.8.1/mizani.egg-info/not-zip-safe
--rw-r--r--   0 hassan     (503) staff       (20)      222 2022-09-28 13:42:35.000000 mizani-0.8.1/mizani.egg-info/requires.txt
--rw-r--r--   0 hassan     (503) staff       (20)        7 2022-09-28 13:42:35.000000 mizani-0.8.1/mizani.egg-info/top_level.txt
--rw-r--r--   0 hassan     (503) staff       (20)      684 2022-06-23 11:43:31.000000 mizani-0.8.1/pyproject.toml
--rw-r--r--   0 hassan     (503) staff       (20)      176 2022-06-23 11:43:31.000000 mizani-0.8.1/pytest.ini
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.297025 mizani-0.8.1/requirements/
--rw-r--r--   0 hassan     (503) staff       (20)       98 2022-06-23 11:43:31.000000 mizani-0.8.1/requirements/dev.txt
--rw-r--r--   0 hassan     (503) staff       (20)       41 2022-06-23 11:43:31.000000 mizani-0.8.1/requirements/rtd.txt
--rw-r--r--   0 hassan     (503) staff       (20)     1251 2022-09-28 13:42:35.301220 mizani-0.8.1/setup.cfg
--rw-r--r--   0 hassan     (503) staff       (20)       38 2022-06-23 11:43:31.000000 mizani-0.8.1/setup.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2022-09-28 13:42:35.298792 mizani-0.8.1/tools/
--rwxr-xr-x   0 hassan     (503) staff       (20)      862 2022-06-23 11:43:31.000000 mizani-0.8.1/tools/build_theme.sh
--rw-r--r--   0 hassan     (503) staff       (20)     2140 2018-10-03 08:09:15.000000 mizani-0.8.1/tools/release.sh
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.802698 mizani-0.9.0/
+-rw-r--r--   0 hassan     (503) staff       (20)       32 2016-06-28 12:36:41.000000 mizani-0.9.0/.gitattributes
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.738633 mizani-0.9.0/.github/
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.747629 mizani-0.9.0/.github/workflows/
+-rw-r--r--   0 hassan     (503) staff       (20)     2869 2023-03-18 11:25:34.000000 mizani-0.9.0/.github/workflows/testing.yml
+-rw-r--r--   0 hassan     (503) staff       (20)      751 2022-07-06 06:38:46.000000 mizani-0.9.0/.gitignore
+-rw-r--r--   0 hassan     (503) staff       (20)      271 2023-04-05 12:30:47.000000 mizani-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 hassan     (503) staff       (20)      528 2023-03-18 11:25:34.000000 mizani-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 hassan     (503) staff       (20)     1478 2016-06-28 12:36:41.000000 mizani-0.9.0/LICENSE
+-rw-r--r--   0 hassan     (503) staff       (20)     1565 2023-04-15 14:59:50.000000 mizani-0.9.0/Makefile
+-rw-r--r--   0 hassan     (503) staff       (20)     3753 2023-04-15 15:00:08.801986 mizani-0.9.0/PKG-INFO
+-rw-r--r--   0 hassan     (503) staff       (20)     1043 2023-04-15 14:59:50.000000 mizani-0.9.0/README.md
+-rw-r--r--   0 hassan     (503) staff       (20)      375 2023-02-27 19:00:09.000000 mizani-0.9.0/codecov.yml
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.752917 mizani-0.9.0/doc/
+-rw-r--r--   0 hassan     (503) staff       (20)     1134 2023-02-27 19:00:09.000000 mizani-0.9.0/doc/Makefile
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.753629 mizani-0.9.0/doc/_static/
+-rw-r--r--   0 hassan     (503) staff       (20)     3143 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/_static/copybutton.js
+-rw-r--r--   0 hassan     (503) staff       (20)     2494 2022-06-23 11:43:31.000000 mizani-0.9.0/doc/_static/custom.css
+-rw-r--r--   0 hassan     (503) staff       (20)      148 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/bounds.rst
+-rw-r--r--   0 hassan     (503) staff       (20)      182 2022-04-01 15:37:12.000000 mizani-0.9.0/doc/breaks.rst
+-rw-r--r--   0 hassan     (503) staff       (20)    12437 2023-04-15 14:59:50.000000 mizani-0.9.0/doc/changelog.rst
+-rw-r--r--   0 hassan     (503) staff       (20)    11659 2023-03-18 11:25:34.000000 mizani-0.9.0/doc/conf.py
+-rw-r--r--   0 hassan     (503) staff       (20)      118 2022-06-23 11:43:31.000000 mizani-0.9.0/doc/docutils.conf
+-rw-r--r--   0 hassan     (503) staff       (20)      158 2020-06-03 18:30:42.000000 mizani-0.9.0/doc/formatters.rst
+-rw-r--r--   0 hassan     (503) staff       (20)      362 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/index.rst
+-rw-r--r--   0 hassan     (503) staff       (20)      967 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/installation.rst
+-rw-r--r--   0 hassan     (503) staff       (20)      170 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/palettes.rst
+-rw-r--r--   0 hassan     (503) staff       (20)      116 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/scale.rst
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.754597 mizani-0.9.0/doc/sphinxext/
+-rw-r--r--   0 hassan     (503) staff       (20)        0 2016-06-28 12:36:41.000000 mizani-0.9.0/doc/sphinxext/__init__.py
+-rw-r--r--   0 hassan     (503) staff       (20)      368 2023-03-18 11:25:34.000000 mizani-0.9.0/doc/sphinxext/inline_code_highlight.py
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.764599 mizani-0.9.0/doc/theme/
+-rw-r--r--   0 hassan     (503) staff       (20)      455 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/globaltoc.html
+-rw-r--r--   0 hassan     (503) staff       (20)     3664 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/layout.html
+-rw-r--r--   0 hassan     (503) staff       (20)       10 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/localtoc.html
+-rw-r--r--   0 hassan     (503) staff       (20)     2002 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbar-2.html
+-rw-r--r--   0 hassan     (503) staff       (20)     2072 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbar.html
+-rw-r--r--   0 hassan     (503) staff       (20)      360 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbarsearchbox.html
+-rw-r--r--   0 hassan     (503) staff       (20)      305 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbartoc.html
+-rw-r--r--   0 hassan     (503) staff       (20)     1111 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/relations.html
+-rw-r--r--   0 hassan     (503) staff       (20)     2614 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/search.html
+-rw-r--r--   0 hassan     (503) staff       (20)      327 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/searchbox.html
+-rw-r--r--   0 hassan     (503) staff       (20)     1120 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/searchresults.html
+-rw-r--r--   0 hassan     (503) staff       (20)      195 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/sourcelink.html
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.766241 mizani-0.9.0/doc/theme/static/
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.739888 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.766967 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/css/
+-rw-r--r--   0 hassan     (503) staff       (20)   124135 2023-02-27 19:00:09.000000 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.768253 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/js/
+-rw-r--r--   0 hassan     (503) staff       (20)    40021 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
+-rw-r--r--   0 hassan     (503) staff       (20)     5924 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/bootstrap-sphinx.css_t
+-rw-r--r--   0 hassan     (503) staff       (20)     5162 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/bootstrap-sphinx.js_t
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.770288 mizani-0.9.0/doc/theme/static/js/
+-rw-r--r--   0 hassan     (503) staff       (20)    97163 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/js/jquery-1.12.4.min.js
+-rw-r--r--   0 hassan     (503) staff       (20)       90 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/js/jquery-fix.js
+-rw-r--r--   0 hassan     (503) staff       (20)     1895 2023-02-27 19:00:09.000000 mizani-0.9.0/doc/theme/theme.conf
+-rw-r--r--   0 hassan     (503) staff       (20)      188 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/transforms.rst
+-rw-r--r--   0 hassan     (503) staff       (20)     1344 2022-06-23 11:43:31.000000 mizani-0.9.0/how-to-release.rst
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.773038 mizani-0.9.0/licences/
+-rw-r--r--   0 hassan     (503) staff       (20)     1059 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/HUSL_LICENSE
+-rw-r--r--   0 hassan     (503) staff       (20)       77 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/SCALES_LICENSE
+-rw-r--r--   0 hassan     (503) staff       (20)     1498 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/SEABORN_LICENSE
+-rw-r--r--   0 hassan     (503) staff       (20)     1066 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/SIX_LICENSE
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.781426 mizani-0.9.0/mizani/
+-rw-r--r--   0 hassan     (503) staff       (20)      172 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/__init__.py
+-rw-r--r--   0 hassan     (503) staff       (20)    15042 2023-03-18 11:55:22.000000 mizani-0.9.0/mizani/bounds.py
+-rw-r--r--   0 hassan     (503) staff       (20)    26005 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/breaks.py
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.786220 mizani-0.9.0/mizani/colors/
+-rw-r--r--   0 hassan     (503) staff       (20)        0 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/__init__.py
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.789042 mizani-0.9.0/mizani/colors/brewer/
+-rw-r--r--   0 hassan     (503) staff       (20)     1717 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/__init__.py
+-rw-r--r--   0 hassan     (503) staff       (20)    17728 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/diverging.py
+-rw-r--r--   0 hassan     (503) staff       (20)    11725 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/qualitative.py
+-rw-r--r--   0 hassan     (503) staff       (20)    24032 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/sequential.py
+-rw-r--r--   0 hassan     (503) staff       (20)     1942 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/color_palette.py
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.792109 mizani-0.9.0/mizani/external/
+-rw-r--r--   0 hassan     (503) staff       (20)      104 2018-10-03 08:09:15.000000 mizani-0.9.0/mizani/external/__init__.py
+-rw-r--r--   0 hassan     (503) staff       (20)     5055 2018-10-03 08:09:15.000000 mizani-0.9.0/mizani/external/crayon_rgb.py
+-rw-r--r--   0 hassan     (503) staff       (20)     6488 2017-01-28 08:50:04.000000 mizani-0.9.0/mizani/external/husl.py
+-rw-r--r--   0 hassan     (503) staff       (20)    28029 2018-10-03 08:09:15.000000 mizani-0.9.0/mizani/external/xkcd_rgb.py
+-rw-r--r--   0 hassan     (503) staff       (20)    23347 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/formatters.py
+-rw-r--r--   0 hassan     (503) staff       (20)    22690 2023-04-05 12:44:26.000000 mizani-0.9.0/mizani/palettes.py
+-rw-r--r--   0 hassan     (503) staff       (20)     7476 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/scale.py
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.799531 mizani-0.9.0/mizani/tests/
+-rw-r--r--   0 hassan     (503) staff       (20)        0 2022-06-23 11:43:31.000000 mizani-0.9.0/mizani/tests/__init__.py
+-rw-r--r--   0 hassan     (503) staff       (20)    13788 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_bounds.py
+-rw-r--r--   0 hassan     (503) staff       (20)     8245 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_breaks.py
+-rw-r--r--   0 hassan     (503) staff       (20)     7749 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_formatters.py
+-rw-r--r--   0 hassan     (503) staff       (20)     6085 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/tests/test_palettes.py
+-rw-r--r--   0 hassan     (503) staff       (20)     3719 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_scale.py
+-rw-r--r--   0 hassan     (503) staff       (20)     7102 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_transforms.py
+-rw-r--r--   0 hassan     (503) staff       (20)     4229 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_utils.py
+-rw-r--r--   0 hassan     (503) staff       (20)    21685 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/transforms.py
+-rw-r--r--   0 hassan     (503) staff       (20)      698 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/typing.py
+-rw-r--r--   0 hassan     (503) staff       (20)     6684 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/utils.py
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.785058 mizani-0.9.0/mizani.egg-info/
+-rw-r--r--   0 hassan     (503) staff       (20)     3753 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/PKG-INFO
+-rw-r--r--   0 hassan     (503) staff       (20)     2038 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/SOURCES.txt
+-rw-r--r--   0 hassan     (503) staff       (20)        1 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/dependency_links.txt
+-rw-r--r--   0 hassan     (503) staff       (20)      377 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/requires.txt
+-rw-r--r--   0 hassan     (503) staff       (20)        7 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/top_level.txt
+-rw-r--r--   0 hassan     (503) staff       (20)     3412 2023-04-15 14:59:50.000000 mizani-0.9.0/pyproject.toml
+-rw-r--r--   0 hassan     (503) staff       (20)       38 2023-04-15 15:00:08.802884 mizani-0.9.0/setup.cfg
+drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.800991 mizani-0.9.0/tools/
+-rwxr-xr-x   0 hassan     (503) staff       (20)      862 2022-06-23 11:43:31.000000 mizani-0.9.0/tools/build_theme.sh
+-rw-r--r--   0 hassan     (503) staff       (20)     2116 2023-04-15 14:59:50.000000 mizani-0.9.0/tools/release.sh
```

### Comparing `mizani-0.8.1/.gitignore` & `mizani-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/.readthedocs.yml` & `mizani-0.9.0/.readthedocs.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# .readthedocs.yml
+# .readthedocs.yaml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
+# Set the version of Python and other tools you might need
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: doc/conf.py
 
-# Build documentation with MkDocs
-#mkdocs:
-#  configuration: mkdocs.yml
-
-# Optionally build your docs in additional formats such as PDF
-# formats:
-#   - pdf
-
-# Optionally set the version of Python and requirements required to build your docs
-# system_packages includes numpy, ...
+# Optionally declare the Python requirements required to build your docs
 python:
-  version: 3.8
   install:
-    - requirements: requirements/rtd.txt
     - method: pip
       path: .
-  system_packages: true
+      extra_requirements:
+        - doc
```

### Comparing `mizani-0.8.1/LICENSE` & `mizani-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/Makefile` & `mizani-0.9.0/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.PHONY: clean-pyc clean-build doc clean
+.PHONY: clean-pyc clean-build doc clean build
 BROWSER := python -mwebbrowser
 
 help:
 	@echo "clean - remove all build, test, coverage and Python artifacts"
 	@echo "clean-build - remove build artifacts"
 	@echo "clean-pyc - remove Python file artifacts"
 	@echo "clean-test - remove test and coverage artifacts"
@@ -16,32 +16,41 @@
 	@echo "install - install the package to the active Python's site-packages"
 
 clean: clean-build clean-pyc clean-test
 
 clean-build:
 	rm -fr build/
 	rm -fr dist/
-	rm -fr .eggs/
-	find . -name '*.egg-info' -exec rm -fr {} +
-	find . -name '*.egg' -exec rm -f {} +
 
 clean-pyc:
-	find . -name '*.pyc' -exec rm -f {} +
-	find . -name '*.pyo' -exec rm -f {} +
-	find . -name '*~' -exec rm -f {} +
 	find . -name '__pycache__' -exec rm -fr {} +
 
 clean-test:
-	rm -fr .tox/
 	rm -f .coverage
 	rm -f coverage.xml
 	rm -fr htmlcov/
 
-lint:
-	flake8 mizani
+ruff:
+	ruff mizani $(args)
+
+ruff-isort:
+	ruff --select I001 --quiet mizani $(args)
+
+format:
+	black . --check
+
+format-fix:
+	black .
+
+lint: ruff ruff-isort
+
+lint-fix:
+	make lint args="--fix"
+
+fix: format-fix lint-fix
 
 test:
 	pytest
 
 test-all:
 	tox
 
@@ -54,13 +63,19 @@
 	$(MAKE) -C doc clean
 	$(MAKE) -C doc html
 	$(BROWSER) doc/_build/html/index.html
 
 release: clean
 	bash ./tools/release.sh
 
-dist: clean
-	python setup.py sdist bdist_wheel
+build: clean
+	python -m build
+
+dist: build
 	ls -l dist
 
+develop: clean-pyc
+	pip install -e ".[all]"
+
 install: clean
-	python setup.py install
+	ls -l dist
+	pip install .
```

### Comparing `mizani-0.8.1/doc/_static/copybutton.js` & `mizani-0.9.0/doc/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/_static/custom.css` & `mizani-0.9.0/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/changelog.rst` & `mizani-0.9.0/doc/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,37 @@
 Changelog
 =========
 
+v0.9.0
+------
+
+*2023-04-15*
+
+API Changes
+************
+
+- `palettable` dropped as a dependency.
+
+Bug Fixes
+*********
+
+- Fixed bug in :class:`~mizani.transforms.datetime_trans` where
+  a pandas series with an index that did not start at 0 could not
+  be transformed.
+
+- Install tzdata on pyiodide/emscripten. :issue:`27`
+
 v0.8.1
 ------
 
 *2022-09-28*
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7120121.svg
+   :target: https://doi.org/10.5281/zenodo.7120121
+
 Bug Fixes
 *********
 
 - Fixed regression bug in :class:`~mizani.formatters.log_format` for
   where formatting for bases 2, 8 and 16 would fail if the values were
   float-integers.
 
@@ -19,14 +41,17 @@
   for bases other than base 10.
 
 v0.8.0
 ------
 
 *2022-09-26*
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7113103.svg
+   :target: https://doi.org/10.5281/zenodo.7113103
+
 API Changes
 ***********
 
 - The ``lut`` parameter of :class:`~mizani.palettes.cmap_pal` and
   :class:`~mizani.palettes.cmap_d_pal` has been deprecated and will
   removed in a future version.
```

### Comparing `mizani-0.8.1/doc/conf.py` & `mizani-0.9.0/doc/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,108 +8,110 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys
 import os
-
+import sys
 from pathlib import Path
 
-on_rtd = os.environ.get('READTHEDOCS') == 'True'
+on_rtd = os.environ.get("READTHEDOCS") == "True"
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 CUR_PATH = Path(__file__).parent
 PROJECT_PATH = CUR_PATH.parent
 
 sys.path.insert(0, str(CUR_PATH))
 sys.path.insert(0, str(PROJECT_PATH))
 
 if on_rtd:
-    import mock
     from pprint import pprint
+
+    import mock
+
     MOCK_MODULES = [
-        'pandas',
-        'pandas.core',
-        'pandas.core.common',
-        'pandas.core.dtypes.common',
-        'pandas.api',
-        'pandas.api.types']
+        "pandas",
+        "pandas.core",
+        "pandas.core.common",
+        "pandas.core.dtypes.common",
+        "pandas.api",
+        "pandas.api.types",
+    ]
     for mod_name in MOCK_MODULES:
         sys.modules[mod_name] = mock.Mock()
     pprint(os.environ)
     pprint(sys.path)
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-needs_sphinx = '3.0.0'
+needs_sphinx = "3.0.0"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.doctest',
-    'sphinx.ext.extlinks',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.ifconfig',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.autosummary',
-
-    'sphinxext.inline_code_highlight',
-    'numpydoc',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.extlinks",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autosummary",
+    "sphinxext.inline_code_highlight",
+    "numpydoc",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'Mizani'
-copyright = '2022, Hassan Kibirige'
+project = "Mizani"
+copyright = "2023, Hassan Kibirige"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 # The short X.Y version.
 try:
     from importlib.metadata import version as _version
 finally:
-    version = _version('mizani')
+    version = _version("mizani")
 
 # readthedocs modifies the repository which messes up the version.
 # 1. remove +dirty if readthedocs modifies the repo,
 # 2. remove the 0.0 version created by setuptools_scm when clone is too shallow
 if on_rtd:
     import re
-    p1 = re.compile(r'\+dirty$')
+
+    p1 = re.compile(r"\+dirty$")
     if p1.match(version):
-        version = p1.sub('', version)
+        version = p1.sub("", version)
 
-    p2 = re.compile(r'^0\.0\.post\d+\+g')
+    p2 = re.compile(r"^0\.0\.post\d+\+g")
     if p2.match(version):
-        commit = p2.sub('', version)
-        version = f'Commit: {commit}'
+        commit = p2.sub("", version)
+        version = f"Commit: {commit}"
 
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
@@ -118,17 +120,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = [
-    '_build'
-]
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
@@ -138,48 +138,48 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-highlight_language = 'python3'
+pygments_style = "sphinx"
+highlight_language = "python3"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
 # I want the sphinx-build -W to emit "warnings as errors" as part of my test
 # & build infrastructure, to ensure that there are no mistakes in the
 # documentation. New in 1.4.2
-suppress_warnings = ['image.nonlocal_uri']
+suppress_warnings = ["image.nonlocal_uri"]
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'theme'
+html_theme = "theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # https://github.com/ryan-roemer/sphinx-bootstrap-theme
 html_theme_options = {
-    'navbar_title': 'mizani',
-    'globaltoc_depth': 2,
-    'globaltoc_includehidden': 'true',
-    'source_link_position': 'footer',
-    'navbar_sidebarrel': False,
+    "navbar_title": "mizani",
+    "globaltoc_depth": 2,
+    "globaltoc_includehidden": "true",
+    "source_link_position": "footer",
+    "navbar_sidebarrel": False,
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
-html_theme_path = ['.']
+html_theme_path = ["."]
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
@@ -192,15 +192,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 # html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
@@ -241,40 +241,42 @@
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'mizanidoc'
+htmlhelp_basename = "mizanidoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
-    'papersize': 'a4paper',
-
+    "papersize": "a4paper",
     # The font size ('10pt', '11pt' or '12pt').
-    'pointsize': '12pt',
-
+    "pointsize": "12pt",
     # Additional stuff for the LaTeX preamble.
-    'preamble': r"""
+    "preamble": r"""
         \usepackage{charter}
         \usepackage[defaultsans]{lato}
         \usepackage{inconsolata}
     """,
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'mizani.tex',
-   'Mizani Documentation',
-   'Hassan Kibirige', 'manual'),
+    (
+        master_doc,
+        "mizani.tex",
+        "Mizani Documentation",
+        "Hassan Kibirige",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -295,35 +297,36 @@
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'mizani',
-     'Mizani Documentation',
-     ['Hassan Kibirige'], 1)
+    (master_doc, "mizani", "Mizani Documentation", ["Hassan Kibirige"], 1)
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'mizani',
-   'Mizani Documentation',
-   'Hassan Kibirige',
-   'mizani',
-   'One line description of project.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "mizani",
+        "Mizani Documentation",
+        "Hassan Kibirige",
+        "mizani",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
@@ -333,51 +336,49 @@
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3/', None),
-    'matplotlib': ('https://matplotlib.org/stable', None),
-    'numpy': ('https://numpy.org/doc/stable', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy', None),
+    "python": ("https://docs.python.org/3/", None),
+    "matplotlib": ("https://matplotlib.org/stable", None),
+    "numpy": ("https://numpy.org/doc/stable", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy", None),
 }
 
 
 # -- Extension configuration ----------------------------------------------
-autodoc_member_order = 'bysource'
+autodoc_member_order = "bysource"
 autosummary_generate = True
 
-extlinks = {
-    'issue': ('https://github.com/has2k1/mizani/issues/%s', 'GH')
-}
+extlinks = {"issue": ("https://github.com/has2k1/mizani/issues/%s", "#%s")}
 
 # numpydoc
 numpydoc_show_class_members = False
 numpydoc_class_members_toctree = False
 numpydoc_xref_param_type = True
 numpydoc_xref_aliases = {
     # python
-    'sequence': ':term:`python:sequence`',
-    'iterable': ':term:`python:iterable`',
-    'string': 'str',
-    'tuples': 'tuple',
-    'boolean': 'bool',
+    "sequence": ":term:`python:sequence`",
+    "iterable": ":term:`python:iterable`",
+    "string": "str",
+    "tuples": "tuple",
+    "boolean": "bool",
     # numpy
-    'array': 'numpy.ndarray',
-    'np.array': 'numpy.ndarray',
-    'ndarray': 'numpy.ndarray',
-    'array-like': ':term:`array-like<numpy:array_like>`',
-    'array_like': ':term:`numpy:array_like`',
+    "array": "numpy.ndarray",
+    "np.array": "numpy.ndarray",
+    "ndarray": "numpy.ndarray",
+    "array-like": ":term:`array-like<numpy:array_like>`",
+    "array_like": ":term:`numpy:array_like`",
     # pandas
-    'dataframe': 'pandas.DataFrame',
-    'DataFrame': 'pandas.DataFrame',
-    'Series': 'pandas.Series',
-    'series': 'pandas.Series',
+    "dataframe": "pandas.DataFrame",
+    "DataFrame": "pandas.DataFrame",
+    "Series": "pandas.Series",
+    "series": "pandas.Series",
 }
-numpydoc_xref_ignore = {'type', 'optional', 'default'}
+numpydoc_xref_ignore = {"type", "optional", "default"}
 
 
 def setup(app):
-    app.add_js_file('copybutton.js')
-    app.add_css_file('custom.css')
+    app.add_js_file("copybutton.js")
+    app.add_css_file("custom.css")
```

### Comparing `mizani-0.8.1/doc/installation.rst` & `mizani-0.9.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/layout.html` & `mizani-0.9.0/doc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/navbar-2.html` & `mizani-0.9.0/doc/theme/navbar-2.html`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/navbar.html` & `mizani-0.9.0/doc/theme/navbar.html`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/relations.html` & `mizani-0.9.0/doc/theme/relations.html`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/search.html` & `mizani-0.9.0/doc/theme/search.html`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/searchresults.html` & `mizani-0.9.0/doc/theme/searchresults.html`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css` & `mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 /*!
  * Bootstrap v3.4.1 (https://getbootstrap.com/)
  * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
- *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:none;text-decoration:underline;text-decoration:underline dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{font-size:2em;margin:.67em 0}mark{background:#ff0;color:#000}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{box-sizing:content-box;height:0}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{color:inherit;font:inherit;margin:0}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}input{line-height:normal}input[type=checkbox],input[type=radio]{box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-appearance:textfield;box-sizing:content-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}legend{border:0;padding:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:"Glyphicons Halflings";src:url("../fonts/glyphicons-halflings-regular.eot");src:url("../fonts/glyphicons-halflings-regular.eot?#iefix") format("embedded-opentype"),url("../fonts/glyphicons-halflings-regular.woff2") format("woff2"),url("../fonts/glyphicons-halflings-regular.woff") format("woff"),url("../fonts/glyphicons-halflings-regular.ttf") format("truetype"),url("../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular") format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:"Glyphicons Halflings";font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:transparent}body{font-family:-apple-system;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#145fce;text-decoration:none}a:focus,a:hover{color:#0d3f88;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out;display:inline-block;max-width:100%;height:auto}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:-apple-system;font-weight:700;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#aea79f}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#aea79f}.text-primary{color:#145fce}a.text-primary:focus,a.text-primary:hover{color:#0f4aa0}.text-success{color:#468847}a.text-success:focus,a.text-success:hover{color:#356635}.text-info{color:#3a87ad}a.text-info:focus,a.text-info:hover{color:#2d6987}.text-warning{color:#c09853}a.text-warning:focus,a.text-warning:hover{color:#a47e3c}.text-danger{color:#b94a48}a.text-danger:focus,a.text-danger:hover{color:#953b39}.bg-primary{color:#fff;background-color:#145fce}a.bg-primary:focus,a.bg-primary:hover{background-color:#0f4aa0}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none;margin-left:-5px}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;clear:left;text-align:right;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#aea79f}blockquote .small:before,blockquote footer:before,blockquote small:before{content:"\2014 \00A0"}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:""}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:"\00A0 \2014"}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.row-no-gutters{margin-right:0;margin-left:0}.row-no-gutters [class*=col-]{padding-right:0;padding-left:0}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}caption{padding-top:8px;padding-bottom:8px;color:#aea79f;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;-webkit-appearance:none;appearance:none}input[type=checkbox],input[type=radio]{margin:4px 0 0;line-height:normal}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:9px;font-size:14px;line-height:1.42857143;color:#333}.form-control{display:block;width:100%;height:38px;padding:8px 12px;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#aea79f;opacity:1}.form-control:-ms-input-placeholder{color:#aea79f}.form-control::-webkit-input-placeholder{color:#aea79f}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=datetime-local].form-control,input[type=month].form-control,input[type=time].form-control{line-height:38px}.input-group-sm input[type=date],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],.input-group-sm input[type=time],input[type=date].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm,input[type=time].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],.input-group-lg input[type=time],input[type=date].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg,input[type=time].input-lg{line-height:54px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}.form-control-static{min-height:34px;padding-top:9px;padding-bottom:9px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:54px;padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:54px;line-height:54px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:54px;padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:54px;line-height:54px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:54px;min-height:38px;padding:15px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:47.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:38px;height:38px;line-height:38px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:54px;height:54px;line-height:54px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#468847}.has-success .form-control{border-color:#468847;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#356635;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #7aba7b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #7aba7b}.has-success .input-group-addon{color:#468847;background-color:#dff0d8;border-color:#468847}.has-success .form-control-feedback{color:#468847}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#c09853}.has-warning .form-control{border-color:#c09853;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#a47e3c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #dbc59e;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #dbc59e}.has-warning .input-group-addon{color:#c09853;background-color:#fcf8e3;border-color:#c09853}.has-warning .form-control-feedback{color:#c09853}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#b94a48}.has-error .form-control{border-color:#b94a48;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#953b39;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #d59392;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #d59392}.has-error .input-group-addon{color:#b94a48;background-color:#f2dede;border-color:#b94a48}.has-error .form-control-feedback{color:#b94a48}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:9px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:29px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:9px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:15px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;margin-bottom:0;font-weight:400;text-align:center;white-space:nowrap;vertical-align:middle;touch-action:manipulation;cursor:pointer;background-image:none;border:1px solid transparent;padding:8px 12px;font-size:14px;line-height:1.42857143;border-radius:4px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#fff;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;opacity:.65;-webkit-box-shadow:none;box-shadow:none}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#fff;background-color:#aea79f;border-color:#aea79f}.btn-default.focus,.btn-default:focus{color:#fff;background-color:#978e83;border-color:#6f675e}.btn-default:hover{color:#fff;background-color:#978e83;border-color:#92897e}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#fff;background-color:#978e83;background-image:none;border-color:#92897e}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#fff;background-color:#867c71;border-color:#6f675e}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#aea79f;border-color:#aea79f}.btn-default .badge{color:#aea79f;background-color:#fff}.btn-primary{color:#fff;background-color:#145fce;border-color:#145fce}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#0f4aa0;border-color:#09295a}.btn-primary:hover{color:#fff;background-color:#0f4aa0;border-color:#0f4596}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#0f4aa0;background-image:none;border-color:#0f4596}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#0c3b7f;border-color:#09295a}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#145fce;border-color:#145fce}.btn-primary .badge{color:#145fce;background-color:#fff}.btn-success{color:#fff;background-color:#38b44a;border-color:#38b44a}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#2c8d3a;border-color:#1a5322}.btn-success:hover{color:#fff;background-color:#2c8d3a;border-color:#298537}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#2c8d3a;background-image:none;border-color:#298537}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#23722f;border-color:#1a5322}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#38b44a;border-color:#38b44a}.btn-success .badge{color:#38b44a;background-color:#fff}.btn-info{color:#fff;background-color:#772953;border-color:#772953}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#511c39;border-color:#180811}.btn-info:hover{color:#fff;background-color:#511c39;border-color:#491933}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#511c39;background-image:none;border-color:#491933}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#371326;border-color:#180811}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#772953;border-color:#772953}.btn-info .badge{color:#772953;background-color:#fff}.btn-warning{color:#fff;background-color:#efb73e;border-color:#efb73e}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#e7a413;border-color:#a0720d}.btn-warning:hover{color:#fff;background-color:#e7a413;border-color:#dd9d12}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#e7a413;background-image:none;border-color:#dd9d12}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#c68c10;border-color:#a0720d}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#efb73e;border-color:#efb73e}.btn-warning .badge{color:#efb73e;background-color:#fff}.btn-danger{color:#fff;background-color:#df382c;border-color:#df382c}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#bc271c;border-color:#791912}.btn-danger:hover{color:#fff;background-color:#bc271c;border-color:#b3251b}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#bc271c;background-image:none;border-color:#b3251b}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#9d2118;border-color:#791912}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#df382c;border-color:#df382c}.btn-danger .badge{color:#df382c;background-color:#fff}.btn-link{font-weight:400;color:#145fce;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#0d3f88;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#aea79f;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-property:height,visibility;transition-property:height,visibility;-webkit-transition-duration:.35s;transition-duration:.35s;-webkit-transition-timing-function:ease;transition-timing-function:ease}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#fff;text-decoration:none;background-color:#145fce}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#145fce;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#aea79f}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#aea79f;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:54px;padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:54px;line-height:54px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:8px 12px;font-size:14px;font-weight:400;line-height:1;color:#333;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:14px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#aea79f}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#aea79f;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#145fce}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#777;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#145fce}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;border-top:1px solid transparent;box-shadow:inset 0 1px 0 rgba(255,255,255,.1);-webkit-overflow-scrolling:touch}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-right:15px;margin-top:8px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-right:-15px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);margin-top:6px;margin-bottom:6px}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:6px;margin-bottom:6px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#145fce;border-color:#1151b0}.navbar-default .navbar-brand{color:#fff}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#fff;background-color:none}.navbar-default .navbar-text{color:#fff}.navbar-default .navbar-nav>li>a{color:#fff}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#fff;background-color:#0d3f88}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#fff;background-color:#0f4aa0}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#fff;background-color:#0f4aa0}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#fff}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:#0d3f88}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#0f4aa0}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-toggle{border-color:#0d3f88}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#0d3f88}.navbar-default .navbar-toggle .icon-bar{background-color:#fff}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#1151b0}.navbar-default .navbar-link{color:#fff}.navbar-default .navbar-link:hover{color:#fff}.navbar-default .btn-link{color:#fff}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#fff}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#772953;border-color:#511c39}.navbar-inverse .navbar-brand{color:#fff}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:none}.navbar-inverse .navbar-text{color:#fff}.navbar-inverse .navbar-nav>li>a{color:#fff}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:#3e152b}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#511c39}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#511c39}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#511c39}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#511c39}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#fff}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:#3e152b}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#511c39}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-inverse .navbar-toggle{border-color:#3e152b}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#3e152b}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#5c2040}.navbar-inverse .navbar-link{color:#fff}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#fff}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#ccc}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#aea79f}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:8px 12px;margin-left:-1px;line-height:1.42857143;color:#145fce;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#0d3f88;background-color:#eee;border-color:#ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#aea79f;cursor:default;background-color:#f5f5f5;border-color:#ddd}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#aea79f;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:14px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#aea79f;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#aea79f}.label-default[href]:focus,.label-default[href]:hover{background-color:#978e83}.label-primary{background-color:#145fce}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#0f4aa0}.label-success{background-color:#38b44a}.label-success[href]:focus,.label-success[href]:hover{background-color:#2c8d3a}.label-info{background-color:#772953}.label-info[href]:focus,.label-info[href]:hover{background-color:#511c39}.label-warning{background-color:#efb73e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#e7a413}.label-danger{background-color:#df382c}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#bc271c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#aea79f;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#145fce;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#145fce}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#468847;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#356635}.alert-info{color:#3a87ad;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#2d6987}.alert-warning{color:#c09853;background-color:#fcf8e3;border-color:#fbeed5}.alert-warning hr{border-top-color:#f8e5be}.alert-warning .alert-link{color:#a47e3c}.alert-danger{color:#b94a48;background-color:#f2dede;border-color:#eed3d7}.alert-danger hr{border-top-color:#e6c1c7}.alert-danger .alert-link{color:#953b39}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0%;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#145fce;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#38b44a}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#772953}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#efb73e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#df382c}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#aea79f;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#aea79f}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#145fce;border-color:#145fce}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#b6d1f8}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item-success{color:#468847;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#468847}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#468847;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#468847;border-color:#468847}.list-group-item-info{color:#3a87ad;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#3a87ad}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#3a87ad;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#3a87ad;border-color:#3a87ad}.list-group-item-warning{color:#c09853;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#c09853}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#c09853;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#c09853;border-color:#c09853}.list-group-item-danger{color:#b94a48;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#b94a48}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#b94a48;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#b94a48;border-color:#b94a48}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#145fce}.panel-primary>.panel-heading{color:#fff;background-color:#145fce;border-color:#145fce}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#145fce}.panel-primary>.panel-heading .badge{color:#145fce;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#145fce}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#468847;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#468847}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#3a87ad;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#3a87ad}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#fbeed5}.panel-warning>.panel-heading{color:#c09853;background-color:#fcf8e3;border-color:#fbeed5}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#fbeed5}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#c09853}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#fbeed5}.panel-danger{border-color:#eed3d7}.panel-danger>.panel-heading{color:#b94a48;background-color:#f2dede;border-color:#eed3d7}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#eed3d7}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#b94a48}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#eed3d7}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;opacity:.5}button.close{padding:0;cursor:pointer;background:0 0;border:0;-webkit-appearance:none;appearance:none}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%);-webkit-transition:-webkit-transform .3s ease-out;-moz-transition:-moz-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:transform .3s ease-out}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5);outline:0}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{opacity:0}.modal-backdrop.in{opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:20px}.modal-footer{padding:20px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:-apple-system;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:12px;opacity:0}.tooltip.in{opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:-apple-system;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:14px;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2)}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover>.arrow{border-width:11px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-moz-transition:-moz-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:transform .6s ease-in-out;-webkit-backface-visibility:hidden;-moz-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;-moz-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);left:0}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);left:0}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0);left:0}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;outline:0;opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:"\2039"}.carousel-control .icon-next:before{content:"\203a"}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}@font-face{font-family:Ubuntu;font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/ubuntu/v20/4iCs6KVjbNBYlgoKfw7z.ttf) format('truetype')}@font-face{font-family:Ubuntu;font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/ubuntu/v20/4iCv6KVjbNBYlgoCxCvjsGyI.ttf) format('truetype')}.navbar-default .badge{background-color:#fff;color:#145fce}.navbar-inverse .badge{background-color:#fff;color:#772953}@media (max-width:767px){.navbar .dropdown-menu a{color:#fff}}h1{font-size:2em}h2{font-size:1.5em}h3{font-size:1.17em}h4{font-size:1em}h5{font-size:.83em}h6{font-size:.67em}.content dl:not(.docutils){margin-bottom:24px}.content dl.function>dt,.content dl:not(.docutils).class>dt{display:inline-block;margin:6px 0;line-height:normal;background:#e5eefc;border-top:solid 3px #70a4f1;color:#5996ef;padding:6px;position:relative;font-family:Consolas,"Andale Mono WT","Andale Mono","Lucida Console","Lucida Sans Typewriter","DejaVu Sans Mono","Bitstream Vera Sans Mono","Liberation Mono","Nimbus Mono L",Monaco,"Courier New",Courier,monospace}.content dl dd{margin:0 0 12px 24px}.content td.field-body dd{margin:0 0 6px 24px}.content dl:not(.docutils).class dl.classmethod>dt,.content dl:not(.docutils).class dl.method>dt,.content dl:not(.docutils).class dl.staticmethod>dt{display:inline-block;margin:6px 0;line-height:normal;border:none;border-left:solid 3px #bfbfbf;background:#ebebeb;color:grey;padding:6px;font-family:Consolas,"Andale Mono WT","Andale Mono","Lucida Console","Lucida Sans Typewriter","DejaVu Sans Mono","Bitstream Vera Sans Mono","Liberation Mono","Nimbus Mono L",Monaco,"Courier New",Courier,monospace}.content td.field-body{padding:0 0 0 8px}.content td.field-body dl.docutils>dt{background:0 0;border-left:none;color:#333}.content td.field-body dl.docutils>dt span.classifier{font-weight:400}.content dl:not(.docutils) .property{padding-right:8px}.content dl:not(.docutils) code.descclassname,.content dl:not(.docutils) code.descname{background-color:transparent;border:none;padding:0}.content code,code{white-space:nowrap;max-width:100%;background-color:#ecf0f3;font-size:96.5%;border:none padding: 0 1px;font-family:Consolas,"Andale Mono WT","Andale Mono","Lucida Console","Lucida Sans Typewriter","DejaVu Sans Mono","Bitstream Vera Sans Mono","Liberation Mono","Nimbus Mono L",Monaco,"Courier New",Courier,monospace;color:#333;overflow-x:auto}.content code{color:#333;border-radius:3px}.content code.descname{font-size:120%}.content code.xref,a .content code{font-weight:700;color:#145fce;border:none;padding:0;background-color:transparent}.content .viewcode-back,.content .viewcode-link{display:inline-block;color:#0d3f88;font-size:80%;padding-left:24px}.content .sig-paren{padding-left:2px}.content blockquote{padding:10px 20px;margin:0 0 20px;font-size:inherit;border-left:3px solid #eee;border-right:3px solid #eee;background:#f9f9f9}code span.hll{background-color:#ffc}code span.n{color:#333}code span.p{color:#333}code span.c{color:#408090;font-style:italic}code span.err{border:1px solid red}code span.k{color:#007020;font-weight:700}code span.o{color:#666}code span.ch{color:#408090;font-style:italic}code span.cm{color:#408090;font-style:italic}code span.cp{color:#007020}code span.cpf{color:#408090;font-style:italic}code span.c1{color:#408090;font-style:italic}code span.cs{color:#408090;background-color:#fff0f0}code span.gd{color:#a00000}code span.ge{font-style:italic}code span.gr{color:red}code span.gh{color:navy;font-weight:700}code span.gi{color:#00a000}code span.go{color:#333}code span.gp{color:#c65d09;font-weight:700}code span.gs{font-weight:700}code span.gu{color:purple;font-weight:700}code span.gt{color:#04d}code span.kc{color:#007020;font-weight:700}code span.kd{color:#007020;font-weight:700}code span.kn{color:#007020;font-weight:700}code span.kp{color:#007020}code span.kr{color:#007020;font-weight:700}code span.kt{color:#902000}code span.m{color:#208050}code span.s{color:#4070a0}code span.na{color:#4070a0}code span.nb{color:#007020}code span.nc{color:#0e84b5;font-weight:700}code span.no{color:#60add5}code span.nd{color:#555;font-weight:700}code span.ni{color:#d55537;font-weight:700}code span.ne{color:#007020}code span.nf{color:#06287e}code span.nl{color:#002070;font-weight:700}code span.nn{color:#0e84b5;font-weight:700}code span.nt{color:#062873;font-weight:700}code span.nv{color:#bb60d5}code span.ow{color:#007020;font-weight:700}code span.w{color:#bbb}code span.mb{color:#208050}code span.mf{color:#208050}code span.mh{color:#208050}code span.mi{color:#208050}code span.mo{color:#208050}code span.sa{color:#4070a0}code span.sb{color:#4070a0}code span.sc{color:#4070a0}code span.dl{color:#4070a0}code span.sd{color:#4070a0;font-style:italic}code span.s2{color:#4070a0}code span.se{color:#4070a0;font-weight:700}code span.sh{color:#4070a0}code span.si{color:#70a0d0;font-style:italic}code span.sx{color:#c65d09}code span.sr{color:#235388}code span.s1{color:#4070a0}code span.ss{color:#517918}code span.bp{color:#007020}code span.fm{color:#06287e}code span.vc{color:#bb60d5}code span.vg{color:#bb60d5}code span.vi{color:#bb60d5}code span.vm{color:#bb60d5}code span.il{color:#208050}
+ *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:none;text-decoration:underline;text-decoration:underline dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{font-size:2em;margin:.67em 0}mark{background:#ff0;color:#000}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{box-sizing:content-box;height:0}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{color:inherit;font:inherit;margin:0}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}input{line-height:normal}input[type=checkbox],input[type=radio]{box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-appearance:textfield;box-sizing:content-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}legend{border:0;padding:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:"Glyphicons Halflings";src:url("../fonts/glyphicons-halflings-regular.eot");src:url("../fonts/glyphicons-halflings-regular.eot?#iefix") format("embedded-opentype"),url("../fonts/glyphicons-halflings-regular.woff2") format("woff2"),url("../fonts/glyphicons-halflings-regular.woff") format("woff"),url("../fonts/glyphicons-halflings-regular.ttf") format("truetype"),url("../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular") format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:"Glyphicons Halflings";font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:transparent}body{font-family:system-ui;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#145fce;text-decoration:none}a:focus,a:hover{color:#0d3f88;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out;display:inline-block;max-width:100%;height:auto}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:system-ui;font-weight:700;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#aea79f}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#aea79f}.text-primary{color:#145fce}a.text-primary:focus,a.text-primary:hover{color:#0f4aa0}.text-success{color:#468847}a.text-success:focus,a.text-success:hover{color:#356635}.text-info{color:#3a87ad}a.text-info:focus,a.text-info:hover{color:#2d6987}.text-warning{color:#c09853}a.text-warning:focus,a.text-warning:hover{color:#a47e3c}.text-danger{color:#b94a48}a.text-danger:focus,a.text-danger:hover{color:#953b39}.bg-primary{color:#fff;background-color:#145fce}a.bg-primary:focus,a.bg-primary:hover{background-color:#0f4aa0}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none;margin-left:-5px}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;clear:left;text-align:right;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#aea79f}blockquote .small:before,blockquote footer:before,blockquote small:before{content:"\2014 \00A0"}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:""}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:"\00A0 \2014"}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.row-no-gutters{margin-right:0;margin-left:0}.row-no-gutters [class*=col-]{padding-right:0;padding-left:0}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}caption{padding-top:8px;padding-bottom:8px;color:#aea79f;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;-webkit-appearance:none;appearance:none}input[type=checkbox],input[type=radio]{margin:4px 0 0;line-height:normal}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:9px;font-size:14px;line-height:1.42857143;color:#333}.form-control{display:block;width:100%;height:38px;padding:8px 12px;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#aea79f;opacity:1}.form-control:-ms-input-placeholder{color:#aea79f}.form-control::-webkit-input-placeholder{color:#aea79f}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=datetime-local].form-control,input[type=month].form-control,input[type=time].form-control{line-height:38px}.input-group-sm input[type=date],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],.input-group-sm input[type=time],input[type=date].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm,input[type=time].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],.input-group-lg input[type=time],input[type=date].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg,input[type=time].input-lg{line-height:54px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}.form-control-static{min-height:34px;padding-top:9px;padding-bottom:9px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:54px;padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:54px;line-height:54px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:54px;padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:54px;line-height:54px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:54px;min-height:38px;padding:15px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:47.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:38px;height:38px;line-height:38px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:54px;height:54px;line-height:54px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#468847}.has-success .form-control{border-color:#468847;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#356635;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #7aba7b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #7aba7b}.has-success .input-group-addon{color:#468847;background-color:#dff0d8;border-color:#468847}.has-success .form-control-feedback{color:#468847}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#c09853}.has-warning .form-control{border-color:#c09853;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#a47e3c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #dbc59e;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #dbc59e}.has-warning .input-group-addon{color:#c09853;background-color:#fcf8e3;border-color:#c09853}.has-warning .form-control-feedback{color:#c09853}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#b94a48}.has-error .form-control{border-color:#b94a48;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#953b39;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #d59392;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #d59392}.has-error .input-group-addon{color:#b94a48;background-color:#f2dede;border-color:#b94a48}.has-error .form-control-feedback{color:#b94a48}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:9px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:29px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:9px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:15px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;margin-bottom:0;font-weight:400;text-align:center;white-space:nowrap;vertical-align:middle;touch-action:manipulation;cursor:pointer;background-image:none;border:1px solid transparent;padding:8px 12px;font-size:14px;line-height:1.42857143;border-radius:4px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#fff;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;opacity:.65;-webkit-box-shadow:none;box-shadow:none}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#fff;background-color:#aea79f;border-color:#aea79f}.btn-default.focus,.btn-default:focus{color:#fff;background-color:#978e83;border-color:#6f675e}.btn-default:hover{color:#fff;background-color:#978e83;border-color:#92897e}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#fff;background-color:#978e83;background-image:none;border-color:#92897e}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#fff;background-color:#867c71;border-color:#6f675e}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#aea79f;border-color:#aea79f}.btn-default .badge{color:#aea79f;background-color:#fff}.btn-primary{color:#fff;background-color:#145fce;border-color:#145fce}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#0f4aa0;border-color:#09295a}.btn-primary:hover{color:#fff;background-color:#0f4aa0;border-color:#0f4596}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#0f4aa0;background-image:none;border-color:#0f4596}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#0c3b7f;border-color:#09295a}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#145fce;border-color:#145fce}.btn-primary .badge{color:#145fce;background-color:#fff}.btn-success{color:#fff;background-color:#38b44a;border-color:#38b44a}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#2c8d3a;border-color:#1a5322}.btn-success:hover{color:#fff;background-color:#2c8d3a;border-color:#298537}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#2c8d3a;background-image:none;border-color:#298537}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#23722f;border-color:#1a5322}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#38b44a;border-color:#38b44a}.btn-success .badge{color:#38b44a;background-color:#fff}.btn-info{color:#fff;background-color:#772953;border-color:#772953}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#511c39;border-color:#180811}.btn-info:hover{color:#fff;background-color:#511c39;border-color:#491933}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#511c39;background-image:none;border-color:#491933}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#371326;border-color:#180811}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#772953;border-color:#772953}.btn-info .badge{color:#772953;background-color:#fff}.btn-warning{color:#fff;background-color:#efb73e;border-color:#efb73e}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#e7a413;border-color:#a0720d}.btn-warning:hover{color:#fff;background-color:#e7a413;border-color:#dd9d12}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#e7a413;background-image:none;border-color:#dd9d12}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#c68c10;border-color:#a0720d}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#efb73e;border-color:#efb73e}.btn-warning .badge{color:#efb73e;background-color:#fff}.btn-danger{color:#fff;background-color:#df382c;border-color:#df382c}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#bc271c;border-color:#791912}.btn-danger:hover{color:#fff;background-color:#bc271c;border-color:#b3251b}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#bc271c;background-image:none;border-color:#b3251b}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#9d2118;border-color:#791912}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#df382c;border-color:#df382c}.btn-danger .badge{color:#df382c;background-color:#fff}.btn-link{font-weight:400;color:#145fce;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#0d3f88;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#aea79f;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-property:height,visibility;transition-property:height,visibility;-webkit-transition-duration:.35s;transition-duration:.35s;-webkit-transition-timing-function:ease;transition-timing-function:ease}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#fff;text-decoration:none;background-color:#145fce}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#145fce;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#aea79f}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#aea79f;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:54px;padding:14px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:54px;line-height:54px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:8px 12px;font-size:14px;font-weight:400;line-height:1;color:#333;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:14px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#aea79f}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#aea79f;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#145fce}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#777;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#145fce}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;border-top:1px solid transparent;box-shadow:inset 0 1px 0 rgba(255,255,255,.1);-webkit-overflow-scrolling:touch}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-right:15px;margin-top:8px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-right:-15px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);margin-top:6px;margin-bottom:6px}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:6px;margin-bottom:6px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#145fce;border-color:#1151b0}.navbar-default .navbar-brand{color:#fff}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#fff;background-color:none}.navbar-default .navbar-text{color:#fff}.navbar-default .navbar-nav>li>a{color:#fff}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#fff;background-color:#0d3f88}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#fff;background-color:#0f4aa0}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#fff;background-color:#0f4aa0}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#fff}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:#0d3f88}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#0f4aa0}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-toggle{border-color:#0d3f88}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#0d3f88}.navbar-default .navbar-toggle .icon-bar{background-color:#fff}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#1151b0}.navbar-default .navbar-link{color:#fff}.navbar-default .navbar-link:hover{color:#fff}.navbar-default .btn-link{color:#fff}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#fff}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#772953;border-color:#511c39}.navbar-inverse .navbar-brand{color:#fff}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:none}.navbar-inverse .navbar-text{color:#fff}.navbar-inverse .navbar-nav>li>a{color:#fff}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:#3e152b}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#511c39}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#511c39}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#511c39}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#511c39}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#fff}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:#3e152b}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#511c39}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-inverse .navbar-toggle{border-color:#3e152b}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#3e152b}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#5c2040}.navbar-inverse .navbar-link{color:#fff}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#fff}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#ccc}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#aea79f}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:8px 12px;margin-left:-1px;line-height:1.42857143;color:#145fce;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#0d3f88;background-color:#eee;border-color:#ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#aea79f;cursor:default;background-color:#f5f5f5;border-color:#ddd}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#aea79f;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:14px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#aea79f;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#aea79f}.label-default[href]:focus,.label-default[href]:hover{background-color:#978e83}.label-primary{background-color:#145fce}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#0f4aa0}.label-success{background-color:#38b44a}.label-success[href]:focus,.label-success[href]:hover{background-color:#2c8d3a}.label-info{background-color:#772953}.label-info[href]:focus,.label-info[href]:hover{background-color:#511c39}.label-warning{background-color:#efb73e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#e7a413}.label-danger{background-color:#df382c}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#bc271c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#aea79f;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#145fce;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#145fce}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#468847;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#356635}.alert-info{color:#3a87ad;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#2d6987}.alert-warning{color:#c09853;background-color:#fcf8e3;border-color:#fbeed5}.alert-warning hr{border-top-color:#f8e5be}.alert-warning .alert-link{color:#a47e3c}.alert-danger{color:#b94a48;background-color:#f2dede;border-color:#eed3d7}.alert-danger hr{border-top-color:#e6c1c7}.alert-danger .alert-link{color:#953b39}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0%;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#145fce;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#38b44a}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#772953}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#efb73e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#df382c}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#aea79f;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#aea79f}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#145fce;border-color:#145fce}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#b6d1f8}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item-success{color:#468847;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#468847}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#468847;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#468847;border-color:#468847}.list-group-item-info{color:#3a87ad;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#3a87ad}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#3a87ad;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#3a87ad;border-color:#3a87ad}.list-group-item-warning{color:#c09853;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#c09853}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#c09853;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#c09853;border-color:#c09853}.list-group-item-danger{color:#b94a48;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#b94a48}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#b94a48;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#b94a48;border-color:#b94a48}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#145fce}.panel-primary>.panel-heading{color:#fff;background-color:#145fce;border-color:#145fce}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#145fce}.panel-primary>.panel-heading .badge{color:#145fce;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#145fce}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#468847;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#468847}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#3a87ad;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#3a87ad}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#fbeed5}.panel-warning>.panel-heading{color:#c09853;background-color:#fcf8e3;border-color:#fbeed5}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#fbeed5}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#c09853}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#fbeed5}.panel-danger{border-color:#eed3d7}.panel-danger>.panel-heading{color:#b94a48;background-color:#f2dede;border-color:#eed3d7}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#eed3d7}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#b94a48}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#eed3d7}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;opacity:.5}button.close{padding:0;cursor:pointer;background:0 0;border:0;-webkit-appearance:none;appearance:none}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%);-webkit-transition:-webkit-transform .3s ease-out;-moz-transition:-moz-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:transform .3s ease-out}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5);outline:0}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{opacity:0}.modal-backdrop.in{opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:20px}.modal-footer{padding:20px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:system-ui;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:12px;opacity:0}.tooltip.in{opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:system-ui;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:14px;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2)}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover>.arrow{border-width:11px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-moz-transition:-moz-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:transform .6s ease-in-out;-webkit-backface-visibility:hidden;-moz-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;-moz-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);left:0}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);left:0}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0);left:0}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;outline:0;opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:"\2039"}.carousel-control .icon-next:before{content:"\203a"}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}@font-face{font-family:Ubuntu;font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/ubuntu/v20/4iCs6KVjbNBYlgoKfw7z.ttf) format('truetype')}@font-face{font-family:Ubuntu;font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/ubuntu/v20/4iCv6KVjbNBYlgoCxCvjsGyI.ttf) format('truetype')}.navbar-default .badge{background-color:#fff;color:#145fce}.navbar-inverse .badge{background-color:#fff;color:#772953}@media (max-width:767px){.navbar .dropdown-menu a{color:#fff}}h1{font-size:2em}h2{font-size:1.5em}h3{font-size:1.17em}h4{font-size:1em}h5{font-size:.83em}h6{font-size:.67em}.content dl:not(.docutils){margin-bottom:24px}.content dl.function>dt,.content dl:not(.docutils).class>dt{display:inline-block;margin:6px 0;line-height:normal;background:#e5eefc;border-top:solid 3px #70a4f1;color:#5996ef;padding:6px;position:relative;font-family:Consolas,Menlo,'DejaVu Sans Mono','Bitstream Vera Sans Mono',monospace}.content dl dd{margin:0 0 12px 24px}.content td.field-body dd{margin:0 0 6px 24px}.content dl:not(.docutils).class dl.classmethod>dt,.content dl:not(.docutils).class dl.method>dt,.content dl:not(.docutils).class dl.staticmethod>dt{display:inline-block;margin:6px 0;line-height:normal;border:none;border-left:solid 3px #bfbfbf;background:#ebebeb;color:grey;padding:6px;font-family:Consolas,Menlo,'DejaVu Sans Mono','Bitstream Vera Sans Mono',monospace}.content td.field-body{padding:0 0 0 8px}.content td.field-body dl.docutils>dt{background:0 0;border-left:none;color:#333}.content td.field-body dl.docutils>dt span.classifier{font-weight:400}.content dl:not(.docutils) .property{padding-right:8px}.content dl:not(.docutils) code.descclassname,.content dl:not(.docutils) code.descname{background-color:transparent;border:none;padding:0}.content code,code{white-space:nowrap;max-width:100%;background-color:#ecf0f3;font-size:96.5%;border:none padding: 0 1px;font-family:Consolas,Menlo,'DejaVu Sans Mono','Bitstream Vera Sans Mono',monospace;color:#333;overflow-x:auto}.content code{color:#333;border-radius:3px}.content code.descname{font-size:120%}.content code.xref,a .content code{font-weight:700;color:#145fce;border:none;padding:0;background-color:transparent}.content .viewcode-back,.content .viewcode-link{display:inline-block;color:#0d3f88;font-size:80%;padding-left:24px}.content .sig-paren{padding-left:2px}.content blockquote{padding:10px 20px;margin:0 0 20px;font-size:inherit;border-left:3px solid #eee;border-right:3px solid #eee;background:#f9f9f9}code span.hll{background-color:#ffc}code span.n{color:#333}code span.p{color:#333}code span.c{color:#408090;font-style:italic}code span.err{border:1px solid red}code span.k{color:#007020;font-weight:700}code span.o{color:#666}code span.ch{color:#408090;font-style:italic}code span.cm{color:#408090;font-style:italic}code span.cp{color:#007020}code span.cpf{color:#408090;font-style:italic}code span.c1{color:#408090;font-style:italic}code span.cs{color:#408090;background-color:#fff0f0}code span.gd{color:#a00000}code span.ge{font-style:italic}code span.gr{color:red}code span.gh{color:navy;font-weight:700}code span.gi{color:#00a000}code span.go{color:#333}code span.gp{color:#c65d09;font-weight:700}code span.gs{font-weight:700}code span.gu{color:purple;font-weight:700}code span.gt{color:#04d}code span.kc{color:#007020;font-weight:700}code span.kd{color:#007020;font-weight:700}code span.kn{color:#007020;font-weight:700}code span.kp{color:#007020}code span.kr{color:#007020;font-weight:700}code span.kt{color:#902000}code span.m{color:#208050}code span.s{color:#4070a0}code span.na{color:#4070a0}code span.nb{color:#007020}code span.nc{color:#0e84b5;font-weight:700}code span.no{color:#60add5}code span.nd{color:#555;font-weight:700}code span.ni{color:#d55537;font-weight:700}code span.ne{color:#007020}code span.nf{color:#06287e}code span.nl{color:#002070;font-weight:700}code span.nn{color:#0e84b5;font-weight:700}code span.nt{color:#062873;font-weight:700}code span.nv{color:#bb60d5}code span.ow{color:#007020;font-weight:700}code span.w{color:#bbb}code span.mb{color:#208050}code span.mf{color:#208050}code span.mh{color:#208050}code span.mi{color:#208050}code span.mo{color:#208050}code span.sa{color:#4070a0}code span.sb{color:#4070a0}code span.sc{color:#4070a0}code span.dl{color:#4070a0}code span.sd{color:#4070a0;font-style:italic}code span.s2{color:#4070a0}code span.se{color:#4070a0;font-weight:700}code span.sh{color:#4070a0}code span.si{color:#70a0d0;font-style:italic}code span.sx{color:#c65d09}code span.sr{color:#235388}code span.s1{color:#4070a0}code span.ss{color:#517918}code span.bp{color:#007020}code span.fm{color:#06287e}code span.vc{color:#bb60d5}code span.vg{color:#bb60d5}code span.vi{color:#bb60d5}code span.vm{color:#bb60d5}code span.il{color:#208050}
```

### Comparing `mizani-0.8.1/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js` & `mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/static/bootstrap-sphinx.css_t` & `mizani-0.9.0/doc/theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/static/bootstrap-sphinx.js_t` & `mizani-0.9.0/doc/theme/static/bootstrap-sphinx.js_t`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/static/js/jquery-1.12.4.min.js` & `mizani-0.9.0/doc/theme/static/js/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/doc/theme/theme.conf` & `mizani-0.9.0/doc/theme/theme.conf`

 * *Files 5% similar despite different names*

```diff
@@ -59,7 +59,10 @@
 # Options are nothing (default) or the name of a valid theme such as
 # "cosmo" or "sandstone".
 bootswatch_theme =
 
 # Switch Bootstrap version?
 # Values: "3" (default) or "2"
 bootstrap_version = 3
+
+# basic.css
+body_max_width = none
```

### Comparing `mizani-0.8.1/how-to-release.rst` & `mizani-0.9.0/how-to-release.rst`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/licences/HUSL_LICENSE` & `mizani-0.9.0/licences/HUSL_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/licences/SEABORN_LICENSE` & `mizani-0.9.0/licences/SEABORN_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/licences/SIX_LICENSE` & `mizani-0.9.0/licences/SIX_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/mizani/bounds.py` & `mizani-0.9.0/mizani/bounds.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,27 @@
 
 import datetime
 
 import numpy as np
 import pandas as pd
 import pandas.api.types as pdtypes
 
-from matplotlib.dates import date2num
-
 from .utils import first_element
 
-
-__all__ = ['censor', 'expand_range', 'rescale', 'rescale_max',
-           'rescale_mid', 'squish_infinite', 'zero_range',
-           'expand_range_distinct', 'squish']
+__all__ = [
+    "censor",
+    "expand_range",
+    "rescale",
+    "rescale_max",
+    "rescale_mid",
+    "squish_infinite",
+    "zero_range",
+    "expand_range_distinct",
+    "squish",
+]
 
 
 def rescale(x, to=(0, 1), _from=None):
     """
     Rescale numeric vector to have specified minimum and maximum.
 
     Parameters
@@ -102,23 +107,23 @@
 
     try:
         len(x)
     except TypeError:
         array_like = False
         x = [x]
 
-    if not hasattr(x, 'dtype'):
+    if not hasattr(x, "dtype"):
         x = np.asarray(x)
 
     if _from is None:
         _from = np.array([np.min(x), np.max(x)])
     else:
         _from = np.asarray(_from)
 
-    if (zero_range(_from) or zero_range(to)):
+    if zero_range(_from) or zero_range(to):
         out = np.repeat(np.mean(to), len(x))
     else:
         extent = 2 * np.max(np.abs(_from - mid))
         out = (x - mid) / extent * np.diff(to) + np.mean(to)
 
     if not array_like:
         out = out[0]
@@ -178,26 +183,26 @@
 
     try:
         len(x)
     except TypeError:
         array_like = False
         x = [x]
 
-    if not hasattr(x, 'dtype'):
+    if not hasattr(x, "dtype"):
         x = np.asarray(x)
 
     if _from is None:
         _from = (np.min(x), np.max(x))
 
     if np.any(x < 0):
         out = rescale(x, (0, to[1]), _from)
     elif np.all(x == 0) and _from[1] == 0:
         out = np.repeat(to[1], len(x))
     else:
-        out = x/_from[1] * to[1]
+        out = x / _from[1] * to[1]
 
     if not array_like:
         out = out[0]
     return out
 
 
 def squish_infinite(x, range=(0, 1)):
@@ -222,15 +227,15 @@
     >>> squish_infinite([0, .5, .25, np.inf, .44])
     [0.0, 0.5, 0.25, 1.0, 0.44]
     >>> squish_infinite([0, -np.inf, .5, .25, np.inf], (-10, 9))
     [0.0, -10.0, 0.5, 0.25, 9.0]
     """
     xtype = type(x)
 
-    if not hasattr(x, 'dtype'):
+    if not hasattr(x, "dtype"):
         x = np.asarray(x)
 
     x[x == -np.inf] = range[0]
     x[x == np.inf] = range[1]
 
     if not isinstance(x, xtype):
         x = xtype(x)
@@ -261,15 +266,15 @@
     [0.0, 0.2, 0.5, 0.8, 1.0, 1.0]
 
     >>> squish([-np.inf, -1.5, 0.2, 0.5, 0.8, 1.0, np.inf], only_finite=False)
     [0.0, 0.0, 0.2, 0.5, 0.8, 1.0, 1.0]
     """
     xtype = type(x)
 
-    if not hasattr(x, 'dtype'):
+    if not hasattr(x, "dtype"):
         x = np.asarray(x)
 
     finite = np.isfinite(x) if only_finite else True
 
     x[np.logical_and(x < range[0], finite)] = range[0]
     x[np.logical_and(x > range[1], finite)] = range[1]
 
@@ -320,69 +325,74 @@
     - :class:`datetime.timedelta` : :py:`np.timedelta64(NaT)`
 
     """
     if not len(x):
         return x
 
     py_time_types = (datetime.datetime, datetime.timedelta)
-    np_pd_time_types = (pd.Timestamp, pd.Timedelta,
-                        np.datetime64, np.timedelta64)
+    np_pd_time_types = (
+        pd.Timestamp,
+        pd.Timedelta,
+        np.datetime64,
+        np.timedelta64,
+    )
     x0 = first_element(x)
 
     # Yes, we want type not isinstance
     if type(x0) in py_time_types:
-        return _censor_with(x, range, 'NaT')
+        return _censor_with(x, range, "NaT")
 
-    if not hasattr(x, 'dtype') and isinstance(x0, np_pd_time_types):
-        return _censor_with(x, range, type(x0)('NaT'))
+    if not hasattr(x, "dtype") and isinstance(x0, np_pd_time_types):
+        return _censor_with(x, range, type(x0)("NaT"))
 
     x_array = np.asarray(x)
     if pdtypes.is_number(x0) and not isinstance(x0, np.timedelta64):
-        null = float('nan')
+        null = float("nan")
     elif isinstance(x0, pd.Timestamp):
-        null = pd.Timestamp('NaT')
+        null = pd.Timestamp("NaT")
     elif pdtypes.is_datetime64_dtype(x_array):
-        null = np.datetime64('NaT')
+        null = np.datetime64("NaT")
     elif isinstance(x0, pd.Timedelta):
-        null = pd.Timedelta('NaT')
+        null = pd.Timedelta("NaT")
     elif pdtypes.is_timedelta64_dtype(x_array):
-        null = np.timedelta64('NaT')
+        null = np.timedelta64("NaT")
     else:
         raise ValueError(
-            "Do not know how to censor values of type "
-            "{}".format(type(x0)))
+            "Do not know how to censor values of type " "{}".format(type(x0))
+        )
 
     if only_finite:
         try:
             finite = np.isfinite(x)
         except TypeError:
             finite = np.repeat(True, len(x))
     else:
         finite = np.repeat(True, len(x))
 
-    if hasattr(x, 'dtype'):
+    if hasattr(x, "dtype"):
         # Ignore RuntimeWarning when x contains nans
-        with np.errstate(invalid='ignore'):
+        with np.errstate(invalid="ignore"):
             outside = (x < range[0]) | (x > range[1])
         bool_idx = finite & outside
         x = x.copy()
         x[bool_idx] = null
     else:
-        x = [null if not range[0] <= val <= range[1] and f else val
-             for val, f in zip(x, finite)]
+        x = [
+            null if not range[0] <= val <= range[1] and f else val
+            for val, f in zip(x, finite)
+        ]
 
     return x
 
 
 def _censor_with(x, range, value=None):
     """
     Censor any values outside of range with ``None``
     """
-    return [val if range[0] <= val <= range[1] else value
-            for val in x]
+    return [val if range[0] <= val <= range[1] else value for val in x]
 
 
 def zero_range(x, tol=np.finfo(float).eps * 100):
     """
     Determine if range of vector is close to zero.
 
     Parameters
@@ -413,22 +423,24 @@
     try:
         if len(x) == 1:
             return True
     except TypeError:
         return True
 
     if len(x) != 2:
-        raise ValueError('x must be length 1 or 2')
+        raise ValueError("x must be length 1 or 2")
 
     # Also deals with array_likes that have non-standard indices
     x = sorted(x)
     low, high = x
 
     # datetime - pandas, cpython
     if isinstance(low, (pd.Timestamp, datetime.datetime)):
+        from matplotlib.dates import date2num
+
         # date2num include timezone info, .toordinal() does not
         low, high = date2num(x)
     # datetime - numpy
     elif isinstance(low, np.datetime64):
         return low == high
     # timedelta - pandas, cpython
     elif isinstance(low, (pd.Timedelta, datetime.timedelta)):
@@ -509,18 +521,18 @@
     try:
         x[0]
     except TypeError:
         x = (x, x)
 
     # The expansion cases
     if zero_range(x):
-        new = x[0]-zero_width/2, x[0]+zero_width/2
+        new = x[0] - zero_width / 2, x[0] + zero_width / 2
     else:
         dx = (x[1] - x[0]) * mul + add
-        new = x[0]-dx, x[1]+dx
+        new = x[0] - dx, x[1] + dx
 
     return new
 
 
 def expand_range_distinct(range, expand=(0, 0, 0, 0), zero_width=1):
     """
     Expand a range with a multiplicative or additive constants
```

### Comparing `mizani-0.8.1/mizani/breaks.py` & `mizani-0.9.0/mizani/breaks.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,44 +7,69 @@
 have ticks and values to help gauge the speed of the vehicle.
 
 The named markers are what we call breaks. Properly calculated
 breaks make interpretation straight forward. These functions
 provide ways to calculate good(hopefully) breaks.
 """
 import sys
+from itertools import product
 
 import numpy as np
 import pandas as pd
-from matplotlib.dates import MinuteLocator, HourLocator, DayLocator
-from matplotlib.dates import WeekdayLocator, MonthLocator, YearLocator
-from matplotlib.dates import AutoDateLocator, SecondLocator
-from matplotlib.dates import num2date, YEARLY
+from matplotlib.dates import (
+    YEARLY,
+    AutoDateLocator,
+    DayLocator,
+    HourLocator,
+    MinuteLocator,
+    MonthLocator,
+    SecondLocator,
+    WeekdayLocator,
+    YearLocator,
+    num2date,
+)
 from matplotlib.ticker import MaxNLocator
 
-from .utils import min_max, SECONDS, NANOSECONDS
+from .utils import NANOSECONDS, SECONDS, log, min_max
 
-
-__all__ = ['mpl_breaks', 'log_breaks', 'minor_breaks',
-           'trans_minor_breaks', 'date_breaks',
-           'timedelta_breaks', 'extended_breaks']
+__all__ = [
+    "mpl_breaks",
+    "log_breaks",
+    "minor_breaks",
+    "trans_minor_breaks",
+    "date_breaks",
+    "timedelta_breaks",
+    "extended_breaks",
+]
 
 
 # The break calculations rely on MPL locators to do
 # the heavylifting. It may be more convinient to lift
 # the calculations out of MPL.
 
-class DateLocator(AutoDateLocator):
 
+class DateLocator(AutoDateLocator):
     def __init__(self):
-        AutoDateLocator.__init__(self, minticks=5,
-                                 interval_multiples=True)
+        AutoDateLocator.__init__(self, minticks=5, interval_multiples=True)
         # Remove 4 and 400
         self.intervald[YEARLY] = [
-            1, 2, 5, 10, 20, 50, 100, 200, 500,
-            1000, 2000, 5000, 10000]
+            1,
+            2,
+            5,
+            10,
+            20,
+            50,
+            100,
+            200,
+            500,
+            1000,
+            2000,
+            5000,
+            10000,
+        ]
         self.create_dummy_axis()
 
     def tick_values(self, vmin, vmax):
         # get locator
         # if yearlocator
         # change the vmin to turn of decade or half-decade
         ticks = AutoDateLocator.tick_values(self, vmin, vmax)
@@ -63,14 +88,15 @@
     >>> x = range(10)
     >>> limits = (0, 9)
     >>> mpl_breaks()(limits)
     array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.])
     >>> mpl_breaks(nbins=2)(limits)
     array([  0.,   5.,  10.])
     """
+
     def __init__(self, *args, **kwargs):
         self.locator = MaxNLocator(*args, **kwargs)
 
     def __call__(self, limits):
         """
         Compute breaks
 
@@ -135,48 +161,34 @@
             Sequence of breaks points
         """
         if any(np.isinf(limits)):
             return []
 
         n = self.n
         base = self.base
-        if base == 10:
-            rng = np.log10(limits)
-        elif base == 2:
-            rng = np.log2(limits)
-        elif base == np.e:
-            rng = np.log(limits)
-        else:
-            rng = np.log(limits)/np.log(base)
+        rng = log(limits, base)
         _min = int(np.floor(rng[0]))
         _max = int(np.ceil(rng[1]))
 
         # Prevent overflow
         if float(base) ** _max > sys.maxsize:
             base = float(base)
 
-        # numpy arrays with -ve number(s) and of dtype=int
-        # cannot be powers i.e. base ** arr fails
-        dtype = float if _min < 0 or _max < 0 else int
-
         if _max == _min:
-            return base ** _min
+            return base**_min
 
         # Try getting breaks at the integer powers of the base
         # e.g [1, 100, 10000, 1000000]
         # If there are too few breaks, try other points using the
         # _log_sub_breaks
-        by = int(np.floor((_max-_min)/n)) + 1
+        by = int(np.floor((_max - _min) / n)) + 1
         for step in range(by, 0, -1):
-            breaks = base ** np.arange(_min, _max+1, step=step, dtype=dtype)
-            relevant_breaks = (
-                (limits[0] <= breaks) &
-                (breaks <= limits[1])
-            )
-            if np.sum(relevant_breaks) >= n-2:
+            breaks = np.array([base**i for i in range(_min, _max + 1, step)])
+            relevant_breaks = (limits[0] <= breaks) & (breaks <= limits[1])
+            if np.sum(relevant_breaks) >= n - 2:
                 return breaks
 
         return _log_sub_breaks(n=n, base=base)(limits)
 
 
 class _log_sub_breaks:
     """
@@ -201,64 +213,57 @@
     def __init__(self, n=5, base=10):
         self.n = n
         self.base = base
 
     def __call__(self, limits):
         base = self.base
         n = self.n
-        rng = np.log(limits)/np.log(base)
+        rng = log(limits, base)
         _min = int(np.floor(rng[0]))
         _max = int(np.ceil(rng[1]))
-        dtype = float if _min < 0 or _max < 0 else int
         steps = [1]
 
         # Prevent overflow
         if float(base) ** _max > sys.maxsize:
             base = float(base)
 
         def delta(x):
             """
             Calculates the smallest distance in the log scale between the
-            currectly selected breaks and a new candidate 'x'
+            currently selected breaks and a new candidate 'x'
             """
             arr = np.sort(np.hstack([x, steps, base]))
-            if base == 10:
-                log_arr = np.log10(arr)
-            else:
-                log_arr = np.log(arr) / np.log(base)
+            log_arr = log(arr, base)
             return np.min(np.diff(log_arr))
 
         if self.base == 2:
-            return base ** np.arange(_min, _max+1, dtype=dtype)
+            return [base**i for i in range(_min, _max + 1)]
 
-        candidate = np.arange(base+1)
+        candidate = np.arange(base + 1)
         candidate = np.compress(
-            (1 < candidate) & (candidate < base), candidate)
+            (1 < candidate) & (candidate < base), candidate
+        )
 
         while len(candidate):
             best = np.argmax([delta(x) for x in candidate])
             steps.append(candidate[best])
             candidate = np.delete(candidate, best)
+            _factors = [base**i for i in range(_min, _max + 1)]
+            breaks = np.array([f * s for f, s in product(_factors, steps)])
+            relevant_breaks = (limits[0] <= breaks) & (breaks <= limits[1])
 
-            breaks = np.outer(
-                base ** np.arange(_min, _max+1, dtype=dtype), steps).ravel()
-            relevant_breaks = (
-                (limits[0] <= breaks) & (breaks <= limits[1]))
-
-            if np.sum(relevant_breaks) >= n-2:
+            if np.sum(relevant_breaks) >= n - 2:
                 breaks = np.sort(breaks)
-                lower_end = np.max([
-                    np.min(np.where(limits[0] <= breaks))-1,
-                    0
-                ])
-                upper_end = np.min([
-                    np.max(np.where(breaks <= limits[1]))+1,
-                    len(breaks)
-                ])
-                return breaks[lower_end:upper_end+1]
+                lower_end = np.max(
+                    [np.min(np.where(limits[0] <= breaks)) - 1, 0]
+                )
+                upper_end = np.min(
+                    [np.max(np.where(breaks <= limits[1])) + 1, len(breaks)]
+                )
+                return breaks[lower_end : upper_end + 1]
         else:
             return extended_breaks(n=n)(limits)
 
 
 class minor_breaks:
     """
     Compute minor breaks
@@ -281,14 +286,15 @@
     More than 1 minor break.
 
     >>> minor_breaks(3)([1, 2], (1, 2))
     array([1.25, 1.5 , 1.75])
     >>> minor_breaks()([1, 2], (1, 2), 3)
     array([1.25, 1.5 , 1.75])
     """
+
     def __init__(self, n=1):
         self.n = n
 
     def __call__(self, major, limits=None, n=None):
         """
         Minor breaks
 
@@ -320,27 +326,24 @@
 
         # Try to infer additional major breaks so that
         # minor breaks can be generated beyond the first
         # and last major breaks
         diff = np.diff(major)
         step = diff[0]
         if len(diff) > 1 and all(diff == step):
-            major = np.hstack([major[0]-step,
-                               major,
-                               major[-1]+step])
+            major = np.hstack([major[0] - step, major, major[-1] + step])
 
         mbreaks = []
-        factors = np.arange(1, n+1)
+        factors = np.arange(1, n + 1)
         for lhs, rhs in zip(major[:-1], major[1:]):
-            sep = (rhs - lhs)/(n+1)
+            sep = (rhs - lhs) / (n + 1)
             mbreaks.append(lhs + factors * sep)
 
         minor = np.hstack(mbreaks)
-        minor = minor.compress((limits[0] <= minor) &
-                               (minor <= limits[1]))
+        minor = minor.compress((limits[0] <= minor) & (minor <= limits[1]))
         return minor
 
 
 class trans_minor_breaks:
     """
     Compute minor breaks for transformed scales
 
@@ -374,14 +377,15 @@
     More than 1 minor break
 
     >>> major = [1, 10]
     >>> limits = [1, 10]
     >>> sqrt_trans().minor_breaks(major, limits, 4)
     array([2.8, 4.6, 6.4, 8.2])
     """
+
     def __init__(self, trans, n=1):
         self.trans = trans
         self.n = n
 
     def __call__(self, major, limits=None, n=None):
         """
         Minor breaks for transformed scales
@@ -402,15 +406,16 @@
         -------
         out : array_like
             Minor breaks
         """
         if not self.trans.dataspace_is_numerical:
             raise TypeError(
                 "trans_minor_breaks can only be used for data "
-                "whose format is numerical.")
+                "whose format is numerical."
+            )
 
         if limits is None:
             limits = min_max(major)
 
         if n is None:
             n = self.n
 
@@ -430,32 +435,32 @@
         breaks (in transformed space) before the minor break call
         is made. How the breaks depends on the type of transform.
         """
         trans = self.trans
         trans = trans if isinstance(trans, type) else trans.__class__
         # so far we are only certain about this extending stuff
         # making sense for log transform
-        is_log = trans.__name__.startswith('log')
+        is_log = trans.__name__.startswith("log")
         diff = np.diff(major)
         step = diff[0]
         if is_log and all(diff == step):
-            major = np.hstack([major[0]-step, major, major[-1]+step])
+            major = np.hstack([major[0] - step, major, major[-1] + step])
         return major
 
 
 # Matplotlib's YearLocator uses different named
 # arguments than the others
 LOCATORS = {
-    'second': SecondLocator,
-    'minute': MinuteLocator,
-    'hour': HourLocator,
-    'day': DayLocator,
-    'week': WeekdayLocator,
-    'month': MonthLocator,
-    'year': lambda interval: YearLocator(base=interval)
+    "second": SecondLocator,
+    "minute": MinuteLocator,
+    "hour": HourLocator,
+    "day": DayLocator,
+    "week": WeekdayLocator,
+    "month": MonthLocator,
+    "year": lambda interval: YearLocator(base=interval),
 }
 
 
 class date_breaks:
     """
     Regularly spaced dates
 
@@ -481,22 +486,23 @@
 
     Breaks at 4 year intervals
 
     >>> breaks = date_breaks('4 year')
     >>> [d.year for d in breaks(limits)]
     [2008, 2012, 2016, 2020, 2024, 2028]
     """
+
     def __init__(self, width=None):
         if not width:
             locator = DateLocator()
         else:
             # Parse the width specification
             # e.g. '10 weeks' => (10, week)
             _n, units = width.strip().lower().split()
-            interval, units = int(_n), units.rstrip('s')
+            interval, units = int(_n), units.rstrip("s")
             locator = LOCATORS[units](interval=interval)
         self.locator = locator
 
     def __call__(self, limits):
         """
         Compute breaks
 
@@ -537,14 +543,15 @@
     >>> breaks = timedelta_breaks()
     >>> x = [timedelta(days=i*365) for i in range(25)]
     >>> limits = min(x), max(x)
     >>> major = breaks(limits)
     >>> [val.total_seconds()/(365*24*60*60)for val in major]
     [0.0, 5.0, 10.0, 15.0, 20.0, 25.0]
     """
+
     def __init__(self, n=5, Q=(1, 2, 5, 10)):
         self._breaks_func = extended_breaks(n=n, Q=Q)
 
     def __call__(self, limits):
         """
         Compute breaks
 
@@ -590,31 +597,32 @@
        formatted and get back a tuple of numeric values and
        the units for those values.
     2. Format the values with a general purpose formatting
        routing.
 
     See, :func:`timedelta_format`
     """
+
     def __init__(self, x, units=None):
         self.x = x
         self.type = type(x[0])
         self.package = self.determine_package(x[0])
         _limits = min(x), max(x)
         self.limits = self.value(_limits[0]), self.value(_limits[1])
         self.units = units or self.best_units(_limits)
         self.factor = self.get_scaling_factor(self.units)
 
     @classmethod
     def determine_package(cls, td):
-        if hasattr(td, 'components'):
-            package = 'pandas'
-        elif hasattr(td, 'total_seconds'):
-            package = 'cpython'
+        if hasattr(td, "components"):
+            package = "pandas"
+        elif hasattr(td, "total_seconds"):
+            package = "cpython"
         else:
-            msg = '{} format not yet supported.'
+            msg = "{} format not yet supported."
             raise ValueError(msg.format(td.__class__))
         return package
 
     @classmethod
     def format_info(cls, x, units=None):
         helper = cls(x, units)
         return helper.timedelta_to_numeric(x), helper.units
@@ -626,95 +634,97 @@
         # Read
         #   [(0.9, 's'),
         #    (9, 'm)]
         # as, break ranges between 0.9 seconds (inclusive)
         # and 9 minutes are represented in seconds. And so on.
         ts_range = self.value(max(sequence)) - self.value(min(sequence))
         package = self.determine_package(sequence[0])
-        if package == 'pandas':
+        if package == "pandas":
             cuts = [
-                (0.9, 'us'),
-                (0.9, 'ms'),
-                (0.9, 's'),
-                (9, 'm'),
-                (6, 'h'),
-                (4, 'd'),
-                (4, 'w'),
-                (4, 'M'),
-                (3, 'y')]
+                (0.9, "us"),
+                (0.9, "ms"),
+                (0.9, "s"),
+                (9, "m"),
+                (6, "h"),
+                (4, "d"),
+                (4, "w"),
+                (4, "M"),
+                (3, "y"),
+            ]
             denomination = NANOSECONDS
-            base_units = 'ns'
+            base_units = "ns"
         else:
             cuts = [
-                (0.9, 's'),
-                (9, 'm'),
-                (6, 'h'),
-                (4, 'd'),
-                (4, 'w'),
-                (4, 'M'),
-                (3, 'y')]
+                (0.9, "s"),
+                (9, "m"),
+                (6, "h"),
+                (4, "d"),
+                (4, "w"),
+                (4, "M"),
+                (3, "y"),
+            ]
             denomination = SECONDS
-            base_units = 'ms'
+            base_units = "ms"
 
         for size, units in reversed(cuts):
-            if ts_range >= size*denomination[units]:
+            if ts_range >= size * denomination[units]:
                 return units
 
         return base_units
 
     def value(self, td):
         """
         Return the numeric value representation on a timedelta
         """
-        if self.package == 'pandas':
+        if self.package == "pandas":
             return td.value
         else:
             return td.total_seconds()
 
     def scaled_limits(self):
         """
         Minimum and Maximum to use for computing breaks
         """
-        _min = self.limits[0]/self.factor
-        _max = self.limits[1]/self.factor
+        _min = self.limits[0] / self.factor
+        _max = self.limits[1] / self.factor
         return _min, _max
 
     def timedelta_to_numeric(self, timedeltas):
         """
         Convert sequence of timedelta to numerics
         """
         return [self.to_numeric(td) for td in timedeltas]
 
     def numeric_to_timedelta(self, numerics):
         """
         Convert sequence of numerics to timedelta
         """
-        if self.package == 'pandas':
-            return [self.type(int(x*self.factor), units='ns')
-                    for x in numerics]
+        if self.package == "pandas":
+            return [
+                self.type(int(x * self.factor), units="ns") for x in numerics
+            ]
         else:
-            return [self.type(seconds=x*self.factor)
-                    for x in numerics]
+            return [self.type(seconds=x * self.factor) for x in numerics]
 
     def get_scaling_factor(self, units):
-        if self.package == 'pandas':
+        if self.package == "pandas":
             return NANOSECONDS[units]
         else:
             return SECONDS[units]
 
     def to_numeric(self, td):
         """
         Convert timedelta to a number corresponding to the
         appropriate units. The appropriate units are those
         determined with the object is initialised.
         """
-        if self.package == 'pandas':
-            return td.value/NANOSECONDS[self.units]
+        if self.package == "pandas":
+            return td.value / NANOSECONDS[self.units]
         else:
-            return td.total_seconds()/SECONDS[self.units]
+            return td.total_seconds() / SECONDS[self.units]
 
 
 class extended_breaks:
     """
     An extension of Wilkinson's tick position algorithm
 
     Parameters
@@ -744,65 +754,74 @@
     - Talbot, J., Lin, S., Hanrahan, P. (2010) An Extension of
       Wilkinson's Algorithm for Positioning Tick Labels on Axes,
       InfoVis 2010.
 
     Additional Credit to Justin Talbot on whose code this
     implementation is almost entirely based.
     """
-    def __init__(self, n=5, Q=[1, 5, 2, 2.5, 4, 3],
-                 only_inside=False, w=[0.25, 0.2, 0.5, 0.05]):
+
+    def __init__(
+        self,
+        n=5,
+        Q=[1, 5, 2, 2.5, 4, 3],
+        only_inside=False,
+        w=[0.25, 0.2, 0.5, 0.05],
+    ):
         self.Q = Q
         self.only_inside = only_inside
         self.w = w
         self.n = n
         # Used for lookups during the computations
         self.Q_index = {q: i for i, q in enumerate(Q)}
 
     def coverage(self, dmin, dmax, lmin, lmax):
-        p1 = (dmax-lmax)**2
-        p2 = (dmin-lmin)**2
-        p3 = (0.1*(dmax-dmin))**2
-        return 1 - 0.5*(p1+p2)/p3
+        p1 = (dmax - lmax) ** 2
+        p2 = (dmin - lmin) ** 2
+        p3 = (0.1 * (dmax - dmin)) ** 2
+        return 1 - 0.5 * (p1 + p2) / p3
 
     def coverage_max(self, dmin, dmax, span):
-        range = dmax-dmin
+        range = dmax - dmin
         if span > range:
-            half = (span-range)/2.0
-            return 1 - (half**2) / (0.1*range)**2
+            half = (span - range) / 2.0
+            return 1 - (half**2) / (0.1 * range) ** 2
         else:
             return 1
 
     def density(self, k, dmin, dmax, lmin, lmax):
-        r = (k-1.0) / (lmax-lmin)
-        rt = (self.n-1) / (max(lmax, dmax) - min(lmin, dmin))
-        return 2 - max(r/rt, rt/r)
+        r = (k - 1.0) / (lmax - lmin)
+        rt = (self.n - 1) / (max(lmax, dmax) - min(lmin, dmin))
+        return 2 - max(r / rt, rt / r)
 
     def density_max(self, k):
         if k >= self.n:
-            return 2 - (k-1.0)/(self.n-1.0)
+            return 2 - (k - 1.0) / (self.n - 1.0)
         else:
             return 1
 
     def simplicity(self, q, j, lmin, lmax, lstep):
         eps = 1e-10
         n = len(self.Q)
-        i = self.Q_index[q]+1
+        i = self.Q_index[q] + 1
 
-        if ((lmin % lstep < eps or (lstep - lmin % lstep) < eps) and
-                lmin <= 0 and lmax >= 0):
+        if (
+            (lmin % lstep < eps or (lstep - lmin % lstep) < eps)
+            and lmin <= 0
+            and lmax >= 0
+        ):
             v = 1
         else:
             v = 0
-        return (n-i)/(n-1.0) + v - j
+        return (n - i) / (n - 1.0) + v - j
 
     def simplicity_max(self, q, j):
         n = len(self.Q)
-        i = self.Q_index[q]+1
+        i = self.Q_index[q] + 1
         v = 1
-        return (n-i)/(n-1.0) + v - j
+        return (n - i) / (n - 1.0) + v - j
 
     def legibility(self, lmin, lmax, lstep):
         # Legibility depends on fontsize, rotation, overlap ... i.e.
         # it requires drawing or simulating drawn breaks then calculating
         # a score. Return 1 ignores all that.
         return 1
 
@@ -839,65 +858,69 @@
             dmin, dmax = dmax, dmin
         elif dmin == dmax:
             return np.array([dmin])
 
         best_score = -2
         j = 1
 
-        while j < float('inf'):
+        while j < float("inf"):
             for q in Q:
                 sm = simplicity_max(q, j)
 
-                if w[0]*sm + w[1] + w[2] + w[3] < best_score:
-                    j = float('inf')
+                if w[0] * sm + w[1] + w[2] + w[3] < best_score:
+                    j = float("inf")
                     break
 
                 k = 2
-                while k < float('inf'):
+                while k < float("inf"):
                     dm = density_max(k)
 
-                    if w[0]*sm + w[1] + w[2]*dm + w[3] < best_score:
+                    if w[0] * sm + w[1] + w[2] * dm + w[3] < best_score:
                         break
 
-                    delta = (dmax-dmin)/(k+1)/j/q
+                    delta = (dmax - dmin) / (k + 1) / j / q
                     z = ceil(log10(delta))
 
-                    while z < float('inf'):
-                        step = j*q*(10**z)
-                        cm = coverage_max(dmin, dmax, step*(k-1))
-
-                        if w[0]*sm + w[1]*cm + w[2]*dm + w[3] < best_score:
+                    while z < float("inf"):
+                        step = j * q * (10**z)
+                        cm = coverage_max(dmin, dmax, step * (k - 1))
+
+                        if (
+                            w[0] * sm + w[1] * cm + w[2] * dm + w[3]
+                            < best_score
+                        ):
                             break
 
-                        min_start = int(floor(dmax/step)*j - (k-1)*j)
-                        max_start = int(ceil(dmin/step)*j)
+                        min_start = int(floor(dmax / step) * j - (k - 1) * j)
+                        max_start = int(ceil(dmin / step) * j)
 
                         if min_start > max_start:
-                            z = z+1
+                            z = z + 1
                             break
 
-                        for start in range(min_start, max_start+1):
-                            lmin = start * (step/j)
-                            lmax = lmin + step*(k-1)
+                        for start in range(min_start, max_start + 1):
+                            lmin = start * (step / j)
+                            lmax = lmin + step * (k - 1)
                             lstep = step
 
                             s = simplicity(q, j, lmin, lmax, lstep)
                             c = coverage(dmin, dmax, lmin, lmax)
                             d = density(k, dmin, dmax, lmin, lmax)
                             l = legibility(lmin, lmax, lstep)
 
-                            score = w[0]*s + w[1]*c + w[2]*d + w[3]*l
+                            score = w[0] * s + w[1] * c + w[2] * d + w[3] * l
 
-                            if (score > best_score and
-                                    (not only_inside or
-                                     (lmin >= dmin and lmax <= dmax))):
+                            if score > best_score and (
+                                not only_inside
+                                or (lmin >= dmin and lmax <= dmax)
+                            ):
                                 best_score = score
                                 best = (lmin, lmax, lstep, q, k)
-                        z = z+1
-                    k = k+1
-            j = j+1
+                        z = z + 1
+                    k = k + 1
+            j = j + 1
 
         try:
-            locs = best[0] + np.arange(best[4])*best[2]
+            locs = best[0] + np.arange(best[4]) * best[2]
         except UnboundLocalError:
             locs = []
         return locs
```

### Comparing `mizani-0.8.1/mizani/external/crayon_rgb.py` & `mizani-0.9.0/mizani/external/crayon_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/mizani/external/husl.py` & `mizani-0.9.0/mizani/external/husl.py`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/mizani/external/xkcd_rgb.py` & `mizani-0.9.0/mizani/external/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/mizani/formatters.py` & `mizani-0.9.0/mizani/formatters.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,38 +15,33 @@
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     # python < 3.9
     from backports.zoneinfo import ZoneInfo
 
-
 import numpy as np
-from matplotlib.dates import DateFormatter, date2num
-from matplotlib.ticker import ScalarFormatter
 
 from .breaks import timedelta_helper
-from .utils import round_any, precision, match
-from .utils import same_log10_order_of_magnitude
-
+from .utils import match, precision, round_any, same_log10_order_of_magnitude
 
 __all__ = [
-    'comma_format',
-    'custom_format',
-    'currency_format',
-    'dollar_format',
-    'percent_format',
-    'scientific_format',
-    'date_format',
-    'mpl_format',
-    'log_format',
-    'timedelta_format',
-    'pvalue_format',
-    'ordinal_format',
-    'number_bytes_format'
+    "comma_format",
+    "custom_format",
+    "currency_format",
+    "dollar_format",
+    "percent_format",
+    "scientific_format",
+    "date_format",
+    "mpl_format",
+    "log_format",
+    "timedelta_format",
+    "pvalue_format",
+    "ordinal_format",
+    "number_bytes_format",
 ]
 
 
 class custom_format:
     """
     Custom format
 
@@ -63,15 +58,16 @@
 
     Examples
     --------
     >>> formatter = custom_format('{:.2f} USD')
     >>> formatter([3.987, 2, 42.42])
     ['3.99 USD', '2.00 USD', '42.42 USD']
     """
-    def __init__(self, fmt='{}', style='new'):
+
+    def __init__(self, fmt="{}", style="new"):
         self.fmt = fmt
         self.style = style
 
     def __call__(self, x):
         """
         Format a sequence of inputs
 
@@ -81,21 +77,20 @@
             Input
 
         Returns
         -------
         out : list
             List of strings.
         """
-        if self.style == 'new':
+        if self.style == "new":
             return [self.fmt.format(val) for val in x]
-        elif self.style == 'old':
+        elif self.style == "old":
             return [self.fmt % val for val in x]
         else:
-            raise ValueError(
-                "style should be either 'new' or 'old'")
+            raise ValueError("style should be either 'new' or 'old'")
 
 
 # formatting functions
 class currency_format:
     """
     Currency formatter
 
@@ -115,15 +110,16 @@
     --------
     >>> x = [1.232, 99.2334, 4.6, 9, 4500]
     >>> currency_format()(x)
     ['$1.23', '$99.23', '$4.60', '$9.00', '$4500.00']
     >>> currency_format('C$', digits=0, big_mark=',')(x)
     ['C$1', 'C$99', 'C$5', 'C$9', 'C$4,500']
     """
-    def __init__(self, prefix='$', suffix='', digits=2, big_mark=''):
+
+    def __init__(self, prefix="$", suffix="", digits=2, big_mark=""):
         self.prefix = prefix
         self.suffix = suffix
         self.digits = digits
         self.big_mark = big_mark
 
     def __call__(self, x):
         """
@@ -137,21 +133,30 @@
         Returns
         -------
         out : list
             List of strings.
         """
         # create {:.2f} or {:,.2f}
         big_mark = self.big_mark
-        comma = ',' if big_mark else ''
-        tpl = ''.join((self.prefix, '{:', comma, '.',
-                       str(self.digits), 'f}', self.suffix))
+        comma = "," if big_mark else ""
+        tpl = "".join(
+            (
+                self.prefix,
+                "{:",
+                comma,
+                ".",
+                str(self.digits),
+                "f}",
+                self.suffix,
+            )
+        )
 
         labels = [tpl.format(val) for val in x]
-        if big_mark and big_mark != ',':
-            labels = [val.replace(',', big_mark) for val in labels]
+        if big_mark and big_mark != ",":
+            labels = [val.replace(",", big_mark) for val in labels]
         return labels
 
 
 dollar_format = currency_format
 dollar = dollar_format()
 
 
@@ -165,17 +170,19 @@
         Number of digits after the decimal point.
 
     Examples
     --------
     >>> comma_format()([1000, 2, 33000, 400])
     ['1,000', '2', '33,000', '400']
     """
+
     def __init__(self, digits=0):
         self.formatter = currency_format(
-            prefix='', digits=digits, big_mark=',')
+            prefix="", digits=digits, big_mark=","
+        )
 
     def __call__(self, x):
         """
         Format a sequence of inputs
 
         Parameters
         ----------
@@ -206,16 +213,17 @@
     --------
     >>> formatter = percent_format()
     >>> formatter([.45, 9.515, .01])
     ['45%', '952%', '1%']
     >>> formatter([.654, .8963, .1])
     ['65.4%', '89.6%', '10.0%']
     """
+
     def __init__(self, use_comma=False):
-        self.big_mark = ',' if use_comma else ''
+        self.big_mark = "," if use_comma else ""
 
     def __call__(self, x):
         """
         Format a sequence of inputs
 
         Parameters
         ----------
@@ -235,23 +243,22 @@
 
         # When the precision is less than 1, we show
         if _precision > 1:
             digits = 0
         else:
             digits = abs(int(np.log10(_precision)))
 
-        formatter = currency_format(prefix='',
-                                    suffix='%',
-                                    digits=digits,
-                                    big_mark=self.big_mark)
+        formatter = currency_format(
+            prefix="", suffix="%", digits=digits, big_mark=self.big_mark
+        )
         labels = formatter(x)
         # Remove unnecessary zeros after the decimal
-        pattern = re.compile(r'\.0+%$')
+        pattern = re.compile(r"\.0+%$")
         if all(pattern.search(val) for val in labels):
-            labels = [pattern.sub('%', val) for val in labels]
+            labels = [pattern.sub("%", val) for val in labels]
         return labels
 
 
 percent = percent_format()
 
 
 class scientific_format:
@@ -272,36 +279,37 @@
     Notes
     -----
     Be careful when using many digits (15+ on a 64
     bit computer). Consider of the `machine epsilon`_.
 
     .. _machine epsilon: https://en.wikipedia.org/wiki/Machine_epsilon
     """
+
     def __init__(self, digits=3):
-        tpl = ''.join(['{:.', str(digits), 'e}'])
+        tpl = "".join(["{:.", str(digits), "e}"])
         self.formatter = custom_format(tpl)
 
     def __call__(self, x):
         if len(x) == 0:
             return []
 
-        zeros_re = re.compile(r'(0+)e')
+        zeros_re = re.compile(r"(0+)e")
 
         def count_zeros(s):
             match = zeros_re.search(s)
             if match:
                 return len(match.group(1))
             else:
                 return 0
 
         # format and then remove superfluous zeros
         labels = self.formatter(x)
         n = min([count_zeros(val) for val in labels])
         if n:
-            labels = [val.replace('0'*n+'e', 'e') for val in labels]
+            labels = [val.replace("0" * n + "e", "e") for val in labels]
         return labels
 
 
 scientific = scientific_format()
 
 
 def _format(formatter, x):
@@ -315,37 +323,39 @@
     try:
         oom = int(formatter.orderOfMagnitude)
     except AttributeError:
         oom = 0
     labels = [formatter(tick) for tick in x]
 
     # Remove unnecessary decimals
-    pattern = re.compile(r'\.0+$')
+    pattern = re.compile(r"\.0+$")
     for i, label in enumerate(labels):
         match = pattern.search(label)
         if match:
-            labels[i] = pattern.sub('', label)
+            labels[i] = pattern.sub("", label)
 
     # MPL does not add the exponential component
     if oom:
-        labels = ['{}e{}'.format(s, oom) if s != '0' else s
-                  for s in labels]
+        labels = ["{}e{}".format(s, oom) if s != "0" else s for s in labels]
     return labels
 
 
 class mpl_format:
     """
     Format using MPL formatter for scalars
 
     Examples
     --------
     >>> mpl_format()([.654, .8963, .1])
     ['0.6540', '0.8963', '0.1000']
     """
+
     def __init__(self):
+        from matplotlib.ticker import ScalarFormatter
+
         self.formatter = ScalarFormatter(useOffset=False)
 
     def __call__(self, x):
         """
         Format a sequence of inputs
 
         Parameters
@@ -411,50 +421,50 @@
             Labels
         """
 
         def remove_zeroes(s):
             """
             Remove unnecessary zeros for float string s
             """
-            tup = s.split('e')
+            tup = s.split("e")
             if len(tup) == 2:
-                mantissa = tup[0].rstrip('0').rstrip('.')
+                mantissa = tup[0].rstrip("0").rstrip(".")
                 exponent = int(tup[1])
                 if exponent:
-                    s = '%se%d' % (mantissa, exponent)
+                    s = "%se%d" % (mantissa, exponent)
                 else:
                     s = mantissa
             return s
 
         def as_exp(s):
             """
             Float string s as in exponential format
             """
-            return s if 'e' in s else '{:1.0e}'.format(float(s))
+            return s if "e" in s else "{:1.0e}".format(float(s))
 
         def as_mathtex(s):
             """
             Mathtex for maplotlib
             """
-            if 'e' not in s:
-                assert s == '1', f"Unexpected value {s = }, instead of '1'"
+            if "e" not in s:
+                assert s == "1", f"Unexpected value {s = }, instead of '1'"
                 return f"${self.base}^{{0}}$"
 
-            exp = s.split('e')[1]
+            exp = s.split("e")[1]
             return f"${self.base}^{{{exp}}}$"
 
         # If any are in exponential format, make all of
         # them expontential
-        has_e = ['e' in x for x in labels]
+        has_e = ["e" in x for x in labels]
         if not all(has_e) and sum(has_e):
             labels = [as_exp(x) for x in labels]
 
         labels = [remove_zeroes(x) for x in labels]
 
-        has_e = ['e' in x for x in labels]
+        has_e = ["e" in x for x in labels]
         if self.mathtex and any(has_e):
             labels = [as_mathtex(x) for x in labels]
 
         return labels
 
     def __call__(self, x):
         """
@@ -474,47 +484,47 @@
             return []
 
         # Decide on using exponents
         if self.base == 10:
             xmin = int(np.floor(np.log10(np.min(x))))
             xmax = int(np.ceil(np.log10(np.max(x))))
             emin, emax = self.exponent_limits
-            all_multiples = np.all(
-                [np.log10(num).is_integer() for num in x])
+            all_multiples = np.all([np.log10(num).is_integer() for num in x])
             # Order of magnitude of the minimum and maximum
             if same_log10_order_of_magnitude(x):
                 f = mpl_format()
                 f.formatter.set_powerlimits((emin, emax))
                 return f(x)
             elif all_multiples and (xmin <= emin or xmax >= emax):
-                fmt = '{:1.0e}'
+                fmt = "{:1.0e}"
             else:
-                fmt = '{:g}'
+                fmt = "{:g}"
             labels = [fmt.format(num) for num in x]
             return self._tidyup_labels(labels)
         else:
+
             def _exp(num, base):
-                e = np.log(num)/np.log(base)
+                e = np.log(num) / np.log(base)
                 e_round = np.round(e)
                 if np.isclose(e, e_round):
                     e = int(e_round)
                 else:
                     e = np.round(e, 3)
                 return e
 
-            base_txt = f'{self.base}'
+            base_txt = f"{self.base}"
             if self.base == np.e:
-                base_txt = 'e'
+                base_txt = "e"
 
             if self.mathtex:
-                fmt_parts = (f'${base_txt}^', '{{{e}}}$')
+                fmt_parts = (f"${base_txt}^", "{{{e}}}$")
             else:
-                fmt_parts = (f'{base_txt}^', '{e}')
+                fmt_parts = (f"{base_txt}^", "{e}")
 
-            fmt = ''.join(fmt_parts)
+            fmt = "".join(fmt_parts)
             exps = [_exp(num, self.base) for num in x]
             labels = [fmt.format(e=e) for e in exps]
             return labels
 
 
 class date_format:
     """
@@ -560,17 +570,20 @@
     Format with a specific time zone
 
     >>> date_format('%Y-%m-%d %H:%M', tz=UTC)(x_tz)
     ['2010-01-01 05:00', '2010-01-01 12:00']
     >>> date_format('%Y-%m-%d %H:%M', tz='EST')(x_tz)
     ['2010-01-01 00:00', '2010-01-01 07:00']
     """
-    def __init__(self, fmt='%Y-%m-%d', tz=None):
+
+    def __init__(self, fmt="%Y-%m-%d", tz=None):
         if isinstance(tz, str):
             tz = ZoneInfo(tz)
+        from matplotlib.dates import DateFormatter
+
         self.formatter = DateFormatter(fmt, tz=tz)
         self.tz = tz
 
     def __call__(self, x):
         """
         Format a sequence of inputs
 
@@ -580,23 +593,27 @@
             Input
 
         Returns
         -------
         out : list
             List of strings.
         """
+        from matplotlib.dates import date2num
+
         # Formatter timezone
         if self.tz is None and len(x):
             tz = self.formatter.tz = x[0].tzinfo
 
             if not all(value.tzinfo == tz for value in x):
-                msg = ("Dates have different time zones. "
-                       "Choosen `{}` the time zone of the first date. "
-                       "To use a different time zone, create a "
-                       "formatter and pass the time zone.")
+                msg = (
+                    "Dates have different time zones. "
+                    "Choosen `{}` the time zone of the first date. "
+                    "To use a different time zone, create a "
+                    "formatter and pass the time zone."
+                )
                 warn(msg.format(tz.key))
 
         # The formatter is tied to axes and takes
         # breaks in ordinal format.
         x = [date2num(val) for val in x]
         return _format(self.formatter, x)
 
@@ -637,52 +654,54 @@
     >>> timedelta_format()(x)
     ['0', '1 month', '2 months', '3 months', '4 months']
     >>> timedelta_format(units='d')(x)
     ['0', '31 days', '62 days', '93 days', '124 days']
     >>> timedelta_format(units='d', add_units=False)(x)
     ['0', '31', '62', '93', '124']
     """
+
     abbreviations = {
-        'ns': 'ns',
-        'us': 'us',
-        'ms': 'ms',
-        's': 's',
-        'm': ' minute',
-        'h': ' hour',
-        'd': ' day',
-        'w': ' week',
-        'M': ' month',
-        'y': ' year'}
+        "ns": "ns",
+        "us": "us",
+        "ms": "ms",
+        "s": "s",
+        "m": " minute",
+        "h": " hour",
+        "d": " day",
+        "w": " week",
+        "M": " month",
+        "y": " year",
+    }
 
     def __init__(self, units=None, add_units=True, usetex=False):
         self.units = units
         self.add_units = add_units
         self.usetex = usetex
         self._mpl_format = mpl_format()
 
     def __call__(self, x):
         if len(x) == 0:
             return []
 
         labels = []
         values, _units = timedelta_helper.format_info(x, self.units)
-        plural = '' if _units.endswith('s') else 's'
+        plural = "" if _units.endswith("s") else "s"
         ulabel = self.abbreviations[_units]
-        if ulabel == 'us' and self.usetex:
-            ulabel = r'$\mu s$'
+        if ulabel == "us" and self.usetex:
+            ulabel = r"$\mu s$"
         _labels = self._mpl_format(values)
 
         if not self.add_units:
             return _labels
 
         for num, num_label in zip(values, _labels):
-            s = '' if num == 1 else plural
+            s = "" if num == 1 else plural
             # 0 has no units
-            _ulabel = '' if num == 0 else ulabel+s
-            labels.append(''.join([num_label, _ulabel]))
+            _ulabel = "" if num == 0 else ulabel + s
+            labels.append("".join([num_label, _ulabel]))
 
         return labels
 
 
 class pvalue_format:
     """
     p-values Formatter
@@ -723,42 +742,41 @@
         out : list
             List of strings.
         """
         x = round_any(x, self.accuracy)
         below = [num < self.accuracy for num in x]
 
         if self.add_p:
-            eq_fmt = 'p={:g}'.format
-            below_label = 'p<{:g}'.format(self.accuracy)
+            eq_fmt = "p={:g}".format
+            below_label = "p<{:g}".format(self.accuracy)
         else:
-            eq_fmt = '{:g}'.format
-            below_label = '<{:g}'.format(self.accuracy)
+            eq_fmt = "{:g}".format
+            below_label = "<{:g}".format(self.accuracy)
 
-        labels = [below_label if b else eq_fmt(i)
-                  for i, b in zip(x, below)]
+        labels = [below_label if b else eq_fmt(i) for i, b in zip(x, below)]
         return labels
 
 
-def ordinal(n, prefix='', suffix='', big_mark=''):
+def ordinal(n, prefix="", suffix="", big_mark=""):
     # General Case: 0th, 1st, 2nd, 3rd, 4th, 5th, 6th, 7th, 8th, 9th
     # Special Case: 10th, 11th, 12th, 13th
     n = int(n)
     idx = np.min((n % 10, 4))
-    _suffix = ['th', 'st', 'nd', 'rd', 'th'][idx]
+    _suffix = ["th", "st", "nd", "rd", "th"][idx]
     if 11 <= (n % 100) <= 13:
-        _suffix = 'th'
+        _suffix = "th"
 
     if big_mark:
-        s = '{:,}'.format(n)
-        if big_mark != ',':
-            s = s.replace(',', big_mark)
+        s = "{:,}".format(n)
+        if big_mark != ",":
+            s = s.replace(",", big_mark)
     else:
-        s = '{}'.format(n)
+        s = "{}".format(n)
 
-    return '{}{}{}{}'.format(prefix, s, _suffix, suffix)
+    return "{}{}{}{}".format(prefix, s, _suffix, suffix)
 
 
 class ordinal_format:
     """
     Ordinal Formatter
 
     Parameters
@@ -774,22 +792,24 @@
     Examples
     --------
     >>> ordinal_format()(range(8))
     ['0th', '1st', '2nd', '3rd', '4th', '5th', '6th', '7th']
     >>> ordinal_format(suffix=' Number')(range(11, 15))
     ['11th Number', '12th Number', '13th Number', '14th Number']
     """
-    def __init__(self, prefix='', suffix='', big_mark=''):
+
+    def __init__(self, prefix="", suffix="", big_mark=""):
         self.prefix = prefix
         self.suffix = suffix
         self.big_mark = big_mark
 
     def __call__(self, x):
-        labels = [ordinal(num, self.prefix, self.suffix, self.big_mark)
-                  for num in x]
+        labels = [
+            ordinal(num, self.prefix, self.suffix, self.big_mark) for num in x
+        ]
         return labels
 
 
 class number_bytes_format:
     """
     Bytes Formatter
 
@@ -809,49 +829,67 @@
     --------
     >>> x = [1000, 1000000, 4e5]
     >>> number_bytes_format()(x)
     ['1000 B', '977 KiB', '391 KiB']
     >>> number_bytes_format(units='si')(x)
     ['1 kB', '1 MB', '400 kB']
     """
-    def __init__(self, symbol='auto', units='binary', fmt='{:.0f} '):
+
+    def __init__(self, symbol="auto", units="binary", fmt="{:.0f} "):
         self.symbol = symbol
         self.units = units
         self.fmt = fmt
 
-        if units == 'si':
+        if units == "si":
             self.base = 1000
             self._all_symbols = [
-                'B', 'kB', 'MB', 'GB', 'TB',
-                'PB', 'EB', 'ZB', 'YB']
+                "B",
+                "kB",
+                "MB",
+                "GB",
+                "TB",
+                "PB",
+                "EB",
+                "ZB",
+                "YB",
+            ]
         else:
             self.base = 1024
             self._all_symbols = [
-                'B', 'KiB', 'MiB', 'GiB', 'TiB',
-                'PiB', 'EiB', 'ZiB', 'YiB']
+                "B",
+                "KiB",
+                "MiB",
+                "GiB",
+                "TiB",
+                "PiB",
+                "EiB",
+                "ZiB",
+                "YiB",
+            ]
 
         # possible exponents of base: eg 1000^1, 1000^2, 1000^3, ...
-        exponents = np.arange(1, len(self._all_symbols)+1, dtype=float)
-        self._powers = self.base ** exponents
-        self._validate_symbol(symbol, ['auto'] + self._all_symbols)
+        exponents = np.arange(1, len(self._all_symbols) + 1, dtype=float)
+        self._powers = self.base**exponents
+        self._validate_symbol(symbol, ["auto"] + self._all_symbols)
 
     def __call__(self, x):
         _all_symbols = self._all_symbols
         symbol = self.symbol
-        if symbol == 'auto':
+        if symbol == "auto":
             power = [bisect_right(self._powers, val) for val in x]
             symbols = [_all_symbols[p] for p in power]
         else:
             power = np.array(match([symbol], _all_symbols))
             symbols = [symbol] * len(x)
 
         x = np.asarray(x)
         power = np.asarray(power, dtype=float)
         values = x / self.base**power
-        fmt = (self.fmt + '{}').format
+        fmt = (self.fmt + "{}").format
         labels = [fmt(v, s) for v, s in zip(values, symbols)]
         return labels
 
     def _validate_symbol(self, symbol, allowed_symbols):
         if symbol not in allowed_symbols:
             raise ValueError(
-                "Symbol must be one of {}".format(allowed_symbols))
+                "Symbol must be one of {}".format(allowed_symbols)
+            )
```

### Comparing `mizani-0.8.1/mizani/palettes.py` & `mizani-0.9.0/mizani/palettes.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,37 +9,54 @@
 that they can intelligibly represent. For example, the size of
 a point should be significantly smaller than the plot panel
 onto which it is plotted or else it would be hard to compare
 two or more points. Therefore palettes must be created that
 enforce such restrictions. This is the reason for the ``*_pal``
 functions that create and return the actual palette functions.
 """
+from __future__ import annotations
+
 import colorsys
+import typing
 from warnings import warn
 
 import numpy as np
 import pandas as pd
-import matplotlib as mpl
-import matplotlib.colors as mcolors
-from palettable import colorbrewer
 
-from .external import husl, xkcd_rgb, crayon_rgb
 from .bounds import rescale
+from .external import crayon_rgb, husl, xkcd_rgb
 from .utils import identity
 
+if typing.TYPE_CHECKING:
+    from typing import Literal
+
+    from mizani.colors.typing import ColorScheme, ColorSchemeShort
+
 
-__all__ = ['hls_palette', 'husl_palette', 'rescale_pal',
-           'area_pal', 'abs_area', 'grey_pal', 'hue_pal',
-           'brewer_pal', 'gradient_n_pal', 'cmap_pal',
-           'cmap_d_pal',
-           'desaturate_pal', 'manual_pal', 'xkcd_palette',
-           'crayon_palette', 'cubehelix_pal']
+__all__ = [
+    "hls_palette",
+    "husl_palette",
+    "rescale_pal",
+    "area_pal",
+    "abs_area",
+    "grey_pal",
+    "hue_pal",
+    "brewer_pal",
+    "gradient_n_pal",
+    "cmap_pal",
+    "cmap_d_pal",
+    "desaturate_pal",
+    "manual_pal",
+    "xkcd_palette",
+    "crayon_palette",
+    "cubehelix_pal",
+]
 
 
-def hls_palette(n_colors=6, h=.01, l=.6, s=.65):
+def hls_palette(n_colors=6, h=0.01, l=0.6, s=0.65):
     """
     Get a set of evenly spaced colors in HLS hue space.
 
     h, l, and s should be between 0 and 1
 
     Parameters
     ----------
@@ -74,15 +91,15 @@
     hues += h
     hues %= 1
     hues -= hues.astype(int)
     palette = [colorsys.hls_to_rgb(h_i, l, s) for h_i in hues]
     return palette
 
 
-def husl_palette(n_colors=6, h=.01, s=.9, l=.65):
+def husl_palette(n_colors=6, h=0.01, s=0.9, l=0.65):
     """
     Get a set of evenly spaced colors in HUSL hue space.
 
     h, s, and l should be between 0 and 1
 
     Parameters
     ----------
@@ -150,16 +167,18 @@
     The returned palette expects inputs in the ``[0, 1]``
     range. Any value outside those limits is clipped to
     ``range[0]`` or ``range[1]``.
 
     >>> palette([-2, -1, 0.2, .4, .8, 2, 3])
     array([0.1 , 0.1 , 0.28, 0.46, 0.82, 1.  , 1.  ])
     """
+
     def _rescale(x):
         return rescale(x, range, _from=(0, 1))
+
     return _rescale
 
 
 def area_pal(range=(1, 6)):
     """
     Point area palette (continuous).
 
@@ -182,16 +201,18 @@
     >>> palette = area_pal()
     >>> palette(x)
     array([1. , 1.5, 2. , 2.5, 3. , 3.5])
 
     The results are equidistant because the input ``x`` is in
     area space, i.e it is squared.
     """
+
     def area_palette(x):
         return rescale(np.sqrt(x), to=range, _from=(0, 1))
+
     return area_palette
 
 
 def abs_area(max):
     """
     Point area palette (continuous), with area proportional to value.
 
@@ -215,16 +236,18 @@
     array([0. , 0.5, 1. , 1.5, 2. , 2.5, 3. , 3.5])
 
     Compared to :func:`area_pal`, :func:`abs_area` will handle values
     in the range ``[-1, 0]`` without returning ``np.nan``. And values
     whose absolute value is greater than 1 will be clipped to the
     maximum.
     """
+
     def abs_area_palette(x):
         return rescale(np.sqrt(np.abs(x)), to=(0, max), _from=(0, 1))
+
     return abs_area_palette
 
 
 def grey_pal(start=0.2, end=0.8):
     """
     Utility for creating continuous grey scale palette
 
@@ -244,31 +267,33 @@
 
     Examples
     --------
     >>> palette = grey_pal()
     >>> palette(5)
     ['#333333', '#737373', '#989898', '#b5b5b5', '#cccccc']
     """
+    import matplotlib.colors as mcolors
+
     gamma = 2.2
     ends = ((0.0, start, start), (1.0, end, end))
-    cdict = {'red': ends, 'green': ends, 'blue': ends}
-    grey_cmap = mcolors.LinearSegmentedColormap('grey', cdict)
+    cdict = {"red": ends, "green": ends, "blue": ends}
+    grey_cmap = mcolors.LinearSegmentedColormap("grey", cdict)
 
     def continuous_grey_palette(n):
         # The grey scale points are linearly separated in
         # gamma encoded space
         x = np.linspace(start**gamma, end**gamma, n)
         # Map points onto the [0, 1] palette domain
-        vals = (x ** (1./gamma) - start) / (end - start)
+        vals = (x ** (1.0 / gamma) - start) / (end - start)
         return ratios_to_colors(vals, grey_cmap)
 
     return continuous_grey_palette
 
 
-def hue_pal(h=.01, l=.6, s=.65, color_space='hls'):
+def hue_pal(h=0.01, l=0.6, s=0.65, color_space="hls"):
     """
     Utility for making hue palettes for color schemes.
 
     Parameters
     ----------
     h : float
         first hue. In the [0, 1] range
@@ -292,34 +317,42 @@
     Examples
     --------
     >>> hue_pal()(5)
     ['#db5f57', '#b9db57', '#57db94', '#5784db', '#c957db']
     >>> hue_pal(color_space='husl')(5)
     ['#e0697e', '#9b9054', '#569d79', '#5b98ab', '#b675d7']
     """
+    import matplotlib.colors as mcolors
+
     if not all([0 <= val <= 1 for val in (h, l, s)]):
-        msg = ("hue_pal expects values to be between 0 and 1. "
-               " I got h={}, l={}, s={}".format(h, l, s))
+        msg = (
+            "hue_pal expects values to be between 0 and 1. "
+            " I got h={}, l={}, s={}".format(h, l, s)
+        )
         raise ValueError(msg)
 
-    if color_space not in ('hls', 'husl'):
+    if color_space not in ("hls", "husl"):
         msg = "color_space should be one of ['hls', 'husl']"
         raise ValueError(msg)
 
-    name = '{}_palette'.format(color_space)
+    name = "{}_palette".format(color_space)
     palette = globals()[name]
 
     def _hue_pal(n):
         colors = palette(n, h=h, l=l, s=s)
         return [mcolors.rgb2hex(c) for c in colors]
 
     return _hue_pal
 
 
-def brewer_pal(type='seq', palette=1, direction=1):
+def brewer_pal(
+    type: ColorScheme | ColorSchemeShort = "seq",
+    palette: int = 1,
+    direction: Literal[1, -1] = 1,
+):
     """
     Utility for making a brewer palette
 
     Parameters
     ----------
     type : 'sequential' | 'qualitative' | 'diverging'
         Type of palette. Sequential, Qualitative or
@@ -353,53 +386,43 @@
     ['#1B9E77', '#D95F02', '#7570B3', '#E7298A', '#66A61E']
     >>> brewer_pal('seq', 'PuBuGn')(5)
     ['#F6EFF7', '#BDC9E1', '#67A9CF', '#1C9099', '#016C59']
 
     The available color names for each palette type can be
     obtained using the following code::
 
-        import palettable.colorbrewer as brewer
+        from mizani.colors.brewer import get_palette_names
 
-        print([k for k in brewer.COLOR_MAPS['Sequential'].keys()])
-        print([k for k in brewer.COLOR_MAPS['Qualitative'].keys()])
-        print([k for k in brewer.COLOR_MAPS['Diverging'].keys()])
+        print(get_palette_names("sequential"))
+        print(get_palette_names("qualitative"))
+        print(get_palette_names("diverging"))
     """
+    from .colors import brewer
+
     if direction != 1 and direction != -1:
         raise ValueError("direction should be 1 or -1.")
 
-    type = brewer_helper.full_type_name(type)
-    if isinstance(palette, int):
-        palette_name = brewer_helper.number_to_name(type, palette)
-    else:
-        palette_name = palette
-
-    # Get the number of colors in the palette
-    n_max = brewer_helper.num_colors(type, palette_name)
+    pal = brewer.get_color_palette(type, palette)
 
     def _brewer_pal(n):
         # Only draw the maximum allowable colors from the palette
         # and fill any remaining spots with None
-        _n = n if n <= n_max else n_max
-        try:
-            bmap = colorbrewer.get_map(palette_name, type, _n)
-        except ValueError:
-            # Some palettes have a minimum no. of colors
-            # We get around that restriction.
-            n_min = brewer_helper.min_num_colors(type, palette_name)
-            bmap = colorbrewer.get_map(palette_name, type, n_min)
-
-        hex_colors = bmap.hex_colors[:n]
-        if n > n_max:
-            msg = ("Warning message:"
-                   f"Brewer palette {palette_name} has a maximum "
-                   f"of {n_max} colors Returning the palette you "
-                   "asked for with that many colors")
+        _n = min(max(n, pal.min_colors), pal.max_colors)
+        color_map = pal.get_hex_swatch(_n)
+        colors = color_map[:n]
+        if n > pal.max_colors:
+            msg = (
+                "Warning message:"
+                f"Brewer palette {pal.name} has a maximum "
+                f"of {pal.max_colors} colors Returning the palette you "
+                "asked for with that many colors"
+            )
             warn(msg)
-            hex_colors = hex_colors + [None] * (n - n_max)
-        return hex_colors[::direction]
+            colors = colors + [None] * (n - pal.max_colors)
+        return colors[::direction]
 
     return _brewer_pal
 
 
 def ratios_to_colors(values, colormap):
     """
     Map values in the range [0, 1] onto colors
@@ -412,14 +435,16 @@
         Matplotlib colormap to use for the mapping
 
     Returns
     -------
     out : list | float
         Color(s) corresponding to the values
     """
+    import matplotlib.colors as mcolors
+
     iterable = True
     try:
         iter(values)
     except TypeError:
         iterable = False
         values = [values]
 
@@ -431,15 +456,15 @@
         hex_colors = [
             np.nan if is_nan else color
             for color, is_nan in zip(hex_colors, nan_bool_idx)
         ]
     return hex_colors if iterable else hex_colors[0]
 
 
-def gradient_n_pal(colors, values=None, name='gradientn'):
+def gradient_n_pal(colors, values=None, name="gradientn"):
     """
     Create a n color gradient palette
 
     Parameters
     ----------
     colors : list
         list of colors
@@ -463,23 +488,25 @@
     --------
     >>> palette = gradient_n_pal(['red', 'blue'])
     >>> palette([0, .25, .5, .75, 1])
     ['#ff0000', '#bf0040', '#7f0080', '#3f00c0', '#0000ff']
     >>> palette([-np.inf, 0, np.nan, 1, np.inf])
     [nan, '#ff0000', nan, '#0000ff', nan]
     """
+    import matplotlib.colors as mcolors
+
     # Note: For better results across devices and media types,
     # it would be better to do the interpolation in
     # Lab color space.
     if values is None:
-        colormap = mcolors.LinearSegmentedColormap.from_list(
-            name, colors)
+        colormap = mcolors.LinearSegmentedColormap.from_list(name, colors)
     else:
         colormap = mcolors.LinearSegmentedColormap.from_list(
-            name, list(zip(values, colors)))
+            name, list(zip(values, colors))
+        )
 
     def _gradient_n_pal(vals):
         return ratios_to_colors(vals, colormap)
 
     return _gradient_n_pal
 
 
@@ -506,25 +533,26 @@
 
     Examples
     --------
     >>> palette = cmap_pal('viridis')
     >>> palette([.1, .2, .3, .4, .5])
     ['#482475', '#414487', '#355f8d', '#2a788e', '#21918c']
     """
+    import matplotlib as mpl
+
     colormap = mpl.colormaps[name]
 
     if lut is not None:
         warn(
             "The lut parameter has been deprecated and will "
             "be removed in a future version.",
-            FutureWarning
+            FutureWarning,
         )
         resample = getattr(
-            colormap, 'resampled',
-            getattr(colormap, '_resample', None)
+            colormap, "resampled", getattr(colormap, "_resample", None)
         )
         colormap = resample(lut)
 
     def _cmap_pal(vals):
         return ratios_to_colors(vals, colormap)
 
     return _cmap_pal
@@ -552,47 +580,51 @@
 
     Examples
     --------
     >>> palette = cmap_d_pal('viridis')
     >>> palette(5)
     ['#440154', '#3b528b', '#21918c', '#5cc863', '#fde725']
     """
+    import matplotlib as mpl
+    import matplotlib.colors as mcolors
+
     colormap = mpl.colormaps[name]
 
     if lut is not None:
         warn(
             "The lut parameter has been deprecated and will "
             "be removed in a future version.",
-            FutureWarning
+            FutureWarning,
         )
         resample = getattr(
-            colormap, 'resampled',
-            getattr(colormap, '_resample', None)
+            colormap, "resampled", getattr(colormap, "_resample", None)
         )
         colormap = resample(lut)
 
     if not isinstance(colormap, mcolors.ListedColormap):
         raise ValueError(
             "For a discrete palette, cmap must be of type "
-            "matplotlib.colors.ListedColormap")
+            "matplotlib.colors.ListedColormap"
+        )
 
     ncolors = len(colormap.colors)
 
     def _cmap_d_pal(n):
         if n > ncolors:
             raise ValueError(
                 "cmap `{}` has {} colors you requested {} "
-                "colors.".format(name, ncolors, n))
+                "colors.".format(name, ncolors, n)
+            )
 
         if ncolors < 256:
             return [mcolors.rgb2hex(c) for c in colormap.colors[:n]]
         else:
             # Assume these are continuous and get colors equally spaced
             # intervals  e.g. viridis is defined with 256 colors
-            idx = np.linspace(0, ncolors-1, n).round().astype(int)
+            idx = np.linspace(0, ncolors - 1, n).round().astype(int)
             return [mcolors.rgb2hex(colormap.colors[i]) for i in idx]
 
     return _cmap_d_pal
 
 
 def desaturate_pal(color, prop, reverse=False):
     """
@@ -619,29 +651,31 @@
 
     Examples
     --------
     >>> palette = desaturate_pal('red', .1)
     >>> palette([0, .25, .5, .75, 1])
     ['#ff0000', '#e21d1d', '#c53a3a', '#a95656', '#8c7373']
     """
+    import matplotlib.colors as mcolors
+
     if not 0 <= prop <= 1:
         raise ValueError("prop must be between 0 and 1")
 
     # Get rgb tuple rep
     # Convert to hls
     # Desaturate the saturation channel
     # Convert back to rgb
     rgb = mcolors.colorConverter.to_rgb(color)
     h, l, s = colorsys.rgb_to_hls(*rgb)
     s *= prop
     desaturated_color = colorsys.hls_to_rgb(h, l, s)
     colors = [color, desaturated_color]
     if reverse:
         colors = colors[::-1]
-    return gradient_n_pal(colors, name='desaturated')
+    return gradient_n_pal(colors, name="desaturated")
 
 
 def manual_pal(values):
     """
     Create a palette from a list of values
 
     Parameters
@@ -661,16 +695,18 @@
     >>> palette(3)
     ['a', 'b', 'c']
     """
     max_n = len(values)
 
     def _manual_pal(n):
         if n > max_n:
-            msg = ("Palette can return a maximum of {} values. "
-                   "{} values requested.")
+            msg = (
+                "Palette can return a maximum of {} values. "
+                "{} values requested."
+            )
             warn(msg.format(max_n, n))
 
         return values[:n]
 
     return _manual_pal
 
 
@@ -729,16 +765,17 @@
     >>> from mizani.external import crayon_rgb
     >>> list(sorted(crayon_rgb.keys()))[:5]
     ['almond', 'antique brass', 'apricot', 'aquamarine', 'asparagus']
     """
     return [crayon_rgb[name] for name in colors]
 
 
-def cubehelix_pal(start=0, rot=.4, gamma=1.0, hue=0.8,
-                  light=.85, dark=.15, reverse=False):
+def cubehelix_pal(
+    start=0, rot=0.4, gamma=1.0, hue=0.8, light=0.85, dark=0.15, reverse=False
+):
     """
     Utility for creating continuous palette from the cubehelix system.
 
     This produces a colormap with linearly-decreasing (or increasing)
     brightness. That means that information will be preserved if printed to
     black and white or viewed by someone who is colorblind.
 
@@ -776,16 +813,19 @@
 
     Examples
     --------
     >>> palette = cubehelix_pal()
     >>> palette(5)
     ['#edd1cb', '#d499a7', '#aa688f', '#6e4071', '#2d1e3e']
     """
+    import matplotlib as mpl
+    import matplotlib.colors as mcolors
+
     cdict = mpl._cm.cubehelix(gamma, start, rot, hue)
-    cubehelix_cmap = mpl.colors.LinearSegmentedColormap('cubehelix', cdict)
+    cubehelix_cmap = mcolors.LinearSegmentedColormap("cubehelix", cdict)
 
     def cubehelix_palette(n):
         values = np.linspace(light, dark, n)
         return [mcolors.rgb2hex(cubehelix_cmap(x)) for x in values]
 
     return cubehelix_palette
 
@@ -805,64 +845,7 @@
     >>> palette = identity_pal()
     >>> palette(9)
     9
     >>> palette([2, 4, 6])
     [2, 4, 6]
     """
     return identity
-
-
-def _first_last(it):
-    """
-    First and Last value of iterator as integers
-    """
-    lst = list(it)
-    return int(lst[0]), int(lst[-1])
-
-
-class brewer_helper:
-    """
-    Helper function for useing colorbrewer
-    """
-    _ncolor_range = {
-        t: {
-            palette: _first_last(info.keys())
-            for palette, info in colorbrewer.COLOR_MAPS[t].items()
-           }
-        for t in colorbrewer.COLOR_MAPS
-    }
-
-    @classmethod
-    def num_colors(cls, type, palette):
-        return cls._ncolor_range[type][palette][1]
-
-    @classmethod
-    def min_num_colors(cls, type, palette):
-        return cls._ncolor_range[type][palette][0]
-
-    @staticmethod
-    def full_type_name(text):
-        abbrevs = {
-            'seq': 'Sequential',
-            'qual': 'Qualitative',
-            'div': 'Diverging'
-        }
-        text = abbrevs.get(text, text)
-        return text.title()
-
-    @staticmethod
-    def number_to_name(ctype, n):
-        """
-        Return palette name that corresponds to a given number
-
-        Uses alphabetical ordering
-        """
-        _n = n - 1
-        palettes = sorted(colorbrewer.COLOR_MAPS[ctype].keys())
-        if _n < len(palettes):
-            return palettes[_n]
-
-        npalettes = len(palettes)
-        raise ValueError(
-            f"There are only '{npalettes}' palettes of type {ctype}. "
-            f"You requested palette no. {n}"
-        )
```

### Comparing `mizani-0.8.1/mizani/scale.py` & `mizani-0.9.0/mizani/scale.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,23 @@
 The **apply** methods are simple examples of how to put it all together.
 """
 import numpy as np
 import pandas as pd
 import pandas.api.types as pdtypes
 
 from .bounds import censor, rescale
-from .utils import CONTINUOUS_KINDS, DISCRETE_KINDS, min_max, match
-from .utils import get_categories
+from .utils import (
+    CONTINUOUS_KINDS,
+    DISCRETE_KINDS,
+    get_categories,
+    match,
+    min_max,
+)
 
-
-__all__ = ['scale_continuous', 'scale_discrete']
+__all__ = ["scale_continuous", "scale_discrete"]
 
 
 class scale_continuous:
     """
     Continuous scale
     """
 
@@ -88,20 +92,19 @@
         -------
         out : tuple
             Limits(range) of the scale
         """
         if not len(new_data):
             return old
 
-        if not hasattr(new_data, 'dtype'):
+        if not hasattr(new_data, "dtype"):
             new_data = np.asarray(new_data)
 
         if new_data.dtype.kind not in CONTINUOUS_KINDS:
-            raise TypeError(
-                "Discrete value supplied to continuous scale")
+            raise TypeError("Discrete value supplied to continuous scale")
 
         if old is not None:
             new_data = np.hstack([new_data, old])
 
         return min_max(new_data, na_rm=True, finite=True)
 
     @classmethod
@@ -192,21 +195,20 @@
             old = []
         else:
             old = list(old)
 
         # Get the missing values (NaN & Nones) locations and remove them
         nan_bool_idx = pd.isnull(new_data)
         has_na = np.any(nan_bool_idx)
-        if not hasattr(new_data, 'dtype'):
+        if not hasattr(new_data, "dtype"):
             new_data = np.asarray(new_data)
         new_data = new_data[~nan_bool_idx]
 
         if new_data.dtype.kind not in DISCRETE_KINDS:
-            raise TypeError(
-                "Continuous value supplied to discrete scale")
+            raise TypeError("Continuous value supplied to discrete scale")
 
         # Train i.e. get the new values
         if pdtypes.is_categorical_dtype(new_data):
             categories = get_categories(new_data)
             if drop:
                 present = set(new_data.drop_duplicates())
                 new = [i for i in categories if i in present]
```

### Comparing `mizani-0.8.1/mizani/tests/test_bounds.py` & `mizani-0.9.0/mizani/tests/test_bounds.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,131 +4,124 @@
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pandas.testing as pdt
 import pytest
 from pytest import approx
 
-from mizani.bounds import (censor, expand_range, rescale, rescale_max,
-                           rescale_mid, squish_infinite, zero_range,
-                           expand_range_distinct, squish)
+from mizani.bounds import (
+    censor,
+    expand_range,
+    expand_range_distinct,
+    rescale,
+    rescale_max,
+    rescale_mid,
+    squish,
+    squish_infinite,
+    zero_range,
+)
 
 NaT_type = type(pd.NaT)
 
 
 def test_censor():
     x = list(range(10))
     xx = censor(x, (2, 8))
     assert np.isnan(xx[0])
     assert np.isnan(xx[1])
     assert np.isnan(xx[9])
 
-    df = pd.DataFrame({'x': x, 'y': range(10)})
-    df['x'] = censor(df['x'], (2, 8))
-    assert np.isnan(df['x'][0])
-    assert np.isnan(df['x'][1])
-    assert np.isnan(df['x'][9])
+    df = pd.DataFrame({"x": x, "y": range(10)})
+    df["x"] = censor(df["x"], (2, 8))
+    assert np.isnan(df["x"][0])
+    assert np.isnan(df["x"][1])
+    assert np.isnan(df["x"][9])
 
-    df['y'] = censor(df['y'], (-2, 18))
-    assert issubclass(df['y'].dtype.type, np.integer)
+    df["y"] = censor(df["y"], (-2, 18))
+    assert issubclass(df["y"].dtype.type, np.integer)
 
     # datetime
     limits = datetime(2010, 1, 1), datetime(2020, 1, 1)
     x = [datetime(year, 1, 1) for year in range(2008, 2023)]
     result = censor(x, limits)
     assert result[2:-2] == x[2:-2]
-    assert result[:2] == ['NaT', 'NaT']
-    assert result[-2:] == ['NaT', 'NaT']
+    assert result[:2] == ["NaT", "NaT"]
+    assert result[-2:] == ["NaT", "NaT"]
 
     # timedelta
     limits = timedelta(seconds=2010), timedelta(seconds=2020)
     x = [timedelta(seconds=i) for i in range(2008, 2023)]
     result = censor(x, limits)
     assert result[2:-2] == x[2:-2]
-    assert result[:2] == ['NaT', 'NaT']
-    assert result[-2:] == ['NaT', 'NaT']
+    assert result[:2] == ["NaT", "NaT"]
+    assert result[-2:] == ["NaT", "NaT"]
 
     # pd.timestamp
-    limits = pd.Timestamp(200*1e16), pd.Timestamp(205*1e16)
-    x = [pd.Timestamp(i*1e16) for i in range(198, 208)]
+    limits = pd.Timestamp(200 * 1e16), pd.Timestamp(205 * 1e16)
+    x = [pd.Timestamp(i * 1e16) for i in range(198, 208)]
     result = censor(x, limits)
     assert result[2:-2] == x[2:-2]
-    assert all(isinstance(val, NaT_type)
-               for val in result[:2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[-2:])
+    assert all(isinstance(val, NaT_type) for val in result[:2])
+    assert all(isinstance(val, NaT_type) for val in result[-2:])
 
     x1 = np.array(x)
     result = censor(x1, limits)
     npt.assert_array_equal(result[2:-2], x1[2:-2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[:2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[-2:])
+    assert all(isinstance(val, NaT_type) for val in result[:2])
+    assert all(isinstance(val, NaT_type) for val in result[-2:])
 
     x2 = pd.Series(x)
     result = censor(x2, limits)
     pdt.assert_series_equal(result[2:-2], x2[2:-2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[:2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[-2:])
+    assert all(isinstance(val, NaT_type) for val in result[:2])
+    assert all(isinstance(val, NaT_type) for val in result[-2:])
 
     # np.datetime
-    limits = np.datetime64(200, 'D'), np.datetime64(205, 'D')
-    x = [np.datetime64(i, 'D') for i in range(198, 208)]
+    limits = np.datetime64(200, "D"), np.datetime64(205, "D")
+    x = [np.datetime64(i, "D") for i in range(198, 208)]
     x2 = np.array(x)
     result = censor(x2, limits)
     npt.assert_array_equal(result[2:-2], x2[2:-2])
-    assert all(isinstance(val, np.datetime64)
-               for val in result[:2])
-    assert all(isinstance(val, np.datetime64)
-               for val in result[-2:])
+    assert all(isinstance(val, np.datetime64) for val in result[:2])
+    assert all(isinstance(val, np.datetime64) for val in result[-2:])
 
     # pd.Timedelta
     limits = pd.Timedelta(seconds=2010), pd.Timedelta(seconds=2020)
     x = [pd.Timedelta(seconds=i) for i in range(2008, 2023)]
     result = censor(x, limits)
     assert isinstance(result, list)
     assert result[2:-2] == x[2:-2]
-    assert all(isinstance(val, NaT_type)
-               for val in result[:2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[-2:])
+    assert all(isinstance(val, NaT_type) for val in result[:2])
+    assert all(isinstance(val, NaT_type) for val in result[-2:])
 
     x4 = np.array(x)
     result = censor(x4, limits)
     npt.assert_array_equal(result[2:-2], x4[2:-2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[:2])
-    assert all(isinstance(val, NaT_type)
-               for val in result[-2:])
+    assert all(isinstance(val, NaT_type) for val in result[:2])
+    assert all(isinstance(val, NaT_type) for val in result[-2:])
 
     # np.timedelta64
-    limits = np.timedelta64(200, 'D'), np.timedelta64(205, 'D')
-    x = [np.timedelta64(i, 'D') for i in range(198, 208)]
+    limits = np.timedelta64(200, "D"), np.timedelta64(205, "D")
+    x = [np.timedelta64(i, "D") for i in range(198, 208)]
     x5 = np.array(x)
     result = censor(x5, limits)
     npt.assert_array_equal(result[2:-2], x5[2:-2])
-    assert all(isinstance(val, np.timedelta64)
-               for val in result[:2])
-    assert all(isinstance(val, np.timedelta64)
-               for val in result[-2:])
+    assert all(isinstance(val, np.timedelta64) for val in result[:2])
+    assert all(isinstance(val, np.timedelta64) for val in result[-2:])
 
     # branches #
     x = np.array([1, 2, np.inf, 3, 4, 11])
     result = censor(x, (0, 10), only_finite=False)
-    npt.assert_array_equal(
-        result, np.array([1, 2, np.nan, 3, 4, np.nan]))
+    npt.assert_array_equal(result, np.array([1, 2, np.nan, 3, 4, np.nan]))
 
     result = censor([], (-2, 18))
     assert len(result) == 0
 
     with pytest.raises(ValueError):
-        result = censor(['a', 'b', 'c'], ('a', 'z'))
+        result = censor(["a", "b", "c"], ("a", "z"))
 
 
 def test_expand_range():
     assert expand_range((0, 1)) == (0, 1)
     assert expand_range((0, 1), mul=2) == (-2, 3)
     assert expand_range((0, 1), add=2) == (-2, 3)
     assert expand_range((0, 1), mul=2, add=2) == (-4, 5)
@@ -138,84 +131,84 @@
     def diff(x):
         return x[1] - x[0]
 
     # datetime
     one_day = datetime(2010, 1, 2) - datetime(2010, 1, 1)
     limits = datetime(2010, 1, 1), datetime(2010, 1, 2)
     result = expand_range(limits, add=one_day)
-    diff(result) == diff(limits) + 2*one_day
+    diff(result) == diff(limits) + 2 * one_day
 
     limits = datetime(2010, 1, 1), datetime(2010, 1, 1)  # zero range
-    result = expand_range(limits, zero_width=30*one_day)
-    diff(result) == diff(limits) + 30*one_day
+    result = expand_range(limits, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 30 * one_day
 
     # pd.Timestamp
-    one_day = pd.Timestamp('2010-01-02') - pd.Timestamp('2010-01-01')
-    limits = pd.Timestamp('2010-01-01'), pd.Timestamp('2010-01-02')
+    one_day = pd.Timestamp("2010-01-02") - pd.Timestamp("2010-01-01")
+    limits = pd.Timestamp("2010-01-01"), pd.Timestamp("2010-01-02")
     result = expand_range(limits, add=one_day)
-    diff(result) == diff(limits) + 2*one_day
+    diff(result) == diff(limits) + 2 * one_day
 
     result = expand_range(limits, mul=0.5, add=one_day)
-    diff(result) == 2*diff(limits) + 2*one_day
+    diff(result) == 2 * diff(limits) + 2 * one_day
 
-    limits = pd.Timestamp('2010-01-01'), pd.Timestamp('2010-01-01')
-    result = expand_range(limits, zero_width=30*one_day)
-    diff(result) == diff(limits) + 30*one_day
+    limits = pd.Timestamp("2010-01-01"), pd.Timestamp("2010-01-01")
+    result = expand_range(limits, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 30 * one_day
 
     # np.datetime64
-    one_day = np.datetime64(1, 'D') - np.datetime64(0, 'D')
-    limits = np.datetime64(14610, 'D'), np.datetime64(14611, 'D')
+    one_day = np.datetime64(1, "D") - np.datetime64(0, "D")
+    limits = np.datetime64(14610, "D"), np.datetime64(14611, "D")
     result = expand_range(limits, add=one_day)
-    diff(result) == diff(limits) + 2*one_day
+    diff(result) == diff(limits) + 2 * one_day
 
     result = expand_range(limits, mul=0.5, add=one_day)
-    diff(result) == 2*diff(limits) + 2*one_day
+    diff(result) == 2 * diff(limits) + 2 * one_day
 
-    limits = np.datetime64(14610, 'D'), np.datetime64(14611, 'D')
-    result = expand_range(limits, zero_width=30*one_day)
-    diff(result) == diff(limits) + 30*one_day
+    limits = np.datetime64(14610, "D"), np.datetime64(14611, "D")
+    result = expand_range(limits, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 30 * one_day
 
     # timedelta
     one_day = timedelta(days=1)
     limits = timedelta(days=1), timedelta(days=10)
-    result = expand_range(limits, add=one_day, zero_width=30*one_day)
-    diff(result) == diff(limits) + 2*one_day
+    result = expand_range(limits, add=one_day, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 2 * one_day
 
     result = expand_range(limits, mul=0.5, add=one_day)
-    diff(result) == 2*diff(limits) + 2*one_day
+    diff(result) == 2 * diff(limits) + 2 * one_day
 
     limits = timedelta(days=10), timedelta(days=10)
-    result = expand_range(limits, add=one_day, zero_width=30*one_day)
-    diff(result) == diff(limits) + 30*one_day
+    result = expand_range(limits, add=one_day, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 30 * one_day
 
     # pd.Timedelta
     one_day = pd.Timedelta(days=1)
     limits = pd.Timedelta(days=1), pd.Timedelta(days=10)
-    result = expand_range(limits, add=one_day, zero_width=30*one_day)
-    diff(result) == diff(limits) + 2*one_day
+    result = expand_range(limits, add=one_day, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 2 * one_day
 
     result = expand_range(limits, mul=0.5, add=one_day)
-    diff(result) == 2*diff(limits) + 2*one_day
+    diff(result) == 2 * diff(limits) + 2 * one_day
 
     limits = pd.Timedelta(days=10), pd.Timedelta(days=10)
-    result = expand_range(limits, add=one_day, zero_width=30*one_day)
-    diff(result) == diff(limits) + 30*one_day
+    result = expand_range(limits, add=one_day, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 30 * one_day
 
     # timedelta64
-    one_day = np.timedelta64(1, 'D')
-    limits = np.timedelta64(1, 'D'), np.timedelta64(10, 'D')
-    result = expand_range(limits, add=one_day, zero_width=30*one_day)
-    diff(result) == diff(limits) + 2*one_day
+    one_day = np.timedelta64(1, "D")
+    limits = np.timedelta64(1, "D"), np.timedelta64(10, "D")
+    result = expand_range(limits, add=one_day, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 2 * one_day
 
     result = expand_range(limits, mul=0.5, add=one_day)
-    diff(result) == 2*diff(limits) + 2*one_day
+    diff(result) == 2 * diff(limits) + 2 * one_day
 
-    limits = np.timedelta64(1, 'D'), np.timedelta64(1, 'D')
-    result = expand_range(limits, add=one_day, zero_width=30*one_day)
-    diff(result) == diff(limits) + 30*one_day
+    limits = np.timedelta64(1, "D"), np.timedelta64(1, "D")
+    result = expand_range(limits, add=one_day, zero_width=30 * one_day)
+    diff(result) == diff(limits) + 30 * one_day
 
 
 def test_expand_range_distinct():
     assert expand_range_distinct((0, 1)) == (0, 1)
     assert expand_range_distinct((0, 1), (2, 0)) == (-2, 3)
     assert expand_range_distinct((0, 1), (2, 0, 2, 0)) == (-2, 3)
     assert expand_range_distinct((0, 1), (0, 2)) == (-2, 3)
@@ -225,26 +218,26 @@
 
 
 def test_rescale():
     # [0, 10] -> [0, 1]
     # Results are invariant to uniformly translated
     # or expanded inputs
     a = np.arange(0, 11)
-    npt.assert_allclose(rescale(a), a*.1)
-    npt.assert_allclose(rescale(a), rescale(a-42))
-    npt.assert_allclose(rescale(a), rescale(a+42))
-    npt.assert_allclose(rescale(a), rescale(a/np.pi))
-    npt.assert_allclose(rescale(a), rescale(a*np.pi))
+    npt.assert_allclose(rescale(a), a * 0.1)
+    npt.assert_allclose(rescale(a), rescale(a - 42))
+    npt.assert_allclose(rescale(a), rescale(a + 42))
+    npt.assert_allclose(rescale(a), rescale(a / np.pi))
+    npt.assert_allclose(rescale(a), rescale(a * np.pi))
 
     # Some more
     n = 6
     a = np.arange(0, n)
-    npt.assert_allclose(rescale(a), a/(n-1))
-    npt.assert_allclose(rescale(a, _from=(0, 10)), a*.1)
-    npt.assert_allclose(rescale(a, to=(0, n*(n-1))), a*n)
+    npt.assert_allclose(rescale(a), a / (n - 1))
+    npt.assert_allclose(rescale(a, _from=(0, 10)), a * 0.1)
+    npt.assert_allclose(rescale(a, to=(0, n * (n - 1))), a * n)
 
 
 def test_rescale_max():
     a = np.arange(0, 11)
     # Max & first element has no effect
     assert max(rescale_max(a, to=(0, 5))) == 5
     assert max(rescale_max(a, to=(4, 5))) == 5
@@ -269,67 +262,63 @@
     assert result == approx([0, 1, 2, 3, 4, 5])
 
 
 def test_rescale_mid():
     a = [1, 2, 3]
     # no change
     npt.assert_allclose(rescale_mid(a, to=(1, 3), mid=2), a)
-    npt.assert_allclose(
-        rescale_mid(a, to=(1, 4), _from=(1, 4), mid=2.5), a)
+    npt.assert_allclose(rescale_mid(a, to=(1, 4), _from=(1, 4), mid=2.5), a)
 
-    npt.assert_allclose(rescale_mid(a, mid=1), [.5, .75, 1])
-    npt.assert_allclose(rescale_mid(a, mid=2), [0, .5, 1])
-    npt.assert_allclose(rescale_mid(a, mid=3), [0, .25, .5])
+    npt.assert_allclose(rescale_mid(a, mid=1), [0.5, 0.75, 1])
+    npt.assert_allclose(rescale_mid(a, mid=2), [0, 0.5, 1])
+    npt.assert_allclose(rescale_mid(a, mid=3), [0, 0.25, 0.5])
 
     # branches #
     npt.assert_allclose(rescale_mid(2, to=(1, 3), mid=2), 2)
-    npt.assert_allclose(
-        rescale_mid([2], _from=(2, 2), to=(2, 2), mid=2),
-        [2])
+    npt.assert_allclose(rescale_mid([2], _from=(2, 2), to=(2, 2), mid=2), [2])
 
     # Maintains the same index
     s = pd.Series([1, 2, 3], index=[3, 2, 1])
     result = rescale_mid(s, mid=1)
     assert s.index.equals(result.index)
 
 
 def test_squish_infinite():
     a = [-np.inf, np.inf, -np.inf, np.inf]
     npt.assert_allclose(squish_infinite(a), [0, 1, 0, 1])
-    npt.assert_allclose(squish_infinite(a, (-100, 100)),
-                        [-100, 100, -100, 100])
+    npt.assert_allclose(
+        squish_infinite(a, (-100, 100)), [-100, 100, -100, 100]
+    )
 
     b = np.array([5, -np.inf, 2, 3, 6])
-    npt.assert_allclose(squish_infinite(b, (1, 10)),
-                        [5, 1, 2, 3, 6])
+    npt.assert_allclose(squish_infinite(b, (1, 10)), [5, 1, 2, 3, 6])
 
     # Maintains the same index
     s = pd.Series([1, 2, 3, 4], index=[4, 3, 2, 1])
     result = squish_infinite(s)
     assert s.index.equals(result.index)
 
 
 def test_squish():
     a = [-np.inf, np.inf, -np.inf, np.inf]
     npt.assert_allclose(squish(a, only_finite=False), [0, 1, 0, 1])
     npt.assert_allclose(squish(a, only_finite=True), a)
-    npt.assert_allclose(squish(a, (-100, 100), only_finite=False),
-                        [-100, 100, -100, 100])
+    npt.assert_allclose(
+        squish(a, (-100, 100), only_finite=False), [-100, 100, -100, 100]
+    )
 
     b = np.array([5, 0, -2, 3, 10])
-    npt.assert_allclose(squish(b, (0, 5)),
-                        [5, 0, 0, 3, 5])
+    npt.assert_allclose(squish(b, (0, 5)), [5, 0, 0, 3, 5])
 
     c = np.array([5, -np.inf, 2, 3, 6])
-    npt.assert_allclose(squish(c, (1, 10), only_finite=False),
-                        [5, 1, 2, 3, 6])
+    npt.assert_allclose(squish(c, (1, 10), only_finite=False), [5, 1, 2, 3, 6])
     npt.assert_allclose(squish(c, (1, 10)), c)
 
     # Maintains the same index
-    s = pd.Series([.1, .2, .3, 9], index=[4, 3, 2, 1])
+    s = pd.Series([0.1, 0.2, 0.3, 9], index=[4, 3, 2, 1])
     result = squish(s)
     assert s.index.equals(result.index)
 
 
 def test_zero_range():
     c = np.array
     eps = np.finfo(float).eps
@@ -345,16 +334,16 @@
     assert not zero_range(c((1, 1 + 2 * eps)), tol=eps)
 
     # Scaling up or down all the values has no effect since
     # the values are rescaled to 1 before checking against
     # the tolerance
     assert zero_range(100000 * c((1, 1 + eps)))
     assert not zero_range(100000 * c((1, 1 + 200 * eps)))
-    assert zero_range(.00001 * c((1, 1 + eps)))
-    assert not zero_range(.00001 * c((1, 1 + 200 * eps)))
+    assert zero_range(0.00001 * c((1, 1 + eps)))
+    assert not zero_range(0.00001 * c((1, 1 + 200 * eps)))
 
     # NA values
     assert zero_range((1, np.nan))
 
     # Infinite values
     assert not zero_range((1, np.inf))
     assert not zero_range((-np.inf, np.inf))
@@ -367,49 +356,53 @@
     # length greater than 2
     with pytest.raises(ValueError):
         zero_range([1, 2, 3])
 
     # datetime - pandas, cpython
     x = datetime(2010, 1, 1), datetime(2010, 1, 1)
     x2 = datetime(2010, 1, 1), datetime(2020, 1, 1)
-    x3 = (pd.Timestamp('2010-01-01', tz='US/Eastern'),
-          pd.Timestamp('2010-01-01', tz='US/Central'))
+    x3 = (
+        pd.Timestamp("2010-01-01", tz="US/Eastern"),
+        pd.Timestamp("2010-01-01", tz="US/Central"),
+    )
     assert zero_range(x)
     assert not zero_range(x2)
     assert not zero_range(x3)
 
     # datetime - numpy
-    x = np.datetime64(7, 'D'), np.datetime64(7, 'D')
-    x2 = np.datetime64(7, 'D'), np.datetime64(1, 'W')
-    x3 = np.datetime64(7, 'D'), np.datetime64(1, 'D')
+    x = np.datetime64(7, "D"), np.datetime64(7, "D")
+    x2 = np.datetime64(7, "D"), np.datetime64(1, "W")
+    x3 = np.datetime64(7, "D"), np.datetime64(1, "D")
     assert zero_range(x)
     assert zero_range(x2)
     assert not zero_range(x3)
 
     # timedelta - pandas, cpython
     x = timedelta(seconds=2010), timedelta(seconds=2010)
-    x2 = (timedelta(seconds=2010, microseconds=90),
-          timedelta(seconds=2010, microseconds=34))
-    x3 = pd.Timedelta(200, 'D'), pd.Timedelta(203, 'D')
+    x2 = (
+        timedelta(seconds=2010, microseconds=90),
+        timedelta(seconds=2010, microseconds=34),
+    )
+    x3 = pd.Timedelta(200, "D"), pd.Timedelta(203, "D")
     assert zero_range(x)
     assert not zero_range(x2)
     assert not zero_range(x3)
 
     # timedelta - numpy
-    x = np.timedelta64(7, 'D'), np.timedelta64(7, 'D')
-    x2 = np.timedelta64(7, 'D'), np.timedelta64(1, 'W')
-    x3 = np.timedelta64(7, 'D'), np.timedelta64(2, 'D')
+    x = np.timedelta64(7, "D"), np.timedelta64(7, "D")
+    x2 = np.timedelta64(7, "D"), np.timedelta64(1, "W")
+    x3 = np.timedelta64(7, "D"), np.timedelta64(2, "D")
     assert zero_range(x)
     assert zero_range(x2)
     assert not zero_range(x3)
 
     # branches #
-    assert str(zero_range([4, float('nan')])) == 'nan'
-    assert not zero_range([4, float('inf')])
+    assert str(zero_range([4, float("nan")])) == "nan"
+    assert not zero_range([4, float("inf")])
     with pytest.raises(TypeError):
-        zero_range(['a', 'b'])
+        zero_range(["a", "b"])
 
     # are handled without error
     x = np.array([8, 4], dtype=np.uint64)
     with warnings.catch_warnings():
-        warnings.simplefilter('error')
+        warnings.simplefilter("error")
         zero_range(x)
```

### Comparing `mizani-0.8.1/mizani/tests/test_breaks.py` & `mizani-0.9.0/mizani/tests/test_breaks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from datetime import datetime, timedelta
 
-import pandas as pd
 import numpy as np
 import numpy.testing as npt
+import pandas as pd
 import pytest
 
-from mizani.breaks import (mpl_breaks, log_breaks, minor_breaks,
-                           trans_minor_breaks, date_breaks,
-                           timedelta_breaks, extended_breaks)
-from mizani.transforms import trans, log_trans
+from mizani.breaks import (
+    date_breaks,
+    extended_breaks,
+    log_breaks,
+    minor_breaks,
+    mpl_breaks,
+    timedelta_breaks,
+    trans_minor_breaks,
+)
+from mizani.transforms import log_trans, trans
 
 
 def test_mpl_breaks():
     x = np.arange(100)
     limits = min(x), max(x)
     for nbins in (5, 7, 10, 13, 31):
         breaks = mpl_breaks(nbins=nbins)
-        assert len(breaks(limits)) <= nbins+1
+        assert len(breaks(limits)) <= nbins + 1
 
-    limits = float('-inf'), float('inf')
+    limits = float("-inf"), float("inf")
     breaks = mpl_breaks(nbins=5)
     assert len(breaks(limits)) == 0
 
     # Zero range discrete
     limits = [1, 1]
     assert len(breaks(limits)) == 1
     assert breaks(limits)[0] == limits[1]
@@ -41,92 +47,93 @@
 
     breaks = log_breaks(3)(limits)
     npt.assert_array_equal(breaks, [1, 100, 10000])
 
     breaks = log_breaks()((10000, 10000))
     npt.assert_array_equal(breaks, [10000])
 
-    breaks = log_breaks()((float('-inf'), float('inf')))
+    breaks = log_breaks()((float("-inf"), float("inf")))
     assert len(breaks) == 0
 
     # When the limits are in the same order of magnitude
     breaks = log_breaks()([35, 60])
     assert len(breaks) > 0
     assert all([1 < b < 100 for b in breaks])
 
     breaks = log_breaks()([200, 800])
-    npt.assert_array_equal(breaks, [100,  200,  300,  500, 1000])
+    npt.assert_array_equal(breaks, [100, 200, 300, 500, 1000])
 
     breaks = log_breaks()((1664, 14008))
     npt.assert_array_equal(breaks, [1000, 3000, 5000, 10000, 30000])
 
     breaks = log_breaks()([407, 3430])
-    npt.assert_array_equal(breaks, [300,  500, 1000, 3000, 5000])
+    npt.assert_array_equal(breaks, [300, 500, 1000, 3000, 5000])
 
     breaks = log_breaks()([1761, 8557])
     npt.assert_array_equal(breaks, [1000, 2000, 3000, 5000, 10000])
 
     # log_breaks -> _log_sub_breaks -> extended_breaks
     breaks = log_breaks(13)([1, 10])
-    npt.assert_array_almost_equal(
-        breaks,
-        np.arange(0, 11)
-    )
+    npt.assert_array_almost_equal(breaks, np.arange(0, 11))
 
     # No overflow effects
     breaks = log_breaks(n=6)([1e25, 1e30])
-    npt.assert_array_almost_equal(
-        breaks,
-        [1e25, 1e26, 1e27, 1e28, 1e29, 1e30]
-    )
+    npt.assert_array_almost_equal(breaks, [1e25, 1e26, 1e27, 1e28, 1e29, 1e30])
 
     # No overflow effects in _log_sub_breaks
     breaks = log_breaks()([2e19, 8e19])
     npt.assert_array_almost_equal(
-        breaks,
-        [1.e+19, 2.e+19, 3.e+19, 5.e+19, 1.e+20]
+        breaks, [1.0e19, 2.0e19, 3.0e19, 5.0e19, 1.0e20]
     )
 
     # _log_sub_breaks for base != 10
     breaks = log_breaks(n=5, base=60)([2e5, 8e5])
     npt.assert_array_almost_equal(
-        breaks,
-        [129600, 216000, 432000, 648000, 1080000]
+        breaks, [129600, 216000, 432000, 648000, 1080000]
     )
 
     breaks = log_breaks(n=5, base=2)([20, 80])
-    npt.assert_array_almost_equal(
-        breaks,
-        [16, 32, 64, 128]
-    )
+    npt.assert_array_almost_equal(breaks, [16, 32, 64, 128])
 
     # bases & negative breaks
     breaks = log_breaks(base=2)([0.9, 2.9])
-    npt.assert_array_almost_equal(
-        breaks,
-        [0.5, 1., 2., 4.]
-    )
+    npt.assert_array_almost_equal(breaks, [0.5, 1.0, 2.0, 4.0])
 
 
 def test_minor_breaks():
     # equidistant breaks
     major = [1, 2, 3, 4]
     limits = [0, 5]
     breaks = minor_breaks()(major, limits)
-    npt.assert_array_equal(breaks, [.5, 1.5, 2.5, 3.5, 4.5])
+    npt.assert_array_equal(breaks, [0.5, 1.5, 2.5, 3.5, 4.5])
     minor = minor_breaks(3)(major, [2, 3])
     npt.assert_array_equal(minor, [2.25, 2.5, 2.75])
 
     # More than 1 minor breaks
     breaks = minor_breaks()(major, limits, 3)
-    npt.assert_array_equal(breaks, [.25, .5, .75,
-                                    1.25, 1.5, 1.75,
-                                    2.25, 2.5, 2.75,
-                                    3.25, 3.5, 3.75,
-                                    4.25, 4.5, 4.75])
+    npt.assert_array_equal(
+        breaks,
+        [
+            0.25,
+            0.5,
+            0.75,
+            1.25,
+            1.5,
+            1.75,
+            2.25,
+            2.5,
+            2.75,
+            3.25,
+            3.5,
+            3.75,
+            4.25,
+            4.5,
+            4.75,
+        ],
+    )
 
     # non-equidistant breaks
     major = [1, 2, 4, 8]
     limits = [0, 10]
     minor = minor_breaks()(major, limits)
     npt.assert_array_equal(minor, [1.5, 3, 6])
 
@@ -153,23 +160,23 @@
         def __init__(self):
             self.minor_breaks = trans_minor_breaks(weird_trans)
 
     major = [1, 2, 3, 4]
     limits = [0, 5]
     regular_minors = trans().minor_breaks(major, limits)
     npt.assert_allclose(
-        regular_minors,
-        identity_trans().minor_breaks(major, limits))
+        regular_minors, identity_trans().minor_breaks(major, limits)
+    )
 
     # Transform the input major breaks and check against
     # the inverse of the output minor breaks
     squared_input_minors = square_trans().minor_breaks(
-        np.square(major), np.square(limits))
-    npt.assert_allclose(regular_minors,
-                        np.sqrt(squared_input_minors))
+        np.square(major), np.square(limits)
+    )
+    npt.assert_allclose(regular_minors, np.sqrt(squared_input_minors))
 
     t = weird_trans()
     with pytest.raises(TypeError):
         t.minor_breaks(major)
 
     # Test minor_breaks for log scales are 2 less than the base
     base = 10
@@ -186,96 +193,100 @@
 
     t = log_trans()
     major = t.transform([1, 10, 100])
     limits = t.transform([1, 100])
     result = trans_minor_breaks(t)(major, limits, n=4)
     npt.assert_allclose(
         result,
-        [1.02961942, 1.5260563, 1.85629799, 2.10413415,
-         3.33220451, 3.8286414, 4.15888308, 4.40671925]
+        [
+            1.02961942,
+            1.5260563,
+            1.85629799,
+            2.10413415,
+            3.33220451,
+            3.8286414,
+            4.15888308,
+            4.40671925,
+        ],
     )
 
 
 def test_date_breaks():
     # cpython
     x = [datetime(year, 1, 1) for year in [2010, 2026, 2015]]
     limits = min(x), max(x)
 
-    breaks = date_breaks('5 Years')
+    breaks = date_breaks("5 Years")
     years = [d.year for d in breaks(limits)]
-    npt.assert_array_equal(
-        years, [2010, 2015, 2020, 2025, 2030])
+    npt.assert_array_equal(years, [2010, 2015, 2020, 2025, 2030])
 
-    breaks = date_breaks('10 Years')
+    breaks = date_breaks("10 Years")
     years = [d.year for d in breaks(limits)]
     npt.assert_array_equal(years, [2010, 2020, 2030])
 
     # numpy
-    x = [np.datetime64(i*10, 'D') for i in range(1, 10)]
-    breaks = date_breaks('10 Years')
+    x = [np.datetime64(i * 10, "D") for i in range(1, 10)]
+    breaks = date_breaks("10 Years")
     limits = min(x), max(x)
     with pytest.raises(AttributeError):
         breaks(limits)
 
     # NaT
-    limits = np.datetime64('NaT'), datetime(2017, 1, 1)
-    breaks = date_breaks('10 Years')
+    limits = np.datetime64("NaT"), datetime(2017, 1, 1)
+    breaks = date_breaks("10 Years")
     assert len(breaks(limits)) == 0
 
 
 def test_timedelta_breaks():
     breaks = timedelta_breaks()
 
     # cpython
-    x = [timedelta(days=i*365) for i in range(25)]
+    x = [timedelta(days=i * 365) for i in range(25)]
     limits = min(x), max(x)
     major = breaks(limits)
-    years = [val.total_seconds()/(365*24*60*60)for val in major]
-    npt.assert_array_equal(
-        years, [0, 5, 10, 15, 20, 25])
+    years = [val.total_seconds() / (365 * 24 * 60 * 60) for val in major]
+    npt.assert_array_equal(years, [0, 5, 10, 15, 20, 25])
 
     x = [timedelta(microseconds=i) for i in range(25)]
     limits = min(x), max(x)
     major = breaks(limits)
-    mseconds = [val.total_seconds()*10**6 for val in major]
-    npt.assert_array_equal(
-        mseconds, [0, 5, 10, 15, 20, 25])
+    mseconds = [val.total_seconds() * 10**6 for val in major]
+    npt.assert_array_equal(mseconds, [0, 5, 10, 15, 20, 25])
 
     # pandas
-    x = [pd.Timedelta(seconds=i*60) for i in range(10)]
+    x = [pd.Timedelta(seconds=i * 60) for i in range(10)]
     limits = min(x), max(x)
     major = breaks(limits)
-    minutes = [val.total_seconds()/60 for val in major]
-    npt.assert_allclose(
-        minutes, [0, 2, 4, 6, 8])
+    minutes = [val.total_seconds() / 60 for val in major]
+    npt.assert_allclose(minutes, [0, 2, 4, 6, 8])
 
     # numpy
-    x = [np.timedelta64(i*10, 'D') for i in range(1, 10)]
+    x = [np.timedelta64(i * 10, "D") for i in range(1, 10)]
     limits = min(x), max(x)
     with pytest.raises(ValueError):
         breaks(limits)
 
     # NaT
-    limits = pd.NaT, pd.Timedelta(seconds=9*60)
+    limits = pd.NaT, pd.Timedelta(seconds=9 * 60)
     assert len(breaks(limits)) == 0
 
 
 def test_extended_breaks():
     x = np.arange(100)
     limits = min(x), max(x)
     for n in (5, 7, 10, 13, 31):
         breaks = extended_breaks(n=n)
-        assert len(breaks(limits)) <= n+1
+        assert len(breaks(limits)) <= n + 1
 
     # Reverse limits
     breaks = extended_breaks(n=7)
     npt.assert_array_equal(breaks((0, 6)), breaks((6, 0)))
 
     # Infinite limits
-    limits = float('-inf'), float('inf')
+    limits = float("-inf"), float("inf")
     breaks = extended_breaks(n=5)
     assert len(breaks(limits)) == 0
 
     # Zero range discrete
     limits = [1, 1]
     assert len(breaks(limits)) == 1
     assert breaks(limits)[0] == limits[1]
```

### Comparing `mizani-0.8.1/mizani/tests/test_formatters.py` & `mizani-0.9.0/mizani/tests/test_formatters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,216 +1,251 @@
 # -*- coding: utf-8 -*-
 import warnings
 from datetime import datetime, timedelta
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 import pytest
+
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     # python < 3.9
     from backports.zoneinfo import ZoneInfo
 
-from mizani.formatters import (custom_format, comma_format,
-                               currency_format, percent_format,
-                               scientific_format, date_format,
-                               mpl_format, log_format, timedelta_format,
-                               pvalue_format, ordinal_format,
-                               number_bytes_format)
+from mizani.formatters import (
+    comma_format,
+    currency_format,
+    custom_format,
+    date_format,
+    log_format,
+    mpl_format,
+    number_bytes_format,
+    ordinal_format,
+    percent_format,
+    pvalue_format,
+    scientific_format,
+    timedelta_format,
+)
 
 
 def test_custom_format():
     x = [3.987, 2, 42.42]
-    labels = ['3.99 USD', '2.00 USD', '42.42 USD']
-    formatter = custom_format('{:.2f} USD')
+    labels = ["3.99 USD", "2.00 USD", "42.42 USD"]
+    formatter = custom_format("{:.2f} USD")
     assert formatter(x) == labels
 
-    formatter = custom_format('%.2f USD', style='old')
+    formatter = custom_format("%.2f USD", style="old")
     assert formatter(x) == labels
 
-    formatter = custom_format('%.2f USD', style='ancient')
+    formatter = custom_format("%.2f USD", style="ancient")
     with pytest.raises(ValueError):
         formatter(x)
 
 
 def test_currency_format():
     x = [1.232, 99.2334, 4.6, 9, 4500]
-    formatter = currency_format('C$', digits=0, big_mark=',')
+    formatter = currency_format("C$", digits=0, big_mark=",")
     result = formatter(x)
-    assert result == ['C$1', 'C$99', 'C$5', 'C$9', 'C$4,500']
+    assert result == ["C$1", "C$99", "C$5", "C$9", "C$4,500"]
 
-    formatter = currency_format('C$', digits=0, big_mark=' ')
+    formatter = currency_format("C$", digits=0, big_mark=" ")
     result = formatter(x)
-    assert result == ['C$1', 'C$99', 'C$5', 'C$9', 'C$4 500']
+    assert result == ["C$1", "C$99", "C$5", "C$9", "C$4 500"]
 
-    formatter = currency_format('$', digits=2)
+    formatter = currency_format("$", digits=2)
     result = formatter(x)
-    assert result == ['$1.23', '$99.23', '$4.60', '$9.00', '$4500.00']
+    assert result == ["$1.23", "$99.23", "$4.60", "$9.00", "$4500.00"]
 
 
 def test_comma_format():
     x = [1000, 2, 33000, 400]
     result = comma_format()(x)
-    assert result == ['1,000', '2', '33,000', '400']
+    assert result == ["1,000", "2", "33,000", "400"]
 
 
 def test_percent_format():
     formatter = percent_format()
     # same/nearly same precision values
-    assert formatter([.12, .23, .34, .45]) == \
-        ['12%', '23%', '34%', '45%']
+    assert formatter([0.12, 0.23, 0.34, 0.45]) == ["12%", "23%", "34%", "45%"]
 
-    assert formatter([.12, .23, .34, 4.5]) == \
-        ['12%', '23%', '34%', '450%']
+    assert formatter([0.12, 0.23, 0.34, 4.5]) == ["12%", "23%", "34%", "450%"]
 
     # mixed precision values
-    assert formatter([.12, .23, .34, 45]) == \
-        ['10%', '20%', '30%', '4500%']
+    assert formatter([0.12, 0.23, 0.34, 45]) == ["10%", "20%", "30%", "4500%"]
 
 
 def test_scientific():
     formatter = scientific_format(2)
-    assert formatter([.12, .2376, .34, 45]) == \
-        ['1.20e-01', '2.38e-01', '3.40e-01', '4.50e+01']
-
-    assert formatter([.12, 230, .34*10**5, .4]) == \
-        ['1.2e-01', '2.3e+02', '3.4e+04', '4.0e-01']
+    assert formatter([0.12, 0.2376, 0.34, 45]) == [
+        "1.20e-01",
+        "2.38e-01",
+        "3.40e-01",
+        "4.50e+01",
+    ]
+
+    assert formatter([0.12, 230, 0.34 * 10**5, 0.4]) == [
+        "1.2e-01",
+        "2.3e+02",
+        "3.4e+04",
+        "4.0e-01",
+    ]
 
 
 def test_mpl_format():
     formatter = mpl_format()
-    assert formatter([5, 10, 100, 150]) == ['5', '10', '100', '150']
+    assert formatter([5, 10, 100, 150]) == ["5", "10", "100", "150"]
 
     # trigger the order of magnitude correction (not any more)
-    assert formatter([5, 10, 100, 150e8]) == ['5', '10', '100', '15000000000']
+    assert formatter([5, 10, 100, 150e8]) == ["5", "10", "100", "15000000000"]
 
 
 def test_log_format():
     formatter = log_format()
-    assert formatter([0.001, 0.1, 100]) == ['0.001', '0.1', '100']
-    assert formatter([0.001, 0.1, 10000]) == ['1e-3', '1e-1', '1e4']
-    assert formatter([35, 60]) == ['35', '60']
-    assert formatter([34.99999999999, 60.0000000001]) == ['35', '60']
-    assert formatter([3000.0000000000014, 4999.999999999999]) == \
-        ['3000', '5000']
-    assert formatter([1, 35, 60, 1000]) == ['1', '35', '60', '1000']
-    assert formatter([1, 35, 60, 10000]) == ['1', '35', '60', '10000']
-    assert formatter([3.000000000000001e-05]) == ['3e-5']
-    assert formatter([1, 1e4]) == ['1', '1e4']
-    assert formatter([1, 35, 60, 1e6]) == ['1', '4e1', '6e1', '1e6']
+    assert formatter([0.001, 0.1, 100]) == ["0.001", "0.1", "100"]
+    assert formatter([0.001, 0.1, 10000]) == ["1e-3", "1e-1", "1e4"]
+    assert formatter([35, 60]) == ["35", "60"]
+    assert formatter([34.99999999999, 60.0000000001]) == ["35", "60"]
+    assert formatter([3000.0000000000014, 4999.999999999999]) == [
+        "3000",
+        "5000",
+    ]
+    assert formatter([1, 35, 60, 1000]) == ["1", "35", "60", "1000"]
+    assert formatter([1, 35, 60, 10000]) == ["1", "35", "60", "10000"]
+    assert formatter([3.000000000000001e-05]) == ["3e-5"]
+    assert formatter([1, 1e4]) == ["1", "1e4"]
+    assert formatter([1, 35, 60, 1e6]) == ["1", "4e1", "6e1", "1e6"]
 
     formatter = log_format(base=2)
-    assert formatter([1, 2, 4, 8]) == ['2^0', '2^1', '2^2', '2^3']
-    assert formatter([0b1, 0b10, 0b11]) == ['2^0', '2^1', '2^1.585']
+    assert formatter([1, 2, 4, 8]) == ["2^0", "2^1", "2^2", "2^3"]
+    assert formatter([0b1, 0b10, 0b11]) == ["2^0", "2^1", "2^1.585"]
 
     formatter = log_format(base=8)
-    assert formatter([1, 4, 8, 64]) == ['8^0', '8^0.667', '8^1', '8^2']
+    assert formatter([1, 4, 8, 64]) == ["8^0", "8^0.667", "8^1", "8^2"]
 
     formatter = log_format(base=5)
-    assert formatter([1, 5, 25, 125]) == ['5^0', '5^1', '5^2', '5^3']
+    assert formatter([1, 5, 25, 125]) == ["5^0", "5^1", "5^2", "5^3"]
 
     formatter = log_format(base=np.e)
-    assert formatter([1, np.pi, np.e**2, np.e**3]) == \
-        ['e^0', 'e^1.145', 'e^2', 'e^3']
+    assert formatter([1, np.pi, np.e**2, np.e**3]) == [
+        "e^0",
+        "e^1.145",
+        "e^2",
+        "e^3",
+    ]
 
     # mathtex
     formatter = log_format(mathtex=True)
-    assert formatter([0.001, 0.1, 10000]) == \
-        ['$10^{-3}$', '$10^{-1}$', '$10^{4}$']
-    assert formatter([35, 60]) == ['35', '60']
-    assert formatter([1, 10000]) == ['$10^{0}$', '$10^{4}$']
+    assert formatter([0.001, 0.1, 10000]) == [
+        "$10^{-3}$",
+        "$10^{-1}$",
+        "$10^{4}$",
+    ]
+    assert formatter([35, 60]) == ["35", "60"]
+    assert formatter([1, 10000]) == ["$10^{0}$", "$10^{4}$"]
 
     formatter = log_format(base=8, mathtex=True)
-    assert formatter([1, 4, 64]) == ['$8^{0}$', '$8^{0.667}$', '$8^{2}$']
+    assert formatter([1, 4, 64]) == ["$8^{0}$", "$8^{0.667}$", "$8^{2}$"]
 
 
 def test_date_format():
-    x = pd.date_range('1/1/2010', periods=4, freq='4AS')
-    result = date_format('%Y')(x)
-    assert result == ['2010', '2014', '2018', '2022']
-
-    x = [datetime(year=2005+i, month=i, day=i) for i in range(1, 5)]
-    result = date_format('%Y:%m:%d')(x)
-    assert result == \
-        ['2006:01:01', '2007:02:02', '2008:03:03', '2009:04:04']
+    x = pd.date_range("1/1/2010", periods=4, freq="4AS")
+    result = date_format("%Y")(x)
+    assert result == ["2010", "2014", "2018", "2022"]
+
+    x = [datetime(year=2005 + i, month=i, day=i) for i in range(1, 5)]
+    result = date_format("%Y:%m:%d")(x)
+    assert result == ["2006:01:01", "2007:02:02", "2008:03:03", "2009:04:04"]
 
     # Different timezones
-    PCT = ZoneInfo('US/Pacific')
-    UG = ZoneInfo('Africa/Kampala')
-    x = [datetime(2010, 1, 1, tzinfo=UG),
-         datetime(2010, 1, 1, tzinfo=PCT)]
+    PCT = ZoneInfo("US/Pacific")
+    UG = ZoneInfo("Africa/Kampala")
+    x = [datetime(2010, 1, 1, tzinfo=UG), datetime(2010, 1, 1, tzinfo=PCT)]
     with pytest.warns(UserWarning, match=r"different time zones"):
         date_format()(x)
 
 
 def test_timedelta_format():
-    x = [timedelta(days=7*i) for i in range(5)]
+    x = [timedelta(days=7 * i) for i in range(5)]
     labels = timedelta_format()(x)
-    assert labels == ['0', '1 week', '2 weeks', '3 weeks', '4 weeks']
+    assert labels == ["0", "1 week", "2 weeks", "3 weeks", "4 weeks"]
 
-    x = [pd.Timedelta(seconds=600*i) for i in range(5)]
+    x = [pd.Timedelta(seconds=600 * i) for i in range(5)]
     labels = timedelta_format()(x)
-    assert labels == \
-        ['0', '10 minutes', '20 minutes', '30 minutes', '40 minutes']
+    assert labels == [
+        "0",
+        "10 minutes",
+        "20 minutes",
+        "30 minutes",
+        "40 minutes",
+    ]
 
     # specific units
-    labels = timedelta_format(units='h')(x)
-    assert labels == \
-        ['0', '0.1667 hours', '0.3333 hours', '0.5000 hours',
-         '0.6667 hours']
+    labels = timedelta_format(units="h")(x)
+    assert labels == [
+        "0",
+        "0.1667 hours",
+        "0.3333 hours",
+        "0.5000 hours",
+        "0.6667 hours",
+    ]
     # usetex
-    x = [timedelta(microseconds=7*i) for i in range(5)]
-    labels = timedelta_format(units='us', usetex=True)(x)
-    assert labels == \
-        ['0', '7$\\mu s$', '14$\\mu s$', '21$\\mu s$', '28$\\mu s$']
+    x = [timedelta(microseconds=7 * i) for i in range(5)]
+    labels = timedelta_format(units="us", usetex=True)(x)
+    assert labels == [
+        "0",
+        "7$\\mu s$",
+        "14$\\mu s$",
+        "21$\\mu s$",
+        "28$\\mu s$",
+    ]
 
 
 def test_pvalue_format():
-    x = [.90, .15, .015, .009, 0.0005]
+    x = [0.90, 0.15, 0.015, 0.009, 0.0005]
     labels = pvalue_format()(x)
-    assert labels == ['0.9', '0.15', '0.015', '0.009', '<0.001']
+    assert labels == ["0.9", "0.15", "0.015", "0.009", "<0.001"]
 
     labels = pvalue_format(add_p=True)(x)
-    assert labels == ['p=0.9', 'p=0.15', 'p=0.015', 'p=0.009', 'p<0.001']
+    assert labels == ["p=0.9", "p=0.15", "p=0.015", "p=0.009", "p<0.001"]
 
     with warnings.catch_warnings(record=True) as record:
-        x = [.90, .15, np.nan, .015, .009, 0.0005]
+        x = [0.90, 0.15, np.nan, 0.015, 0.009, 0.0005]
         labels = pvalue_format()(x)
-        assert labels == ['0.9', '0.15', 'nan', '0.015', '0.009', '<0.001']
+        assert labels == ["0.9", "0.15", "nan", "0.015", "0.009", "<0.001"]
         assert not record, "Issued an unexpected warning"
 
     # NaN is handled without any warning
     assert len(record) == 0
 
 
 def test_ordinal_format():
     labels = ordinal_format()(range(110, 115))
-    assert labels == ['110th', '111th', '112th', '113th', '114th']
+    assert labels == ["110th", "111th", "112th", "113th", "114th"]
 
     labels = ordinal_format()(range(120, 125))
-    assert labels == ['120th', '121st', '122nd', '123rd', '124th']
+    assert labels == ["120th", "121st", "122nd", "123rd", "124th"]
 
-    labels = ordinal_format(big_mark=',')(range(1200, 1205))
-    assert labels == ['1,200th', '1,201st', '1,202nd', '1,203rd', '1,204th']
+    labels = ordinal_format(big_mark=",")(range(1200, 1205))
+    assert labels == ["1,200th", "1,201st", "1,202nd", "1,203rd", "1,204th"]
 
-    labels = ordinal_format(big_mark='.')(range(1200, 1205))
-    assert labels == ['1.200th', '1.201st', '1.202nd', '1.203rd', '1.204th']
+    labels = ordinal_format(big_mark=".")(range(1200, 1205))
+    assert labels == ["1.200th", "1.201st", "1.202nd", "1.203rd", "1.204th"]
 
 
 def test_number_bytes_format():
     x = [1000, 1000000, 4e5]
-    labels = number_bytes_format(symbol='MiB')(x)
-    assert labels == ['0 MiB', '1 MiB', '0 MiB']
+    labels = number_bytes_format(symbol="MiB")(x)
+    assert labels == ["0 MiB", "1 MiB", "0 MiB"]
 
-    labels = number_bytes_format(symbol='MiB', fmt='{:.2f} ')(x)
-    assert labels == ['0.00 MiB', '0.95 MiB', '0.38 MiB']
+    labels = number_bytes_format(symbol="MiB", fmt="{:.2f} ")(x)
+    assert labels == ["0.00 MiB", "0.95 MiB", "0.38 MiB"]
 
     with pytest.raises(ValueError):
-        number_bytes_format(symbol='Bad')(x)
+        number_bytes_format(symbol="Bad")(x)
 
 
 def test_empty_breaks():
     x = []
     assert custom_format()(x) == []
     assert comma_format()(x) == []
     assert currency_format()(x) == []
```

### Comparing `mizani-0.8.1/mizani/tests/test_palettes.py` & `mizani-0.9.0/mizani/tests/test_palettes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-import pytest
+import matplotlib as mpl
 import numpy as np
 import numpy.testing as npt
-import matplotlib as mpl
+import pytest
 
-from mizani.palettes import (hls_palette, husl_palette, rescale_pal,
-                             area_pal, abs_area, grey_pal, hue_pal,
-                             brewer_pal, gradient_n_pal, cmap_pal,
-                             cmap_d_pal,
-                             desaturate_pal, manual_pal, xkcd_palette,
-                             crayon_palette, cubehelix_pal, identity_pal)
-from mizani.palettes import ratios_to_colors
+from mizani.palettes import (
+    abs_area,
+    area_pal,
+    brewer_pal,
+    cmap_d_pal,
+    cmap_pal,
+    crayon_palette,
+    cubehelix_pal,
+    desaturate_pal,
+    gradient_n_pal,
+    grey_pal,
+    hls_palette,
+    hue_pal,
+    husl_palette,
+    identity_pal,
+    manual_pal,
+    ratios_to_colors,
+    rescale_pal,
+    xkcd_palette,
+)
 
 
 def test_hls_palette():
     colors = hls_palette(10)
     assert len(colors) == 10
     assert all(len(c) == 3 for c in colors)
 
@@ -22,189 +35,209 @@
     colors = husl_palette(5)
     assert len(colors) == 5
     assert all(len(c) == 3 for c in colors)
 
 
 def test_rescale_pal():
     palette = rescale_pal()
-    x = np.arange(0, 1+.01, 0.1)
+    x = np.arange(0, 1 + 0.01, 0.1)
     result = palette(x)
     assert min(result) == 0.1
     assert max(result) == 1
 
     palette = rescale_pal((20, 100))
     result = palette(x)
     assert min(result) == 20
     assert max(result) == 100
 
 
 def test_area_pal():
     palette = area_pal((0, 10))
     x = np.arange(0, 11)
-    xsq = (x * .1)**2
+    xsq = (x * 0.1) ** 2
     result = palette(xsq)
     npt.assert_allclose(result, x)
 
 
 def test_abs_area():
-    x = np.arange(0, 1.03, .1)**2
+    x = np.arange(0, 1.03, 0.1) ** 2
     palette = abs_area(5)
     result = palette(x)
     assert min(result) == 0
     assert max(result) == 5
 
 
 def test_grey_pal():
     palette = grey_pal()
     result = palette(5)
     # Same rgb values
-    assert all(s[1:3]*3 == s[1:] for s in result)
+    assert all(s[1:3] * 3 == s[1:] for s in result)
 
 
 def test_hue_pal():
     palette = hue_pal()
     result = palette(5)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
     # branches #
     with pytest.raises(ValueError):
-        hue_pal(.1, 2.3, 3)
+        hue_pal(0.1, 2.3, 3)
 
     with pytest.raises(ValueError):
-        hue_pal(color_space='slh')
+        hue_pal(color_space="slh")
 
 
 def test_brewer_pal():
     result = brewer_pal()(5)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
-    result = brewer_pal('qual', 2)(5)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    result = brewer_pal("qual", 2)(5)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
-    result = brewer_pal('div', 2)(5)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    result = brewer_pal("div", 2)(5)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
     with pytest.raises(ValueError):
-        brewer_pal('div', 200)(5)
+        brewer_pal("div", 200)(5)
 
-    result = brewer_pal('seq', 'Greens')(5)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    result = brewer_pal("seq", "Greens")(5)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
     with pytest.warns(UserWarning):
         brewer_pal()(100)
 
-    result = brewer_pal('seq', 'Blues')(2)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    result = brewer_pal("seq", "Blues")(2)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
-    result1 = brewer_pal('seq', 'Blues', direction=1)(2)
-    result2 = brewer_pal('seq', 'Blues', direction=-1)(2)
+    result1 = brewer_pal("seq", "Blues", direction=1)(2)
+    result2 = brewer_pal("seq", "Blues", direction=-1)(2)
     assert result1 == result2[::-1]
 
     with pytest.raises(ValueError):
         brewer_pal(direction=-2)(100)
 
 
+def test_brewer_palette_names():
+    from mizani.colors.brewer import get_palette_names
+
+    names = get_palette_names("sequential")
+    assert len(names) > 0
+
+    names = get_palette_names("qualitative")
+    assert len(names) > 0
+
+    names = get_palette_names("diverging")
+    assert len(names) > 0
+
+
+def test_brewer_palette_modules():
+    from mizani.colors.brewer import get_palette_module
+
+    with pytest.raises(ValueError):
+        get_palette_module("cyclic")
+
+
 def test_gradient_n_pal():
-    palette = gradient_n_pal(['red', 'blue'])
-    result = palette([0, .25, .5, .75, 1])
-    assert result[0].lower() == '#ff0000'
-    assert result[-1].lower() == '#0000ff'
-    assert palette([0])[0].lower() == '#ff0000'
+    palette = gradient_n_pal(["red", "blue"])
+    result = palette([0, 0.25, 0.5, 0.75, 1])
+    assert result[0].lower() == "#ff0000"
+    assert result[-1].lower() == "#0000ff"
+    assert palette([0])[0].lower() == "#ff0000"
 
     # symmetric gradient
-    palette = gradient_n_pal(['red', 'blue', 'red'], [0, 0.5, 1])
+    palette = gradient_n_pal(["red", "blue", "red"], [0, 0.5, 1])
     result = palette([0.2, 0.8])
     assert result[0] == result[1]
 
     # single color
-    result = palette(.25)
-    assert result.lower().startswith('#')
+    result = palette(0.25)
+    assert result.lower().startswith("#")
 
 
 def test_cmap_pal():
-    palette = cmap_pal('viridis')
-    result = palette([0, .25, .5, .75, 1])
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    palette = cmap_pal("viridis")
+    result = palette([0, 0.25, 0.5, 0.75, 1])
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
     with pytest.warns(FutureWarning):
-        cmap_pal('viridis', 5)
+        cmap_pal("viridis", 5)
 
 
 def test_cmap_d_pal():
-    palette = cmap_d_pal('viridis')
+    palette = cmap_d_pal("viridis")
     result = palette(6)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
     assert len(result) == 6
 
     # More colors than palette
-    palette = cmap_d_pal('Accent')
+    palette = cmap_d_pal("Accent")
     result = palette(5)
-    assert all(s[0] == '#' and len(s) == 7 for s in result)
+    assert all(s[0] == "#" and len(s) == 7 for s in result)
 
     with pytest.raises(ValueError):
         result = palette(10)
 
     # Bad palette
     with pytest.raises(ValueError):
-        palette = cmap_d_pal('Greens')
+        palette = cmap_d_pal("Greens")
 
     with pytest.warns(FutureWarning):
-        cmap_d_pal('viridis', 5)
+        cmap_d_pal("viridis", 5)
 
 
 def test_desaturate_pal():
-    x = [0, .25, .5, .75, 1]
+    x = [0, 0.25, 0.5, 0.75, 1]
     # When desaturating pure red, green and blue
     # the other 2 colors get matching values,
     # we test that.
-    result = desaturate_pal('red', .1)(x)
+    result = desaturate_pal("red", 0.1)(x)
     assert all(s[3:5] == s[5:] for s in result)
 
-    result = desaturate_pal('green', .2)(x)
+    result = desaturate_pal("green", 0.2)(x)
     assert all(s[1:3] == s[-2:] for s in result)
 
-    result = desaturate_pal('blue', .3)(x)
+    result = desaturate_pal("blue", 0.3)(x)
     assert all(s[1:3] == s[3:5] for s in result)
 
-    result = desaturate_pal('blue', .3, reverse=True)(x)
+    result = desaturate_pal("blue", 0.3, reverse=True)(x)
     assert all(s[1:3] == s[3:5] for s in result)
 
     with pytest.raises(ValueError):
-        desaturate_pal('green', 2.3)
+        desaturate_pal("green", 2.3)
 
 
 def test_manual_pal():
     size = 5
     n = 3
     values = list(range(size))
     palette = manual_pal(values)
     result = palette(n)
     assert result == values[:n]
 
     with pytest.warns(UserWarning):
-        result = palette(size+4)
+        result = palette(size + 4)
 
 
 def test_xkcd_palette():
-    values = xkcd_palette(['apple green', 'red', 'tan brown'])
+    values = xkcd_palette(["apple green", "red", "tan brown"])
     assert len(values) == 3
-    assert all(s[0] == '#' and len(s) == 7 for s in values)
+    assert all(s[0] == "#" and len(s) == 7 for s in values)
 
 
 def test_crayon_palette():
-    values = crayon_palette(['banana mania', 'red', 'yellow'])
+    values = crayon_palette(["banana mania", "red", "yellow"])
     assert len(values) == 3
-    assert all(s[0] == '#' and len(s) == 7 for s in values)
+    assert all(s[0] == "#" and len(s) == 7 for s in values)
 
 
 def test_cubehelix_pal():
     palette = cubehelix_pal()
     values = palette(5)
     assert len(values) == 5
-    assert all(s[0] == '#' and len(s) == 7 for s in values)
+    assert all(s[0] == "#" and len(s) == 7 for s in values)
 
 
 def test_identity_pal():
     palette = identity_pal()
 
     x = [1, 2, 3]
     values = palette(x)
@@ -212,9 +245,9 @@
 
     value = palette(10)
     assert value == 10
 
 
 def test_ratios_to_colors():
     x = 0.5
-    result = ratios_to_colors(x, mpl.colormaps['viridis'])
-    assert result[0] == '#'
+    result = ratios_to_colors(x, mpl.colormaps["viridis"])
+    assert result[0] == "#"
```

### Comparing `mizani-0.8.1/mizani/tests/test_scale.py` & `mizani-0.9.0/mizani/tests/test_scale.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,69 +8,68 @@
 from mizani.transforms import identity_trans
 
 
 def test_scale_continuous():
     x = np.arange(11)
     # apply
     scaled = scale_continuous.apply(x, rescale)
-    npt.assert_allclose(scaled, x*0.1)
-    npt.assert_allclose(scaled, x*0.1)
+    npt.assert_allclose(scaled, x * 0.1)
+    npt.assert_allclose(scaled, x * 0.1)
 
     # Train
     limits = scale_continuous.train(x)
     npt.assert_allclose(limits, [0, 10])
     # Additional training
     limits = scale_continuous.train(np.arange(-4, 11), limits)
     npt.assert_allclose(limits, [-4, 10])
     limits = scale_continuous.train([], limits)
     npt.assert_allclose(limits, [-4, 10])
 
     # branches #
-    scaled = scale_continuous.apply(x, rescale,
-                                    trans=identity_trans())
+    scaled = scale_continuous.apply(x, rescale, trans=identity_trans())
     mapped = scale_continuous.map(x, list, [0, 10])
-    npt.assert_allclose(mapped, x*0.1)
+    npt.assert_allclose(mapped, x * 0.1)
 
     with pytest.raises(TypeError):
         # discrete data
-        limits = scale_continuous.train(['a', 'b', 'c'])
+        limits = scale_continuous.train(["a", "b", "c"])
 
 
 def test_scale_discrete():
     def assert_equal_with_nan(lst1, lst2):
         assert lst1[:-1] == lst2[:-1] and np.isnan(lst2[-1])
 
     def SCategorical(*args, **kwargs):
         return pd.Series(pd.Categorical(*args, **kwargs))
 
-    x = ['a', 'b', 'c', 'a']
+    x = ["a", "b", "c", "a"]
     # apply
     scaled = scale_discrete.apply(x, np.arange)
     npt.assert_allclose(scaled, [0, 1, 2, 0])
 
     # Train
     limits = scale_discrete.train(x)
-    assert limits == ['a', 'b', 'c']
+    assert limits == ["a", "b", "c"]
 
     # Additional training
-    limits = scale_discrete.train(['b', 'c', 'd'], limits)
-    assert limits == ['a', 'b', 'c', 'd']
+    limits = scale_discrete.train(["b", "c", "d"], limits)
+    assert limits == ["a", "b", "c", "d"]
     limits = scale_discrete.train([], limits)
-    assert limits == ['a', 'b', 'c', 'd']
-    limits = scale_discrete.train([None, 'e'], limits)
-    assert_equal_with_nan(limits, ['a', 'b', 'c', 'd', 'e', np.nan])
+    assert limits == ["a", "b", "c", "d"]
+    limits = scale_discrete.train([None, "e"], limits)
+    assert_equal_with_nan(limits, ["a", "b", "c", "d", "e", np.nan])
 
     # Train (Deal with missing values)
-    x1 = ['a', 'b', np.nan, 'c']
+    x1 = ["a", "b", np.nan, "c"]
     x2 = pd.Categorical([1, 2, 3, np.nan])
     limits = scale_discrete.train(x1, na_rm=True)
-    assert limits == ['a', 'b', 'c']
+    assert limits == ["a", "b", "c"]
 
     limits = scale_discrete.train(x1, na_rm=False)
-    assert_equal_with_nan(limits, ['a', 'b', 'c', np.nan])
+    assert_equal_with_nan(limits, ["a", "b", "c", np.nan])
 
     limits = scale_discrete.train(x2, na_rm=True)
     assert limits == [1, 2, 3]
 
     limits = scale_discrete.train(x2, na_rm=False)
     assert_equal_with_nan(limits, [1, 2, 3, np.nan])
 
@@ -80,35 +79,35 @@
 
     # branches #
 
     with pytest.raises(TypeError):
         # continuous data
         limits = scale_discrete.train([1, 2, 3])
 
-    x = pd.Categorical(['a', 'b'])
+    x = pd.Categorical(["a", "b"])
     limits = scale_discrete.train(x)
-    assert limits == ['a', 'b']
+    assert limits == ["a", "b"]
 
-    x = pd.Series(['a', 'b', 'c'], dtype='category')
+    x = pd.Series(["a", "b", "c"], dtype="category")
     limits = scale_discrete.train(x[:1], drop=True)
-    assert limits == ['a']
+    assert limits == ["a"]
 
     limits = scale_discrete.train(x[:2], drop=False)
-    assert limits == ['a', 'b', 'c']
+    assert limits == ["a", "b", "c"]
 
     # Disrete Scale training maintains order of categoricals
-    cats = ['x0', 'x1', 'x2', 'x3', 'x4']
-    s1 = SCategorical(['x1', 'x2'], categories=cats)
-    s2 = SCategorical(['x0', 'x2'], categories=cats)
+    cats = ["x0", "x1", "x2", "x3", "x4"]
+    s1 = SCategorical(["x1", "x2"], categories=cats)
+    s2 = SCategorical(["x0", "x2"], categories=cats)
     limits = scale_discrete.train(s1, drop=True)
     limits = scale_discrete.train(s2, limits, drop=True)
-    assert limits == ['x0', 'x1', 'x2']
+    assert limits == ["x0", "x1", "x2"]
 
     # Trainning on mixed categories, the last data determines
     # the location of a value that is in two categoricals
     # eg. a & e are ordered right!
-    x1 = pd.Categorical(['a', 'b', 'c', 'e'])
-    x2 = pd.Categorical(['d', 'f', 'e', 'a'])
+    x1 = pd.Categorical(["a", "b", "c", "e"])
+    x2 = pd.Categorical(["d", "f", "e", "a"])
     limits = scale_discrete.train(x1)
     limits = scale_discrete.train(x2, old=limits)
     # assert limits == list('abcedf')
-    assert limits == list('adefbc')
+    assert limits == list("adefbc")
```

### Comparing `mizani-0.8.1/mizani/tests/test_transforms.py` & `mizani-0.9.0/mizani/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,82 +1,96 @@
-from types import FunctionType, MethodType
 from datetime import datetime, timedelta
+from types import FunctionType, MethodType
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     # python < 3.9
     from backports.zoneinfo import ZoneInfo
 
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pytest
 
-from mizani.breaks import mpl_breaks, minor_breaks
+from mizani.breaks import minor_breaks, mpl_breaks
 from mizani.transforms import (
-    trans,
-    asn_trans, atanh_trans, boxcox_trans, modulus_trans,
+    asn_trans,
+    atanh_trans,
+    boxcox_trans,
     datetime_trans,
-    exp_trans, identity_trans, log10_trans, log1p_trans,
-    log2_trans, log_trans, probability_trans, reverse_trans,
-    sqrt_trans, timedelta_trans, pd_timedelta_trans,
-    pseudo_log_trans, reciprocal_trans,
-    trans_new, gettrans)
+    exp_trans,
+    gettrans,
+    identity_trans,
+    log1p_trans,
+    log2_trans,
+    log10_trans,
+    log_trans,
+    modulus_trans,
+    pd_timedelta_trans,
+    probability_trans,
+    pseudo_log_trans,
+    reciprocal_trans,
+    reverse_trans,
+    sqrt_trans,
+    timedelta_trans,
+    trans,
+    trans_new,
+)
 
 arr = np.arange(1, 100)
 
 
 def test_trans():
     with pytest.raises(KeyError):
         trans(universe=True)
 
 
 def test_trans_new():
-    t = trans_new('bounded_identity',
-                  staticmethod(lambda x: x),
-                  classmethod(lambda x: x),
-                  _format=lambda x: str(x),
-                  domain=(-999, 999),
-                  doc='Bounded Identity transform')
+    t = trans_new(
+        "bounded_identity",
+        staticmethod(lambda x: x),
+        classmethod(lambda x: x),
+        _format=lambda x: str(x),
+        domain=(-999, 999),
+        doc="Bounded Identity transform",
+    )
 
-    assert t.__name__ == 'bounded_identity_trans'
+    assert t.__name__ == "bounded_identity_trans"
     assert isinstance(t.transform, FunctionType)
     assert isinstance(t.inverse, MethodType)
     assert isinstance(t.format, FunctionType)
     assert t.domain == (-999, 999)
-    assert t.__doc__ == 'Bounded Identity transform'
+    assert t.__doc__ == "Bounded Identity transform"
 
     # ticks do not go beyond the bounds
     major = t().breaks((-1999, 1999))
     assert min(major) >= -999
     assert max(major) <= 999
 
 
 def test_gettrans():
     t0 = identity_trans()
     t1 = gettrans(t0)
     t2 = gettrans(identity_trans)
-    t3 = gettrans('identity')
-    assert all(
-        isinstance(x, identity_trans) for x in (t0, t1, t2, t3))
+    t3 = gettrans("identity")
+    assert all(isinstance(x, identity_trans) for x in (t0, t1, t2, t3))
 
     t = gettrans(exp_trans)
-    assert t.__class__.__name__ == 'power_e_trans'
+    assert t.__class__.__name__ == "power_e_trans"
 
     with pytest.raises(ValueError):
         gettrans(object)
 
 
 def _test_trans(trans, x):
     t = gettrans(trans())
     xt = t.transform(x)
     x2 = t.inverse(xt)
-    is_log_trans = ('log' in t.__class__.__name__ and
-                    hasattr(t, 'base'))
+    is_log_trans = "log" in t.__class__.__name__ and hasattr(t, "base")
     # round trip
     npt.assert_allclose(x, x2)
     major = t.breaks([min(x), max(x)])
     minor = t.minor_breaks(t.transform(major))
     # Breaks and they are finite
     assert len(major)
     if is_log_trans and int(t.base) == 2:
@@ -90,23 +104,23 @@
     assert all(major >= t.domain[0])
     assert all(major <= t.domain[1])
     assert all(minor >= t.domain[0])
     assert all(minor <= t.domain[1])
 
 
 def test_asn_trans():
-    _test_trans(asn_trans, arr*0.01),
+    _test_trans(asn_trans, arr * 0.01),
 
 
 def test_atanh_trans():
-    _test_trans(atanh_trans, arr*0.001),
+    _test_trans(atanh_trans, arr * 0.001),
 
 
 def test_boxcox_trans():
-    _test_trans(boxcox_trans(0.5), arr*10)
+    _test_trans(boxcox_trans(0.5), arr * 10)
     _test_trans(boxcox_trans(1), arr)
     with pytest.raises(ValueError):
         x = np.arange(-4, 4)
         _test_trans(boxcox_trans(0.5), x)
 
     # Special case, small p and p = 0
     with pytest.warns(RuntimeWarning):
@@ -120,22 +134,22 @@
     xti = t.inverse(xt)
     assert np.isneginf(xt[0])
     npt.assert_array_almost_equal(x, xti)
 
 
 def test_modulus_trans():
     _test_trans(modulus_trans(0), arr)
-    _test_trans(modulus_trans(0.5), arr*10)
+    _test_trans(modulus_trans(0.5), arr * 10)
 
 
 def test_exp_trans():
     _test_trans(exp_trans, arr)
 
     exp2_trans = exp_trans(2)
-    _test_trans(exp2_trans, arr*0.1)
+    _test_trans(exp2_trans, arr * 0.1)
 
 
 def test_identity_trans():
     _test_trans(identity_trans, arr)
 
 
 def test_log10_trans():
@@ -162,105 +176,105 @@
     _test_trans(sqrt_trans, arr)
 
 
 def test_logn_trans():
     log3_trans = log_trans(3)
     _test_trans(log3_trans, arr)
 
-    log4_trans = log_trans(4, domain=(0.1, 100),
-                           breaks=mpl_breaks(),
-                           minor_breaks=minor_breaks())
+    log4_trans = log_trans(
+        4, domain=(0.1, 100), breaks=mpl_breaks(), minor_breaks=minor_breaks()
+    )
     _test_trans(log4_trans, arr)
 
 
 def test_reciprocal_trans():
     x = np.arange(10, 21)
     _test_trans(reciprocal_trans, x)
 
 
 def test_pseudo_log_trans():
     p = np.arange(-4, 4)
     pos = [10 ** int(x) for x in p]
     arr = np.hstack([-np.array(pos[::-1]), pos])
     _test_trans(pseudo_log_trans, arr)
     _test_trans(pseudo_log_trans(base=16), arr)
-    _test_trans(
-        pseudo_log_trans(base=10, minor_breaks=minor_breaks(n=5)),
-        arr
-    )
+    _test_trans(pseudo_log_trans(base=10, minor_breaks=minor_breaks(n=5)), arr)
 
 
 def test_probability_trans():
     with pytest.raises(ValueError):
-        t = probability_trans('unknown_distribution')
+        t = probability_trans("unknown_distribution")
 
     # cdf of the normal is centered at 0 and
     # The values either end of 0 are symmetric
     x = [-3, -2, -1, 0, 1, 2, 3]
-    t = probability_trans('norm')
+    t = probability_trans("norm")
     xt = t.transform(x)
     x2 = t.inverse(xt)
     assert xt[3] == 0.5
-    npt.assert_allclose(xt[:3], 1-xt[-3:][::-1])
+    npt.assert_allclose(xt[:3], 1 - xt[-3:][::-1])
     npt.assert_allclose(x, x2)
 
 
 def test_datetime_trans():
-    UTC = ZoneInfo('UTC')
+    UTC = ZoneInfo("UTC")
 
     x = [datetime(year, 1, 1, tzinfo=UTC) for year in [2010, 2015, 2020, 2026]]
     t = datetime_trans()
     xt = t.transform(x)
     x2 = t.inverse(xt)
     assert all(a == b for a, b in zip(x, x2))
 
     # numpy datetime64
-    x = [np.datetime64(i, 'D') for i in range(1, 11)]
+    x = [np.datetime64(i, "D") for i in range(1, 11)]
     t = datetime_trans()
     xt = t.transform(x)
     x2 = t.inverse(xt)
     assert all(isinstance(val, datetime) for val in x2)
 
     # pandas timestamp
-    x = pd.date_range(start='1/1/2022', end='1/2/2022', freq='3H', tz='EST')
+    x = pd.date_range(start="1/1/2022", end="1/2/2022", freq="3H", tz="EST")
     t = datetime_trans()
     xt = t.transform(x)
     x2 = t.inverse(xt)
     assert all(x == x2)
 
+    # Irregular index
+    s = pd.Series(x, index=range(11, len(x) + 11))
+    st = t.transform(s)
+    s2 = t.inverse(st)
+    assert all(s == s2)
+
     # Scalar
     x = datetime(2022, 1, 20, tzinfo=UTC)
     t = datetime_trans()
     xt = t.transform(x)
     x2 = t.inverse(xt)
     assert x == x2
 
 
 def test_datetime_trans_tz():
-    EST = ZoneInfo('EST')
-    UTC = ZoneInfo('UTC')
+    EST = ZoneInfo("EST")
+    UTC = ZoneInfo("UTC")
 
-    x = [
-        datetime(2022, 1, 1, 0 + 3 * i, 0, 0, tzinfo=EST)
-        for i in range(8)
-    ]
+    x = [datetime(2022, 1, 1, 0 + 3 * i, 0, 0, tzinfo=EST) for i in range(8)]
 
     # Same trans as data
     t = datetime_trans()
     x2 = t.inverse(t.transform(x))
     assert x == x2
     assert all(val.tzinfo == EST for val in x2)
 
     # UTC trans
     t = datetime_trans(UTC)
     x2 = t.inverse(t.transform(x))
     assert x == x2
     assert all(val.tzinfo == UTC for val in x2)
 
-    t = datetime_trans('MST')
+    t = datetime_trans("MST")
     assert t.tzinfo == t.tz
     assert t.transform([]) == []
 
 
 def test_timedelta_trans():
     x = [timedelta(days=i) for i in range(1, 11)]
     t = timedelta_trans()
```

### Comparing `mizani-0.8.1/mizani/tests/test_utils.py` & `mizani-0.9.0/mizani/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import numpy as np
 import pandas as pd
 import pytest
 
-
-from mizani.utils import (round_any, min_max, match, precision,
-                          first_element, multitype_sort,
-                          same_log10_order_of_magnitude, get_categories)
+from mizani.utils import (
+    first_element,
+    get_categories,
+    match,
+    min_max,
+    multitype_sort,
+    precision,
+    round_any,
+    same_log10_order_of_magnitude,
+)
 
 
 def test_round_any():
     x = 4.632
     assert round_any(x, 1) == 5
     assert round_any(x, 2) == 4
     assert round_any(x, 3) == 6
@@ -25,67 +31,67 @@
 
 def test_min_max():
     x = [1, 2, 3, 4, 5]
     _min, _max = min_max(x)
     assert _min == 1
     assert _max == 5
 
-    x = [1, float('-inf'), 3, 4, 5]
+    x = [1, float("-inf"), 3, 4, 5]
     _min, _max = min_max(x)
     assert _min == 1
     assert _max == 5
 
     _min, _max = min_max(x, finite=False)
-    assert _min == float('-inf')
+    assert _min == float("-inf")
     assert _max == 5
 
-    x = [1, 2, float('nan'), 4, 5]
+    x = [1, 2, float("nan"), 4, 5]
     _min, _max = min_max(x, na_rm=True)
     assert _min == 1
     assert _max == 5
 
-    x = [1, 2, float('nan'), 4, 5, float('inf')]
+    x = [1, 2, float("nan"), 4, 5, float("inf")]
     _min, _max = min_max(x, na_rm=True, finite=False)
     assert _min == 1
-    assert _max == float('inf')
+    assert _max == float("inf")
 
     _min, _max = min_max(x)
-    assert str(_min) == 'nan'
-    assert str(_max) == 'nan'
+    assert str(_min) == "nan"
+    assert str(_max) == "nan"
 
-    x = [float('nan'), float('nan'), float('nan')]
+    x = [float("nan"), float("nan"), float("nan")]
     _min, _max = min_max(x, na_rm=True)
-    assert _min == float('-inf')
-    assert _max == float('inf')
+    assert _min == float("-inf")
+    assert _max == float("inf")
 
 
 def test_match():
     v1 = [0, 1, 2, 3, 4, 5]
     v2 = [5, 4, 3, 2, 1, 0]
     result = match(v1, v2)
     assert result == v2
 
     # Positions of the first match
-    result = match(v1, v2+v2)
+    result = match(v1, v2 + v2)
     assert result == v2
 
     result = match(v1, v2, incomparables=[1, 2])
     assert result == [5, -1, -1, 2, 1, 0]
 
     result = match(v1, v2, start=1)
     assert result == [6, 5, 4, 3, 2, 1]
 
     v2 = [5, 99, 3, 2, 1, 0]
     result = match(v1, v2)
     assert result == [5, 4, 3, 2, -1, 0]
 
 
 def test_precision():
-    assert precision(0.0037) == .001
-    assert precision(0.5) == .1
+    assert precision(0.0037) == 0.001
+    assert precision(0.5) == 0.1
     assert precision(9) == 1
     assert precision(24) == 10
     assert precision(784) == 100
     assert precision([0, 0]) == 1
 
 
 def test_first_element():
@@ -103,24 +109,23 @@
         first_element([])
 
     with pytest.raises(RuntimeError):
         first_element(iter(x))
 
 
 def test_multitype_sort():
-    a = ['c', float('nan'), 1, 'b', 'a', 2.0, 0]
+    a = ["c", float("nan"), 1, "b", "a", 2.0, 0]
     result = multitype_sort(a)
     # Any consecutive elements of the sametype are
     # sorted
     for i, x in enumerate(result[1:], start=1):
-        x_prev = result[i-1]
-        if (type(x_prev) is type(x)):
+        x_prev = result[i - 1]
+        if type(x_prev) is type(x):
             # cannot compare nan with anything
-            if (isinstance(x, float) and
-                    (np.isnan(x_prev) or np.isnan(x))):
+            if isinstance(x, float) and (np.isnan(x_prev) or np.isnan(x)):
                 continue
             assert x_prev <= x
 
 
 def test_same_log10_order_of_magnitude():
     # Default delta
     assert same_log10_order_of_magnitude((2, 8))
@@ -138,15 +143,15 @@
     # delta = 0
     assert same_log10_order_of_magnitude((1, 9.9), delta=0)
     assert same_log10_order_of_magnitude((35, 91), delta=0)
     assert same_log10_order_of_magnitude((232.3, 950), delta=0)
 
 
 def test_get_categories():
-    lst = list('abcd')
+    lst = list("abcd")
     s = pd.Series(lst)
     c = pd.Categorical(lst)
     sc = pd.Series(c)
 
     categories = pd.Index(lst)
     assert categories.equals(get_categories(c))
     assert categories.equals(get_categories(sc))
```

### Comparing `mizani-0.8.1/mizani/transforms.py` & `mizani-0.9.0/mizani/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,48 +14,66 @@
 `Variable` and `scale` transformations are similar in-that they lead to
 plotted objects that are indistinguishable. Typically, *variable*
 transformation is done outside the graphics system and so the system
 cannot provide transformation specific guides & decorations for the
 plot. The :class:`trans` is aimed at being useful for *scale* and
 *coordinate* transformations.
 """
-import sys
 import datetime
+import sys
 from collections.abc import Iterable
 from types import MethodType
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     # python < 3.9
     from backports.zoneinfo import ZoneInfo
 
 import numpy as np
 import pandas as pd
-import scipy.stats as stats
 from matplotlib.dates import date2num, num2date
 
-from .breaks import (extended_breaks, log_breaks, minor_breaks,
-                     trans_minor_breaks, date_breaks,
-                     timedelta_breaks)
-from .formatters import mpl_format, date_format, timedelta_format
-from .formatters import log_format
-
-
-__all__ = ['asn_trans', 'atanh_trans', 'boxcox_trans',
-           'modulus_trans',
-           'datetime_trans', 'exp_trans', 'identity_trans',
-           'log10_trans', 'log1p_trans', 'log2_trans',
-           'log_trans', 'logit_trans', 'probability_trans',
-           'probit_trans', 'reverse_trans', 'sqrt_trans',
-           'timedelta_trans', 'pd_timedelta_trans',
-           'pseudo_log_trans', 'reciprocal_trans',
-           'trans', 'trans_new', 'gettrans']
+from .breaks import (
+    date_breaks,
+    extended_breaks,
+    log_breaks,
+    minor_breaks,
+    timedelta_breaks,
+    trans_minor_breaks,
+)
+from .formatters import date_format, log_format, mpl_format, timedelta_format
+
+__all__ = [
+    "asn_trans",
+    "atanh_trans",
+    "boxcox_trans",
+    "modulus_trans",
+    "datetime_trans",
+    "exp_trans",
+    "identity_trans",
+    "log10_trans",
+    "log1p_trans",
+    "log2_trans",
+    "log_trans",
+    "logit_trans",
+    "probability_trans",
+    "probit_trans",
+    "reverse_trans",
+    "sqrt_trans",
+    "timedelta_trans",
+    "pd_timedelta_trans",
+    "pseudo_log_trans",
+    "reciprocal_trans",
+    "trans",
+    "trans_new",
+    "gettrans",
+]
 
-UTC = ZoneInfo('UTC')
+UTC = ZoneInfo("UTC")
 
 
 class trans:
     """
     Base class for all transforms
 
     This class is used to transform data and also tell the
@@ -83,14 +101,15 @@
 
     Create a trans that returns 4 minor breaks
 
     >>> t = trans(minor_breaks=minor_breaks(4))
     >>> t.minor_breaks(major)
     array([0.2, 0.4, 0.6, 0.8, 1.2, 1.4, 1.6, 1.8])
     """
+
     #: Aesthetic that the transform works on
     aesthetic = None
 
     #: Whether the untransformed data is numerical
     dataspace_is_numerical = True
 
     #: Limits of the transformed data
@@ -106,24 +125,21 @@
     format = staticmethod(mpl_format())
 
     def __init__(self, **kwargs):
         for attr in kwargs:
             if hasattr(self, attr):
                 setattr(self, attr, kwargs[attr])
             else:
-                raise KeyError(
-                    "Unknown Parameter {!r}".format(attr))
+                raise KeyError("Unknown Parameter {!r}".format(attr))
 
         # Defaults
-        if (self.breaks_ is None and
-                'breaks_' not in kwargs):
+        if self.breaks_ is None and "breaks_" not in kwargs:
             self.breaks_ = extended_breaks(n=5)
 
-        if (self.minor_breaks is None and
-                'minor_breaks' not in kwargs):
+        if self.minor_breaks is None and "minor_breaks" not in kwargs:
             self.minor_breaks = minor_breaks(1)
 
     @staticmethod
     def transform(x):
         """
         Transform of x
         """
@@ -169,22 +185,31 @@
         vmin = np.max([self.domain[0], limits[0]])
         vmax = np.min([self.domain[1], limits[1]])
         breaks = np.asarray(self.breaks_([vmin, vmax]))
 
         # Some methods(mpl_breaks, extended_breaks) that
         # calculate breaks take the limits as guide posts and
         # not hard limits.
-        breaks = breaks.compress((breaks >= self.domain[0]) &
-                                 (breaks <= self.domain[1]))
+        breaks = breaks.compress(
+            (breaks >= self.domain[0]) & (breaks <= self.domain[1])
+        )
         return breaks
 
 
-def trans_new(name, transform, inverse, breaks=None,
-              minor_breaks=None, _format=None,
-              domain=(-np.inf, np.inf), doc='', **kwargs):
+def trans_new(
+    name,
+    transform,
+    inverse,
+    breaks=None,
+    minor_breaks=None,
+    _format=None,
+    domain=(-np.inf, np.inf),
+    doc="",
+    **kwargs,
+):
     """
     Create a transformation class object
 
     Parameters
     ----------
     name : str
         Name of the transformation
@@ -214,36 +239,39 @@
         in kwargs, then `t.base` would be a valied attribute.
 
     Returns
     -------
     out : trans
         Transform class
     """
+
     def _get(func):
         if isinstance(func, (classmethod, staticmethod, MethodType)):
             return func
         else:
             return staticmethod(func)
 
-    klass_name = '{}_trans'.format(name)
+    klass_name = "{}_trans".format(name)
 
-    d = {'transform': _get(transform),
-         'inverse': _get(inverse),
-         'domain': domain,
-         '__doc__': doc,
-         **kwargs}
+    d = {
+        "transform": _get(transform),
+        "inverse": _get(inverse),
+        "domain": domain,
+        "__doc__": doc,
+        **kwargs,
+    }
 
     if breaks:
-        d['breaks_'] = _get(breaks)
+        d["breaks_"] = _get(breaks)
 
     if minor_breaks:
-        d['minor_breaks'] = _get(minor_breaks)
+        d["minor_breaks"] = _get(minor_breaks)
 
     if _format:
-        d['format'] = _get(_format)
+        d["format"] = _get(_format)
 
     return type(klass_name, (trans,), d)
 
 
 def log_trans(base=None, **kwargs):
     """
     Create a log transform class for *base*
@@ -261,53 +289,53 @@
     Returns
     -------
     out : type
         Log transform class
     """
     # transform function
     if base is None:
-        name = 'log'
+        name = "log"
         base = np.exp(1)
         transform = np.log
     elif base == 10:
-        name = 'log10'
+        name = "log10"
         transform = np.log10
     elif base == 2:
-        name = 'log2'
+        name = "log2"
         transform = np.log2
     else:
-        name = 'log{}'.format(base)
+        name = "log{}".format(base)
 
         def transform(x):
-            return np.log(x)/np.log(base)
+            return np.log(x) / np.log(base)
 
     # inverse function
     def inverse(x):
         return np.power(base, x)
 
-    if 'domain' not in kwargs:
-        kwargs['domain'] = (sys.float_info.min, np.inf)
+    if "domain" not in kwargs:
+        kwargs["domain"] = (sys.float_info.min, np.inf)
 
-    if 'breaks' not in kwargs:
-        kwargs['breaks'] = log_breaks(base=base)
+    if "breaks" not in kwargs:
+        kwargs["breaks"] = log_breaks(base=base)
 
-    kwargs['base'] = base
-    kwargs['_format'] = log_format(base)
+    kwargs["base"] = base
+    kwargs["_format"] = log_format(base)
 
     _trans = trans_new(name, transform, inverse, **kwargs)
 
-    if 'minor_breaks' not in kwargs:
+    if "minor_breaks" not in kwargs:
         n = int(base) - 2
         _trans.minor_breaks = trans_minor_breaks(_trans, n=n)
 
     return _trans
 
 
-log10_trans = log_trans(10, doc='Log 10 Transformation')
-log2_trans = log_trans(2, doc='Log 2 Transformation')
+log10_trans = log_trans(10, doc="Log 10 Transformation")
+log2_trans = log_trans(2, doc="Log 2 Transformation")
 
 
 def exp_trans(base=None, **kwargs):
     """
     Create a exponential transform class for *base*
 
     This is inverse of the log transform.
@@ -324,80 +352,86 @@
     Returns
     -------
     out : type
         Exponential transform class
     """
     # default to e
     if base is None:
-        name = 'power_e'
+        name = "power_e"
         base = np.exp(1)
     else:
-        name = 'power_{}'.format(base)
+        name = "power_{}".format(base)
 
     # transform function
     def transform(x):
         return np.power(base, x)
 
     # inverse function
     def inverse(x):
-        return np.log(x)/np.log(base)
+        return np.log(x) / np.log(base)
 
-    kwargs['base'] = base
+    kwargs["base"] = base
     return trans_new(name, transform, inverse, **kwargs)
 
 
 class log1p_trans(trans):
     """
     Log plus one Transformation
     """
+
     transform = staticmethod(np.log1p)
     inverse = staticmethod(np.expm1)
 
 
 class identity_trans(trans):
     """
     Identity Transformation
     """
+
     pass
 
 
 class reverse_trans(trans):
     """
     Reverse Transformation
     """
+
     transform = staticmethod(np.negative)
     inverse = staticmethod(np.negative)
 
 
 class sqrt_trans(trans):
     """
     Square-root Transformation
     """
+
     transform = staticmethod(np.sqrt)
     inverse = staticmethod(np.square)
     domain = (0, np.inf)
 
 
 class asn_trans(trans):
     """
     Arc-sin square-root Transformation
     """
+
     @staticmethod
     def transform(x):
-        return 2*np.arcsin(np.sqrt(x))
+        return 2 * np.arcsin(np.sqrt(x))
 
     @staticmethod
     def inverse(x):
-        return np.sin(x/2)**2
+        return np.sin(x / 2) ** 2
 
 
 class atanh_trans(trans):
     """
     Arc-tangent Transformation
     """
+
     transform = staticmethod(np.arctanh)
     inverse = staticmethod(np.tanh)
 
 
 def boxcox_trans(p, offset=0, **kwargs):
     r"""
     Boxcox Transformation
@@ -437,38 +471,39 @@
       `<http://www.jstor.org/stable/2986305>`_
 
     See Also
     --------
     :func:`~mizani.transforms.modulus_trans`
 
     """
+
     def transform(x):
         x = np.asarray(x)
         if np.any((x + offset) < 0):
             raise ValueError(
                 "boxcox_trans must be given only positive values. "
                 "Consider using modulus_trans instead?"
             )
         if np.abs(p) < 1e-7:
             return np.log(x + offset)
         else:
-            return ((x + offset)**p - 1)/p
+            return ((x + offset) ** p - 1) / p
 
     def inverse(x):
         x = np.asarray(x)
         if np.abs(p) < 1e-7:
             return np.exp(x) - offset
         else:
-            return (x*p + 1) ** (1/p) - offset
+            return (x * p + 1) ** (1 / p) - offset
 
-    kwargs['p'] = p
-    kwargs['offset'] = offset
-    kwargs['name'] = kwargs.get('name', 'pow_{}'.format(p))
-    kwargs['transform'] = transform
-    kwargs['inverse'] = inverse
+    kwargs["p"] = p
+    kwargs["offset"] = offset
+    kwargs["name"] = kwargs.get("name", "pow_{}".format(p))
+    kwargs["transform"] = transform
+    kwargs["inverse"] = inverse
     return trans_new(**kwargs)
 
 
 def modulus_trans(p, offset=1, **kwargs):
     r"""
     Modulus Transformation
 
@@ -510,35 +545,38 @@
       `<http://www.jstor.org/stable/2986305>`_
 
     See Also
     --------
     :func:`~mizani.transforms.boxcox_trans`
     """
     if np.abs(p) < 1e-7:
+
         def transform(x):
             x = np.asarray(x)
             return np.sign(x) * np.log(np.abs(x) + offset)
 
         def inverse(x):
             x = np.asarray(x)
             return np.sign(x) * (np.exp(np.abs(x)) - offset)
+
     else:
+
         def transform(x):
             x = np.asarray(x)
-            return np.sign(x) * ((np.abs(x) + offset)**p - 1) / p
+            return np.sign(x) * ((np.abs(x) + offset) ** p - 1) / p
 
         def inverse(x):
             x = np.asarray(x)
-            return np.sign(x) * ((np.abs(x) * p + 1)**(1 / p) - offset)
+            return np.sign(x) * ((np.abs(x) * p + 1) ** (1 / p) - offset)
 
-    kwargs['p'] = p
-    kwargs['offset'] = offset
-    kwargs['name'] = kwargs.get('name', 'mt_pow_{}'.format(p))
-    kwargs['transform'] = transform
-    kwargs['inverse'] = inverse
+    kwargs["p"] = p
+    kwargs["offset"] = offset
+    kwargs["name"] = kwargs.get("name", "mt_pow_{}".format(p))
+    kwargs["transform"] = transform
+    kwargs["inverse"] = inverse
     return trans_new(**kwargs)
 
 
 def probability_trans(distribution, *args, **kwargs):
     """
     Probability Transformation
 
@@ -556,45 +594,46 @@
     Notes
     -----
     Make sure that the distribution is a good enough
     approximation for the data. When this is not the case,
     computations may run into errors. Absence of any errors
     does not imply that the distribution fits the data.
     """
-    cdists = {k for k in dir(stats)
-              if hasattr(getattr(stats, k), 'cdf')}
+    import scipy.stats as stats
+
+    cdists = {k for k in dir(stats) if hasattr(getattr(stats, k), "cdf")}
     if distribution not in cdists:
         msg = "Unknown distribution '{}'"
         raise ValueError(msg.format(distribution))
 
     try:
-        doc = kwargs.pop('_doc')
+        doc = kwargs.pop("_doc")
     except KeyError:
-        doc = ''
+        doc = ""
 
     try:
-        name = kwargs.pop('_name')
+        name = kwargs.pop("_name")
     except KeyError:
-        name = 'prob_{}'.format(distribution)
+        name = "prob_{}".format(distribution)
 
     def transform(x):
         return getattr(stats, distribution).cdf(x, *args, **kwargs)
 
     def inverse(x):
         return getattr(stats, distribution).ppf(x, *args, **kwargs)
 
-    return trans_new(name,
-                     transform, inverse, domain=(0, 1),
-                     doc=doc)
+    return trans_new(name, transform, inverse, domain=(0, 1), doc=doc)
 
 
-logit_trans = probability_trans('logistic', _name='logit',
-                                _doc='Logit Transformation')
-probit_trans = probability_trans('norm', _name='norm',
-                                 _doc='Probit Transformation')
+logit_trans = probability_trans(
+    "logistic", _name="logit", _doc="Logit Transformation"
+)
+probit_trans = probability_trans(
+    "norm", _name="norm", _doc="Probit Transformation"
+)
 
 
 class datetime_trans(trans):
     """
     Datetime Transformation
 
     Parameters
@@ -616,18 +655,19 @@
     >>> x.tzinfo == x2.tzinfo
     False
     >>> x.tzinfo.key
     'UTC'
     >>> x2.tzinfo.key
     'EST'
     """
+
     dataspace_is_numerical = False
     domain = (
         datetime.datetime(datetime.MINYEAR, 1, 1, tzinfo=UTC),
-        datetime.datetime(datetime.MAXYEAR, 12, 31, tzinfo=UTC)
+        datetime.datetime(datetime.MAXYEAR, 12, 31, tzinfo=UTC),
     )
     breaks_ = staticmethod(date_breaks())
     format = staticmethod(date_format())
     tz = None
 
     def __init__(self, tz=None, **kwargs):
         if isinstance(tz, str):
@@ -641,14 +681,16 @@
         Transform from date to a numerical format
         """
         if isinstance(x, Iterable) and not len(x):
             return []
 
         try:
             tz = x[0].tzinfo
+        except KeyError:
+            tz = x.iloc[0].tzinfo
         except TypeError:
             tz = x.tzinfo
         except AttributeError:
             tz = None
 
         if tz and self.tz is None:
             self.tz = tz
@@ -669,29 +711,30 @@
         return self.tz
 
 
 class timedelta_trans(trans):
     """
     Timedelta Transformation
     """
+
     dataspace_is_numerical = False
     domain = (datetime.timedelta.min, datetime.timedelta.max)
     breaks_ = staticmethod(timedelta_breaks())
     format = staticmethod(timedelta_format())
 
     @staticmethod
     def transform(x):
         """
         Transform from Timeddelta to numerical format
         """
         # microseconds
         try:
-            x = np.array([_x.total_seconds()*10**6 for _x in x])
+            x = np.array([_x.total_seconds() * 10**6 for _x in x])
         except TypeError:
-            x = x.total_seconds()*10**6
+            x = x.total_seconds() * 10**6
         return x
 
     @staticmethod
     def inverse(x):
         """
         Transform to Timedelta from numerical format
         """
@@ -702,14 +745,15 @@
         return x
 
 
 class pd_timedelta_trans(trans):
     """
     Pandas timedelta Transformation
     """
+
     dataspace_is_numerical = False
     domain = (pd.Timedelta.min, pd.Timedelta.max)
     breaks_ = staticmethod(timedelta_breaks())
     format = staticmethod(timedelta_format())
 
     @staticmethod
     def transform(x):
@@ -771,25 +815,25 @@
         the `transform` or `inverse`.
     """
     if base is None:
         base = np.exp(1)
 
     def transform(x):
         x = np.asarray(x)
-        return np.arcsinh(x/(2*sigma)) / np.log(base)
+        return np.arcsinh(x / (2 * sigma)) / np.log(base)
 
     def inverse(x):
         x = np.asarray(x)
         return 2 * sigma * np.sinh(x * np.log(base))
 
-    kwargs['base'] = base
-    kwargs['sigma'] = sigma
-    _trans = trans_new('pseudo_log', transform, inverse, **kwargs)
+    kwargs["base"] = base
+    kwargs["sigma"] = sigma
+    _trans = trans_new("pseudo_log", transform, inverse, **kwargs)
 
-    if 'minor_breaks' not in kwargs:
+    if "minor_breaks" not in kwargs:
         n = int(base) - 2
         _trans.minor_breaks = trans_minor_breaks(_trans, n=n)
 
     return _trans
 
 
 def gettrans(t):
@@ -804,15 +848,15 @@
     Returns
     -------
     out : trans
     """
     obj = t
     # Make sure trans object is instantiated
     if isinstance(obj, str):
-        name = '{}_trans'.format(obj)
+        name = "{}_trans".format(obj)
         obj = globals()[name]()
     if callable(obj):
         obj = obj()
     if isinstance(obj, type):
         obj = obj()
 
     if not isinstance(obj, trans):
```

### Comparing `mizani-0.8.1/mizani/utils.py` & `mizani-0.9.0/mizani/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,64 @@
-from itertools import chain
 from collections import OrderedDict, defaultdict
 from collections.abc import Iterator
+from itertools import chain
 
 import numpy as np
 
-__all__ = ['round_any', 'min_max', 'match',
-           'precision', 'first_element', 'multitype_sort',
-           'same_log10_order_of_magnitude',
-           'identity', 'get_categories'
-           ]
-
-DISCRETE_KINDS = 'ObUS'
-CONTINUOUS_KINDS = 'ifuc'
-
-SECONDS = OrderedDict([
-    ('ns', 1e-9),        # nanosecond
-    ('us', 1e-6),        # microsecond
-    ('ms', 1e-3),        # millisecond
-    ('s', 1),            # second
-    ('m', 60),           # month
-    ('h', 3600),         # hour
-    ('d', 24*3600),      # day
-    ('w', 7*24*3600),    # week
-    ('M', 31*24*3600),   # month
-    ('y', 365*24*3600),  # year
-])
-
-NANOSECONDS = OrderedDict([
-    ('ns', 1),             # nanosecond
-    ('us', 1e3),           # microsecond
-    ('ms', 1e6),           # millisecond
-    ('s', 1e9),            # second
-    ('m', 60e9),           # month
-    ('h', 3600e9),         # hour
-    ('d', 24*3600e9),      # day
-    ('w', 7*24*3600e9),    # week
-    ('M', 31*24*3600e9),   # month
-    ('y', 365*24*3600e9),  # year
-])
+__all__ = [
+    "round_any",
+    "min_max",
+    "match",
+    "precision",
+    "first_element",
+    "multitype_sort",
+    "same_log10_order_of_magnitude",
+    "identity",
+    "get_categories",
+]
+
+DISCRETE_KINDS = "ObUS"
+CONTINUOUS_KINDS = "ifuc"
+
+SECONDS = OrderedDict(
+    [
+        ("ns", 1e-9),  # nanosecond
+        ("us", 1e-6),  # microsecond
+        ("ms", 1e-3),  # millisecond
+        ("s", 1),  # second
+        ("m", 60),  # month
+        ("h", 3600),  # hour
+        ("d", 24 * 3600),  # day
+        ("w", 7 * 24 * 3600),  # week
+        ("M", 31 * 24 * 3600),  # month
+        ("y", 365 * 24 * 3600),  # year
+    ]
+)
+
+NANOSECONDS = OrderedDict(
+    [
+        ("ns", 1),  # nanosecond
+        ("us", 1e3),  # microsecond
+        ("ms", 1e6),  # millisecond
+        ("s", 1e9),  # second
+        ("m", 60e9),  # month
+        ("h", 3600e9),  # hour
+        ("d", 24 * 3600e9),  # day
+        ("w", 7 * 24 * 3600e9),  # week
+        ("M", 31 * 24 * 3600e9),  # month
+        ("y", 365 * 24 * 3600e9),  # year
+    ]
+)
 
 
 def round_any(x, accuracy, f=np.round):
     """
     Round to multiple of any number.
     """
-    if not hasattr(x, 'dtype'):
+    if not hasattr(x, "dtype"):
         x = np.asarray(x)
 
     return f(x / accuracy) * accuracy
 
 
 def min_max(x, na_rm=False, finite=True):
     """
@@ -64,30 +74,30 @@
         Whether to consider only finite values.
 
     Returns
     -------
     out : tuple
         (minimum, maximum) of x
     """
-    if not hasattr(x, 'dtype'):
+    if not hasattr(x, "dtype"):
         x = np.asarray(x)
 
     if na_rm and finite:
         x = x[np.isfinite(x)]
     elif not na_rm and np.any(np.isnan(x)):
         return np.nan, np.nan
     elif na_rm:
         x = x[~np.isnan(x)]
     elif finite:
         x = x[~np.isinf(x)]
 
-    if (len(x)):
+    if len(x):
         return np.min(x), np.max(x)
     else:
-        return float('-inf'), float('inf')
+        return float("-inf"), float("inf")
 
 
 def match(v1, v2, nomatch=-1, incomparables=None, start=0):
     """
     Return a vector of the positions of (first)
     matches of its first argument in its second.
 
@@ -182,16 +192,15 @@
     Returns
     -------
     out : object
         First element of `obj`. Raise a class:`StopIteration`
         exception if `obj` is empty.
     """
     if isinstance(obj, Iterator):
-        raise RuntimeError(
-            "Cannot get the first element of an iterator")
+        raise RuntimeError("Cannot get the first element of an iterator")
     return next(iter(obj))
 
 
 def multitype_sort(a):
     """
     Sort elements of multiple types
 
@@ -210,15 +219,15 @@
     """
     types = defaultdict(list)
     numbers = {int, float, complex}
 
     for x in a:
         t = type(x)
         if t in numbers:
-            types['number'].append(x)
+            types["number"].append(x)
         else:
             types[t].append(x)
 
     for t in types:
         types[t] = np.sort(types[t])
 
     return list(chain.from_iterable(types[t] for t in types))
@@ -238,16 +247,16 @@
     ----------
     x : array-like
          Values in base 10. Must be size 2 and
         ``rng[0] <= rng[1]``.
     delta : float
         Fuzz factor for approximation. It is multiplicative.
     """
-    dmin = np.log10(np.min(x)*(1-delta))
-    dmax = np.log10(np.max(x)*(1+delta))
+    dmin = np.log10(np.min(x) * (1 - delta))
+    dmax = np.log10(np.max(x) * (1 + delta))
     return np.floor(dmin) == np.floor(dmax)
 
 
 def identity(*args):
     """
     Return whatever is passed in
     """
@@ -268,10 +277,38 @@
     out : Index
         Categories of x
     """
     try:
         return x.cat.categories  # series
     except AttributeError:
         try:
-            return x.categories   # plain categorical
+            return x.categories  # plain categorical
         except AttributeError:
             raise TypeError("x is the wrong type, it has no categories")
+
+
+def log(x, base):
+    """
+    Calculate the log of x
+
+    Parameters
+    ----------
+    x : category_like
+        Input Values
+
+    base : float
+        Base of logarithm
+
+    Returns
+    -------
+    out : float
+        Log of x
+    """
+    if base == 10:
+        res = np.log10(x)
+    elif base == 2:
+        res = np.log2(x)
+    elif base == np.e:
+        res = np.log(x)
+    else:
+        res = np.log(x) / np.log(base)
+    return res
```

### Comparing `mizani-0.8.1/mizani.egg-info/SOURCES.txt` & `mizani-0.9.0/mizani.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 .gitattributes
 .gitignore
-.readthedocs.yml
+.pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
-MANIFEST.in
 Makefile
-README.rst
+README.md
 codecov.yml
 how-to-release.rst
 pyproject.toml
-pytest.ini
-setup.cfg
-setup.py
 .github/workflows/testing.yml
 doc/Makefile
 doc/bounds.rst
 doc/breaks.rst
 doc/changelog.rst
 doc/conf.py
 doc/docutils.conf
@@ -54,30 +51,34 @@
 mizani/__init__.py
 mizani/bounds.py
 mizani/breaks.py
 mizani/formatters.py
 mizani/palettes.py
 mizani/scale.py
 mizani/transforms.py
+mizani/typing.py
 mizani/utils.py
 mizani.egg-info/PKG-INFO
 mizani.egg-info/SOURCES.txt
 mizani.egg-info/dependency_links.txt
-mizani.egg-info/not-zip-safe
 mizani.egg-info/requires.txt
 mizani.egg-info/top_level.txt
+mizani/colors/__init__.py
+mizani/colors/color_palette.py
+mizani/colors/brewer/__init__.py
+mizani/colors/brewer/diverging.py
+mizani/colors/brewer/qualitative.py
+mizani/colors/brewer/sequential.py
 mizani/external/__init__.py
 mizani/external/crayon_rgb.py
 mizani/external/husl.py
 mizani/external/xkcd_rgb.py
 mizani/tests/__init__.py
 mizani/tests/test_bounds.py
 mizani/tests/test_breaks.py
 mizani/tests/test_formatters.py
 mizani/tests/test_palettes.py
 mizani/tests/test_scale.py
 mizani/tests/test_transforms.py
 mizani/tests/test_utils.py
-requirements/dev.txt
-requirements/rtd.txt
 tools/build_theme.sh
 tools/release.sh
```

### Comparing `mizani-0.8.1/tools/build_theme.sh` & `mizani-0.9.0/tools/build_theme.sh`

 * *Files identical despite different names*

### Comparing `mizani-0.8.1/tools/release.sh` & `mizani-0.9.0/tools/release.sh`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 VERSION=$(echo $describe | grep "^v${release_re}${pre_re}$")
 
 # Partial recognition of a nice version, and maybe more stuff
 # This may give us the previous version.
 PREVIOUS_VERSION=$(echo $describe | grep "^v${release_re}${pre_re}")
 
 if [[ $VERSION ]];  then
-   python setup.py sdist bdist_wheel
+   make dist
    twine upload dist/*
 
 elif [[ $PREVIOUS_VERSION ]]; then
   last_release=$(echo $PREVIOUS_VERSION | tr -d v)
   major_minor=$(echo $last_release | grep -o '^[0-9]\+\.[0-9]\+')
   major=$(echo $last_release | grep -o '^[0-9]\+')
   minor=$(echo $major_minor | grep -o '[0-9]\+$')
```

