# Comparing `tmp/pymediawikidocker-0.9.7.tar.gz` & `tmp/pymediawikidocker-0.9.8.tar.gz`

## Comparing `pymediawikidocker-0.9.7.tar` & `pymediawikidocker-0.9.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.pydevproject
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/__init__.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/config.py
--rw-r--r--   0        0        0    23212 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/docker.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/html_table.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/logger.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/mariadb.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/mw.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/mwcluster.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/version.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/webscrape.py
--rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/extensions.json
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/addCronTabEntry.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/addSysopUser.sh
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/initdb.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/installExtensions.sh
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/lang.sh
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwCompose.yml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwDockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings.php
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings127.php
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings131.php
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings135.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings136.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings137.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings138.php
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings139.php
--rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki127.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki131.sql
--rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki135.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki136.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki137.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki138.sql
--rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki139.sql
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/phpinfo.php
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/plantuml.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/startRunJobs.sh
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/update.sh
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/upload.ini
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/scripts/install
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/basetest.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_config.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_extensions.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_html_tables.py
--rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_install.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.pydevproject
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/.DS_Store
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/__init__.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/config.py
+-rw-r--r--   0        0        0    23216 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/docker.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/html_table.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/logger.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/mariadb.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/mw.py
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/mwcluster.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/version.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/webscrape.py
+-rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/extensions.json
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/addCronTabEntry.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/addSysopUser.sh
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/initdb.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/installExtensions.sh
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/lang.sh
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwCompose.yml
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwDockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings.php
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings127.php
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings131.php
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings135.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings136.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings137.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings138.php
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings139.php
+-rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki127.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki131.sql
+-rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki135.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki136.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki137.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki138.sql
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki139.sql
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/phpinfo.php
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/plantuml.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/startRunJobs.sh
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/update.sh
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/upload.ini
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/scripts/install
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/basetest.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_config.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_extensions.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_html_tables.py
+-rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_install.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/PKG-INFO
```

### Comparing `pymediawikidocker-0.9.7/.github/workflows/build.yml` & `pymediawikidocker-0.9.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/.github/workflows/upload-to-pypi.yml` & `pymediawikidocker-0.9.8/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/.DS_Store` & `pymediawikidocker-0.9.8/mwdocker/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/config.py` & `pymediawikidocker-0.9.8/mwdocker/config.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/docker.py` & `pymediawikidocker-0.9.8/mwdocker/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,25 +253,25 @@
         return env
     
     def initDB(self):
         '''
         initialize my SQL database
         '''
         # restore the mySQL dump data
-        self.execute("/tmp/initdb.sh")
+        self.execute("/root/initdb.sh")
         # update the database e.g. to initialize Semantic MediaWiki tables
-        self.execute("/tmp/update.sh")
+        self.execute("/root/update.sh")
         # add an initial sysop user as specified
-        self.execute("/tmp/addSysopUser.sh")
+        self.execute("/root/addSysopUser.sh")
             
     def installExtensions(self):
         '''
         install all extensions
         '''
-        self.execute("/tmp/installExtensions.sh")
+        self.execute("/root/installExtensions.sh")
         
     def startUp(self):
         '''
         run startUp scripts
         '''
         self.execute("/root/addCronTabEntry.sh")
```

### Comparing `pymediawikidocker-0.9.7/mwdocker/html_table.py` & `pymediawikidocker-0.9.8/mwdocker/html_table.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/logger.py` & `pymediawikidocker-0.9.8/mwdocker/logger.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/mariadb.py` & `pymediawikidocker-0.9.8/mwdocker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/mw.py` & `pymediawikidocker-0.9.8/mwdocker/mw.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/mwcluster.py` & `pymediawikidocker-0.9.8/mwdocker/mwcluster.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/version.py` & `pymediawikidocker-0.9.8/mwdocker/version.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/webscrape.py` & `pymediawikidocker-0.9.8/mwdocker/webscrape.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/extensions.json` & `pymediawikidocker-0.9.8/mwdocker/resources/extensions.json`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/lang.sh` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/lang.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwCompose.yml` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwCompose.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwDockerfile` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwDockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 # copy phpinfo.php
 COPY phpinfo.php /var/www/html
 
 # copy the SQL dump
 COPY wiki.sql /tmp
 
 # copy the initdb.sh script
-COPY initdb.sh /tmp
+COPY initdb.sh /root
 
 # copy the installExtensions.sh script
-COPY installExtensions.sh /tmp
+COPY installExtensions.sh /root
 
 # copy the update.sh script
-COPY update.sh /tmp
+COPY update.sh /root
 
 # copy the addSysopUser.sh script
-COPY addSysopUser.sh /tmp
+COPY addSysopUser.sh /root
 
 #copy the startRunJobs.sh script
 COPY startRunJobs.sh /root
 
 # copy the script to add a crontab entry
 COPY addCronTabEntry.sh /root
 
@@ -82,12 +82,12 @@
 COPY lang.sh /root
 
 # copy the plantuml script
 COPY plantuml.sh /root
 
 
 # make the scripts executable
-RUN chmod +x /tmp/initdb.sh /tmp/update.sh /tmp/addSysopUser.sh /tmp/installExtensions.sh /root/addCronTabEntry.sh /root/startRunJobs.sh /root/plantuml.sh
+RUN chmod +x /root/initdb.sh /root/update.sh /root/addSysopUser.sh /root/installExtensions.sh /root/addCronTabEntry.sh /root/startRunJobs.sh /root/plantuml.sh
 
 # restore the mediawiki initial database backup
 # can not do this before SQL server is up see https://docs.docker.com/compose/startup-order/
 # RUN /tmp/initdb.sh
```

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings127.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings127.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings131.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings131.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings135.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings135.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings136.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings136.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings137.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings137.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings138.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings138.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings139.php` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings139.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki127.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki127.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki131.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki131.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki135.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki135.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki136.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki136.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki137.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki137.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki138.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki138.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki139.sql` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki139.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/mwdocker/resources/templates/plantuml.sh` & `pymediawikidocker-0.9.8/mwdocker/resources/templates/plantuml.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/tests/basetest.py` & `pymediawikidocker-0.9.8/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/tests/test_config.py` & `pymediawikidocker-0.9.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/tests/test_extensions.py` & `pymediawikidocker-0.9.8/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/tests/test_html_tables.py` & `pymediawikidocker-0.9.8/tests/test_html_tables.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/tests/test_install.py` & `pymediawikidocker-0.9.8/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/.gitignore` & `pymediawikidocker-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/LICENSE` & `pymediawikidocker-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/README.md` & `pymediawikidocker-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/pyproject.toml` & `pymediawikidocker-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.7/PKG-INFO` & `pymediawikidocker-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawikidocker
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python controlled (semantic) mediawiki docker application cluster installation
 Project-URL: Home, https://github.com/WolfgangFahl/pymediawikidocker
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/pymediawikidocker
 Project-URL: Source, https://github.com/WolfgangFahl/pymediawikidocker
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License: Apache-2.0
```

