# Comparing `tmp/dataspace-0.0.8.tar.gz` & `tmp/dataspace-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspace-0.0.8.tar", last modified: Sat Feb  4 15:33:26 2023, max compression
+gzip compressed data, was "dataspace-0.0.9.tar", last modified: Fri Feb 10 11:10:50 2023, max compression
```

## Comparing `dataspace-0.0.8.tar` & `dataspace-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1061 2023-02-03 10:55:25.000000 dataspace-0.0.8/LICENSE
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1356 2023-02-04 15:33:26.993226 dataspace-0.0.8/PKG-INFO
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      800 2023-02-04 14:24:14.000000 dataspace-0.0.8/README.md
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.989226 dataspace-0.0.8/dataspace/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      244 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/__init__.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.989226 dataspace-0.0.8/dataspace/calculations/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       58 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/calculations/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     3524 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/calculations/diff.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       43 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/calculations/regression.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.989226 dataspace-0.0.8/dataspace/charts/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       61 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/__init__.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.989226 dataspace-0.0.8/dataspace/charts/altair/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      118 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/altair/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     7541 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/altair/altair.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     7468 2023-02-04 15:30:43.000000 dataspace-0.0.8/dataspace/charts/altair/charts.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     2108 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/base.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/charts/bokeh/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      137 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/bokeh/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     3129 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/bokeh/bokeh.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     4396 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/charts/bokeh/charts.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/clean/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      420 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/clean/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      877 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/clean/convert.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1864 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/clean/dates.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      854 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/clean/nulls.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1173 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/clean/values.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/core/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       53 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/core/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)    32737 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/core/core.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      405 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/core/env.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1814 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/core/load.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/count/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       77 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/count/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1381 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/count/count.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/info/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       48 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/info/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      328 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/info/info.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1022 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/info/view.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/io/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)        0 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/io/__init__.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/io/export/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      398 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/io/export/__init__.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/report/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       59 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/report/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     2138 2023-02-04 15:24:26.000000 dataspace-0.0.8/dataspace/report/base.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/transform/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      182 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/transform/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      710 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/transform/dataframe.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1570 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/transform/resample.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      724 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/transform/values.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      370 2023-02-04 14:08:48.000000 dataspace-0.0.8/dataspace/types.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.993226 dataspace-0.0.8/dataspace/utils/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)        0 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/utils/__init__.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     2047 2023-02-03 10:55:25.000000 dataspace-0.0.8/dataspace/utils/colors.py
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     2102 2023-02-03 19:19:24.000000 dataspace-0.0.8/dataspace/utils/messages.py
-drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-04 15:33:26.989226 dataspace-0.0.8/dataspace.egg-info/
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1356 2023-02-04 15:33:26.000000 dataspace-0.0.8/dataspace.egg-info/PKG-INFO
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1306 2023-02-04 15:33:26.000000 dataspace-0.0.8/dataspace.egg-info/SOURCES.txt
--rw-rw-r--   0 ggg       (1000) ggg       (1000)        1 2023-02-04 15:33:26.000000 dataspace-0.0.8/dataspace.egg-info/dependency_links.txt
--rw-rw-r--   0 ggg       (1000) ggg       (1000)        1 2023-02-04 14:10:51.000000 dataspace-0.0.8/dataspace.egg-info/not-zip-safe
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       24 2023-02-04 15:33:26.000000 dataspace-0.0.8/dataspace.egg-info/requires.txt
--rw-rw-r--   0 ggg       (1000) ggg       (1000)       10 2023-02-04 15:33:26.000000 dataspace-0.0.8/dataspace.egg-info/top_level.txt
--rw-rw-r--   0 ggg       (1000) ggg       (1000)      157 2023-02-04 15:33:26.993226 dataspace-0.0.8/setup.cfg
--rw-rw-r--   0 ggg       (1000) ggg       (1000)     1001 2023-02-04 15:32:58.000000 dataspace-0.0.8/setup.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.122917 dataspace-0.0.9/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1061 2023-02-03 10:55:25.000000 dataspace-0.0.9/LICENSE
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     5217 2023-02-10 11:10:50.122917 dataspace-0.0.9/PKG-INFO
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     4661 2023-02-05 15:52:44.000000 dataspace-0.0.9/README.md
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.114917 dataspace-0.0.9/dataspace/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      244 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/__init__.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/calculations/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       58 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/calculations/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     3524 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/calculations/diff.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       43 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/calculations/regression.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/charts/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       61 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/charts/__init__.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/charts/altair/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      118 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/charts/altair/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     7559 2023-02-09 17:04:16.000000 dataspace-0.0.9/dataspace/charts/altair/altair.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     9250 2023-02-09 17:04:16.000000 dataspace-0.0.9/dataspace/charts/altair/charts.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     2108 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/charts/base.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/charts/bokeh/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      137 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/charts/bokeh/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     3129 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/charts/bokeh/bokeh.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     5037 2023-02-09 17:04:16.000000 dataspace-0.0.9/dataspace/charts/bokeh/charts.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/clean/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      420 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/clean/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      877 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/clean/convert.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1864 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/clean/dates.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      854 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/clean/nulls.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1173 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/clean/values.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/core/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       53 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/core/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)    33806 2023-02-10 10:53:50.000000 dataspace-0.0.9/dataspace/core/core.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      405 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/core/env.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1814 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/core/load.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/count/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       77 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/count/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1381 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/count/count.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/info/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       48 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/info/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      328 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/info/info.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1022 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/info/view.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/io/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)        0 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/io/__init__.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/io/export/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      398 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/io/export/__init__.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.118917 dataspace-0.0.9/dataspace/report/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       59 2023-02-04 14:08:48.000000 dataspace-0.0.9/dataspace/report/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     3611 2023-02-09 17:04:16.000000 dataspace-0.0.9/dataspace/report/base.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.122917 dataspace-0.0.9/dataspace/transform/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      182 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/transform/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      710 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/transform/dataframe.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1570 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/transform/resample.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      724 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/transform/values.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      416 2023-02-09 17:04:16.000000 dataspace-0.0.9/dataspace/types.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.122917 dataspace-0.0.9/dataspace/utils/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)        0 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/utils/__init__.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     2047 2023-02-03 10:55:25.000000 dataspace-0.0.9/dataspace/utils/colors.py
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     2118 2023-02-09 17:04:16.000000 dataspace-0.0.9/dataspace/utils/messages.py
+drwxrwxr-x   0 ggg       (1000) ggg       (1000)        0 2023-02-10 11:10:50.114917 dataspace-0.0.9/dataspace.egg-info/
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     5217 2023-02-10 11:10:50.000000 dataspace-0.0.9/dataspace.egg-info/PKG-INFO
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1306 2023-02-10 11:10:50.000000 dataspace-0.0.9/dataspace.egg-info/SOURCES.txt
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)        1 2023-02-10 11:10:50.000000 dataspace-0.0.9/dataspace.egg-info/dependency_links.txt
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)        1 2023-02-04 14:10:51.000000 dataspace-0.0.9/dataspace.egg-info/not-zip-safe
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       24 2023-02-10 11:10:50.000000 dataspace-0.0.9/dataspace.egg-info/requires.txt
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)       10 2023-02-10 11:10:50.000000 dataspace-0.0.9/dataspace.egg-info/top_level.txt
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)      157 2023-02-10 11:10:50.122917 dataspace-0.0.9/setup.cfg
+-rw-rw-r--   0 ggg       (1000) ggg       (1000)     1001 2023-02-10 11:07:51.000000 dataspace-0.0.9/setup.py
```

### Comparing `dataspace-0.0.8/LICENSE` & `dataspace-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/calculations/diff.py` & `dataspace-0.0.9/dataspace/calculations/diff.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/charts/altair/altair.py` & `dataspace-0.0.9/dataspace/charts/altair/altair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import Dict, Optional, Union
 
 import pandas as pd
 from dataspace.transform import _drop
 
