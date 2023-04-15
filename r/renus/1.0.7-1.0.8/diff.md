# Comparing `tmp/renus-1.0.7.tar.gz` & `tmp/renus-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.0.7.tar", last modified: Sat Apr 15 07:28:05 2023, max compression
+gzip compressed data, was "renus-1.0.8.tar", last modified: Sat Apr 15 09:17:26 2023, max compression
```

## Comparing `renus-1.0.7.tar` & `renus-1.0.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.290665 renus-1.0.7/
--rw-rw-rw-   0        0        0     1514 2022-12-05 06:16:54.000000 renus-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      220 2023-04-15 07:28:05.287653 renus-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.115569 renus-1.0.7/renus/
--rw-rw-rw-   0        0        0       23 2022-08-01 09:27:06.000000 renus-1.0.7/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.0.7/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.145605 renus-1.0.7/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.147586 renus-1.0.7/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.0.7/renus/commands/app/run.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.150581 renus-1.0.7/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.0.7/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.152578 renus-1.0.7/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.0.7/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.161586 renus-1.0.7/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     2272 2023-04-13 07:56:44.000000 renus-1.0.7/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.0.7/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.172588 renus-1.0.7/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.0.7/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.0.7/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.0.7/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.175588 renus-1.0.7/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-03-14 08:51:15.000000 renus-1.0.7/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.270664 renus-1.0.7/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.0.7/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/config.py
--rw-rw-rw-   0        0        0     2442 2023-04-15 07:22:34.000000 renus-1.0.7/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.0.7/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.0.7/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.0.7/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14158 2022-11-02 05:56:07.000000 renus-1.0.7/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.0.7/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.0.7/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.0.7/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.0.7/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.0.7/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.281665 renus-1.0.7/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.0.7/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.0.7/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/websockets.py
--rw-rw-rw-   0        0        0      301 2023-04-15 07:24:18.000000 renus-1.0.7/renus/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.286669 renus-1.0.7/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.0.7/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.129586 renus-1.0.7/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-04-15 07:28:04.000000 renus-1.0.7/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2023-04-15 07:28:05.000000 renus-1.0.7/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 07:28:04.000000 renus-1.0.7/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 07:28:04.000000 renus-1.0.7/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 07:28:05.291665 renus-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      301 2023-04-15 07:24:18.000000 renus-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.516227 renus-1.0.8/
+-rw-rw-rw-   0        0        0     1514 2022-12-05 06:16:54.000000 renus-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      220 2023-04-15 09:17:26.516227 renus-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.363225 renus-1.0.8/renus/
+-rw-rw-rw-   0        0        0       23 2022-08-01 09:27:06.000000 renus-1.0.8/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.0.8/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.381226 renus-1.0.8/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.390226 renus-1.0.8/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.0.8/renus/commands/app/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.398226 renus-1.0.8/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.0.8/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.400226 renus-1.0.8/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.0.8/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.403226 renus-1.0.8/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     2272 2023-04-13 07:56:44.000000 renus-1.0.8/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.0.8/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.408227 renus-1.0.8/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.0.8/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.0.8/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.0.8/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.415228 renus-1.0.8/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-03-14 08:51:15.000000 renus-1.0.8/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.0.8/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.500226 renus-1.0.8/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.0.8/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/config.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.0.8/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.0.8/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.0.8/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.0.8/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14158 2022-11-02 05:56:07.000000 renus-1.0.8/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.0.8/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.0.8/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.0.8/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.0.8/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.0.8/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.512229 renus-1.0.8/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.0.8/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.0.8/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.0.8/renus/core/websockets.py
+-rw-rw-rw-   0        0        0      301 2023-04-15 07:24:18.000000 renus-1.0.8/renus/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.515227 renus-1.0.8/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.8/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.0.8/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:17:26.377225 renus-1.0.8/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-04-15 09:17:26.000000 renus-1.0.8/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2023-04-15 09:17:26.000000 renus-1.0.8/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 09:17:26.000000 renus-1.0.8/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 09:17:26.000000 renus-1.0.8/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 09:17:26.517228 renus-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      301 2023-04-15 09:16:58.000000 renus-1.0.8/setup.py
```

### Comparing `renus-1.0.7/LICENSE` & `renus-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/app.py` & `renus-1.0.8/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/app/run.py` & `renus-1.0.8/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/backup/run.py` & `renus-1.0.8/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/copy/run.py` & `renus-1.0.8/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/default/run.py` & `renus-1.0.8/renus/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/help.py` & `renus-1.0.8/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/install/build.py` & `renus-1.0.8/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/install/run.py` & `renus-1.0.8/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/install/service.py` & `renus-1.0.8/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/commands/permission/run.py` & `renus-1.0.8/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/cache.py` & `renus-1.0.8/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/concurrency.py` & `renus-1.0.8/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/datastructures.py` & `renus-1.0.8/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/exception.py` & `renus-1.0.8/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/formparsers.py` & `renus-1.0.8/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/injection.py` & `renus-1.0.8/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/log.py` & `renus-1.0.8/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/model.py` & `renus-1.0.8/renus/core/model.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/request.py` & `renus-1.0.8/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/response.py` & `renus-1.0.8/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/routing.py` & `renus-1.0.8/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/schedule.py` & `renus-1.0.8/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/serialize.py` & `renus-1.0.8/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/status.py` & `renus-1.0.8/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/validation/rules.py` & `renus-1.0.8/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/validation/validate.py` & `renus-1.0.8/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/core/websockets.py` & `renus-1.0.8/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus/util/helper.py` & `renus-1.0.8/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.7/renus.egg-info/SOURCES.txt` & `renus-1.0.8/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

