# Comparing `tmp/sharrow-2.5.2.tar.gz` & `tmp/sharrow-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharrow-2.5.2.tar", last modified: Fri Jan 13 04:14:02 2023, max compression
+gzip compressed data, was "sharrow-2.6.0.tar", last modified: Sat Apr 15 19:59:00 2023, max compression
```

## Comparing `sharrow-2.5.2.tar` & `sharrow-2.6.0.tar`

### file list

```diff
@@ -1,790 +1,798 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.135922 sharrow-2.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.067922 sharrow-2.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-01-13 04:11:02.000000 sharrow-2.5.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-01-13 04:11:02.000000 sharrow-2.5.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-13 04:11:02.000000 sharrow-2.5.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-13 04:11:02.000000 sharrow-2.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-13 04:11:02.000000 sharrow-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-13 04:14:02.135922 sharrow-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-13 04:11:02.000000 sharrow-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/docs/_script/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_script/hide_test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_script/run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_script/update_version_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_static/ampo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_static/sharrow-docs.css
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/docs/walkthrough/
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/walkthrough/encoding.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/walkthrough/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    45293 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/walkthrough/one-dim.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/walkthrough/sparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28352 2023-01-13 04:11:02.000000 sharrow-2.5.2/docs/walkthrough/two-dim.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.079922 sharrow-2.5.2/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-01-13 04:11:02.000000 sharrow-2.5.2/envs/development.yml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-13 04:11:02.000000 sharrow-2.5.2/envs/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-13 04:11:02.000000 sharrow-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-13 04:14:02.135922 sharrow-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-13 04:11:02.000000 sharrow-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.083922 sharrow-2.5.2/sharrow/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/_infer_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-13 04:14:01.000000 sharrow-2.5.2/sharrow/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/accessors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39718 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/aster.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40567 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/digital_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.083922 sharrow-2.5.2/sharrow/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)   106776 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/households.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/land_use.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/maz_to_maz_walk.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/maz_to_taz.csv
--rw-r--r--   0 runner    (1001) docker     (123)    84654 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/persons.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)  3674745 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.omx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DIST/0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTBIKE/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTBIKE/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTBIKE/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTBIKE/0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTWALK/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTWALK/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTWALK/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTWALK/0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.087922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.091922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.095922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.099922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_TIME/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_TIME/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_DIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_TIME/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.103922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.107922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.111922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.115922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.119922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.123922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.127922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/dtaz/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/dtaz/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/dtaz/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/dtaz/0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/otaz/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/otaz/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/otaz/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/otaz/0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/example_data/skims.zarr/time_period/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/time_period/.zarray
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/time_period/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data/skims.zarr/time_period/0
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/example_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/filewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)   109654 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/nested_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/omx.py
--rw-r--r--   0 runner    (1001) docker     (123)    53320 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.131922 sharrow-2.5.2/sharrow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_nesting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.135922 sharrow-2.5.2/sharrow/tests/test_relationships/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_dict_encoded.csv
--rw-r--r--   0 runner    (1001) docker     (123)   375022 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_get.csv
--rw-r--r--   0 runner    (1001) docker     (123)    80926 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_isin.csv
--rw-r--r--   0 runner    (1001) docker     (123)   138552 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_isin_and_between.csv
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_joint_dict_encoded.csv
--rw-r--r--   0 runner    (1001) docker     (123)   213333 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_mixed_dtypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185444 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_nested_where.csv
--rw-r--r--   0 runner    (1001) docker     (123)   243898 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_shared_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)   240111 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_shared_data_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)   335532 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_shared_data_reversible.csv
--rw-r--r--   0 runner    (1001) docker     (123)   141376 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_tuple_slice.csv
--rw-r--r--   0 runner    (1001) docker     (123)   164893 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships/test_with_2d_base.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33431 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/tests/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-01-13 04:11:02.000000 sharrow-2.5.2/sharrow/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:14:02.083922 sharrow-2.5.2/sharrow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-13 04:14:01.000000 sharrow-2.5.2/sharrow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-01-13 04:14:02.000000 sharrow-2.5.2/sharrow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 04:14:01.000000 sharrow-2.5.2/sharrow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 04:13:45.000000 sharrow-2.5.2/sharrow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-13 04:14:01.000000 sharrow-2.5.2/sharrow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-13 04:14:01.000000 sharrow-2.5.2/sharrow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.643788 sharrow-2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.543786 sharrow-2.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.555786 sharrow-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-15 19:55:58.000000 sharrow-2.6.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-15 19:55:58.000000 sharrow-2.6.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.555786 sharrow-2.6.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 19:55:58.000000 sharrow-2.6.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-15 19:55:58.000000 sharrow-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-15 19:55:58.000000 sharrow-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-15 19:59:00.643788 sharrow-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 19:55:58.000000 sharrow-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.559786 sharrow-2.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.563786 sharrow-2.6.0/docs/_script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_script/hide_test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_script/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_script/update_version_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.563786 sharrow-2.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_static/ampo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_static/sharrow-docs.css
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.567786 sharrow-2.6.0/docs/walkthrough/
+-rw-r--r--   0 runner    (1001) docker     (123)    25859 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/walkthrough/encoding.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/walkthrough/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    45293 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/walkthrough/one-dim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/walkthrough/sparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28292 2023-04-15 19:55:58.000000 sharrow-2.6.0/docs/walkthrough/two-dim.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.567786 sharrow-2.6.0/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-15 19:55:58.000000 sharrow-2.6.0/envs/development.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:58.000000 sharrow-2.6.0/envs/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-15 19:55:58.000000 sharrow-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-15 19:59:00.643788 sharrow-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-15 19:55:58.000000 sharrow-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.575786 sharrow-2.6.0/sharrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/_infer_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 19:59:00.000000 sharrow-2.6.0/sharrow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/accessors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39023 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/aster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/categorical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48101 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/digital_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.579787 sharrow-2.6.0/sharrow/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   106776 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/example_data/households.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/example_data/land_use.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/example_data/maz_to_maz_walk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/example_data/maz_to_taz.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    84654 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/example_data/persons.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  3674745 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.omx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.583787 sharrow-2.6.0/sharrow/example_data/skims.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.583787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DIST/0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.583787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTBIKE/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTBIKE/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTBIKE/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTBIKE/0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.583787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTWALK/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTWALK/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTWALK/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTWALK/0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.583787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.583787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.587787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.591787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.595787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.599787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_TIME/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_TIME/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.603787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_TIME/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_DIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_TIME/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.607787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.611787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.615787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.619787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.623787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.627787 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.631788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/dtaz/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/dtaz/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/dtaz/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/dtaz/0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.635788 sharrow-2.6.0/sharrow/example_data/skims.zarr/otaz/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/otaz/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/otaz/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/otaz/0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.639788 sharrow-2.6.0/sharrow/example_data/skims.zarr/time_period/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/time_period/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/time_period/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/example_data/skims.zarr/time_period/0
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-15 19:55:58.000000 sharrow-2.6.0/sharrow/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/filewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111823 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/nested_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/omx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57403 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.639788 sharrow-2.6.0/sharrow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_nesting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.643788 sharrow-2.6.0/sharrow/tests/test_relationships/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_dict_encoded.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   375022 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_get.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    80926 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_isin.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   138552 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_isin_and_between.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_joint_dict_encoded.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   213333 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_mixed_dtypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   185444 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_nested_where.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   243898 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_shared_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   240111 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_shared_data_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   335532 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_shared_data_reversible.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   141376 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_tuple_slice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   164893 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships/test_with_2d_base.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33448 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/tests/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.643788 sharrow-2.6.0/sharrow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/utils/tar_zst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-15 19:55:59.000000 sharrow-2.6.0/sharrow/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:59:00.575786 sharrow-2.6.0/sharrow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-15 19:59:00.000000 sharrow-2.6.0/sharrow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31648 2023-04-15 19:59:00.000000 sharrow-2.6.0/sharrow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:59:00.000000 sharrow-2.6.0/sharrow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:58:43.000000 sharrow-2.6.0/sharrow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-15 19:59:00.000000 sharrow-2.6.0/sharrow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 19:59:00.000000 sharrow-2.6.0/sharrow.egg-info/top_level.txt
```

### Comparing `sharrow-2.5.2/.github/workflows/run-tests.yml` & `sharrow-2.6.0/.github/workflows/run-tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -42,20 +42,20 @@
       - name: Install sharrow
         run: |
           python -m pip install -e .
       - name: Conda checkup
         run: |
           conda info -a
           conda list
-      - name: Lint with flake8
+      - name: Lint with Ruff
         run: |
           # stop the build if there are Python syntax errors or undefined names
-          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+          ruff check . --select=E9,F63,F7,F82 --statistics
+          # exit-zero treats all errors as warnings.
+          ruff check . --exit-zero --statistics
       - name: Test with pytest
         run: |
           python -m pytest
 
   deploy-docs:
     needs: test
     # only on pushes tagged with v...
```

### Comparing `sharrow-2.5.2/.gitignore` & `sharrow-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/.pre-commit-config.yaml` & `sharrow-2.6.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -9,22 +9,23 @@
   - id: trailing-whitespace
 
 - repo: https://github.com/kynan/nbstripout
   rev: 0.6.1
   hooks:
     - id: nbstripout
 
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.257
+  hooks:
+    - id: ruff
+      args: [--fix, --exit-non-zero-on-fix]
+
 - repo: https://github.com/pycqa/isort
   rev: 5.10.1
   hooks:
   - id: isort
     args: ["--profile", "black", "--filter-files"]
 
 - repo: https://github.com/psf/black
   rev: 22.10.0
   hooks:
     - id: black
-
-- repo: https://github.com/PyCQA/flake8
-  rev: 5.0.4
-  hooks:
-    - id: flake8
```

### Comparing `sharrow-2.5.2/LICENSE` & `sharrow-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/_config.yml` & `sharrow-2.6.0/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/_script/hide_test_cells.py` & `sharrow-2.6.0/docs/_script/hide_test_cells.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 notebooks = glob(
     os.path.join(os.path.dirname(__file__), "..", "**", "*.ipynb"),
     recursive=True,
 )
 
 # Text to look for in adding tags
 text_search_dict = {
-    "# TEST": "remove_cell",  # Remove the whole cell
-    "# HIDDEN": "remove_cell",  # Remove the whole cell
-    "# NO CODE": "remove_input",  # Remove only the input
-    "# HIDE CODE": "hide_input",  # Hide the input w/ a button to show
+    "# TEST": "remove-cell",  # Remove the whole cell
+    "# HIDDEN": "remove-cell",  # Remove the whole cell
+    "# NO CODE": "remove-input",  # Remove only the input
+    "# HIDE CODE": "hide-input",  # Hide the input w/ a button to show
 }
 
 # Search through each notebook and look for th text, add a tag if necessary
 for ipath in notebooks:
     if "/_build/" in ipath:
         continue
     touch = False
