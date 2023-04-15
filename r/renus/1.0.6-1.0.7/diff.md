# Comparing `tmp/renus-1.0.6.tar.gz` & `tmp/renus-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.0.6.tar", last modified: Tue Mar 14 08:54:26 2023, max compression
+gzip compressed data, was "renus-1.0.7.tar", last modified: Sat Apr 15 07:28:05 2023, max compression
```

## Comparing `renus-1.0.6.tar` & `renus-1.0.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:26.101743 renus-1.0.6/
--rw-rw-rw-   0        0        0     1514 2022-12-05 06:16:54.000000 renus-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      220 2023-03-14 08:54:26.100757 renus-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.935738 renus-1.0.6/renus/
--rw-rw-rw-   0        0        0       23 2022-08-01 09:27:06.000000 renus-1.0.6/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.0.6/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.961740 renus-1.0.6/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.964739 renus-1.0.6/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.0.6/renus/commands/app/run.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.966756 renus-1.0.6/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1509 2022-09-11 12:09:39.000000 renus-1.0.6/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.974756 renus-1.0.6/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1740 2022-09-11 12:09:39.000000 renus-1.0.6/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.982756 renus-1.0.6/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     2150 2023-03-14 08:51:15.000000 renus-1.0.6/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1518 2022-09-28 05:36:10.000000 renus-1.0.6/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:26.000739 renus-1.0.6/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.0.6/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.0.6/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.0.6/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:26.008756 renus-1.0.6/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-03-14 08:51:15.000000 renus-1.0.6/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.0.6/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:26.085744 renus-1.0.6/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.0.6/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/config.py
--rw-rw-rw-   0        0        0     2695 2022-09-25 10:07:20.000000 renus-1.0.6/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.0.6/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.0.6/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.0.6/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14158 2022-11-02 05:56:07.000000 renus-1.0.6/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.0.6/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.0.6/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.0.6/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.0.6/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.0.6/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:26.097757 renus-1.0.6/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.0.6/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.0.6/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.0.6/renus/core/websockets.py
--rw-rw-rw-   0        0        0      301 2023-03-14 08:53:09.000000 renus-1.0.6/renus/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:26.099756 renus-1.0.6/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.6/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.0.6/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-03-14 08:54:25.953757 renus-1.0.6/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-03-14 08:54:25.000000 renus-1.0.6/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2023-03-14 08:54:25.000000 renus-1.0.6/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 08:54:25.000000 renus-1.0.6/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-14 08:54:25.000000 renus-1.0.6/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 08:54:26.101743 renus-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      301 2023-03-14 08:53:09.000000 renus-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.290665 renus-1.0.7/
+-rw-rw-rw-   0        0        0     1514 2022-12-05 06:16:54.000000 renus-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      220 2023-04-15 07:28:05.287653 renus-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.115569 renus-1.0.7/renus/
+-rw-rw-rw-   0        0        0       23 2022-08-01 09:27:06.000000 renus-1.0.7/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.0.7/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.145605 renus-1.0.7/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.147586 renus-1.0.7/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.0.7/renus/commands/app/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.150581 renus-1.0.7/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.0.7/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.152578 renus-1.0.7/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.0.7/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.161586 renus-1.0.7/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     2272 2023-04-13 07:56:44.000000 renus-1.0.7/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.0.7/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.172588 renus-1.0.7/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.0.7/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.0.7/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.0.7/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.175588 renus-1.0.7/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-03-14 08:51:15.000000 renus-1.0.7/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.0.7/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.270664 renus-1.0.7/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.0.7/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/config.py
+-rw-rw-rw-   0        0        0     2442 2023-04-15 07:22:34.000000 renus-1.0.7/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.0.7/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.0.7/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.0.7/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14158 2022-11-02 05:56:07.000000 renus-1.0.7/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.0.7/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.0.7/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.0.7/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.0.7/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.0.7/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.281665 renus-1.0.7/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.0.7/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.0.7/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.0.7/renus/core/websockets.py
+-rw-rw-rw-   0        0        0      301 2023-04-15 07:24:18.000000 renus-1.0.7/renus/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.286669 renus-1.0.7/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.7/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.0.7/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:28:05.129586 renus-1.0.7/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-04-15 07:28:04.000000 renus-1.0.7/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2023-04-15 07:28:05.000000 renus-1.0.7/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 07:28:04.000000 renus-1.0.7/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 07:28:04.000000 renus-1.0.7/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 07:28:05.291665 renus-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      301 2023-04-15 07:24:18.000000 renus-1.0.7/setup.py
```

### Comparing `renus-1.0.6/LICENSE` & `renus-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/app.py` & `renus-1.0.7/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/commands/app/run.py` & `renus-1.0.7/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/commands/backup/run.py` & `renus-1.0.7/renus/commands/backup/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     '__pycache__',
     'node_modules',
     '.idea',
     '.git',
     '.github'
 ]
 exclude = [
+    'venv',
     'storage/cache',
     'storage/logs'
 ]
 
 
 def zipdir(path, ziph):
     for dirname, subdirs, files in os.walk(path):
