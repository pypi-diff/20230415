# Comparing `tmp/RiskQuantLib-0.2.7.tar.gz` & `tmp/RiskQuantLib-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskQuantLib-0.2.7.tar", last modified: Wed Apr 12 02:24:20 2023, max compression
+gzip compressed data, was "RiskQuantLib-0.2.8.tar", last modified: Sat Apr 15 13:32:11 2023, max compression
```

## Comparing `RiskQuantLib-0.2.7.tar` & `RiskQuantLib-0.2.8.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.495383 RiskQuantLib-0.2.7/
--rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1120 2023-04-12 02:24:20.495383 RiskQuantLib-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.2.7/README.md
--rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 02:24:20.496382 RiskQuantLib-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1932 2023-04-12 02:18:48.000000 RiskQuantLib-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.358344 RiskQuantLib-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.378347 RiskQuantLib-0.2.7/src/RiskQuantLib/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.407348 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.410388 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/Instrument/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/Instrument/__init__.py
--rw-rw-rw-   0        0        0      388 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.413385 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/InstrumentList/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0      409 2023-01-11 09:39:05.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.423386 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.426385 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.435397 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
--rw-rw-rw-   0        0        0     2677 2022-12-29 14:06:46.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
--rw-rw-rw-   0        0        0      351 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
--rw-rw-rw-   0        0        0      355 2022-12-29 14:55:03.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
--rw-rw-rw-   0        0        0      402 2022-12-29 14:55:03.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.447383 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
--rw-rw-rw-   0        0        0     1474 2023-01-11 09:39:05.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
--rw-rw-rw-   0        0        0     2151 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
--rw-rw-rw-   0        0        0     1515 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
--rw-rw-rw-   0        0        0     1101 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.449385 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/__pycache__/
--rw-rw-rw-   0        0        0      180 2022-12-14 06:06:02.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    14083 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/macro.pyt
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/__init__.py
--rw-rw-rw-   0        0        0    43577 2023-03-21 00:45:45.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/builder.py
--rw-rw-rw-   0        0        0     1640 2023-01-11 02:34:10.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/render.py
--rw-rw-rw-   0        0        0     8835 2023-03-21 00:45:45.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/router.py
--rw-rw-rw-   0        0        0     4736 2023-01-10 08:01:22.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/tree.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.452409 RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/__init__.py
--rw-rw-rw-   0        0        0      935 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.455395 RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/instrumentList.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.458390 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.460384 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/__init__.py
--rw-rw-rw-   0        0        0     1207 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/copula.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.462384 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/__init__.py
--rw-rw-rw-   0        0        0     2181 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/kmv.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/__init__.py
--rw-rw-rw-   0        0        0      274 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/model.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.469385 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/iloc.py
--rw-rw-rw-   0        0        0     1107 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/loc.py
--rw-rw-rw-   0        0        0    60946 2023-03-21 05:30:23.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/operation.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.472401 RiskQuantLib-0.2.7/src/RiskQuantLib/Property/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Property/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-01-11 10:25:57.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Property/property.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.494397 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/
--rw-rw-rw-   0        0        0     4368 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/GUITool.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/__init__.py
--rw-rw-rw-   0        0        0     6514 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/codeBuilderTool.py
--rw-rw-rw-   0        0        0    10785 2023-04-12 02:00:01.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/databaseTool.py
--rw-rw-rw-   0        0        0     1593 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/excelTool.py
--rw-rw-rw-   0        0        0    19343 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/fileTool.py
--rw-rw-rw-   0        0        0     4862 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/githubTool.py
--rw-rw-rw-   0        0        0     2817 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/mathTool.py
--rw-rw-rw-   0        0        0     1158 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/multiThreadTool.py
--rw-rw-rw-   0        0        0     4705 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/outlookTool.py
--rw-rw-rw-   0        0        0     4487 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/plotTool.py
--rw-rw-rw-   0        0        0     9707 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/pptTool.py
--rw-rw-rw-   0        0        0     9605 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/strTool.py
--rw-rw-rw-   0        0        0     6111 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/wordTool.py
--rw-rw-rw-   0        0        0    34418 2023-04-12 02:03:48.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/module.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.405365 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2773 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      619 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:11.068575 RiskQuantLib-0.2.8/
+-rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1120 2023-04-15 13:32:11.068575 RiskQuantLib-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.2.8/README.md
+-rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 13:32:11.072619 RiskQuantLib-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1932 2023-04-15 11:55:34.000000 RiskQuantLib-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.341502 RiskQuantLib-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.426065 RiskQuantLib-0.2.8/src/RiskQuantLib/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.494060 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.499005 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/Instrument/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      388 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.501999 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.590515 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.601278 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.613513 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
+-rw-rw-rw-   0        0        0      351 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
+-rw-rw-rw-   0        0        0      355 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
+-rw-rw-rw-   0        0        0      402 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
+-rw-rw-rw-   0        0        0      369 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/sourceCodeDebugger.pyt
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.622684 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
+-rw-rw-rw-   0        0        0     1474 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
+-rw-rw-rw-   0        0        0     2151 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
+-rw-rw-rw-   0        0        0     1515 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
+-rw-rw-rw-   0        0        0     1101 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.631802 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/__pycache__/
+-rw-rw-rw-   0        0        0      180 2022-12-14 06:06:02.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14083 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/macro.pyt
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/__init__.py
+-rw-rw-rw-   0        0        0    44560 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/builder.py
+-rw-rw-rw-   0        0        0     9222 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/debugger.py
+-rw-rw-rw-   0        0        0     1640 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/render.py
+-rw-rw-rw-   0        0        0     8835 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/router.py
+-rw-rw-rw-   0        0        0     4736 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/tree.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.652874 RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      935 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.665731 RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/instrumentList.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.679567 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.686339 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/__init__.py
+-rw-rw-rw-   0        0        0     1207 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/copula.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.687747 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/__init__.py
+-rw-rw-rw-   0        0        0     2181 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/kmv.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/__init__.py
+-rw-rw-rw-   0        0        0      274 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/model.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.747683 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/iloc.py
+-rw-rw-rw-   0        0        0     1107 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/loc.py
+-rw-rw-rw-   0        0        0    60946 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/operation.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.753870 RiskQuantLib-0.2.8/src/RiskQuantLib/Property/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Property/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Property/property.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:11.067055 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/
+-rw-rw-rw-   0        0        0     4368 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/GUITool.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/__init__.py
+-rw-rw-rw-   0        0        0     6514 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/codeBuilderTool.py
+-rw-rw-rw-   0        0        0    10785 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/databaseTool.py
+-rw-rw-rw-   0        0        0     1593 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/excelTool.py
+-rw-rw-rw-   0        0        0    19343 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/fileTool.py
+-rw-rw-rw-   0        0        0     4862 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/githubTool.py
+-rw-rw-rw-   0        0        0     2817 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/mathTool.py
+-rw-rw-rw-   0        0        0     1158 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/multiThreadTool.py
+-rw-rw-rw-   0        0        0     4705 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/outlookTool.py
+-rw-rw-rw-   0        0        0     4487 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/plotTool.py
+-rw-rw-rw-   0        0        0     9707 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/pptTool.py
+-rw-rw-rw-   0        0        0     9605 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/strTool.py
+-rw-rw-rw-   0        0        0     6111 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/wordTool.py
+-rw-rw-rw-   0        0        0    36938 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/module.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.492935 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2881 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      619 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/top_level.txt
```

### Comparing `RiskQuantLib-0.2.7/LICENSE` & `RiskQuantLib-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/PKG-INFO` & `RiskQuantLib-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.2.7
+Version: 0.2.8
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.2.7/README.md` & `RiskQuantLib-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/setup.py` & `RiskQuantLib-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="RiskQuantLib",
-    version="0.2.7",
+    version="0.2.8",
     author="Syuya_Murakami",
     author_email="wxy135@mail.ustc.edu.cn",
     description="RiskQuantLib is a QuantLib derivative to evaluate risk.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://riskquantlib-doc.readthedocs.io/en/latest/index.html",
     project_urls={
```

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/macro.pyt` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/macro.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/builder.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,15 +482,15 @@
         deprecatedInjectDict = deprecatedRenderTagDF.groupby('file').apply(lambda x:dict(zip(x['tag'],x['content']))).to_dict() if deprecatedRenderTagDF.shape[0]!=0 else {}
         [injectDict[file].update(deprecatedInjectDict[file]) for file in injectDict if file in deprecatedInjectDict]
         [injectDict.update({file:deprecatedInjectDict[file]}) for file in deprecatedInjectDict if file not in injectDict]
         self.bindType[bindType] = set() if persist else aliveRenderTag
 
         [router.persistToFile(file, **(injectDict[file])) if persist else router.injectToFile(file, **(injectDict[file])) for file in injectDict]
 
-    def renderProject(self, sourceCodeDirPath: str = '', bindType: str = 'renderedSourceCode', persist: bool = False, **kwargs):
+    def renderProject(self, sourceCodeDirPath: str = '', bindType: str = 'renderedSourceCode', persist: bool = False, debug: bool = False, **kwargs):
         """
         Render and inject source code into target project.
 
         Parameters
         ----------
         sourceCodeDirPath : str
             The path of dictionary where source code exist. Any sub file in this folder or sub-folder
@@ -500,28 +500,37 @@
             The source code injected by channel A will be not influenced by source code injected by channel B, unless
             the content of tag is overwritten by code in channel B. This is used when you have several builders and
             you want them to build into the same project. In this case, you should give a bindType for each render action
             to make sure they do not conflict with each other.
         persist : bool
             If true, the current source code will be saved as permanent source code. It will not
             be influenced by building action any more. This action can not be cancelled.
+        debug : bool
+            If false, the break point in Src will not be effective, only break point within instrument class will effect.
+            If true, the class method defined in Src directory will be dynamically bound to instrument node class.
+            Then the program will take .py file under .Src directory as a module and import it, bind the class method into
+            specified class. This mode is useful when your code is still under development. You will not have to change between
+            ./Src/somecode.py and target instrument class .py file to edit any code error. The break point will stop right
+            under ./Src/somecode.py.
 
         Returns
         -------
         None
         """
+        self.checkRender()
         sourceCodeDirPath = self.projectPath+os.sep+"Src" if sourceCodeDirPath == '' else sourceCodeDirPath
         if os.path.isdir(sourceCodeDirPath):
             from RiskQuantLib.Build.render import render
             from RiskQuantLib.Build.router import router
+            from RiskQuantLib.Build.debugger import debugger
             sourceCodeRender = render(sourceCodeDirPath)
             content = []
             for root, dirs, files in os.walk(sourceCodeDirPath):
-                contentAndType = [(router.readContent(root+os.sep+file), file, os.path.splitext(file)[-1]) for file in files]
-                contentRendered = [sourceCodeRender.render(file,**kwargs) if ext == '.pyt' else content for content, file, ext in contentAndType]
+                contentAndType = [(router.readContent(root+os.sep+file), file, os.path.splitext(file)[-1]) for file in files if os.path.splitext(file)[-1] in {'.pyt','.py'}]
+                contentRendered = [sourceCodeRender.render(file,**kwargs) if ext == '.pyt' else self.render.render('sourceCodeDebugger.pyt',srcPath=root+os.sep+file, **(debugger.splitSrcByChunkAndFindThoseCanBeDebugged(content))) if debug else content for content, file, ext in contentAndType]
                 contentMerged = "#-><FileStart>\n"+"\n#-><FileEnd>\n#-><FileStart>\n".join(contentRendered)+"\n#-><FileEnd>"
                 content.append(contentMerged)
             self.bindContent("\n".join(content), bindType=bindType, persist=persist)
             self.dumpInfo()
 
     def clearProject(self):
         """
```

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/render.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/render.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/router.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/router.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/tree.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/tree.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/instrument.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/instrumentList.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/instrumentList.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/copula.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/copula.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/kmv.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/kmv.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/iloc.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/iloc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/loc.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/loc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/operation.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/operation.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Property/property.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Property/property.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/GUITool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/GUITool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/codeBuilderTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/codeBuilderTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/databaseTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/databaseTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/excelTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/excelTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/fileTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/fileTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/githubTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/githubTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/mathTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/mathTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/multiThreadTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/multiThreadTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/outlookTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/outlookTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/plotTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/plotTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/pptTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/pptTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/strTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/strTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/wordTool.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/wordTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/__init__.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,20 @@
     PYB.code = codeBuilder(indent=0)
     PYB.code.addLine(r'path = sys.path[0] if not getattr(sys, "frozen", False) else os.path.dirname(sys.executable)')
     PYB.code.addLine(r'parser = argparse.ArgumentParser()')
     PYB.code.addLine(r'parser.add_argument("-a","--auto", help="use auto build model to build project dynamically", action="store_true")')
     PYB.code.addLine(r'parser.add_argument("-t", "--targetPath", type=str, help="the RiskQuantLib project you want to build")')
     PYB.code.addLine(r'parser.add_argument("-r", "--renderFromPath", type=str, help="the dictionary of source code where the template code exists")')
     PYB.code.addLine(r'parser.add_argument("-c", "--channel", type=str, help="if given a channel name, render action in this channel will not delete the result of render in other channel unless it is overwritten by current render")')
+    PYB.code.addLine(r'parser.add_argument("-d", "--debug", help="use debug mode, break point in Src will start to effect", action="store_true")')
     PYB.code.addLine(r'args = parser.parse_args()')
     PYB.code.addLine(r'targetPath = args.targetPath if args.targetPath else path')
     PYB.code.addLine(r'renderFromPath = args.renderFromPath if args.renderFromPath else targetPath+os.sep+"Src"')
     PYB.code.addLine(r'bindType = args.channel if args.channel else "renderedSourceCode"')
-    PYB.code.addLine(r'autoBuildProject(targetPath,renderFromPath,bindType) if args.auto else buildProject(targetPath,renderFromPath,bindType)')
+    PYB.code.addLine(r'autoBuildProject(targetPath,renderFromPath,bindType,args.debug) if args.auto else buildProject(targetPath,renderFromPath,bindType,args.debug)')
     return PYB
 
 def initiateMainFile():
     """
     initiateMainFile() is a function to generate content of main.py source file.
 
     main.py will be created in every RiskQuantLib project when initiating it. It is
@@ -121,15 +122,15 @@
     attributeExcelPath = targetPath + os.sep + "Build_Attr.xlsx"
     buildCachePath = rqlPath + os.sep + "Build" + os.sep + "buildInfo.pkl"
     if checkExist and (not os.path.isdir(rqlPath) or not os.path.exists(instrumentExcelPath) or not os.path.exists(attributeExcelPath)):
         raise Exception("The target dictionary should be a RiskQuantLib project, with Build_Instrument.xlsx and Build_Attr.xlsx in it!")
     return rqlPath, instrumentExcelPath, attributeExcelPath, buildCachePath
 
 def buildProjectFromExcel(targetPath: str, buildCachePath: str, instrumentExcelPath: str, attributeExcelPath: str,
-                          renderFromPath: str, bindType: str = 'renderedSourceCode'):
+                          renderFromPath: str, bindType: str = 'renderedSourceCode', debug: bool = False):
     """
     buildProjectFromExcel() is a function to build project according to excel declaration.
 
     Parameters
     ----------
     targetPath : str
         The path of target RiskQuantLib project dictionary.
@@ -143,28 +144,35 @@
         The path of source code dictionary
     bindType : str
         The channel of binding action. Source code are rendered and injected into project by different channels,
         The source code injected by channel A will be not influenced by source code injected by channel B, unless
         the content of tag is overwritten by code in channel B. This is used when you have several builders and
         you want them to build into the same project. In this case, you should give a bindType for each render action
         to make sure they do not conflict with each other.
+    debug : bool
+        If false, the break point in Src will not be effective, only break point within instrument class will effect.
+        If true, the class method defined in Src directory will be dynamically bound to instrument node class.
+        Then the program will take .py file under .Src directory as a module and import it, bind the class method into
+        specified class. This mode is useful when your code is still under development. You will not have to change between
+        ./Src/somecode.py and target instrument class .py file to edit any code error. The break point will stop right
+        under ./Src/somecode.py.
 
     Returns
     -------
     None
 
     """
     import os
     from RiskQuantLib.Build.builder import excelBuilder
     if os.path.isfile(buildCachePath):
         buildObj = excelBuilder.loadInfo(buildCachePath)
     else:
         buildObj = excelBuilder(targetProjectPath=targetPath)
     buildObj.buildProject(instrumentExcelPath=instrumentExcelPath, attributeExcelPath=attributeExcelPath)
