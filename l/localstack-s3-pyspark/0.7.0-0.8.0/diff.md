# Comparing `tmp/localstack-s3-pyspark-0.7.0.tar.gz` & `tmp/localstack-s3-pyspark-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/localstack-s3-pyspark-0.7.0.tar", last modified: Fri Jan  7 00:03:22 2022, max compression
+gzip compressed data, was "localstack-s3-pyspark-0.8.0.tar", last modified: Fri Jul 22 20:11:11 2022, max compression
```

## Comparing `localstack-s3-pyspark-0.7.0.tar` & `localstack-s3-pyspark-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 DBelai     (501) staff       (20)        0 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/
--rw-r--r--   0 DBelai     (501) staff       (20)     2588 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/PKG-INFO
-drwxr-xr-x   0 DBelai     (501) staff       (20)        0 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/
--rw-r--r--   0 DBelai     (501) staff       (20)        0 2021-02-09 04:57:27.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/__init__.py
--rw-r--r--   0 DBelai     (501) staff       (20)     9512 2022-01-06 22:54:48.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/configure_defaults.py
--rw-r--r--   0 DBelai     (501) staff       (20)        0 2021-11-26 23:15:01.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/py.typed
--rw-r--r--   0 DBelai     (501) staff       (20)      622 2021-02-09 04:57:27.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/boto3.py
--rw-r--r--   0 DBelai     (501) staff       (20)      636 2022-01-06 22:17:42.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/__main__.py
--rw-r--r--   0 DBelai     (501) staff       (20)      204 2021-11-26 23:16:59.000000 localstack-s3-pyspark-0.7.0/pyproject.toml
--rw-r--r--   0 DBelai     (501) staff       (20)     2226 2022-01-06 21:56:13.000000 localstack-s3-pyspark-0.7.0/README.md
--rw-r--r--   0 DBelai     (501) staff       (20)       54 2022-01-06 20:42:08.000000 localstack-s3-pyspark-0.7.0/setup.py
--rw-r--r--   0 DBelai     (501) staff       (20)      792 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/setup.cfg
-drwxr-xr-x   0 DBelai     (501) staff       (20)        0 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/
--rw-r--r--   0 DBelai     (501) staff       (20)     2588 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 DBelai     (501) staff       (20)      489 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 DBelai     (501) staff       (20)       79 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/entry_points.txt
--rw-r--r--   0 DBelai     (501) staff       (20)      131 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/requires.txt
--rw-r--r--   0 DBelai     (501) staff       (20)       22 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/top_level.txt
--rw-r--r--   0 DBelai     (501) staff       (20)        1 2022-01-07 00:03:22.000000 localstack-s3-pyspark-0.7.0/localstack_s3_pyspark.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:11:11.878312 localstack-s3-pyspark-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-07-22 20:11:11.878312 localstack-s3-pyspark-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:11:11.874312 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9512 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/configure_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:11:11.874312 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-07-22 20:11:11.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-07-22 20:11:11.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 20:11:11.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-22 20:11:11.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-07-22 20:11:11.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-22 20:11:11.000000 localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2022-07-22 20:11:11.878312 localstack-s3-pyspark-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-22 20:09:52.000000 localstack-s3-pyspark-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `localstack-s3-pyspark-0.7.0/PKG-INFO` & `localstack-s3-pyspark-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: localstack-s3-pyspark
-Version: 0.7.0
+Version: 0.8.0
 Summary: A CLI to configure pyspark for use with s3 on localstack
 Home-page: https://github.com/enorganic/localstack-s3-pyspark
 Author-email: david@belais.me
 License: MIT
 Platform: UNKNOWN
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: boto3
 Provides-Extra: all
 
 # localstack-s3-pyspark
 
+[![test-distribute](https://github.com/enorganic/localstack-s3-pyspark/actions/workflows/test-distribute.yml/badge.svg)](https://github.com/enorganic/localstack-s3-pyspark/actions/workflows/test-distribute.yml)
+
 This package provides a CLI for configuring pyspark to use
 [localstack](https://github.com/localstack/localstack) for the S3 file system.
 This is intended for testing packages locally (or in your CI/CD pipeline)
 which you intend to deploy on an Amazon EMR cluster.
 
 ## Installation
 
@@ -47,39 +49,41 @@
 ```
 
 ### Tox
 
 Please note that if you are testing your packages with **tox** (highly
 recommended), you will need to:
 