-from altair import Scale, X, Y, data_transformers
+from altair import (
+    Scale,
+    X,
+    Y,
+    data_transformers,
+)
 
 from .charts import AltairChart
 
 data_transformers.disable_max_rows()
 
 
 class AltairChartEngine:
@@ -26,15 +31,15 @@
 
     def chart(
         self,
         df: pd.DataFrame,
         chart_type: str,
         x: Optional[Union[str, X]] = None,
         y: Optional[Union[str, X]] = None,
-        **kwargs
+        **kwargs,
     ) -> AltairChart:
         """
         Get an Altair chart object
         """
         if x is not None and y is not None:
             self.set_axis(x, y)
         self._checkAxis()
@@ -127,15 +132,25 @@
         elif chart_type == "rule":
             chart = (
                 AltairChart(df)
                 .mark_rule(**style)
                 .encode(x=self.x, y=self.y, **encode)
                 .properties(**opts)
             )
-        return chart    
+        return chart
+
+    def set_axis(self, xaxis: Union[str, X], yaxis: Union[str, Y]) -> None:
+        if isinstance(xaxis, X):
+            self.x = xaxis
+        else:
+            self.x = X(xaxis, scale=Scale(zero=False))
+        if isinstance(yaxis, Y):
+            self.y = yaxis
+        else:
+            self.y = Y(yaxis, scale=Scale(zero=False))
 
     def _altair_chart_num_(
         self,
         df: pd.DataFrame,
         chart_type: str,
         opts,
         style,
@@ -203,24 +218,14 @@
         return (
             AltairChart(df)
             .mark_bar(**style)
             .encode(X(self.x.shorthand, bin=True), y="count()", **encode)
             .properties(**opts)
         )
 
-    def set_axis(self, xaxis: Union[str, X], yaxis: Union[str, Y]) -> None:
-        if isinstance(xaxis, X):
-            self.x = xaxis
-        else:
-            self.x = X(xaxis, scale=Scale(zero=False))
-        if isinstance(yaxis, Y):
-            self.y = yaxis
-        else:
-            self.y = Y(yaxis, scale=Scale(zero=False))
-
     def _checkAxis(self) -> None:
         assert self.x is not None and self.y is not None, "Set the chart fields"
 
     def _default_opts(self, opts: Dict) -> Dict:
         if "width" not in opts:
             opts["width"] = self.default_width
         if "height" not in opts:
```

### Comparing `dataspace-0.0.8/dataspace/charts/altair/charts.py` & `dataspace-0.0.9/dataspace/charts/altair/charts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from ctypes import ArgumentError
 from typing import List, Union
+import uuid
 
 from altair import Chart as AltChart
-from altair import Color, Scale, value
+from altair import (
+    Color,
+    Scale,
+    value,
+    VEGA_VERSION,
+    VEGALITE_VERSION,
+    VEGAEMBED_VERSION,
+)
 
 try:
     from altair_saver import save
 except (ModuleNotFoundError, ImportError):
     print("The Altair chart saver is not available in this environment")
 
 
@@ -103,15 +111,15 @@
             ds.area_().color("forestgreen")
 
         :param v: the color value
         :type v: str
         :return: the chart object
         :rtype: Chart
         """
-        return self.configure_mark(color=v)
+        return self.encode(color=value(v))
 
     def opacity(self, v: Union[int, float]) -> "AltairChart":
         """Configure the chart opacity
 
         .. code-block:: python
 
             ds = await load_dataset("sp500")
@@ -259,7 +267,47 @@
     def save_img(self, path: str):
         """Save the chart to a png image
 
         :param path: the filepath
         :type path: str
         """
         save(self, path)
+
+    def get_html_(self) -> str:
+        """
+        Get html for an Altair chart
+        """
+        slug = uuid.uuid4().hex
+        json_data = self.to_json(indent=0)
+        html = '<div id="' + slug + '"></div>\n'
+        html += '<script type="text/javascript">'
+        html += "var spec = " + json_data.replace("\n", "") + ";"
+        html += """
+        var embed_opt = {"mode": "vega-lite"};
+        function showError(altel, error){
+            altel.innerHTML = ('<div class="error">'
+                            + '<p>JavaScript Error: ' + error.message + '</p>'
+                            + "<p>This usually means there's a typo in your "
+                            + "chart specification. "
+                            + "See the javascript console for the full "
+                            + "traceback.</p>"
+                            + '</div>');
+            throw error;
+        };\n"""
+        html += "const el_" + slug + " = document.getElementById('" + slug + "');"
+        html += "vegaEmbed('#" + slug + "', spec, embed_opt)"
+        html += ".catch(error => showError(el_" + slug + ", error));"
+        html += "</script>"
+        return html
+
+    @staticmethod
+    def html_header_():
+        """
+        Returns html script tags for Altair
+        """
+        header = (
+            f'<script src="https://cdn.jsdelivr.net/npm/vega@{VEGA_VERSION}"></script>',
+            f'<script src="https://cdn.jsdelivr.net/npm/vega-lite@{VEGALITE_VERSION}"></script>',
+            f'<script src="https://cdn.jsdelivr.net/npm/vega-embed@{VEGAEMBED_VERSION}"></script>',
+            "<style>.vega-actions {display:none}</style>",
+        )
+        return "\n".join(header)
```

### Comparing `dataspace-0.0.8/dataspace/charts/base.py` & `dataspace-0.0.9/dataspace/charts/base.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/charts/bokeh/bokeh.py` & `dataspace-0.0.9/dataspace/charts/bokeh/bokeh.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/charts/bokeh/charts.py` & `dataspace-0.0.9/dataspace/charts/bokeh/charts.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Tuple, Union
 import holoviews as hv
 from holoviews.core import Store
 from holoviews.util import Dynamic
 from holoviews.element import Chart, Annotation
 from holoviews.plotting import bokeh as plot
 from bokeh.models import HoverTool
+from bokeh.resources import CDN
 
 
 class HvChart(Chart):
     def w(self, v: int):
         self.opts(width=v)
         return self
 
@@ -47,16 +48,16 @@
         self.opts(yaxis=None)
         return self
 
     def title(self, v: str):
         self = self.relabel(v)
         return self
 
-    def tooltip(self, v: Union[str, List[str], List[Tuple[str,str]]]):
-        tt: List[Tuple[str,str]] = []
+    def tooltip(self, v: Union[str, List[str], List[Tuple[str, str]]]):
+        tt: List[Tuple[str, str]] = []
         if isinstance(v, str) is True:
             tt.append((f"{v}", f"@{v}"))
         else:
             for x in v:
                 if isinstance(x, tuple):
                     tt.append(x)
                 else:
@@ -102,15 +103,35 @@
     def save_img(self, path: str):
         """Save the chart to a png image
 
         :param path: the filepath
         :type path: str
         """
         dmap = Dynamic(self)
-        hv.save(dmap, path, fmt='png')
+        hv.save(dmap, path, fmt="png")
+
+    def get_html_(self) -> str:
+        """
+        Get html for a Bokeh chart
+        """
+        renderer = hv.renderer("bokeh")
+        plot = renderer.get_plot(self)
+        html = renderer._figure_data(plot, "html")
+        return html
+
+    @staticmethod
+    def html_header_():
+        """
+        Returns html script tags for Bokeh
+        """
+        url = CDN.js_files[0]
+        tag = f'<script type="text/javascript" src="{url}"></script>'
+        log = '<script type="text/javascript">Bokeh.set_log_level("info")</script>'
+        html_tokens = [tag, log]
+        return "\n".join(html_tokens)
 
 
 class HvAnnotation(Annotation):
     def w(self, v: int):
         self.opts(width=v)
         return self
```

### Comparing `dataspace-0.0.8/dataspace/clean/convert.py` & `dataspace-0.0.9/dataspace/clean/convert.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/clean/dates.py` & `dataspace-0.0.9/dataspace/clean/dates.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/clean/nulls.py` & `dataspace-0.0.9/dataspace/clean/nulls.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/clean/values.py` & `dataspace-0.0.9/dataspace/clean/values.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/core/core.py` & `dataspace-0.0.9/dataspace/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1073,37 +1073,62 @@
 
     def export_csv(self, filepath: str, **kwargs) -> None:
         """
         Write the main dataframe to a csv file
 
         :param filepath: path of the file to save
         :type filepath: str
-        :param \\*\\*kwargs: arguments to pass to ``pd.to_csv``
+        :param **kwargs: arguments to pass to ``pd.to_csv``
 
         :example: `ds.export_csv("myfile.csv", header=false)`
         """
         return export_csv(self.df, filepath, **kwargs)
 
     def report_path(self, path: str):
-        """
-        Set the report path folder
+        """Set the report path folder
+
+        :param path: the path where to save reports: relative or absolute
+        :type path: str
+
+        :example: `ds.report_path("../reports")`
         """
         self._reports.path = path
 
     def stack(
         self,
         chart: ChartType,
         title: Optional[str] = None,
         description: Optional[str] = None,
     ):
-        """
-        Store a chart in the report stack
-        """
-        self._reports.stack(chart, title, description)
-        msg_info("Chart added in the report stack")
+        """Store a chart in the report stack
+
+        :param chart: a chart object
+        :type chart: ChartType
+        :param title: the chart title, defaults to None
+        :type title: Optional[str], optional
+        :param description: the chart description, defaults to None
+        :type description: Optional[str], optional
+        """
+        self._reports.stack(chart, self._charts.engine, title, description)
+        m = "" if not title else title + " "
+        msg_info(f"Chart {m}added in the report stack")
 
     def save_pdf(self, filename: str, clear_stack=True):
-        """
-        Save a report to a pdf file
+        """Save a report to a pdf file
+
+        :param filename: the filename
+        :type filename: str
+        :param clear_stack: clear the reporting stack, defaults to True
+        :type clear_stack: bool, optional
         """
         self._reports.save_pdf(filename, clear_stack)
-        msg_info("Pdf file saved")
+        msg_ok("Pdf file saved")
+
+    def save_html(self, info=False, clear_stack=True):
+        """Save a report to multiple html files, one per stacked item
+
+        :param info: print info about the html headers, defaults to False
+        :type info: bool, optional
+        :param clear_stack: clear the reporting stack, defaults to True
+        :type clear_stack: bool, optional
+        """
+        self._reports.save_html(info, clear_stack)
```

### Comparing `dataspace-0.0.8/dataspace/core/load.py` & `dataspace-0.0.9/dataspace/core/load.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/count/count.py` & `dataspace-0.0.9/dataspace/count/count.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/info/view.py` & `dataspace-0.0.9/dataspace/info/view.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/report/base.py` & `dataspace-0.0.9/dataspace/report/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 import os
 import uuid
 from typing import List, Optional
 
+from slugify import slugify
+
 try:
     from fpdf import FPDF
 except (ModuleNotFoundError, ImportError):
     print("The pdf reporting engine is not available in this environment")
 
 
-from dataspace.types import ReportItemType, ChartType
-from dataspace.utils.messages import msg_info, msg_ok
+from dataspace.types import ChartEngineName, ReportItemType, ChartType
+from dataspace.utils.messages import msg_end, msg_info, msg_ok, msg_start
+from dataspace.charts.altair.charts import AltairChart
+from dataspace.charts.bokeh.charts import HvChart
 
 
 class ReportEngine:
     """
     Class to handle reporting
     """
 
     path: str = ""
     items: List[ReportItemType] = []
+    has_altair_chart = False
+    has_bokeh_chart = False
 
     def stack(
         self,
         chart: ChartType,
+        chart_engine: ChartEngineName,
         title: Optional[str] = None,
         description: Optional[str] = None,
     ):
         """
         Store a chart in the report stack
         """
-        self.items.append(ReportItemType(chart, title, description))
+        id = uuid.uuid4().hex
+        if title is not None:
+            id = slugify(title)
+        self.items.append(ReportItemType(id, chart, chart_engine, title, description))
+        if chart_engine == "altair":
+            self.has_altair_chart = True
+        elif chart_engine == "bokeh":
+            self.has_bokeh_chart = True
 
     def save_pdf(self, filename: str, clear_stack=True):
         """
         Save a report to a pdf file
         """
         if self.path == "":
             raise ValueError("Please set a report path first")
@@ -41,35 +55,62 @@
         pdf.add_page()
         pdf.set_font("helvetica", size=12)
         imgs = []
         for item in self.items:
             if item.title:
                 pdf.write(txt=item.title + "\n")
             if item.description:
-                pdf.cell(txt=item.description + "\n")
-            path = self.path + "/" + uuid.uuid4().hex + ".png"
+                pdf.write(txt=item.description + "\n")
+            path = self.path + "/" + item.id + ".png"
             item.chart.save_img(path)
             imgs.append(path)
             pdf.image(path, w=pdf.epw)
         pdf.output(self.path + "/" + filename)
         if clear_stack is True:
-            self.items = []
+            self._clear_stack()
         # cleanup
         for img in imgs:
             os.remove(img)
 
-    def write_file(self, filename: str, folderpath: str, html: str) -> str:
+    def save_html(self, info=False, clear_stack=True):
+        """
+        Save a report to html files
+        """
+        if self.path == "":
+            raise ValueError("Please set a report path first")
+        msg_start("Exporting report to html files")
+        for item in self.items:
+            self.write_html_file(item.id, self.path, item.chart.get_html_())
+        if info is True:
+            if self.has_altair_chart is True:
+                msg_info(f"Altair html headers:\n{AltairChart.html_header_()}")
+            if self.has_bokeh_chart is True:
+                msg_info(f"Bokeh html headers:\n{HvChart.html_header_()}")
+        msg_end("Report exported to html files")
+        if clear_stack is True:
+            self._clear_stack()
+
+    def write_html_file(self, filename: str, folderpath: str, html: str) -> str:
         """
         Writes some html to a file
         """
+
         # check directories
         if not os.path.isdir(folderpath):
             os.makedirs(folderpath)
             msg_info("Creating directory " + folderpath)
         # construct file path
         filepath = folderpath + "/" + filename + ".html"
         # write the file
         filex = open(filepath, "w")
         filex.write(html)
         filex.close()
         msg_ok("File written to", filepath)
         return filepath
+
+    def _clear_stack(self):
+        """
+        Clear the reporting stack
+        """
+        self.items = []
+        self.has_altair_chart = False
+        self.has_bokeh_chart = False
```

### Comparing `dataspace-0.0.8/dataspace/transform/dataframe.py` & `dataspace-0.0.9/dataspace/transform/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/transform/resample.py` & `dataspace-0.0.9/dataspace/transform/resample.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/transform/values.py` & `dataspace-0.0.9/dataspace/transform/values.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/utils/colors.py` & `dataspace-0.0.9/dataspace/utils/colors.py`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/dataspace/utils/messages.py` & `dataspace-0.0.9/dataspace/utils/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,29 +65,30 @@
     milliseconds = int(rd.microseconds / 1000)
     if milliseconds > 0:
         msg += colors.bold(str(rd.seconds) + "." + str(milliseconds))
     msg += " seconds"
     return msg
 
 
-def msg_end(self, *msg):
+def msg_end(*msg):
     """
     Prints an end message with elapsed time
     """
     global START_TIME
     if START_TIME is None:
         raise Exception(
-            "No start time set: please use start() " "before using this function"
+            "No start time set: please use start() before using this function"
         )
     endtime = datetime.datetime.now()
     rd = relativedelta(endtime, START_TIME)
     endmsg = _endmsg(rd)
     label = colors.purple("END")
-    msg += ("in " + endmsg,)
-    _msg(label, *msg)
+    args = list(msg)
+    args.append("in " + endmsg)
+    _msg(label, *args)
     START_TIME = None
 
 
 def msg_warning(*msg):
     """
     Prints a warning
     """
```

### Comparing `dataspace-0.0.8/dataspace.egg-info/SOURCES.txt` & `dataspace-0.0.9/dataspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataspace-0.0.8/setup.py` & `dataspace-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from os import path
 
-version = "0.0.8"
+version = "0.0.9"
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dataspace",
```