-    buildObj.renderProject(renderFromPath,bindType,persist=False)
+    buildObj.renderProject(renderFromPath,bindType,persist=False, debug=debug)
     print("Build Project Finished")
 
 def newProject(targetPath:str = ''):
     """
     newProject() is a function to create a new RiskQuantLib project.
 
     Use terminal command 'newRQL' to use this function.
@@ -591,15 +599,15 @@
         os.remove(parentProjectPath + os.sep + name + '.zip')
     else:
         filePath = targetPath
         send = fileSender(filePath)
         send.run()
 
 
-def buildProject(targetPath:str = '', renderFromPath:str = '', channel:str = ''):
+def buildProject(targetPath:str = '', renderFromPath:str = '', channel:str = '', debug:bool = False):
     """
     buildProject() is a function to build RiskQuantLib project.
 
     Use terminal command 'bldRQL targetProjectPath' to use this function. The project
     will be built according to the Build_Instrument.xlsx and Build_Attr.xlsx in
     the targetProjectPath.
 
@@ -614,37 +622,46 @@
     targetPath : str
         A terminal command parameter, specify the RiskQuantLib project path you want to build and render.
     renderFromPath : str
         The path of dictionary of source file used to render target project.
     channel : str
         render action in this channel will not delete the result of render in other channel
         unless it is overwritten by current render.