-- Include "localstack-s3-pyspark" in your installation requirements (either in
-  your setup.py or setup.cfg file, or in the tox **deps** argument)
-- Include `localstack-s3-pyspark configure-defaults` prior to your tests
-  in your list of commands for each test environment
-- Include `docker-compose up -d` in **commands_pre** and `docker-compose down`
-  in **commands_post**
-
-Here is an example **tox.ini** for this repository:
+- Include "localstack-s3-pyspark" in your tox **deps**
+- Include `localstack-s3-pyspark configure-defaults` in your tox
+  **commands_pre** (or by other means execute this command prior to your tests)
+
+Here is an example **tox.ini** which starts up localstack using the localstack
+CLI (you could also use `docker-compose` or just `docker run`, if you need
+ greater control or fewer python dependencies, see the the localstack
+documentation
+["Getting Started" page](https://docs.localstack.cloud/get-started)
+for details):
 
 ```ini
 [tox]
-envlist = py36, py37, py38, py39
+envlist = pytest
 
-[testenv]
-extras = test
-deps = localstack-s3-pyspark
+[testenv:pytest]
+deps =
+  localstack-s3-pyspark
+  localstack
 commands_pre =
-    docker-compose -f tests/docker-compose.yml --project-directory tests up -d
-commands =
-    flake8
-    mypy
     localstack-s3-pyspark configure-defaults
+    localstack start -d
+    sleep 20
+commands =
     py.test
 commands_post =
-    docker-compose -f tests/docker-compose.yml --project-directory tests down
+    localstack stop
 ```
 
 ## Patch *boto3*
 
 If your tests interact with S3 using **boto3**, you can patch boto3 from within
 your unit tests as follows:
```

### Comparing `localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/configure_defaults.py` & `localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/configure_defaults.py`

 * *Files identical despite different names*

### Comparing `localstack-s3-pyspark-0.7.0/localstack_s3_pyspark/boto3.py` & `localstack-s3-pyspark-0.8.0/localstack_s3_pyspark/boto3.py`

 * *Files identical despite different names*

### Comparing `localstack-s3-pyspark-0.7.0/README.md` & `localstack-s3-pyspark-0.8.0/localstack_s3_pyspark.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+Metadata-Version: 2.1
+Name: localstack-s3-pyspark
+Version: 0.8.0
+Summary: A CLI to configure pyspark for use with s3 on localstack
+Home-page: https://github.com/enorganic/localstack-s3-pyspark
+Author-email: david@belais.me
+License: MIT
+Platform: UNKNOWN
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: boto3
+Provides-Extra: all
+
 # localstack-s3-pyspark
 
+[![test-distribute](https://github.com/enorganic/localstack-s3-pyspark/actions/workflows/test-distribute.yml/badge.svg)](https://github.com/enorganic/localstack-s3-pyspark/actions/workflows/test-distribute.yml)
+
 This package provides a CLI for configuring pyspark to use
 [localstack](https://github.com/localstack/localstack) for the S3 file system.
 This is intended for testing packages locally (or in your CI/CD pipeline)
 which you intend to deploy on an Amazon EMR cluster.
 
 ## Installation
 
@@ -34,43 +49,47 @@
 ```
 
 ### Tox
 
 Please note that if you are testing your packages with **tox** (highly
 recommended), you will need to:
 
-- Include "localstack-s3-pyspark" in your installation requirements (either in
-  your setup.py or setup.cfg file, or in the tox **deps** argument)
-- Include `localstack-s3-pyspark configure-defaults` prior to your tests
-  in your list of commands for each test environment
-- Include `docker-compose up -d` in **commands_pre** and `docker-compose down`
-  in **commands_post**
-
-Here is an example **tox.ini** for this repository:
+- Include "localstack-s3-pyspark" in your tox **deps**
+- Include `localstack-s3-pyspark configure-defaults` in your tox
+  **commands_pre** (or by other means execute this command prior to your tests)
+
+Here is an example **tox.ini** which starts up localstack using the localstack
+CLI (you could also use `docker-compose` or just `docker run`, if you need
+ greater control or fewer python dependencies, see the the localstack
+documentation
+["Getting Started" page](https://docs.localstack.cloud/get-started)
+for details):
 
 ```ini
 [tox]
-envlist = py36, py37, py38, py39
+envlist = pytest
 
-[testenv]
-extras = test
-deps = localstack-s3-pyspark
+[testenv:pytest]
+deps =
+  localstack-s3-pyspark
+  localstack
 commands_pre =
-    docker-compose -f tests/docker-compose.yml --project-directory tests up -d
-commands =
-    flake8
-    mypy
     localstack-s3-pyspark configure-defaults
+    localstack start -d
+    sleep 20
+commands =
     py.test
 commands_post =
-    docker-compose -f tests/docker-compose.yml --project-directory tests down
+    localstack stop
 ```
 
 ## Patch *boto3*
 
 If your tests interact with S3 using **boto3**, you can patch boto3 from within
 your unit tests as follows:
 
 ```python3
 from localstack_s3_pyspark.boto3 import use_localstack
 use_localstack()
 ```
+
+
```

### Comparing `localstack-s3-pyspark-0.7.0/setup.cfg` & `localstack-s3-pyspark-0.8.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [metadata]
 name = localstack-s3-pyspark
-version = 0.7.0
+version = 0.8.0
 author_email = david@belais.me
 description = A CLI to configure pyspark for use with s3 on localstack
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/enorganic/localstack-s3-pyspark
 
 [options]
 python_requires = ~=3.6
 packages = find:
 include_package_data = True
 install_requires = 
 	dataclasses; python_version == "3.6"
-	localstack-client~=1.29
-	lxml~=4.7
-	pyspark>=2.4,!=2.4.7,!=2.4.8
+	localstack-client~=1.35
+	lxml~=4.9
+	pyspark!=2.4.7,!=2.4.8,>=2.4
 
 [options.extras_require]
 boto3 = 
 	boto3
 all = 
 	boto3
```

