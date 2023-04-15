# Comparing `tmp/opencmiss.zincwidgets-2.3.0.tar.gz` & `tmp/opencmiss.zincwidgets-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.zincwidgets-2.3.0.tar", last modified: Sat Mar 25 00:55:00 2023, max compression
+gzip compressed data, was "opencmiss.zincwidgets-2.3.1.tar", last modified: Sat Apr 15 07:01:18 2023, max compression
```

## Comparing `opencmiss.zincwidgets-2.3.0.tar` & `opencmiss.zincwidgets-2.3.1.tar`

### file list

```diff
@@ -1,94 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:55:00.023119 opencmiss.zincwidgets-2.3.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    15977 2020-11-24 09:14:24.000000 opencmiss.zincwidgets-2.3.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002    20056 2023-03-25 00:55:00.022734 opencmiss.zincwidgets-2.3.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      190 2021-10-30 04:23:06.000000 opencmiss.zincwidgets-2.3.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-03-25 00:55:00.023220 opencmiss.zincwidgets-2.3.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2224 2023-02-09 02:09:35.000000 opencmiss.zincwidgets-2.3.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:54:59.972164 opencmiss.zincwidgets-2.3.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:54:59.973814 opencmiss.zincwidgets-2.3.0/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      125 2020-11-24 09:14:24.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:54:59.997177 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      130 2023-03-25 00:54:08.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      377 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/addviewwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4283 2023-03-01 01:32:24.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/alignmentsceneviewerwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1305 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/base.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14602 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/basesceneviewerwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1028 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/consoleeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1163 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/definitions.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:54:59.998073 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/delegates/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-09-06 01:51:19.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/delegates/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1504 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/delegates/spinboxdelegate.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      671 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/draggablelistwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1863 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/editabletabbar.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3484 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/enumerationchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002       41 2021-11-05 08:49:32.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/errors.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3526 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/exportwebgldialog.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6487 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fieldchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4302 2022-07-21 22:28:35.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fieldconditions.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4642 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fieldeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    10490 2023-03-25 00:53:26.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fieldlisteditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5898 2023-02-09 02:09:35.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fieldpropertieswidget.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:55:00.000656 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fields/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    27292 2023-02-09 02:09:35.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fields/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4003 2023-02-09 02:09:35.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fields/lists.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1326 2022-07-21 22:28:35.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fields/parsers.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14720 2023-02-09 02:09:35.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fields/requirements.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3027 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/fieldtypechooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4055 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/glyphchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    47100 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/graphicseditorwidget.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:55:00.007130 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-10-30 04:23:06.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1900 2021-10-30 04:23:06.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/abstracthandler.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2792 2021-11-05 08:49:32.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/interactionmanager.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      328 2021-11-05 08:49:32.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/keyactivatedhandler.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3296 2023-02-02 23:59:55.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/modelalignment.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1823 2021-11-05 08:49:32.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/scenemanipulation.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12272 2021-11-05 08:49:32.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/sceneselection.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2050 2021-10-30 04:23:06.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/handlers/zoomonly.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4054 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/interactiveconsolewidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1932 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/loggereditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4061 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/materialchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    17810 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/materialeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    21694 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/modelsourceseditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3981 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/regionchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    10084 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/regioneditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     9328 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/sceneeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1302 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/scenelayoutchooserdialog.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13451 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/sceneviewereditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    28671 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/sceneviewerwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3293 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/snapshotdialog.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4307 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/spectrumchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    26324 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/spectrumeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4580 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/tessellationchooserwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     9621 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/tessellationeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7619 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/timeeditorwidget.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:55:00.022020 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-09-06 01:51:20.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   244392 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/icons_rc.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2070 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_addviewwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1496 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_consoleeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3764 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_exportwebglwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3779 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_fieldeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6092 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_fieldlisteditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    37829 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_graphicseditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2094 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_interactiveconsolewidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2370 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_loggereditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     9934 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_materialeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7502 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_modelsourceseditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1432 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_regioneditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7748 2023-02-03 00:05:30.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_sceneeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3179 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_scenelayoutchooserdialog.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14753 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_sceneviewereditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5582 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_snapshotdialog.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    21070 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_spectrumeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5218 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_tessellationeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6012 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/ui/ui_timeeditorwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1214 2023-03-01 01:40:56.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/utils.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3414 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/viewwidget.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      542 2023-01-31 01:20:48.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss/zincwidgets/viewwidgetdescription.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:54:59.975647 opencmiss.zincwidgets-2.3.0/src/opencmiss.zincwidgets.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    20056 2023-03-25 00:54:59.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss.zincwidgets.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3999 2023-03-25 00:54:59.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss.zincwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-03-25 00:54:59.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss.zincwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       93 2023-03-25 00:54:59.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss.zincwidgets.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2023-03-25 00:54:59.000000 opencmiss.zincwidgets-2.3.0/src/opencmiss.zincwidgets.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 07:01:18.315250 opencmiss.zincwidgets-2.3.1/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    15977 2023-04-15 06:57:04.000000 opencmiss.zincwidgets-2.3.1/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      666 2023-04-15 07:01:18.315002 opencmiss.zincwidgets-2.3.1/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      324 2023-04-15 06:59:45.000000 opencmiss.zincwidgets-2.3.1/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 07:01:18.314643 opencmiss.zincwidgets-2.3.1/opencmiss.zincwidgets.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      666 2023-04-15 07:01:18.000000 opencmiss.zincwidgets-2.3.1/opencmiss.zincwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      251 2023-04-15 07:01:18.000000 opencmiss.zincwidgets-2.3.1/opencmiss.zincwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 07:01:18.000000 opencmiss.zincwidgets-2.3.1/opencmiss.zincwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       15 2023-04-15 07:01:18.000000 opencmiss.zincwidgets-2.3.1/opencmiss.zincwidgets.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 07:01:18.000000 opencmiss.zincwidgets-2.3.1/opencmiss.zincwidgets.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-15 07:01:18.315333 opencmiss.zincwidgets-2.3.1/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      662 2023-04-15 07:00:55.000000 opencmiss.zincwidgets-2.3.1/setup.py
```

### Comparing `opencmiss.zincwidgets-2.3.0/LICENSE` & `opencmiss.zincwidgets-2.3.1/LICENSE`

 * *Files identical despite different names*