+    debug : bool
+        If false, the break point in Src will not be effective, only break point within instrument class will effect.
+        If true, the class method defined in Src directory will be dynamically bound to instrument node class.
+        Then the program will take .py file under .Src directory as a module and import it, bind the class method into
+        specified class. This mode is useful when your code is still under development. You will not have to change between
+        ./Src/somecode.py and target instrument class .py file to edit any code error. The break point will stop right
+        under ./Src/somecode.py.
 
     Returns
     -------
     None
     """
 
     if targetPath == '' and renderFromPath == '':
         parser = argparse.ArgumentParser()
         parser.add_argument("targetPath", type=str, help="the RiskQuantLib project you want to build")
         parser.add_argument("-r","--renderFromPath", type=str, help="the dictionary of source code where the template code exists")
         parser.add_argument("-c", "--channel", type=str, help="if given a channel name, render action in this channel will not delete the result of render in other channel unless it is overwritten by current render")
+        parser.add_argument("-d", "--debug", help="use debug mode, break point in Src will start to effect", action="store_true")
         args = parser.parse_args()
         targetPath = args.targetPath
         renderFromPath = args.renderFromPath
         channel = args.channel
+        debug = args.debug
 
     import os
     renderFromPath = renderFromPath if renderFromPath else (targetPath + os.sep + "Src")
     bindType = channel if channel else 'renderedSourceCode'
     rqlPath,instrumentExcelPath,attributeExcelPath,buildCachePath = parseBuildPath(targetPath, checkExist=True)
-    buildProjectFromExcel(targetPath, buildCachePath,instrumentExcelPath,attributeExcelPath, renderFromPath, bindType)
+    buildProjectFromExcel(targetPath, buildCachePath,instrumentExcelPath,attributeExcelPath, renderFromPath, bindType, debug)
 
-def autoBuildProject(targetPath:str = '', renderFromPath:str = '', channel:str = ''):
+def autoBuildProject(targetPath:str = '', renderFromPath:str = '', channel:str = '', debug:bool = False):
     """
     autoBuildProject() is a function to build RiskQuantLib project. This function keeps
     running until catch a KeyboardInterrupt Exception.
 
     Use terminal command 'autoRQL targetProjectPath' to use this function. The project
     will be built according to the Build_Instrument.xlsx and Build_Attr.xlsx in
     the targetProjectPath.