```

### Comparing `sharrow-2.5.2/docs/_static/ampo.png` & `sharrow-2.6.0/docs/_static/ampo.png`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/_static/favicon.png` & `sharrow-2.6.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/api.rst` & `sharrow-2.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/index.md` & `sharrow-2.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/intro.md` & `sharrow-2.6.0/docs/intro.md`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/logo.png` & `sharrow-2.6.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/walkthrough/encoding.ipynb` & `sharrow-2.6.0/docs/walkthrough/encoding.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9690247252747253%*

 * *Differences: {"'cells'": "{1: {'metadata': {'tags': ['remove-cell']}}, 2: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}}, 16: {'metadata': {'tags': ['remove-cell']}}, 23: "*

 * *            "{'metadata': {'tags': ['remove-cell']}}, 28: {'metadata': {'tags': ['remove-cell']}}, "*

 * *            "36: {'metadata': {'tags': ['remove-cell']}}, 39: {'metadata': {'tags': "*

 * *            "['remove-cell']}}, insert: [(50, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'cb219dc3-dd66-44cd-a7c5-2a1da4bc146 […]*

```diff
@@ -12,29 +12,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f17c8818",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# HIDDEN\n",
                 "import warnings\n",
                 "warnings.filterwarnings(\"ignore\", category=DeprecationWarning) "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d4e7246c",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import xarray as xr\n",
                 "from io import StringIO\n",
                 "\n",
@@ -213,15 +215,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ad591bb",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST encoding\n",
                 "assert distance_encoded.dtype == np.int16\n",
                 "np.testing.assert_array_equal(\n",
@@ -292,15 +294,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bd549b5e",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert skims_encoded.digital_encoding.info() == {\n",
                 " 'DIST': {'scale': 0.01, 'offset': 0, 'missing_value': None},\n",
@@ -373,15 +375,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7d74e53e",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "np.testing.assert_array_almost_equal(arr, arr_enc)"
             ]
@@ -473,15 +475,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a016d30f",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST encoding\n",
                 "assert wlwfare_enc.dtype == np.uint8\n",
                 "np.testing.assert_array_equal(\n",
@@ -521,15 +523,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "28afb335",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "xr.testing.assert_equal(array_decode(wlwfare_enc), skims.WLK_LOC_WLK_FAR)"
             ]
@@ -686,14 +688,203 @@
                 "# TEST\n",
                 "assert skims1.digital_encoding.baggage(['WLK_LOC_WLK_FAR']) == {'joined_0_offsets'}\n",
                 "assert (skims1.iat(\n",
                 "    otaz=[0,1,2], dtaz=[0,0,0], time_period=[1,1,1],\n",
                 "    _name='WLK_LOC_WLK_FAR'\n",
                 ").to_series() == [0,152,474]).all()"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "cb219dc3-dd66-44cd-a7c5-2a1da4bc1467",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Pandas Categorical Dtype\n",
+                "\n",
+                "Dictionary encoding is very similar to the approach used for the pandas Categorical dtype, and\n",
+                "can be used to achieve some of the efficiencies of categorical data, even though xarray lacks\n",
+                "a formal native categorical data representation.  Sharrow's `construct` function for creating\n",
+                "Dataset objects will automatically use dictionary encoding for \"category\" data. \n",
+                "\n",
+                "To demonstrate, we'll load some household data and create a categorical data column."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3b765919-69a4-4fb0-b805-9d3b5fed7897",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "hh = sh.example_data.get_households()\n",
+                "hh[\"income_grp\"] = pd.cut(hh.income, bins=[-np.inf,30000,60000,np.inf], labels=['Low', \"Mid\", \"High\"])\n",
+                "hh = hh[[\"income\",\"income_grp\"]]\n",
+                "hh.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "312faa0b-13cf-4649-9835-7a53b5e81a0b",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "hh.info()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "c51a88d2-02b1-4502-9f4b-271fbb126699",
+            "metadata": {},
+            "source": [
+                "We'll then create a Dataset using construct."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cd1c2fd5-59c6-48cb-bd6e-d2f9dde2aa36",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "hh_dataset = sh.dataset.construct(hh[[\"income\",\"income_grp\"]])\n",
+                "hh_dataset"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "033b3629-a16b-47a4-bb18-10af9c7c4f07",
+            "metadata": {},
+            "source": [
+                "Note that the \"income\" variable remains an integer as expected, but the \"income_grp\" variable, \n",
+                "which had been a \"category\" dtype in pandas, is now stored as an `int8`, giving the \n",
+                "category _index_ of each element (it would be an `int16` or larger if needed, but that's\n",
+                "not necessary with only 3 categories). The information about the labels for the categories is \n",
+                "retained not in the data itself but in the `digital_encoding`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "369442af-1c69-41eb-b530-ea398d6eac7a",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "hh_dataset[\"income_grp\"].digital_encoding"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "58db6505-1c90-475e-8d91-0e2e89ec0f0e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# TESTING\n",
+                "assert hh_dataset[\"income_grp\"].dtype == \"int8\"\n",
+                "assert hh_dataset[\"income_grp\"].digital_encoding.keys() == {'dictionary', 'ordered'}\n",
+                "assert all(hh_dataset[\"income_grp\"].digital_encoding['dictionary'] == np.array(['Low', 'Mid', 'High'], dtype='<U4'))\n",
+                "assert hh_dataset[\"income_grp\"].digital_encoding['ordered'] is True"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "38f8a6c9-4bca-4e73-82b0-e0996814565a",
+            "metadata": {},
+            "source": [
+                "If you try to make the return trip to a pandas DataFrame using the regular \n",
+                "`xarray.Dataset.to_pandas()` method, the details of the categorical nature\n",
+                "of this variable are lost, and only the int8 index is available."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ad2f8677-b02c-4d28-892f-3272804bf714",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "hh_dataset.to_pandas()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "95f26992-241f-4982-aa56-f1055a35f969",
+            "metadata": {},
+            "source": [
+                "But, if you use the `single_dim` accessor on the dataset provided by sharrow,\n",
+                "the categorical dtype is restored correctly."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "43b94637-c025-4578-9e97-4b6484cb231e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "hh_dataset.single_dim.to_pandas()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b1b86a4b-c19f-4ae9-8a8b-395f53209bc6",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# TESTING\n",
+                "pd.testing.assert_frame_equal(\n",
+                "    hh_dataset.single_dim.to_pandas(),\n",
+                "    hh\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "5e66c294-747d-414c-8e03-b8b551a0e2a9",
+            "metadata": {},
+            "source": [
+                "Note that this automatic handling of categorical data only applies when constructing\n",
+                "or deconstructing a dataset with a single dimension (i.e. the `index` is not a MultiIndex).\n",
+                "Multidimensional datasets use the normal xarray processing, which will dump string\n",
+                "categoricals back into python objects, which is bad news for high performance applications."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2208108a-d051-4941-ad72-b89a05169d81",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "sh.dataset.construct(\n",
+                "    hh[[\"income\",\"income_grp\"]].reset_index().set_index([\"HHID\", \"income\"])\n",
+                ")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -704,15 +895,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.10.9"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": false,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `sharrow-2.5.2/docs/walkthrough/one-dim.ipynb` & `sharrow-2.6.0/docs/walkthrough/one-dim.ipynb`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/walkthrough/sparse.ipynb` & `sharrow-2.6.0/docs/walkthrough/sparse.ipynb`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/docs/walkthrough/two-dim.ipynb` & `sharrow-2.6.0/docs/walkthrough/two-dim.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996501865671641%*

 * *Differences: {"'cells'": "{2: {'metadata': {'tags': ['remove-cell']}}, 23: {'metadata': {'tags': {delete: "*

 * *            "[1]}}}, 39: {'metadata': {'tags': {delete: [1]}}}, 56: {'metadata': {'tags': {delete: "*

 * *            "[1]}}}, 64: {'metadata': {'tags': ['remove-cell']}}, 66: {'metadata': {'tags': "*

 * *            "['remove-cell']}}}"}*

```diff
@@ -28,15 +28,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1f409525",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST check versions\n",
                 "import packaging\n",
                 "assert packaging.version.parse(xr.__version__) >= packaging.version.parse(\"0.20.2\")"
@@ -284,16 +284,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7b0a4e36",
             "metadata": {
                 "tags": [
-                    "remove-cell",
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST tree_dest attributes\n",
                 "assert tree.dim_order == ('WORKERID', 'TAZ')\n",
                 "assert tree.shape == (4361, 25)"
@@ -519,16 +518,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "03bb0e22",
             "metadata": {
                 "tags": [
-                    "remove-cell",
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST\n",
                 "assert isinstance(arr_pretty, xr.DataArray)\n",
                 "assert arr_pretty.dims == ('WORKERID', 'TAZ', 'expressions')\n",
@@ -756,16 +754,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dfd6d42a",
             "metadata": {
                 "tags": [
-                    "remove-cell",
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST pick count results\n",
                 "for i in range(choices.shape[0]):\n",
                 "    uc, pc = np.unique(choices[i], return_counts=True)\n",
@@ -906,15 +903,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e26a7f58",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST tree_unordered attributes\n",
                 "assert tree_unordered.dim_order is None\n",
                 "assert tree_unordered.shape == (25, 4361)"
@@ -934,15 +931,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4a4fb08e",
             "metadata": {
                 "tags": [
-                    "remove_cell"
+                    "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# TEST flow_unordered\n",
                 "assert arr_unordered.dims == ('TAZ', 'WORKERID', 'expressions')\n",
                 "assert arr_unordered.shape == (25, 4361, 4)"
```

### Comparing `sharrow-2.5.2/setup.cfg` & `sharrow-2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/accessors.py` & `sharrow-2.6.0/sharrow/accessors.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/aster.py` & `sharrow-2.6.0/sharrow/aster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import ast
 import io
 import logging
-import sys
 import tokenize
 
 try:
     from ast import unparse
 except ImportError:
     from astunparse import unparse as _unparse
 
-    unparse = lambda *args: _unparse(*args).strip("\n")
+    def unparse(*args):
+        return _unparse(*args).strip("\n")
+
 
 logger = logging.getLogger("sharrow.aster")
 
 
 def unparse_(*args):
     # spit out a ast dump on error
     try:
         return unparse(*args)
     except Exception:
         logger.warning(ast.dump(*args))
         raise
 
 
-if sys.version_info >= (3, 8):
-    ast_Constant_Type = ast.Constant
-    ast_String_value = lambda x: x.value if isinstance(x, ast.Str) else x
-    ast_TupleIndex_Type = ast.Tuple
-    ast_Index_Value = lambda x: x
-    ast_Constant = ast.Constant
-else:
-    ast_Constant_Type = (ast.Index, ast.Constant, ast.Str, ast.Num)
-    ast_String_value = (
-        lambda x: x.s
-        if isinstance(x, ast.Str)
-        else (ast_String_value(x.value) if isinstance(x, ast.Index) else x)
-    )
-    ast_TupleIndex_Type = (ast.Index, ast.Tuple)
-    ast_Index_Value = lambda x: x.value if isinstance(x, ast.Index) else x
-    ast_Constant = lambda x: ast.Constant(x, kind=None)
+ast_Constant_Type = ast.Constant
+
+
+def ast_String_value(x):
+    return x.value if isinstance(x, ast.Str) else x
+
+
+ast_TupleIndex_Type = ast.Tuple
+
+
+def ast_Index_Value(x):
+    return x
+
+
+ast_Constant = ast.Constant
 
 
 def _isNone(c):
     if c is None:
         return True
     if isinstance(c, ast_Constant_Type) and c.value is None:
         return True
@@ -65,15 +65,14 @@
     for node in ast.walk(z):
         if isinstance(node, ast.Name):
             names.add(node.id)
     return names
 
 
 def extract_names_2(command):
-
     if not isinstance(command, str):
         return set(), dict(), dict()
 
     z = ast.parse(command.lstrip())
 
     # Attribute-Name pairs first
     attribute_name_pairs = dict()
@@ -360,27 +359,30 @@
                 logger.debug(f"RewriteForNumba({self.spacename}|{self.rawalias}).{tag}")
             elif node2 is None:
                 try:
                     unparsed = unparse_(node1)
                 except:  # noqa: E722
                     unparsed = f"{type(node1)} not unparseable"
                 logger.debug(
-                    f"RewriteForNumba({self.spacename}|{self.rawalias}).{tag} [{type(node1).__name__}]= {unparsed}",
+                    f"RewriteForNumba({self.spacename}|{self.rawalias}).{tag} "
+                    f"[{type(node1).__name__}]= {unparsed}",
                 )
             else:
                 try:
                     unparsed1 = unparse_(node1)
                 except:  # noqa: E722
                     unparsed1 = f"{type(node1).__name__} not unparseable"
                 try:
                     unparsed2 = unparse_(node2)
                 except:  # noqa: E722
                     unparsed2 = f"{type(node2).__name__} not unparseable"
                 logger.debug(
-                    f"RewriteForNumba({self.spacename}|{self.rawalias}).{tag} [{type(node1).__name__},{type(node2).__name__}]= {unparsed1} => {unparsed2}",
+                    f"RewriteForNumba({self.spacename}|{self.rawalias}).{tag} "
+                    f"[{type(node1).__name__},{type(node2).__name__}]= "
+                    f"{unparsed1} => {unparsed2}",
                 )
 
     def generic_visit(self, node):
         self.log_event("generic_visit", node)
         return super().generic_visit(node)
 
     def _replacement(
@@ -398,16 +400,16 @@
 
         if self.spacevars is not None:
             if attr not in self.spacevars:
                 if self.get_default or (
                     topname == pref_topname and not self.swallow_errors
                 ):
                     raise KeyError(f"{topname}..{attr}")
-                # we originally raised a KeyError here regardless, but what if we just
-                # give back the original node, and see if other spaces,
+                # we originally raised a KeyError here regardless, but what if
+                # we just give back the original node, and see if other spaces,
                 # possibly fallback spaces, might work?  If nothing works then
                 # it will still eventually error out when compiling?
                 # The swallow errors option allows us to continue processing
                 # using the same rules, then circle back later to clean up
                 # errors, so that as-yet unprocessed Ast elements get the
                 # chance to be seen by the first pass.
                 return original_node
@@ -444,24 +446,17 @@
         if isinstance(dim_slots, (tuple, list)):
             if len(dim_slots):
                 elts = []
                 for n in dim_slots:
                     if isinstance(n, int):
                         elts.append(ast.Name(id=f"_arg{n:02}", ctx=ast.Load()))
                     elif isinstance(n, dict):
-                        if sys.version_info >= (3, 8):
-                            elts.append(
-                                ast.Constant(n=n[missing_dim_value], ctx=ast.Load())
-                            )
-                        else:
-                            elts.append(
-                                ast.Constant(
-                                    n[missing_dim_value], kind=None, ctx=ast.Load()
-                                )
-                            )
+                        elts.append(
+                            ast.Constant(n=n[missing_dim_value], ctx=ast.Load())
+                        )
                     else:
                         elts.append(n)
                     logger.debug(f"ELT {unparse_(elts[-1])}")
                 s = ast.Tuple(
                     elts=elts,
                     ctx=ast.Load(),
                 )
@@ -485,15 +480,14 @@
                 slice=s,
                 ctx=ctx,
             )
             logger.debug(f"one dim_slots on decorated_name {unparse_(result)}")
 
         digital_encoding = self.digital_encodings.get(attr, None)
         if digital_encoding is not None:
-
             dictionary = digital_encoding.get("dictionary", None)
             offset_source = digital_encoding.get("offset_source", None)
             if dictionary is not None:
                 result = ast.Subscript(
                     value=ast.Name(
                         id=f"__encoding_dict__{pref_topname}__{attr}", ctx=ast.Load()
                     ),
@@ -602,15 +596,16 @@
                 )
                 self.log_event(
                     f"visit_Subscript(Raw {ast_String_value(node.slice)})",
                     node,
                     result,
                 )
                 return result
-            # for XXX[YYY,ZZZ], XXX is a space name and YYY is a literal value and ZZZ is a literal value: skims['SOV_TIME','MD']
+            # for XXX[YYY,ZZZ], XXX is a space name and YYY is a literal value and
+            # ZZZ is a literal value: skims['SOV_TIME','MD']
             if (
                 node.value.id == self.spacename
                 and isinstance(ast_Index_Value(node.slice), ast.Tuple)
                 and len(ast_Index_Value(node.slice).elts) == 2
                 and isinstance(ast_Index_Value(node.slice).elts[0], ast_Constant_Type)
                 and isinstance(ast_Index_Value(node.slice).elts[1], ast_Constant_Type)
                 and isinstance(
@@ -722,15 +717,14 @@
         # `x ^ y` -> `np.bool_(x) ^ np.bool_(y)`
         left = self.visit(node.left)
         right = self.visit(node.right)
 
         if self.bool_wrapping and isinstance(
             node.op, (ast.BitAnd, ast.BitOr, ast.BitXor)
         ):
-
             result = ast.BinOp(
                 left=bool_wrap(left),
                 op=node.op,
                 right=bool_wrap(right),
             )
             self.log_event("visit_BinOp(Replacement)", node, result)
         else:
@@ -739,15 +733,14 @@
                 op=node.op,
                 right=right,
             )
             self.log_event("visit_BinOp(no change)", node, result)
         return result
 
     def visit_Call(self, node):
-
         result = None
         # implement ActivitySim's "reverse" skims
         if (
             isinstance(node.func, ast.Attribute) and node.func.attr == "reverse"
         ):  # *.reverse(...)
             if isinstance(node.func.value, ast.Name):  # somename.reverse(...)
                 if node.func.value.id == self.spacename:  # spacename.reverse(...)
```

### Comparing `sharrow-2.5.2/sharrow/dataset.py` & `sharrow-2.6.0/sharrow/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from __future__ import annotations
+
 import ast
 import base64
 import hashlib
 import logging
 import re
-from typing import Any, Hashable, Mapping, Sequence
+from collections.abc import Hashable, Mapping, Sequence
+from typing import Any
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import xarray as xr
 from xarray import DataArray, Dataset
 
 from .accessors import register_dataset_method
 from .aster import extract_all_name_tokens
+from .categorical import _Categorical  # noqa
 from .table import Table
 
 logger = logging.getLogger("sharrow")
 
 well_known_names = {
     "nb",
     "np",
@@ -88,29 +92,29 @@
     Returns
     -------
     Dataset
     """
     if isinstance(source, pd.DataFrame):
         source = dataset_from_dataframe_fast(source)  # xarray default can be slow
     elif isinstance(source, (Table, pa.Table)):
-        source = xr.Dataset.from_table(source)
-    elif isinstance(source, (pa.Table)):
-        source = xr.Dataset.from_table(source)
+        source = from_table(source)
     elif isinstance(source, xr.Dataset):
         pass  # don't do the superclass things
     elif isinstance(source, Sequence) and all(isinstance(i, str) for i in source):
-        source = xr.Dataset.from_table(pa.table({i: [] for i in source}))
+        source = from_table(pa.table({i: [] for i in source}))
     else:
         source = xr.Dataset(source)
     return source
 
 
 def dataset_from_dataframe_fast(
-    dataframe: pd.DataFrame, sparse: bool = False
-) -> "Dataset":
+    dataframe: pd.DataFrame,
+    sparse: bool = False,
+    preserve_cat: bool = True,
+) -> Dataset:
     """Convert a pandas.DataFrame into an xarray.Dataset
 
     Each column will be converted into an independent variable in the
     Dataset. If the dataframe's index is a MultiIndex, it will be expanded
     into a tensor product of one-dimensional indices (filling in missing
     values with NaN). This method will produce a Dataset very similar to
     that on which the 'to_dataframe' method was called, except with
@@ -171,19 +175,34 @@
         idx = dataframe.index.remove_unused_categories()
     else:
         idx = dataframe.index
 
     index_name = idx.name if idx.name is not None else "index"
     # Cast to a NumPy array first, in case the Series is a pandas Extension
     # array (which doesn't have a valid NumPy dtype)
-    arrays = {
-        name: ([index_name], np.asarray(dataframe[name].values))
-        for name in dataframe.columns
-        if name != index_name
-    }
+    arrays = {}
+    for name in dataframe.columns:
+        if name != index_name:
+            if dataframe[name].dtype == "category" and preserve_cat:
+                cat = dataframe[name].cat
+                categories = np.asarray(cat.categories)
+                if categories.dtype.kind == "O":
+                    categories = categories.astype(str)
+                arrays[name] = (
+                    [index_name],
+                    np.asarray(cat.codes),
+                    {
+                        "digital_encoding": {
+                            "dictionary": categories,
+                            "ordered": cat.ordered,
+                        }
+                    },
+                )
+            else:
+                arrays[name] = ([index_name], np.asarray(dataframe[name].values))
     return Dataset(arrays, coords={index_name: (index_name, dataframe.index.values)})
 
 
 def from_table(
     tbl,
     index_name="index",
     index=None,
@@ -193,15 +212,16 @@
 
     Parameters
     ----------
     tbl : Table
         Table from which to use data and indices.
     index_name : str, default 'index'
         This name will be given to the default dimension index, if
-        none is given.  Ignored if `index` is given explicitly.
+        none is given.  Ignored if `index` is given explicitly and
+        it already has a name.
     index : Index-like, optional
         Use this index instead of a default RangeIndex.
 
     Returns
     -------
     New Dataset.
     """
@@ -214,32 +234,49 @@
             raise ValueError(
                 f"length of index ({len(index)}) does not match length of table ({len(tbl)})"
             )
     if isinstance(index, pd.MultiIndex) and not index.is_unique:
         raise ValueError(
             "cannot attach a non-unique MultiIndex and convert into xarray"
         )
-    arrays = [
-        (tbl.column_names[n], np.asarray(tbl.column(n)))
-        for n in range(len(tbl.column_names))
-    ]
+    arrays = []
+    metadata = {}
+    for n in range(len(tbl.column_names)):
+        c = tbl.column(n)
+        if isinstance(c.type, pa.DictionaryType):
+            cc = c.combine_chunks()
+            arrays.append((tbl.column_names[n], np.asarray(cc.indices)))
+            metadata[tbl.column_names[n]] = {
+                "digital_encoding": {
+                    "dictionary": cc.dictionary,
+                    "ordered": cc.type.ordered,
+                }
+            }
+        else:
+            arrays.append((tbl.column_names[n], np.asarray(c)))
     result = xr.Dataset()
     if isinstance(index, pd.MultiIndex):
         dims = tuple(
             name if name is not None else "level_%i" % n
             for n, name in enumerate(index.names)
         )
         for dim, lev in zip(dims, index.levels):
             result[dim] = (dim, lev)
     else:
-        index_name = index.name if index.name is not None else "index"
+        try:
+            if index.name is not None:
+                index_name = index.name
+        except AttributeError:
+            pass
         dims = (index_name,)
         result[index_name] = (dims, index)
 
     result._set_numpy_data_from_dataframe(index, arrays, dims)
+    for k, v in metadata.items():
+        result[k].attrs.update(v)
     return result
 
 
 def from_omx(
     omx,
     index_names=("otaz", "dtaz"),
     indexes="one-based",
@@ -623,35 +660,19 @@
 
 
 def from_zarr_with_attr(*args, **kwargs):
     obj = from_zarr(*args, **kwargs)
     for k in obj:
         attrs = {}
         for aname, avalue in obj[k].attrs.items():
-            if (
-                isinstance(avalue, str)
-                and avalue.startswith(" {")
-                and avalue.endswith("} ")
-            ):
-                avalue = ast.literal_eval(avalue[1:-1])
-            if isinstance(avalue, str) and avalue == " < None > ":
-                avalue = None
-            attrs[aname] = avalue
+            attrs[aname] = _from_evalable_string(avalue)
         obj[k] = obj[k].assign_attrs(attrs)
     attrs = {}
     for aname, avalue in obj.attrs.items():
-        if (
-            isinstance(avalue, str)
-            and avalue.startswith(" {")
-            and avalue.endswith("} ")
-        ):
-            avalue = ast.literal_eval(avalue[1:-1])
-        if isinstance(avalue, str) and avalue == " < None > ":
-            avalue = None
-        attrs[aname] = avalue
+        attrs[aname] = _from_evalable_string(avalue)
     obj = obj.assign_attrs(attrs)
     return obj
 
 
 def coerce_to_range_index(idx):
     if isinstance(idx, pd.RangeIndex):
         return idx
@@ -669,15 +690,15 @@
 class _SingleDim:
     """
     Convenience accessor for single-dimension datasets.
     """
 
     __slots__ = ("dataset", "dim_name")
 
-    def __init__(self, dataset: "Dataset"):
+    def __init__(self, dataset: Dataset):
         self.dataset = dataset
         if len(self.dataset.dims) != 1:
             raise ValueError("single_dim implies a single dimension dataset")
         self.dim_name = self.dataset.dims.__iter__().__next__()
 
     @property
     def coords(self):
@@ -687,29 +708,141 @@
     def index(self):
         return self.dataset.indexes[self.dim_name]
 
     @property
     def size(self):
         return self.dataset.dims[self.dim_name]
 
-    def to_pyarrow(self):
-        return pa.Table.from_pydict(
-            {k: pa.array(v.to_numpy()) for k, v in self.dataset.variables.items()}
+    def _to_pydict(self):
+        columns = [k for k in self.dataset.variables if k != self.dim_name]
+        data = []
+        for k in columns:
+            a = self.dataset._variables[k]
+            if (
+                "digital_encoding" in a.attrs
+                and "dictionary" in a.attrs["digital_encoding"]
+            ):
+                de = a.attrs["digital_encoding"]
+                data.append(
+                    pd.Categorical.from_codes(
+                        a.values,
+                        de["dictionary"],
+                        de.get("ordered"),
+                    )
+                )
+            else:
+                data.append(a.values)
+        return dict(zip(columns, data))
+
+    def to_pyarrow(self) -> pa.Table:
+        columns = [k for k in self.dataset.variables if k != self.dim_name]
+        data = []
+        for k in columns:
+            a = self.dataset._variables[k]
+            if (
+                "digital_encoding" in a.attrs
+                and "dictionary" in a.attrs["digital_encoding"]
+            ):
+                de = a.attrs["digital_encoding"]
+                data.append(
+                    pa.DictionaryArray.from_arrays(
+                        a.values,
+                        de["dictionary"],
+                        ordered=de.get("ordered", False),
+                    )
+                )
+            else:
+                data.append(pa.array(a.values))
+        content = dict(zip(columns, data))
+        content[self.dim_name] = self.index
+        return pa.Table.from_pydict(content)
+
+    def to_parquet(self, filename):
+        import pyarrow.parquet as pq
+
+        t = self.to_pyarrow()
+        pq.write_table(t, filename)
+
+    def to_pandas(self) -> pd.DataFrame:
+        """
+        Convert this dataset into a pandas DataFrame.
+
+        The resulting DataFrame is always a copy of the data in the dataset.
+
+        Returns
+        -------
+        pandas.DataFrame
+        """
+        return pd.DataFrame(self._to_pydict(), index=self.index, copy=True)
+
+    def eval(
+        self,
+        expr: str,
+        parser: str = "pandas",
+        engine: str | None = None,
+        local_dict=None,
+        global_dict=None,
+    ):
+        """
+        Evaluate a Python expression as a string using various backends.
+
+        Parameters
+        ----------
+        expr : str
+            The expression to evaluate. This string cannot contain any Python
+            `statements
+            <https://docs.python.org/3/reference/simple_stmts.html#simple-statements>`__,
+            only Python `expressions
+            <https://docs.python.org/3/reference/simple_stmts.html#expression-statements>`__.
+        parser : {'pandas', 'python'}, default 'pandas'
+            The parser to use to construct the syntax tree from the expression. The
+            default of ``'pandas'`` parses code slightly different than standard
+            Python. Alternatively, you can parse an expression using the
+            ``'python'`` parser to retain strict Python semantics.  See the
+            :ref:`enhancing performance <enhancingperf.eval>` documentation for
+            more details.
+        engine : {'python', 'numexpr'}, default 'numexpr'
+            The engine used to evaluate the expression. Supported engines are
+            - None : tries to use ``numexpr``, falls back to ``python``
+            - ``'numexpr'`` : This default engine evaluates pandas objects using
+              numexpr for large speed ups in complex expressions with large frames.
+            - ``'python'`` : Performs operations as if you had ``eval``'d in top
+              level python. This engine is generally not that useful.
+        local_dict : dict or None, optional
+            A dictionary of local variables, taken from locals() by default.
+        global_dict : dict or None, optional
+            A dictionary of global variables, taken from globals() by default.
+
+        Returns
+        -------
+        DataArray or numeric scalar
+        """
+        result = pd.eval(
+            expr,
+            parser=parser,
+            engine=engine,
+            local_dict=local_dict,
+            global_dict=global_dict,
+            resolvers=[self.dataset],
         )
+        if result.size == self.size:
+            return DataArray(np.asarray(result), coords=self.dataset.coords)
+        else:
+            return result
 
 
 @xr.register_dataarray_accessor("single_dim")
 class _SingleDimArray:
     """
     Convenience accessor for single-dimension datasets.
     """
 
     __slots__ = ("dataarray", "dim_name")
 
-    def __init__(self, dataarray: "DataArray"):
+    def __init__(self, dataarray: DataArray):
         self.dataarray = dataarray
         if len(self.dataarray.dims) != 1:
             raise ValueError("single_dim implies a single dimension dataset")
         self.dim_name = self.dataarray.dims[0]
 
     @property
     def coords(self):
@@ -721,14 +854,47 @@
 
     def rename(self, name: str) -> DataArray:
         """Rename the single dimension."""
         if self.dim_name == name:
             return self.dataarray
         return self.dataarray.rename({self.dim_name: name})
 
+    def to_pandas(self) -> pd.Series:
+        """
+        Convert this array into a pandas Series.
+
+        If this array is categorical (i.e. with a simple dictionary-based
+        digital encoding) then the result will be a Series with categorical dtype.
+
+        The DataArray's `name` attribute is preserved in the result.
+        """
+        if self.dataarray.cat.is_categorical():
+            return pd.Series(
+                pd.Categorical.from_codes(
+                    self.dataarray,
+                    self.dataarray.cat.categories,
+                    self.dataarray.cat.ordered,
+                ),
+                index=self.index,
+                name=self.dataarray.name,
+            )
+        else:
+            result = self.dataarray.to_pandas()
+            if self.dataarray.name:
+                result = result.rename(self.dataarray.name)
+            return result
+
+    def to_pyarrow(self):
+        if self.dataarray.cat.is_categorical():
+            return pa.DictionaryArray.from_arrays(
+                self.dataarray.data, self.dataarray.cat.categories
+            )
+        else:
+            return pa.array(self.dataarray.data)
+
 
 @xr.register_dataset_accessor("iloc")
 class _iLocIndexer:
     """
     Purely integer-location based indexing for selection by position on 1-d Datasets.
 
     In many ways, a dataset with a single dimensions is like a pandas DataFrame,
@@ -738,18 +904,18 @@
     convenient to have iloc functionality enabled. This only works for indexing
     on the rows, but if there’s only the one dimension the complexity of isel
     is not needed.
     """
 
     __slots__ = ("dataset",)
 
-    def __init__(self, dataset: "Dataset"):
+    def __init__(self, dataset: Dataset):
         self.dataset = dataset
 
-    def __getitem__(self, key: Mapping[Hashable, Any]) -> "Dataset":
+    def __getitem__(self, key: Mapping[Hashable, Any]) -> Dataset:
         if not is_dict_like(key):
             if len(self.dataset.dims) == 1:
                 dim_name = self.dataset.dims.__iter__().__next__()
                 key = {dim_name: key}
             else:
                 raise TypeError(
                     "can only lookup dictionaries from Dataset.iloc, "
@@ -854,14 +1020,66 @@
 
             with zarr.ZipStore(args[0], **kwargs) as store:
                 self.to_zarr(store)
             return
     return super().to_zarr(*args, **kwargs)
 
 
+def _to_ast_literal(x):
+    if isinstance(x, dict):
+        return (
+            "{"
+            + ", ".join(
+                f"{_to_ast_literal(k)}: {_to_ast_literal(v)}" for k, v in x.items()
+            )
+            + "}"
+        )
+    elif isinstance(x, list):
+        return "[" + ", ".join(_to_ast_literal(i) for i in x) + "]"
+    elif isinstance(x, tuple):
+        return "(" + ", ".join(_to_ast_literal(i) for i in x) + ")"
+    elif isinstance(x, pd.Index):
+        return _to_ast_literal(x.to_list())
+    elif isinstance(x, np.ndarray):
+        return _to_ast_literal(list(x))
+    else:
+        return repr(x)
+
+
+def _to_evalable_string(x):
+    if x is None:
+        return " < None > "
+    elif x is True:
+        return " < True > "
+    elif x is False:
+        return " < False > "
+    else:
+        return f" {_to_ast_literal(x)} "
+
+
+def _from_evalable_string(x):
+    if isinstance(x, str):
+        # if x.startswith(" {") and x.endswith("} "):
+        #     return ast.literal_eval(x[1:-1])
+        if x == " < None > ":
+            return None
+        if x == " < True > ":
+            return True
+        if x == " < False > ":
+            return False
+        if x.startswith(" ") and x.endswith(" "):
+            try:
+                return ast.literal_eval(x.strip(" "))
+            except Exception:
+                print(x)
+                raise
+    else:
+        return x
+
+
 @register_dataset_method
 def to_zarr_with_attr(self, *args, **kwargs):
     """
     Write dataset contents to a zarr group.
 
     Parameters
     ----------
@@ -934,27 +1152,25 @@
         If not other chunks are found, Zarr uses its own heuristics to
         choose automatic chunk sizes.
     """
     obj = self.copy()
     for k in self:
         attrs = {}
         for aname, avalue in self[k].attrs.items():
-            if isinstance(avalue, dict):
-                avalue = f" {avalue!r} "
-            if avalue is None:
-                avalue = " < None > "
-            attrs[aname] = avalue
+            attrs[aname] = _to_evalable_string(avalue)
         obj[k] = self[k].assign_attrs(attrs)
+    if hasattr(self, "coords"):
+        for k in self.coords:
+            attrs = {}
+            for aname, avalue in self.coords[k].attrs.items():
+                attrs[aname] = _to_evalable_string(avalue)
+            obj.coords[k] = self.coords[k].assign_attrs(attrs)
     attrs = {}
     for aname, avalue in self.attrs.items():
-        if isinstance(avalue, dict):
-            avalue = f" {avalue!r} "
-        if avalue is None:
-            avalue = " < None > "
-        attrs[aname] = avalue
+        attrs[aname] = _to_evalable_string(avalue)
     obj = obj.assign_attrs(attrs)
     return obj.to_zarr(*args, **kwargs)
 
 
 @register_dataset_method
 def to_table(self):
     """
@@ -1084,15 +1300,15 @@
     Dataset
     """
     objs = {}
     for n, a in enumerate(args):
         try:
             name = a.name
         except AttributeError:
-            raise ValueError(f"argument {n} has no name")
+            raise ValueError(f"argument {n} has no name") from None
         if name is None:
             raise ValueError(f"the name for argument {n} is None")
         objs[name] = a
     return xr.Dataset(objs)
 
 
 @register_dataset_method
```

### Comparing `sharrow-2.5.2/sharrow/digital_encoding.py` & `sharrow-2.6.0/sharrow/digital_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,32 +159,43 @@
     u, b = np.unique(values, return_counts=True)
     return smash_bins(u, b, final_width=final_width)
 
 
 def digitize_by_dictionary(arr, bitwidth=8):
     result = arr.copy()
     bins = find_bins(arr, final_width=1 << bitwidth)
-    bin_edges = (bins[1:] - bins[:-1]) / 2 + bins[:-1]
     try:
-        arr_data = arr.data
-    except AttributeError:
-        pass
+        bin_edges = (bins[1:] - bins[:-1]) / 2 + bins[:-1]
+    except TypeError:
+        # bins are not numeric
+        bin_map = {x:n for n,x in enumerate(bins)}
+        u, inv = np.unique(arr.data, return_inverse=True)
+        result.data = np.array([bin_map.get(x) for x in u])[inv].reshape(arr.shape)
+        result.attrs["digital_encoding"] = {
+            "dictionary": bins,
+        }
+        return result
     else:
-        if isinstance(arr_data, da.Array):
-            result.data = da.digitize(arr_data, bin_edges).astype(f"uint{bitwidth}")
-            result.attrs["digital_encoding"] = {
-                "dictionary": bins,
-            }
-            return result
-    # fall back to numpy digitize
-    result.data = np.digitize(arr, bin_edges).astype(f"uint{bitwidth}")
-    result.attrs["digital_encoding"] = {
-        "dictionary": bins,
-    }
-    return result
+        try:
+            arr_data = arr.data
+        except AttributeError:
+            pass
+        else:
+            if isinstance(arr_data, da.Array):
+                result.data = da.digitize(arr_data, bin_edges).astype(f"uint{bitwidth}")
+                result.attrs["digital_encoding"] = {
+                    "dictionary": bins,
+                }
+                return result
+        # fall back to numpy digitize
+        result.data = np.digitize(arr, bin_edges).astype(f"uint{bitwidth}")
+        result.attrs["digital_encoding"] = {
+            "dictionary": bins,
+        }
+        return result
 
 
 @xr.register_dataset_accessor("digital_encoding")
 class _DigitalEncodings:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
```

### Comparing `sharrow-2.5.2/sharrow/example_data/households.csv.gz` & `sharrow-2.6.0/sharrow/example_data/households.csv.gz`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/land_use.csv.gz` & `sharrow-2.6.0/sharrow/example_data/land_use.csv.gz`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/maz_to_taz.csv` & `sharrow-2.6.0/sharrow/example_data/maz_to_taz.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/persons.csv.gz` & `sharrow-2.6.0/sharrow/example_data/persons.csv.gz`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.omx` & `sharrow-2.6.0/sharrow/example_data/skims.omx`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DIST/0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DIST/0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTBIKE/0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTBIKE/0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DISTWALK/0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DISTWALK/0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0` & `sharrow-2.6.0/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/example_data.py` & `sharrow-2.6.0/sharrow/example_data.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/filewrite.py` & `sharrow-2.6.0/sharrow/filewrite.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     try:
         return black.format_file_contents(code, fast=fast, mode=mode)
     except black.NothingChanged:
         return code
     except Exception as err:
         import warnings
 
-        warnings.warn(f"error in blacken: {err!r}")
+        warnings.warn(f"error in blacken: {err!r}", stacklevel=2)
         return code
 
 
 @contextlib.contextmanager
 def rewrite(pth, mode="wt"):
     if not os.path.exists(pth):
         with open(pth, mode) as f:
```

### Comparing `sharrow-2.5.2/sharrow/flows.py` & `sharrow-2.6.0/sharrow/flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,21 @@
 
     def check(self, node):
         if isinstance(node, str):
             node = ast.parse(node)
         if isinstance(node, ast.AST):
             self.visit(node)
         else:
-            for i in node:
-                self.check(i)
+            try:
+                node_iter = iter(node)
+            except TypeError:
+                pass
+            else:
+                for i in node_iter:
+                    self.check(i)
         return self.optional_get_tokens
 
 
 def coerce_to_range_index(idx):
     if isinstance(idx, pd.RangeIndex):
         return idx
     if isinstance(idx, (pd.Int64Index, pd.Float64Index, pd.UInt64Index)):
@@ -199,27 +204,40 @@
             return pd.RangeIndex(idx[0], idx[0] + idx.size)
     return idx
 
 
 FUNCTION_TEMPLATE = """
 
 # {init_expr}
-@nb.jit(cache=False, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=False,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def {fname}(
     {argtokens}
     _outputs,
     {nametokens}
 ):
     return {expr}
 
 """
 
 
 IRUNNER_1D_TEMPLATE = """
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def irunner(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     mask=None,
 ):
     result = np.empty((argshape[0], {len_self_raw_functions}), dtype=dtype)
@@ -232,15 +250,22 @@
                 result[j0, :] = np.nan
                 continue
         linemaker(result[j0], j0, {joined_namespace_names})
     return result
 """
 
 IRUNNER_2D_TEMPLATE = """
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def irunner(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     mask=None,
 ):
     result = np.empty((argshape[0], argshape[1], {len_self_raw_functions}), dtype=dtype)
@@ -254,15 +279,22 @@
                 if not mask[j0, j1]:
                     result[j0, j1, :] = np.nan
             linemaker(result[j0, j1], j0, j1, {joined_namespace_names})
     return result
 """
 
 IDOTTER_1D_TEMPLATE = """
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def idotter(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     dotarray=None,
 ):
     if dotarray is None:
@@ -279,15 +311,22 @@
         for j0 in range(argshape[0]):
             {meta_code_stack_dot}
             np.dot(intermediate, dotarray, out=result[j0,:])
     return result
 """
 
 IDOTTER_2D_TEMPLATE = """
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def idotter(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     dotarray=None,
 ):
     if dotarray is None:
@@ -306,36 +345,54 @@
           for j1 in range(argshape[1]):
             {meta_code_stack_dot}
             np.dot(intermediate, dotarray, out=result[j0,j1,:])
     return result
 """
 
 ILINER_1D_TEMPLATE = """
-@nb.jit(cache=False, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=False,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def linemaker(
     intermediate, j0,
     {joined_namespace_names}
 ):
             {meta_code_stack_dot}
 
 """
 
 ILINER_2D_TEMPLATE = """
-@nb.jit(cache=False, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=False,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def linemaker(
     intermediate, j0, j1,
     {joined_namespace_names}
 ):
             {meta_code_stack_dot}
 
 """
 
 
 MNL_GENERIC_TEMPLATE = """
-@nb.jit(cache=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def _sample_choices_maker(
         prob_array,
         random_array,
         out_choices,
         out_choice_probs,
 ):
     '''
@@ -377,15 +434,21 @@
         while s < sample_size:
             out_choices[s] = a
             out_choice_probs[s] = prob_array[a]
             s += 1
 
 
 
-@nb.jit(cache=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def _sample_choices_maker_counted(
         prob_array,
         random_array,
         out_choices,
         out_choice_probs,
         out_pick_count,
 ):
@@ -442,15 +505,22 @@
 
 MNL_1D_TEMPLATE = (
     MNL_GENERIC_TEMPLATE
     + """
 
 logit_ndims = 1
 
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def mnl_transform_plus1d(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     dotarray=None,
     random_draws=None,
     pick_counted=False,
@@ -492,15 +562,21 @@
                 _sample_choices_maker_counted(partial, random_draws[j0], result[j0], result_p[j0], pick_count[j0])
             else:
                 _sample_choices_maker(partial, random_draws[j0], result[j0], result_p[j0])
     return result, result_p, pick_count, _logsums
 
 """
 )
-# @nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath})
+# @nb.jit(
+#     cache=True,
+#     parallel=True,
+#     error_model='{error_model}',
+#     boundscheck={boundscheck},
+#     nopython={nopython},
+#     fastmath={fastmath})
 # def mnl_transform_plus1d(
 #     argshape,
 #     {joined_namespace_names}
 #     dtype=np.{dtype},
 #     dotarray=None,
 #     random_draws=None,
 #     pick_counted=False,
@@ -529,27 +605,36 @@
 #             shifter = np.max(dotprod)
 #             partial = np.exp(dotprod - shifter)
 #             local_sum = np.sum(partial)
 #             partial /= local_sum
 #             if logsums:
 #                 _logsums[j0,k0] = np.log(local_sum) + shifter
 #             if pick_counted:
-#                 _sample_choices_maker_counted(partial, random_draws[j0,k0], result[j0,k0], result_p[j0,k0], pick_count[j0,k0])
+#                 _sample_choices_maker_counted(
+#                   partial, random_draws[j0,k0], result[j0,k0], result_p[j0,k0], pick_count[j0,k0]
+#                 )
 #             else:
 #                 _sample_choices_maker(partial, random_draws[j0,k0], result[j0,k0], result_p[j0,k0])
 #     return result, result_p, pick_count, _logsums
 
 
 MNL_2D_TEMPLATE = (
     MNL_GENERIC_TEMPLATE
     + """
 
 logit_ndims = 2
 
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def mnl_transform(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     dotarray=None,
     random_draws=None,
     pick_counted=False,
@@ -605,15 +690,22 @@
         if pick_counted:
             _sample_choices_maker_counted(partial, random_draws[j0], result[j0], result_p[j0], pick_count[j0])
         else:
             _sample_choices_maker(partial, random_draws[j0], result[j0], result_p[j0])
     return result, result_p, pick_count, _logsums
 
 
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def mnl_transform_plus1d(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     dotarray=None,
     random_draws=None,
     pick_counted=False,
@@ -660,27 +752,36 @@
             local_sum = np.sum(partial)
             if logsums:
                 _logsums[j0,j1] = np.log(local_sum) + shifter
                 if logsums == 1:
                     continue
             partial /= local_sum
             if pick_counted:
-                _sample_choices_maker_counted(partial, random_draws[j0,j1], result[j0,j1], result_p[j0,j1], pick_count[j0,j1])
+                _sample_choices_maker_counted(
+                    partial, random_draws[j0,j1], result[j0,j1], result_p[j0,j1], pick_count[j0,j1]
+                )
             else:
                 _sample_choices_maker(partial, random_draws[j0,j1], result[j0,j1], result_p[j0,j1])
     return result, result_p, pick_count, _logsums
 
 """
 )
 
 NL_1D_TEMPLATE = """
 
 from sharrow.nested_logit import _utility_to_probability
 
-@nb.jit(cache=True, parallel=True, error_model='{error_model}', boundscheck={boundscheck}, nopython={nopython}, fastmath={fastmath}, nogil={nopython})
+@nb.jit(
+    cache=True,
+    parallel=True,
+    error_model='{error_model}',
+    boundscheck={boundscheck},
+    nopython={nopython},
+    fastmath={fastmath},
+    nogil={nopython})
 def nl_transform(
     argshape,
     {joined_namespace_names}
     dtype=np.{dtype},
     dotarray=None,
     random_draws=None,
     pick_counted=False,
@@ -742,15 +843,17 @@
                 logprob,  # float output shape=[nodes]
                 probability,  # float output shape=[nodes]
             )
             if logsums:
                 _logsums[j0] = utility[-1]
             if logsums != 1:
                 if pick_counted:
-                    _sample_choices_maker_counted(probability[:n_alts], random_draws[j0], result[j0], result_p[j0], pick_count[j0])
+                    _sample_choices_maker_counted(
+                        probability[:n_alts], random_draws[j0], result[j0], result_p[j0], pick_count[j0]
+                    )
                 else:
                     _sample_choices_maker(probability[:n_alts], random_draws[j0], result[j0], result_p[j0])
     return result, result_p, pick_count, _logsums
 
 """
 
 
@@ -849,14 +952,15 @@
         flow_library=None,
         extra_hash_data=(),
         write_hash_audit=True,
         hashing_level=1,
         dim_order=None,
         dim_exclude=None,
         bool_wrapping=False,
+        with_root_node_name=None,
     ):
         assert isinstance(tree, DataTree)
         tree.digitize_relationships(inplace=True)
 
         self = super().__new__(cls)
         # clean defs with hidden values
         defs = {k: _flip_flop_def(v) for k, v in defs.items()}
@@ -891,17 +995,19 @@
             boundscheck=boundscheck,
             nopython=nopython,
             fastmath=fastmath,
             readme=readme,
             parallel=parallel,
             extra_hash_data=extra_hash_data,
             write_hash_audit=write_hash_audit,
+            with_root_node_name=with_root_node_name,
         )
         if flow_library is not None:
             flow_library[self.flow_hash] = self
+        self.with_root_node_name = with_root_node_name
         return self
 
     def __initialize_1(
         self,
         tree,
         defs,
         cache_dir=None,
@@ -933,15 +1039,15 @@
         self._secondary_flows = {}
         self.dim_order = dim_order
         self.dim_exclude = dim_exclude
         self.bool_wrapping = bool_wrapping
 
         all_raw_names = set()
         all_name_tokens = set()
-        for k, expr in defs.items():
+        for _k, expr in defs.items():
             plain_names, attribute_pairs, subscript_pairs = extract_names_2(expr)
             all_raw_names |= plain_names
             if self.tree.root_node_name:
                 all_raw_names |= attribute_pairs.get(self.tree.root_node_name, set())
                 all_raw_names |= subscript_pairs.get(self.tree.root_node_name, set())
 
         dimensions_ordered = presorted(self.tree.dims, self.dim_order, self.dim_exclude)
@@ -1064,23 +1170,27 @@
                 _flow_hash_push(k)
                 parts = k.split("__")
                 if len(parts) > 2:
                     try:
                         digital_encoding = self.tree.subspaces[parts[1]][
                             "__".join(parts[2:])
                         ].attrs["digital_encoding"]
-                    except (AttributeError, KeyError):
+                    except (AttributeError, KeyError) as err:
                         pass
+                        print(f"$$$$/ndigital_encoding=ERR\n{err}\n\n\n$$$")
+
                     else:
+                        print(f"$$$$/n{digital_encoding=}\n\n\n$$$")
                         if digital_encoding:
                             for de_k in sorted(digital_encoding.keys()):
                                 de_v = digital_encoding[de_k]
                                 if de_k == "dictionary":
                                     self.encoding_dictionaries[k] = de_v
                                 _flow_hash_push((k, "digital_encoding", de_k, de_v))
+
         for k in extra_hash_data:
             _flow_hash_push(k)
 
         _flow_hash_push(f"boundscheck={boundscheck}")
         _flow_hash_push(f"error_model={error_model}")
         _flow_hash_push(f"fastmath={fastmath}")
         _flow_hash_push(f"bool_wrapping={bool_wrapping}")
@@ -1166,15 +1276,15 @@
             expr = str(expr).lstrip()
             prior_expr = init_expr = expr
             other_way = True
             while other_way:
                 other_way = False
                 # if other_way is triggered, there may be residual other terms
                 # that were not addressed, so this loop should be applied again.
-                for spacename, spacearrays in self.tree.subspaces.items():
+                for spacename in self.tree.subspaces.keys():
                     dim_slots, digital_encodings, blenders = meta_data[spacename]
                     try:
                         expr = expression_for_numba(
                             expr,
                             spacename,
                             dim_slots,
                             dim_slots,
@@ -1397,14 +1507,15 @@
         boundscheck=False,
         nopython=True,
         fastmath=True,
         readme=None,
         parallel=True,
         extra_hash_data=(),
         write_hash_audit=True,
+        with_root_node_name=None,
     ):
         """
 
         Parameters
         ----------
         tree : DataTree
         defs : Dict[str,str]
@@ -1460,15 +1571,15 @@
 
         # create the package directory for the flow if it does not exist
         os.makedirs(self.cache_dir, exist_ok=True)
 
         # if an existing __init__ file matches the hash, just use it
         init_file = os.path.join(self.cache_dir, self.name, "__init__.py")
         if os.path.isfile(init_file):
-            with open(init_file, "rt") as f:
+            with open(init_file) as f:
                 content = f.read()
             s = re.search("""flow_hash = ['"](.*)['"]""", content)
         else:
             s = None
         if s and s.group(1) == self.flow_hash:
             logger.info(f"using existing flow code {self.flow_hash}")
             writing = False
@@ -1605,17 +1716,20 @@
                 f_code.write("\n\n# function code\n")
                 f_code.write(f"\n\n{blacken(func_code)}")
 
                 f_code.write("\n\n# machinery code\n\n")
 
                 if self.tree.relationships_are_digitized:
 
+                    if with_root_node_name is None:
+                        with_root_node_name = self.tree.root_node_name
+
                     root_dims = list(
                         presorted(
-                            self.tree.root_dataset.dims,
+                            self.tree._graph.nodes[with_root_node_name]["dataset"].dims,
                             self.dim_order,
                             self.dim_exclude,
                         )
                     )
                     n_root_dims = len(root_dims)
 
                     if n_root_dims == 1:
@@ -1759,15 +1873,17 @@
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore", category=nb.NumbaExperimentalFeatureWarning
             )
             assembled_args = [args.get(k) for k in self.arg_name_positions.keys()]
             for aa in assembled_args:
                 if aa.dtype.kind != "i":
-                    warnings.warn("position arguments are not all integers")
+                    warnings.warn(
+                        "position arguments are not all integers", stacklevel=2
+                    )
             try:
                 if runner is None:
                     if dot is None:
                         runner_ = self._runner
                     else:
                         runner_ = self._dotter
                 else:
@@ -1926,15 +2042,21 @@
                     kwargs["logsums"] = logsums
                 if nesting is not None:
                     nesting.pop("edges_1st", None)  # unused in simple NL
                     nesting.pop("edges_alloc", None)  # unused in simple NL
                     kwargs.update(nesting)
                 if mask is not None:
                     kwargs["mask"] = mask
-                tree_root_dims = rg.root_dataset.dims
+
+                if self.with_root_node_name is None:
+                    tree_root_dims = rg.root_dataset.dims
+                else:
+                    tree_root_dims = rg._graph.nodes[self.with_root_node_name][
+                        "dataset"
+                    ].dims
                 argshape = [
                     tree_root_dims[i]
                     for i in presorted(tree_root_dims, self.dim_order, self.dim_exclude)
                 ]
                 if mnl is not None:
                     if nesting is not None:
                         n_alts = nesting["n_alts"]
@@ -2052,15 +2174,17 @@
                                 timers = f"{timers/1e-3:.1f} ms"
                             else:
                                 timers = f"{timers:.2f} s"
                         logger.warning(
                             f"cache miss in {self.flow_hash}{warning_text}\n"
                             f"Compile Time: {timers}"
                         )
-                        warnings.warn(f"{self.flow_hash}", CacheMissWarning)
+                        warnings.warn(
+                            f"{self.flow_hash}", CacheMissWarning, stacklevel=1
+                        )
                         self.compiled_recently = True
                         self._known_cache_misses[runner_name][k] = v
         return self.compiled_recently
 
     @property
     def cache_misses(self):
         """dict[str, dict]: Numba cache misses across all defined flow methods."""
@@ -2136,17 +2260,26 @@
             source = self.tree
         if dtype is None and dot is not None:
             dtype = dot.dtype
 
         if logit_draws is None and logsums == 1:
             logit_draws = np.zeros(source.shape + (0,), dtype=dtype)
 
-        use_dims = list(
-            presorted(source.root_dataset.dims, self.dim_order, self.dim_exclude)
-        )
+        if self.with_root_node_name is None:
+            use_dims = list(
+                presorted(source.root_dataset.dims, self.dim_order, self.dim_exclude)
+            )
+        else:
+            use_dims = list(
+                presorted(
+                    source._graph.nodes[self.with_root_node_name]["dataset"].dims,
+                    self.dim_order,
+                    self.dim_exclude,
+                )
+            )
 
         if logit_draws is not None:
             if dot is None:
                 raise NotImplementedError
             if dot.ndim == 1 or (dot.ndim == 2 and dot.shape[1] == 1):
                 while logit_draws.ndim < self._logit_ndims:
                     logit_draws = np.expand_dims(logit_draws, -1)
@@ -2309,17 +2442,28 @@
             )
         elif as_dataarray:
 
             if result_squeeze:
                 result = squeeze(result, result_squeeze)
                 result_p = squeeze(result_p, result_squeeze)
                 pick_count = squeeze(pick_count, result_squeeze)
-            result_coords = {
-                k: v for k, v in source.root_dataset.coords.items() if k in result_dims
-            }
+            if self.with_root_node_name is None:
+                result_coords = {
+                    k: v
+                    for k, v in source.root_dataset.coords.items()
+                    if k in result_dims
+                }
+            else:
+                result_coords = {
+                    k: v
+                    for k, v in source._graph.nodes[self.with_root_node_name][
+                        "dataset"
+                    ].coords.items()
+                    if k in result_dims
+                }
             if result is not None:
                 result = xr.DataArray(
                     result,
                     dims=result_dims,
                     coords=result_coords,
                 )
                 if "expressions" in result_dims:
@@ -2654,15 +2798,15 @@
         """
         from IPython.display import HTML
         from pygments import highlight
         from pygments.formatters.html import HtmlFormatter
         from pygments.lexers.python import PythonLexer
 
         codefile = os.path.join(self.cache_dir, self.name, "__init__.py")
-        with open(codefile, "rt") as f_code:
+        with open(codefile) as f_code:
             code = f_code.read()
         pretty = highlight(code, PythonLexer(), HtmlFormatter(linenos=linenos))
         css = HtmlFormatter().get_style_defs(".highlight")
         bbedit_url = f"x-bbedit://open?url=file://{codefile}"
         bb_link = f'<a href="{bbedit_url}">{codefile}</a>'
         return HTML(f"<style>{css}</style><p>{bb_link}</p>{pretty}")
```

### Comparing `sharrow-2.5.2/sharrow/logging.py` & `sharrow-2.6.0/sharrow/logging.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/maths.py` & `sharrow-2.6.0/sharrow/maths.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/nested_logit.py` & `sharrow-2.6.0/sharrow/nested_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Mapping
+from collections.abc import Mapping
 
 import numba as nb
 import numpy as np
 
 
 @nb.njit(error_model="numpy", fastmath=True, cache=True)
 def _utility_to_probability(
```

### Comparing `sharrow-2.5.2/sharrow/omx.py` & `sharrow-2.6.0/sharrow/omx.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/relationships.py` & `sharrow-2.6.0/sharrow/relationships.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     sparse_array_type = ()
 
 try:
     from ast import unparse
 except ImportError:
     from astunparse import unparse as _unparse
 
-    unparse = lambda *args: _unparse(*args).strip("\n")
+    def unparse(*args):
+        return _unparse(*args).strip("\n")
 
 
 logger = logging.getLogger("sharrow")
 
 well_known_names = {
     "nb",
     "np",
@@ -43,14 +44,16 @@
     "min",
     "piece",
     "hard_sigmoid",
     "transpose_leading",
     "clip",
 }
 
+NOTSET = "<--NOTSET-->"
+
 
 def _require_string(x):
     if not isinstance(x, str):
         raise ValueError("must be string")
     return x
 
 
@@ -193,26 +196,56 @@
         """str: How the target dimension is used, either by 'label' or 'position'."""
 
         self.analog = analog
         """str: Original variable that defined label-based relationship before digitization."""
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
-            return repr(self) == repr(other)
+            if self.analog:
+                left = (
+                    f"<Relationship by label: "
+                    f"{self.parent_data}[{self.analog!r}] -> "
+                    f"{self.child_data}[{self.child_name!r}]>"
+                )
+            else:
+                left = repr(self)
+            if other.analog:
+                right = (
+                    f"<Relationship by label: "
+                    f"{other.parent_data}[{other.analog!r}] -> "
+                    f"{other.child_data}[{other.child_name!r}]>"
+                )
+            else:
+                right = repr(other)
+            return left == right
 
     def __repr__(self):
-        return f"<Relationship by {self.indexing}: {self.parent_data}[{self.parent_name!r}] -> {self.child_data}[{self.child_name!r}]>"
+        return (
+            f"<Relationship by {self.indexing}: "
+            f"{self.parent_data}[{self.parent_name!r}] -> "
+            f"{self.child_data}[{self.child_name!r}]>"
+        )
 
     def attrs(self):
         return dict(
             parent_name=self.parent_name,
             child_name=self.child_name,
             indexing=self.indexing,
         )
 
+    def to_dict(self):
+        return dict(
+            parent_data=self.parent_data,
+            parent_name=self.parent_name,
+            child_data=self.child_data,
+            child_name=self.child_name,
+            indexing=self.indexing,
+            analog=self.analog,
+        )
+
     @classmethod
     def from_string(cls, s):
         """
         Construct a `Relationship` from a string.
 
         Parameters
         ----------
@@ -253,15 +286,15 @@
 class DataTree:
     """
     A tree representing linked datasets, from which data can flow.
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
-    root_node_name : str
+    root_node_name : str or False
         The name of the node at the root of the tree.
     extra_funcs : Tuple[Callable]
         Additional functions that can be called by Flow objects created
         using this DataTree.  These functions should have defined `__name__`
         attributes, so they can be called in expressions.
     extra_vars : Mapping[str,Any], optional
         Additional named constants that can be referenced by expressions in
@@ -437,23 +470,42 @@
                 if self._graph.in_degree(nodename) == 0:
                     self._root_node_name = nodename
                     break
         return self._root_node_name
 
     @root_node_name.setter
     def root_node_name(self, name):
-        if name is None:
-            self._root_node_name = None
+        if name is None or name is False:
+            self._root_node_name = name
             return
         if not isinstance(name, str):
-            raise TypeError(f"root_node_name must be str not {type(name)}")
+            raise TypeError(
+                f"root_node_name must be one of [str, None, False] not {type(name)}"
+            )
         if name not in self._graph.nodes:
             raise KeyError(name)
         self._root_node_name = name
 
+    @property
+    def root_node_name_str(self):
+        """str: The root node for this data tree, which is only ever a parent.
+
+        This method raises a ValueError if root node cannot be determined.
+        """
+        if self._root_node_name is None:
+            for nodename in self._graph.nodes:
+                if self._graph.in_degree(nodename) == 0:
+                    self._root_node_name = nodename
+                    break
+        if self._root_node_name is None:
+            raise ValueError("root node cannot be determined")
+        if self._root_node_name is False:
+            raise ValueError("root node is False")
+        return self._root_node_name
+
     def add_relationship(self, *args, **kwargs):
         """
         Add a relationship to this DataTree.
 
         The new relationship will point from a variable in one dataset
         to a dimension of another dataset in this tree.  Both the parent
         and the child datasets should already have been added.
@@ -465,36 +517,15 @@
             contructor, unless only a single `str` argument is provided,
             in which case the `Relationship.from_string` class constructor
             is used.
         """
         if len(args) == 1 and isinstance(args[0], Relationship):
             r = args[0]
         elif len(args) == 1 and isinstance(args[0], str):
-            s = args[0]
-            if "->" in s:
-                parent, child = s.split("->", 1)
-                i = "position"
-            elif "@" in s:
-                parent, child = s.split("@", 1)
-                i = "label"
-            else:
-                raise ValueError(f"cannot interpret relationship {s!r}")
-            p1, p2 = parent.split(".", 1)
-            c1, c2 = child.split(".", 1)
-            p1 = p1.strip()
-            p2 = p2.strip()
-            c1 = c1.strip()
-            c2 = c2.strip()
-            r = Relationship(
-                parent_data=p1,
-                parent_name=p2,
-                child_data=c1,
-                child_name=c2,
-                indexing=i,
-            )
+            r = Relationship.from_string(args[0])
         else:
             r = Relationship(*args, **kwargs)
 
         # check for existing relationships, don't duplicate
         for e in self._graph.edges:
             r2 = self._get_relationship(e)
             if r == r2:
@@ -507,14 +538,21 @@
         if self.force_digitization:
             self.digitize_relationships(inplace=True)
 
     def get_relationship(self, parent, child):
         attrs = self._graph.edges[parent, child]
         return Relationship(parent_data=parent, child_data=child, **attrs)
 
+    def list_relationships(self) -> list[Relationship]:
+        """list : List all relationships defined in this tree."""
+        result = []
+        for e in self._graph.edges:
+            result.append(self._get_relationship(e))
+        return result
+
     def add_dataset(self, name, dataset, relationships=(), as_root=False):
         """
         Add a new Dataset node to this DataTree.
 
         Parameters
         ----------
         name : str
@@ -560,27 +598,27 @@
                 else:
                     self.add_dataset(k, v)
         else:
             raise ValueError("add_items requires Sequence or Mapping")
 
     @property
     def root_node(self):
-        return self._graph.nodes[self.root_node_name]
+        return self._graph.nodes[self.root_node_name_str]
 
     @property
     def root_dataset(self):
-        return self._graph.nodes[self.root_node_name]["dataset"]
+        return self._graph.nodes[self.root_node_name_str]["dataset"]
 
     @root_dataset.setter
     def root_dataset(self, x):
         from .dataset import Dataset
 
         if not isinstance(x, Dataset):
             x = construct(x)
-        if self.root_node_name in self.replacement_filters:
+        if self.root_node_name_str in self.replacement_filters:
             x = self.replacement_filters[self.root_node_name](x)
         self._graph.nodes[self.root_node_name]["dataset"] = x
 
     def _get_relationship(self, edge):
         return Relationship(
             parent_data=edge[0], child_data=edge[1], **self._graph.edges[edge]
         )
@@ -626,24 +664,36 @@
                     item, include_blank_dims=True, dim_names_from_top=True
                 )
             except KeyError:
                 if default is None:
                     raise
                 else:
                     result = xr.DataArray(default)
-        root_dataset = self.root_dataset
-        if result.dims != self.root_dims and broadcast:
-            result, _ = xr.broadcast(result, root_dataset)
-        if coords:
-            add_coords = {}
-            for i in result.dims:
-                if i not in result.coords and i in root_dataset.coords:
-                    add_coords[i] = root_dataset.coords[i]
-            if add_coords:
-                result = result.assign_coords(add_coords)
+        if self.root_node_name:
+            root_dataset = self.root_dataset
+            if result.dims != self.root_dims and broadcast:
+                result, _ = xr.broadcast(result, root_dataset)
+            if coords:
+                add_coords = {}
+                for i in result.dims:
+                    if i not in result.coords and i in root_dataset.coords:
+                        add_coords[i] = root_dataset.coords[i]
+                if add_coords:
+                    result = result.assign_coords(add_coords)
+        elif self.root_node_name is False:
+            if "." in item:
+                item_in, item = item.split(".", 1)
+                base_dataset = self._graph.nodes[item_in]["dataset"]
+                if coords:
+                    add_coords = {}
+                    for i in result.dims:
+                        if i not in result.coords and i in base_dataset.coords:
+                            add_coords[i] = base_dataset.coords[i]
+                    if add_coords:
+                        result = result.assign_coords(add_coords)
         return result
 
     def finditem(self, item, maybe_in=None):
         if maybe_in is not None and maybe_in in self._graph.nodes:
             dataset = self._graph.nodes[maybe_in].get("dataset", {})
             if item in dataset:
                 return maybe_in
@@ -661,19 +711,25 @@
         if isinstance(item, (list, tuple)):
             from .dataset import Dataset
 
             return Dataset({k: self[k] for k in item})
 
         if "." in item:
             item_in, item = item.split(".", 1)
+            queue = [self.root_node_name]
+            if self.root_node_name is False:
+                # when root_node_name is False, we don't want to broadcast
+                # back to the root, but instead only to the given `item_in`
+                queue = [item_in]
+                item_in = None
         else:
             item_in = None
-
-        queue = [self.root_node_name]
+            queue = [self.root_node_name_str]
         examined = set()
+        start_from = queue[0]
         while len(queue):
             current_node = queue.pop(0)
             if current_node in examined:
                 continue
             dataset = self._graph.nodes[current_node].get("dataset", {})
             try:
                 by_name = item in dataset and not only_dims
@@ -682,15 +738,15 @@
             try:
                 by_dims = not by_name and include_blank_dims and (item in dataset.dims)
             except TypeError:
                 by_dims = False
             if (by_name or by_dims) and (item_in is None or item_in == current_node):
                 if just_node_name:
                     return current_node
-                if current_node == self.root_node_name:
+                if current_node == start_from:
                     if by_dims:
                         return xr.DataArray(
                             pd.RangeIndex(dataset.dims[item]), dims=item
                         )
                     else:
                         return dataset[item]
                 else:
@@ -707,27 +763,27 @@
                             coords=coords,
                         )
                     else:
                         result = dataset[item]
                     dims_in_result = set(result.dims)
                     top_dim_names = {}
                     for path in nx.algorithms.simple_paths.all_simple_edge_paths(
-                        self._graph, self.root_node_name, current_node
+                        self._graph, start_from, current_node
                     ):
                         if dim_names_from_top:
                             e = path[0]
                             top_dim_name = self._graph.edges[e].get("parent_name")
-                            root_dataset = self.root_dataset
+                            start_dataset = self._graph.nodes[start_from]["dataset"]
                             # deconvert digitized dim names back to native dims
                             if (
-                                top_dim_name not in root_dataset.dims
-                                and top_dim_name in root_dataset.variables
+                                top_dim_name not in start_dataset.dims
+                                and top_dim_name in start_dataset.variables
                             ):
-                                if root_dataset.variables[top_dim_name].ndim == 1:
-                                    top_dim_name = root_dataset.variables[
+                                if start_dataset.variables[top_dim_name].ndim == 1:
+                                    top_dim_name = start_dataset.variables[
                                         top_dim_name
                                     ].dims[0]
                         else:
                             top_dim_name = None
                         path_dim = self._graph.edges[path[-1]].get("child_name")
                         if path_dim not in dims_in_result:
                             continue
@@ -824,14 +880,16 @@
                 )
             elif engine == "numexpr":
                 from xarray import DataArray
 
                 result = DataArray(
                     pd.eval(expression, resolvers=[self], engine="numexpr"),
                 )
+            else:
+                raise ValueError(f"unknown engine {engine}") from None
         return result
 
     @property
     def subspaces(self):
         """Mapping[str,Dataset] : Direct access to node Dataset objects by name."""
         spaces = {}
         for k in self._graph.nodes:
@@ -842,35 +900,71 @@
 
     def subspaces_iter(self):
         for k in self._graph.nodes:
             s = self._graph.nodes[k].get("dataset", None)
             if s is not None:
                 yield (k, s)
 
+    def contains_subspace(self, key) -> bool:
+        """
+        Is this named Dataset in this tree's subspaces
+
+        Parameters
+        ----------
+        key : str
+
+        Returns
+        -------
+        bool
+        """
+        return key in self._graph.nodes
+
+    def get_subspace(self, key, default_empty=False) -> xr.Dataset:
+        """
+        Access named Dataset from this tree's subspaces
+
+        Parameters
+        ----------
+        key : str
+        default_empty : bool, default False
+            Return an empty Dataset if the key is not found.
+
+        Returns
+        -------
+        xr.Dataset
+        """
+        result = self._graph.nodes[key].get("dataset", None)
+        if result is None:
+            if default_empty:
+                result = xr.Dataset()
+            else:
+                raise KeyError(key)
+        return result
+
     def namespace_names(self):
         namespace = set()
         for spacename, spacearrays in self.subspaces_iter():
-            for k, arr in spacearrays.coords.items():
+            for k, _arr in spacearrays.coords.items():
                 namespace.add(f"__{spacename or 'base'}__{k}")
-            for k, arr in spacearrays.items():
+            for k, _arr in spacearrays.items():
                 if k.startswith("_s_"):
                     namespace.add(f"__{spacename or 'base'}__{k}__indptr")
                     namespace.add(f"__{spacename or 'base'}__{k}__indices")
                     namespace.add(f"__{spacename or 'base'}__{k}__data")
                 else:
                     namespace.add(f"__{spacename or 'base'}__{k}")
         return namespace
 
     @property
     def dims(self):
         """
         Mapping from dimension names to lengths across all dataset nodes.
         """
         dims = {}
-        for k, v in self.subspaces_iter():
+        for _k, v in self.subspaces_iter():
             for name, length in v.dims.items():
                 if name in dims:
                     if dims[name] != length:
                         raise ValueError(
                             "inconsistent dimensions\n" + self.dims_detail()
                         )
                 else:
@@ -926,30 +1020,30 @@
             for d in dims:
                 if d in obj.root_dataset.dims:
                     new_root_dataset = new_root_dataset.drop_dims(d)
 
         # remove subspaces that rely on dropped dim
         boot_queue = set()
         booted = set()
-        for (up, dn, n), e in obj._graph.edges.items():
+        for (up, dn, _n), e in obj._graph.edges.items():
             if up == obj.root_node_name:
                 _analog = e.get("analog", "<missing>")
                 if _analog in dims:
                     boot_queue.add(dn)
                 if _analog != "<missing>" and _analog not in new_root_dataset:
                     boot_queue.add(dn)
                 if e.get("parent_name", "<missing>") in dims:
                     boot_queue.add(dn)
                 if e.get("parent_name", "<missing>") not in new_root_dataset:
                     boot_queue.add(dn)
 
         while boot_queue:
             b = boot_queue.pop()
             booted.add(b)
-            for (up, dn, n), e in obj._graph.edges.items():
+            for (up, dn, _n) in obj._graph.edges.keys():
                 if up == b:
                     boot_queue.add(dn)
 
         edges_to_remove = [e for e in obj._graph.edges if e[1] in booted]
         obj._graph.remove_edges_from(edges_to_remove)
         obj._graph.remove_nodes_from(booted)
 
@@ -983,15 +1077,16 @@
         for k in sorted(dims):
             result_k = obj._getitem(k, include_blank_dims=True, only_dims=True)
             if result_shape is None:
                 result_shape = result_k.shape
             if result_shape != result_k.shape:
                 if check_shapes:
                     raise ValueError(
-                        f"inconsistent index shapes {result_k.shape} v {result_shape} (probably an error on {k} or {sorted(dims)[0]})"
+                        f"inconsistent index shapes {result_k.shape} v {result_shape} "
+                        f"(probably an error on {k} or {sorted(dims)[0]})"
                     )
             result[k] = result_k
 
         if as_dict:
             result = {k: _dataarray_to_numpy(v) for k, v in result.items()}
         else:
             result = Dataset(result)
@@ -1070,14 +1165,15 @@
         parallel=True,
         readme=None,
         flow_library=None,
         extra_hash_data=(),
         write_hash_audit=True,
         hashing_level=1,
         dim_exclude=None,
+        with_root_node_name=None,
     ):
         """
         Set up a new Flow for analysis using the structure of this DataTree.
 
         Parameters
         ----------
         definition_spec : Dict[str,str]
@@ -1154,14 +1250,15 @@
             flow_library=flow_library,
             extra_hash_data=extra_hash_data,
             hashing_level=hashing_level,
             error_model=error_model,
             write_hash_audit=write_hash_audit,
             dim_order=self.dim_order,
             dim_exclude=dim_exclude,
+            with_root_node_name=with_root_node_name,
         )
 
     def _spill(self, all_name_tokens=()):
         """
         Write backup code for sharrow-lite.
 
         Parameters
@@ -1233,21 +1330,26 @@
                 c_dataset = obj._graph.nodes[r.child_data].get("dataset", None)
 
                 upstream = p_dataset[r.parent_name]
                 downstream = c_dataset[r.child_name]
 
                 # vectorize version
                 mapper = {i: j for (j, i) in enumerate(_dataarray_to_numpy(downstream))}
+
+                def mapper_get(x, mapper=mapper):
+                    return mapper.get(x, 0)
+
                 if upstream.size:
-                    offsets = xr.apply_ufunc(np.vectorize(mapper.get), upstream)
+                    offsets = xr.apply_ufunc(np.vectorize(mapper_get), upstream)
                 else:
                     offsets = xr.DataArray([], dims=["index"])
                 if offsets.dtype.kind != "i":
                     warnings.warn(
                         f"detected missing values in digitizing {r.parent_data}.{r.parent_name}",
+                        stacklevel=2,
                     )
 
                 # candidate name for write back
                 r_parent_name_new = (
                     f"{self._BY_OFFSET}{r.parent_name}_{r.child_data}_{r.child_name}"
                 )
 
@@ -1349,37 +1451,48 @@
                     spacearrayname=spacearrayname,
                     exclude_dims=exclude_dims,
                     blends=blends,
                 )
                 try:
                     upside = ", ".join(unparse(t) for t in upside_ast)
                 except:  # noqa: E722
-                    for t in upside_ast:
-                        str_t = str(t)
-                        if len(str_t) < 2000:
-                            print(f"t:{str_t}")
-                        else:
-                            print(f"t:{str_t[:200]}...")
-                    raise
-
-                # check for redirection target
-                if retarget is not None:
-                    tokens.append(
-                        f"__{spacename}___digitized_{retarget}_of_{this_dim_name}[__{parent_data}__{parent_name}[{upside}]]"
-                    )
-                else:
-                    tokens.append(f"__{parent_data}__{parent_name}[{upside}]")
+                    if self.root_node_name is False:
+                        upside = None
+                    else:
+                        print(f"{parent_data=}")
+                        print(f"{parent_name=}")
+                        print(f"{spacearrayname=}")
+                        print(f"{exclude_dims=}")
+                        print(f"{blends=}")
+                        for t in upside_ast:
+                            str_t = str(t)
+                            if len(str_t) < 2000:
+                                print(f"t:{str_t}")
+                            else:
+                                print(f"t:{str_t[:200]}...")
+                        raise
+                if upside is not None:
+                    # check for redirection target
+                    if retarget is not None:
+                        tokens.append(
+                            f"__{spacename}___digitized_{retarget}_of_{this_dim_name}[__{parent_data}__{parent_name}[{upside}]]"
+                        )
+                    else:
+                        tokens.append(f"__{parent_data}__{parent_name}[{upside}]")
                 found_token = True
                 break
             if not found_token:
                 if dimname in self.subspaces[spacename].indexes:
-                    ix = self.subspaces[spacename].indexes[dimname]
-                    ix = {i: n for n, i in enumerate(ix)}
-                    tokens.append(ix)
-                    n_missing_tokens += 1
+                    if self.root_node_name is False:
+                        tokens.append(False)
+                    else:
+                        ix = self.subspaces[spacename].indexes[dimname]
+                        ix = {i: n for n, i in enumerate(ix)}
+                        tokens.append(ix)
+                        n_missing_tokens += 1
                 elif dimname.endswith("_indices") or dimname.endswith("_indptr"):
                     tokens.append(None)
                     # this dimension corresponds to a blender
 
         if n_missing_tokens > 1:
             raise ValueError("at most one missing dimension is allowed")
         result = []
@@ -1392,15 +1505,15 @@
         return tuple(result), blends
 
     @property
     def coords(self):
         return self.root_dataset.coords
 
     def get_index(self, dim):
-        for spacename, subspace in self.subspaces.items():
+        for _spacename, subspace in self.subspaces.items():
             if dim in subspace.coords:
                 return subspace.indexes[dim]
 
     def copy(self):
         return type(self)(
             self._graph.copy(), self.root_node_name, **self.__shallow_copy_extras()
         )
```

### Comparing `sharrow-2.5.2/sharrow/selectors.py` & `sharrow-2.6.0/sharrow/selectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,17 +123,24 @@
             _all_names = list(_names) + _baggage
             ds = self._obj[_all_names]
         else:
             _baggage = []
             ds = self._obj
         if _load:
             ds = ds.load()
+        if _func == "isel":
+            # remove coordinates, we don't need them for isel
+            ds_ = ds.drop_vars(ds.coords)
+        else:
+            ds_ = ds
+
         if _names:
+
             result = (
-                getattr(ds, _func)(**loaders)
+                getattr(ds_, _func)(**loaders)
                 .digital_encoding.strip(_names)
                 .drop_vars(_baggage)
             )
             for n in _names:
                 if self._obj.redirection.is_blended(n):
                     dims = self._obj[n].dims
                     result[n] = xr.DataArray(
@@ -145,15 +152,15 @@
                         ),
                         dims=result[n].dims,
                     )
             if _name is not None:
                 result = result[_name]
             return result
         else:
-            result = getattr(ds, _func)(**loaders)
+            result = getattr(ds_, _func)(**loaders)
             names = list(result.keys())
             for n in names:
                 if self._obj.redirection.is_blended(n):
                     dims = self._obj[n].dims
                     result[n] = xr.DataArray(
                         self._obj.redirection.get_blended(
                             n,
@@ -198,33 +205,51 @@
     """
 
     def __call__(
         self, *, _name=None, _names=None, _load=False, _index_name=None, **idxs
     ):
         modified_idxs = {}
         raw_idxs = {}
+
+        keep_raw_idxs = False
+        is_it_blended = []
+        if isinstance(_name, str):
+            is_it_blended = [_name]
+        elif _names is not None:
+            is_it_blended = _names
+        for n in is_it_blended:
+            try:
+                if self._obj.redirection.is_blended(n):
+                    keep_raw_idxs = True
+            except AttributeError:
+                keep_raw_idxs = True
+
         for k, v in idxs.items():
             target = self._obj.redirection.target(k)
             if target is None:
-                raw_idxs[k] = modified_idxs[k] = v
+                modified_idxs[k] = v
+                if keep_raw_idxs:
+                    raw_idxs[k] = v
             else:
                 v_ = np.asarray(v)
                 modified_idxs[target] = self._obj[f"_digitized_{target}_of_{k}"][
                     v_
                 ].to_numpy()
-                raw_idxs[target] = v_  # self._obj[k][v_].to_numpy()
-        return self._filter(
+                if keep_raw_idxs:
+                    raw_idxs[target] = v_  # self._obj[k][v_].to_numpy()
+        out = self._filter(
             _name=_name,
             _names=_names,
             _load=_load,
             _index_name=_index_name,
             _func="isel",
             _raw_idxs=raw_idxs,
             **modified_idxs,
         )
+        return out
 
 
 @xr.register_dataset_accessor("at")
 class _At_Accessor(_Df_Accessor):
     """
     Multi-dimensional fancy indexing by label.
```

### Comparing `sharrow-2.5.2/sharrow/shared_memory.py` & `sharrow-2.6.0/sharrow/shared_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         try:
             result = SharedMemory(
                 name=h,
                 create=True,
                 size=size,
             )
         except FileExistsError:
-            raise FileExistsError(f"sharrow_shared_memory_array:{key}")
+            raise FileExistsError(f"sharrow_shared_memory_array:{key}") from None
         __GLOBAL_MEMORY_ARRAYS[key] = result
         return result
 
     if backing.startswith("memmap:"):
         logger.info(f"create_shared_memory_array:{key} ({backing}, {si_units(size)})")
         mmap_filename = backing[7:]
         if os.path.isfile(mmap_filename):
@@ -134,15 +134,15 @@
         h = _hexhash(f"sharrow__{key}")
         try:
             result = SharedMemory(
                 name=h,
                 create=False,
             )
         except FileNotFoundError:
-            raise FileNotFoundError(f"sharrow_shared_memory_array:{key}")
+            raise FileNotFoundError(f"sharrow_shared_memory_array:{key}") from None
         else:
             logger.info(
                 f"shared memory array from ephemeral memory, {si_units(result.size)}"
             )
             return result
 
     if backing.startswith("memmap:"):
@@ -171,42 +171,42 @@
             raise FileExistsError(f"sharrow_shared_memory_list:{key}")
         try:
             result = ShareableList(
                 content,
                 name=h,
             )
         except FileExistsError:
-            raise FileExistsError(f"sharrow_shared_memory_list:{key}")
+            raise FileExistsError(f"sharrow_shared_memory_list:{key}") from None
         __GLOBAL_MEMORY_LISTS[key] = result
         return result
 
 
 def read_shared_list(key):
     if key.startswith("memmap:"):
         mmap_filename = key[7:]
         with open(mmap_filename + ".meta.pkl", mode="rb") as f:
             return pickle.load(f)
     else:
         logger.info(f"read_shared_list:{key}")
         try:
             sl = ShareableList(name=_hexhash(f"sharrow__list__{key}"))
         except FileNotFoundError:
-            raise FileNotFoundError(f"sharrow_shared_memory_list:{key}")
+            raise FileNotFoundError(f"sharrow_shared_memory_list:{key}") from None
         else:
             return sl
 
 
 def get_shared_list_nbytes(key):
     if key.startswith("memmap:"):
         return 0
     h = _hexhash(f"sharrow__list__{key}")
     try:
         shm = SharedMemory(name=h, create=False)
     except FileNotFoundError:
-        raise FileNotFoundError(f"sharrow_shared_memory_list:{key}")
+        raise FileNotFoundError(f"sharrow_shared_memory_list:{key}") from None
     else:
         return shm.size
 
 
 def delete_shared_memory_files(key):
     if key.startswith("memmap:"):
         logger.info(f"delete_shared_memory_files:{key}")
@@ -393,15 +393,15 @@
         return type(self).from_shared_memory(key, own_data=mem, mode=mode)
 
     @property
     def shared_memory_key(self):
         try:
             return self._shared_memory_key_
         except AttributeError:
-            raise ValueError("this dataset is not in shared memory")
+            raise ValueError("this dataset is not in shared memory") from None
 
     @classmethod
     def from_shared_memory(cls, key, own_data=False, mode="r+"):
         """
         Connect to an existing Dataset in shared memory.
 
         Parameters
@@ -427,15 +427,15 @@
         shr_list = read_shared_list(key)
         try:
             _shared_memory_objs_.append(shr_list.shm)
         except AttributeError:
             # for memmap, list is loaded from pickle, not shared ram
             pass
 
-        if own_data and not (own_data is True):
+        if own_data and own_data is not True:
             mem = own_data
             own_data = True
         else:
             mem = open_shared_memory_array(key, mode=mode)
         _shared_memory_objs_.append(mem)
         if key.startswith("memmap:"):
             buffer = memoryview(mem)
@@ -509,15 +509,15 @@
 
     @property
     def shared_memory_size(self):
         """int : Size (in bytes) in shared memory, raises ValueError if not shared."""
         try:
             return sum(i.size for i in self._shared_memory_objs_)
         except AttributeError:
-            raise ValueError("this dataset is not in shared memory")
+            raise ValueError("this dataset is not in shared memory") from None
 
     @property
     def is_shared_memory(self):
         """bool : Whether this Dataset is in shared memory."""
         try:
             return sum(i.size for i in self._shared_memory_objs_) > 0
         except AttributeError:
```

### Comparing `sharrow-2.5.2/sharrow/sparse.py` & `sharrow-2.6.0/sharrow/sparse.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/table.py` & `sharrow-2.6.0/sharrow/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,26 +253,31 @@
         if not os.path.isdir(path):
             raise NotADirectoryError(path)
         if blockname is not None:
             if isinstance(blockname, int):
                 stopper = blockname
             else:
                 qlog = os.path.join(path, "quilt.log")
-                with open(qlog, "rt") as logreader:
+                with open(qlog) as logreader:
                     existing_info = yaml.safe_load(logreader)
-                for stopper, block in enumerate(existing_info):
+                for _stopper, block in enumerate(existing_info):
                     if block.get("name", None) == blockname:
                         break
                 else:
                     raise KeyError(blockname)
         else:
             stopper = 1e99
         n = 0
-        rowfile = lambda n: os.path.join(path, f"block.{n:03d}.rows")
-        colfile = lambda n: os.path.join(path, f"block.{n:03d}.cols")
+
+        def rowfile(n):
+            return os.path.join(path, f"block.{n:03d}.rows")
+
+        def colfile(n):
+            return os.path.join(path, f"block.{n:03d}.cols")
+
         builder = None
         look = True
         while look and n <= stopper:
             look = False
             if os.path.exists(rowfile(n)):
                 i = pf.read_table(rowfile(n))
                 if builder is None:
@@ -287,29 +292,29 @@
                 else:
                     builder = builder | i
                 look = True
             if look:
                 n += 1
         if builder is not None:
             metadata = builder.schema.metadata
-            metadata[b"quilt_number"] = f"{n}".encode("utf8")
+            metadata[b"quilt_number"] = f"{n}".encode()
             return builder.replace_schema_metadata(metadata)
         return None
 
     def to_quilt(self, path, blockname=None):
         if not os.path.exists(path):
             os.makedirs(path)
         qlog = os.path.join(path, "quilt.log")
 
         if not os.path.exists(qlog):
             ex_rows = 0
             ex_cols = []
             max_block = -1
         else:
-            with open(qlog, "rt") as logreader:
+            with open(qlog) as logreader:
                 existing_info = yaml.safe_load(logreader)
             ex_rows = sum(block.get("rows", 0) for block in existing_info)
             ex_cols = sum((block.get("cols", []) for block in existing_info), [])
             max_block = max(block["block"] for block in existing_info)
 
         with open(qlog, "a") as f:
             quilt_number = max_block + 1
```

### Comparing `sharrow-2.5.2/sharrow/tests/test_nesting.py` & `sharrow-2.6.0/sharrow/tests/test_nesting.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_get.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_get.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_isin.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_isin.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_isin_and_between.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_isin_and_between.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_joint_dict_encoded.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_joint_dict_encoded.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_mixed_dtypes.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_mixed_dtypes.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_nested_where.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_nested_where.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_shared_data.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_shared_data.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_shared_data_2.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_shared_data_2.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_shared_data_reversible.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_shared_data_reversible.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_tuple_slice.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_tuple_slice.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships/test_with_2d_base.csv` & `sharrow-2.6.0/sharrow/tests/test_relationships/test_with_2d_base.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/tests/test_relationships.py` & `sharrow-2.6.0/sharrow/tests/test_relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 @fixture
 def skims():
     return example_data.get_skims()
 
 
 def test_shared_data(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         skims=skims,
         relationships=(
             "base.otaz_idx->skims.otaz",
             "base.dtaz_idx->skims.dtaz",
             "base.timeperiod5->skims.time_period",
@@ -71,15 +70,14 @@
         }
     )
     result2 = s2._load(tree, as_dataframe=True)
     dataframe_regression.check(result2, basename="test_shared_data_2")
 
 
 def test_subspace_fallbacks(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         skims=skims,
         relationships=(
             "base.otaz_idx->skims.otaz",
             "base.dtaz_idx->skims.dtaz",
             "base.timeperiod5->skims.time_period",
@@ -117,15 +115,14 @@
         }
     )
     result3 = flow3._load(tree, as_dataframe=True)
     dataframe_regression.check(result3, basename="test_shared_data_2")
 
 
 def test_shared_data_reversible(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         odt_skims=skims,
         dot_skims=skims,
         relationships=(
             "base.otaz_idx->odt_skims.otaz",
             "base.dtaz_idx->odt_skims.dtaz",
@@ -283,15 +280,14 @@
     )
 
     check_vs = np.dot(result, np.ones([6])).reshape(5000, 25)
     np.testing.assert_array_almost_equal(check_vs, dot_result.to_numpy())
 
 
 def test_mixed_dtypes(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         skims=skims,
         relationships=(
             "base.otaz_idx->skims.otaz",
             "base.dtaz_idx->skims.dtaz",
             "base.timeperiod5->skims.time_period",
@@ -368,15 +364,14 @@
     q.put(skims_.SOV_TIME.sum())
 
 
 @mark.skipif(
     sys.version_info < (3, 8), reason="shared memory requires python3.8 or higher"
 )
 def test_shared_memory(skims):
-
     token = "skims" + secrets.token_hex(5)
 
     skims_2 = skims.shm.to_shared_memory(token)
     target = skims.SOV_TIME.sum()
     assert skims_2.SOV_TIME.sum() == target
 
     # reconstruct in same process
@@ -406,15 +401,14 @@
     assert r.parent_name == "ff"
     assert r.child_data == "Gg"
     assert r.child_name == "hh"
     assert r.indexing == "label"
 
 
 def test_replacement_filters(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         skims=skims,
         relationships=(
             "base.otaz_idx->skims.otaz",
             "base.dtaz_idx->skims.dtaz",
             "base.timeperiod5->skims.time_period",
@@ -444,15 +438,14 @@
     result = ss._load(
         ss.tree.replace_datasets(base=households_malformed), as_dataframe=True
     )
     dataframe_regression.check(result, basename="test_shared_data")
 
 
 def test_name_in_wrong_subspace(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         skims=skims,
         relationships=(
             "base.otaz_idx->skims.otaz",
             "base.dtaz_idx->skims.dtaz",
             "base.timeperiod5->skims.time_period",
@@ -513,15 +506,14 @@
         }
     )
     result = ss_undot._load(tree, as_dataframe=True)
     dataframe_regression.check(result, basename="test_shared_data")
 
 
 def test_shared_data_encoded(dataframe_regression, households, skims):
-
     households = sharrow.dataset.construct(households).digital_encoding.set(
         "income",
         bitwidth=32,
         scale=0.001,
     )
 
     tree = DataTree(
@@ -604,15 +596,14 @@
         extra_hash_data=("joint",),
     )
     arr1 = flow1.load_dataframe()
     dataframe_regression.check(arr1)
 
 
 def test_isin_and_between(dataframe_regression):
-
     data = example_data.get_data()
     persons = data["persons"]
 
     tree = DataTree(
         base=persons,
         extra_vars={
             "pt1": 1,
@@ -687,15 +678,14 @@
         result["pt"].between(3, 5).astype(np.float32).where(mask, np.nan),
         result["pt_tween_35"],
         check_names=False,
     )
 
 
 def test_nested_where(dataframe_regression):
-
     data = example_data.get_data()
     base = persons = data["persons"]
 
     tree = DataTree(
         base=persons,
         extra_vars={
             "pt1": 1,
@@ -809,15 +799,14 @@
         }
     )
     result = qf.load()
     assert result == approx(np.asarray([[0, 0, 1, 1]]).T)
 
 
 def test_get(dataframe_regression, households, skims):
-
     tree = DataTree(
         base=households,
         skims=skims,
         relationships=(
             "base.otaz_idx->skims.otaz",
             "base.dtaz_idx->skims.dtaz",
             "base.timeperiod5->skims.time_period",
@@ -880,16 +869,16 @@
     dataframe_regression.check(result)
 
     # test get when inside another function
     flow5 = tree.setup_flow(
         {
             "income": "np.power(base.get('income', default=0) + df.get('missing_one', 0), 1)",
             "sov_time_by_income": "skims.SOV_TIME/np.power(base.get('income', default=0), 1)",
-            "missing_data": "np.where(np.isnan(df.get('missing_data', default=1)), 0, df.get('missing_data', default=-1))",
-            "missing_skim": "(np.where(np.isnan(df.get('num_escortees', np.nan)), -2 , df.get('num_escortees', np.nan)))",
+            "missing_data": "np.where(np.isnan(df.get('missing_data', default=1)), 0, df.get('missing_data', default=-1))",  # noqa: E501
+            "missing_skim": "(np.where(np.isnan(df.get('num_escortees', np.nan)), -2 , df.get('num_escortees', np.nan)))",  # noqa: E501
             "sov_time_by_income_2": "skims.get('SOV_TIME', default=0)/base.income",
             "sov_cost_by_income_2": "skims.get('HOV3_TIME', default=999)",
         },
     )
     result = flow5._load(tree, as_dataframe=True)
     assert "__skims__HOV3_TIME:True" in flow5._optional_get_tokens
     assert "__df__missing_data:False" in flow5._optional_get_tokens
```

### Comparing `sharrow-2.5.2/sharrow/translate.py` & `sharrow-2.6.0/sharrow/translate.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/viz.py` & `sharrow-2.6.0/sharrow/viz.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow/wrappers.py` & `sharrow-2.6.0/sharrow/wrappers.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.5.2/sharrow.egg-info/SOURCES.txt` & `sharrow-2.6.0/sharrow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 envs/development.yml
 envs/testing.yml
 sharrow/__init__.py
 sharrow/_infer_version.py
 sharrow/_version.py
 sharrow/accessors.py
 sharrow/aster.py
+sharrow/categorical.py
 sharrow/dataset.py
+sharrow/datastore.py
 sharrow/debug.py
 sharrow/digital_encoding.py
 sharrow/example_data.py
 sharrow/filewrite.py
 sharrow/flows.py
 sharrow/logging.py
 sharrow/maths.py
@@ -580,22 +582,27 @@
 sharrow/example_data/skims.zarr/otaz/.zarray
 sharrow/example_data/skims.zarr/otaz/.zattrs
 sharrow/example_data/skims.zarr/otaz/0
 sharrow/example_data/skims.zarr/time_period/.zarray
 sharrow/example_data/skims.zarr/time_period/.zattrs
 sharrow/example_data/skims.zarr/time_period/0
 sharrow/tests/__init__.py
+sharrow/tests/conftest.py
+sharrow/tests/test_categorical.py
 sharrow/tests/test_datasets.py
+sharrow/tests/test_datastore.py
 sharrow/tests/test_nesting.py
 sharrow/tests/test_relationships.py
 sharrow/tests/test_relationships/test_dict_encoded.csv
 sharrow/tests/test_relationships/test_get.csv
 sharrow/tests/test_relationships/test_isin.csv
 sharrow/tests/test_relationships/test_isin_and_between.csv
 sharrow/tests/test_relationships/test_joint_dict_encoded.csv
 sharrow/tests/test_relationships/test_mixed_dtypes.csv
 sharrow/tests/test_relationships/test_nested_where.csv
 sharrow/tests/test_relationships/test_shared_data.csv
 sharrow/tests/test_relationships/test_shared_data_2.csv
 sharrow/tests/test_relationships/test_shared_data_reversible.csv
 sharrow/tests/test_relationships/test_tuple_slice.csv
-sharrow/tests/test_relationships/test_with_2d_base.csv
+sharrow/tests/test_relationships/test_with_2d_base.csv
+sharrow/utils/__init__.py
+sharrow/utils/tar_zst.py
```