```

### Comparing `renus-1.0.6/renus/commands/copy/run.py` & `renus-1.0.7/renus/commands/copy/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,32 +5,33 @@
     '__pycache__',
     'frontend',
     '.idea',
     '.git',
     '.github'
 ]
 exclude = [
+    'venv',
     'storage/cache',
     'storage/logs'
 ]
 
 exclude_ext = [
     '.vue',
     '.js'
     '.css'
     '.scss'
 ]
 
 
 def zipdir(path, ziph):
     for dirname, subdirs, files in os.walk(path):
-        has=False
+        has = False
         for dir in exclude_all:
-            if dirname.find(dir)!=-1:
-                has=True
+            if dirname.find(dir) != -1:
+                has = True
                 break
         for dir in exclude:
             if dirname.startswith(dir):
                 has = True
                 break
         if has:
             continue
@@ -42,36 +43,37 @@
                     if file.endswith(ext):
                         has = True
                         break
                 if has:
                     continue
             ziph.write(os.path.join(dirname, file))
 
+
 def folders():
-    res=[]
+    res = []
     for entry in os.scandir('./'):
         if entry.is_dir():
             res.append(entry.name)
 
     return res
 
+
 def run():
     path = input('copy folder path:<D:/projects/uploads>').lower()
-    if path =='':
-        path='D:/projects/uploads'
+    if path == '':
+        path = 'D:/projects/uploads'
 
-    ff=folders()
+    ff = folders()
 
     app_name = input('copy name:')
     print(f'start copy {app_name}...')
     if not os.path.exists(f'{path}'):
         os.makedirs(f'{path}')
     zipf = zipfile.ZipFile(f'{path}/{app_name}.zip', 'w', zipfile.ZIP_DEFLATED)
     for folder in ff:
         if folder not in exclude_all:
             zipdir(f'{folder}/', zipf)
 
     zipf.write('index.py')
     zipf.close()
 
     print('end')
-
```

### Comparing `renus-1.0.6/renus/commands/default/run.py` & `renus-1.0.7/renus/commands/default/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from renus.core.routing import Router
 from renus.util.helper import hash_new_password
 
 
 def run(args):
     if args[0] == 'setting':
         from app.extension.renus.setting.model import Setting
+        Setting('').where({'_id': {'$ne': 1}}).delete(True)
         with open('extension/renus/setting/db.json','r') as db:
             d=json.loads(db.read())
             for item in d:
                 Setting('').where({
                     'name':item['name']
                 }).update(item, True)
         print('DB Settings Created.')
 
     if args[0] == 'translate':
         from app.extension.renus.translate.model import Translate
+        Translate('').where({'_id':{'$ne':1}}).delete(True)
         with open('extension/renus/translate/db.json','r') as db:
             d=json.loads(db.read())
             for item in d:
                 Translate('').where({
                     'key':item['key']
                 }).update(item, True)
         print('DB Translates Created.')
```

### Comparing `renus-1.0.6/renus/commands/install/build.py` & `renus-1.0.7/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/commands/install/run.py` & `renus-1.0.7/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/commands/install/service.py` & `renus-1.0.7/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/commands/permission/run.py` & `renus-1.0.7/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/cache.py` & `renus-1.0.7/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/concurrency.py` & `renus-1.0.7/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/datastructures.py` & `renus-1.0.7/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/exception.py` & `renus-1.0.7/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/formparsers.py` & `renus-1.0.7/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/injection.py` & `renus-1.0.7/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/log.py` & `renus-1.0.7/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/model.py` & `renus-1.0.7/renus/core/model.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/request.py` & `renus-1.0.7/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/response.py` & `renus-1.0.7/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/routing.py` & `renus-1.0.7/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/schedule.py` & `renus-1.0.7/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/serialize.py` & `renus-1.0.7/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/status.py` & `renus-1.0.7/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/validation/rules.py` & `renus-1.0.7/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/validation/validate.py` & `renus-1.0.7/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/core/websockets.py` & `renus-1.0.7/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus/util/helper.py` & `renus-1.0.7/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.6/renus.egg-info/SOURCES.txt` & `renus-1.0.7/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