@@ -657,37 +674,46 @@
     targetPath : str
         A terminal command parameter, specify the RiskQuantLib project path you want to build and render.
     renderFromPath : str
         The path of dictionary of source file used to render target project.
     channel : str
         render action in this channel will not delete the result of render in other channel
         unless it is overwritten by current render.
+    debug : bool
+        If false, the break point in Src will not be effective, only break point within instrument class will effect.
+        If true, the class method defined in Src directory will be dynamically bound to instrument node class.
+        Then the program will take .py file under .Src directory as a module and import it, bind the class method into
+        specified class. This mode is useful when your code is still under development. You will not have to change between
+        ./Src/somecode.py and target instrument class .py file to edit any code error. The break point will stop right
+        under ./Src/somecode.py.
 
     Returns
     -------
     None
     """
     if targetPath == '' and renderFromPath == '':
         parser = argparse.ArgumentParser()
         parser.add_argument("targetPath", type=str, help="the RiskQuantLib project you want to build automatically")
         parser.add_argument("-r", "--renderFromPath", type=str, help="the dictionary of source code where the template code exists")
         parser.add_argument("-c", "--channel", type=str, help="if given a channel name, render action in this channel will not delete the result of render in other channel unless it is overwritten by current render")
+        parser.add_argument("-d", "--debug", help="use debug mode, break point in Src will start to effect", action="store_true")
         args = parser.parse_args()
         targetPath = args.targetPath
         renderFromPath = args.renderFromPath
         channel = args.channel
+        debug = args.debug
 
     import os
     renderFromPath = renderFromPath if renderFromPath else (targetPath + os.sep + "Src")
     bindType = channel if channel else 'renderedSourceCode'
     rqlPath, instrumentExcelPath, attributeExcelPath, buildCachePath = parseBuildPath(targetPath, checkExist=True)
 
     # The call back function must be a single parameter function
     def build(projectPath=targetPath):
-        buildProjectFromExcel(targetPath,buildCachePath,instrumentExcelPath,attributeExcelPath, renderFromPath, bindType)
+        buildProjectFromExcel(targetPath,buildCachePath,instrumentExcelPath,attributeExcelPath, renderFromPath, bindType, debug)
 
     from RiskQuantLib.Tool.fileTool import systemWatcher
     watchObj = systemWatcher([instrumentExcelPath, attributeExcelPath, renderFromPath], call_back_function_on_any_change=build)
     watchObj.start()
 
 def unBuildProject(targetPath:str = ''):
     """
```

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib/module.py` & `RiskQuantLib-0.2.8/src/RiskQuantLib/module.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/PKG-INFO` & `RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.2.7
+Version: 0.2.8
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/SOURCES.txt` & `RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 src/RiskQuantLib/Auto/__init__.py
 src/RiskQuantLib/Auto/Instrument/__init__.py
 src/RiskQuantLib/Auto/Instrument/instrument.py
 src/RiskQuantLib/Auto/InstrumentList/__init__.py
 src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
 src/RiskQuantLib/Build/__init__.py
 src/RiskQuantLib/Build/builder.py
+src/RiskQuantLib/Build/debugger.py
 src/RiskQuantLib/Build/render.py
 src/RiskQuantLib/Build/router.py
 src/RiskQuantLib/Build/tree.py
 src/RiskQuantLib/Build/Component/__init__.py
 src/RiskQuantLib/Build/Component/macro.pyt
 src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
 src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
 src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
 src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
 src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
+src/RiskQuantLib/Build/Component/ContentGenerator/sourceCodeDebugger.pyt
 src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
 src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
 src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
 src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
 src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
 src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
 src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
```

### Comparing `RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/entry_points.txt` & `RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/entry_points.txt`

 * *Files identical despite different names*

