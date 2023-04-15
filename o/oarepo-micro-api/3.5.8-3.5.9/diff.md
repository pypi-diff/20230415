# Comparing `tmp/oarepo-micro-api-3.5.8.tar.gz` & `tmp/oarepo-micro-api-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-micro-api-3.5.8.tar", last modified: Wed Feb  9 10:07:09 2022, max compression
+gzip compressed data, was "oarepo-micro-api-3.5.9.tar", last modified: Thu Feb 10 17:34:56 2022, max compression
```

## Comparing `oarepo-micro-api-3.5.8.tar` & `oarepo-micro-api-3.5.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/.envrc
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:07:09.268241 oarepo-micro-api-3.5.8/.tx/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/.tx/config
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/oarepo_micro_api/
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/alias_prefix_replacer.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/oarepo_micro_api/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-02-09 10:07:09.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-02-09 10:07:09.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 10:07:09.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-02-09 10:07:09.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 10:06:24.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-02-09 10:07:09.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-09 10:07:09.000000 oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (121)      376 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:07:09.272241 oarepo-micro-api-3.5.8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/api/test_api_wellknown.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/api/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/api/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-02-09 10:03:01.000000 oarepo-micro-api-3.5.8/tests/test_app_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:34:56.496804 oarepo-micro-api-3.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/.envrc
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:34:56.492804 oarepo-micro-api-3.5.9/.tx/
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-02-10 17:34:56.496804 oarepo-micro-api-3.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:34:56.492804 oarepo-micro-api-3.5.9/oarepo_micro_api/
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/alias_prefix_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/oarepo_micro_api/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:34:56.492804 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-02-10 17:34:56.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2022-02-10 17:34:56.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 17:34:56.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-02-10 17:34:56.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 17:34:12.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-02-10 17:34:56.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-10 17:34:56.000000 oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (121)      376 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-02-10 17:34:56.496804 oarepo-micro-api-3.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:34:56.492804 oarepo-micro-api-3.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:34:56.496804 oarepo-micro-api-3.5.9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/api/test_api_wellknown.py
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/api/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/api/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-02-10 17:31:21.000000 oarepo-micro-api-3.5.9/tests/test_app_version.py
```

### Comparing `oarepo-micro-api-3.5.8/.editorconfig` & `oarepo-micro-api-3.5.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/.travis.yml` & `oarepo-micro-api-3.5.9/.travis.yml`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 env:
   global:
     - POSTGRESQL_SQLALCHEMY_DATABASE_URI="postgresql+psycopg2://postgres@localhost:5432/invenio"
     - ES7_DOWNLOAD_URL="https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-7.5.1-linux-x86_64.tar.gz"
     - ES_HOST=127.0.0.1
   matrix:
-    - REQUIREMENTS=release OAREPO_VERSION=3.5.12 EXTRAS=tests-es7 ES=$ES7_DOWNLOAD_URL SQLALCHEMY_DATABASE_URI=$POSTGRESQL_SQLALCHEMY_DATABASE_URI
-    - REQUIREMENTS=release OAREPO_VERSION=3.5.12 EXTRAS=tests-es7 ES=$ES7_DOWNLOAD_URL
+    - REQUIREMENTS=release OAREPO_VERSION=3.5.13 EXTRAS=tests-es7 ES=$ES7_DOWNLOAD_URL SQLALCHEMY_DATABASE_URI=$POSTGRESQL_SQLALCHEMY_DATABASE_URI
+    - REQUIREMENTS=release OAREPO_VERSION=3.5.13 EXTRAS=tests-es7 ES=$ES7_DOWNLOAD_URL
 
 python:
   - "3.8"
 
 before_install:
   - "travis_retry pip install --upgrade pip setuptools py"
   - "travis_retry pip install twine wheel coveralls pydocstyle>=5.0.2 isort requirements-builder pip-tools"
```

### Comparing `oarepo-micro-api-3.5.8/.tx/config` & `oarepo-micro-api-3.5.9/.tx/config`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/CONTRIBUTING.rst` & `oarepo-micro-api-3.5.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/LICENSE` & `oarepo-micro-api-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/MANIFEST.in` & `oarepo-micro-api-3.5.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/PKG-INFO` & `oarepo-micro-api-3.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-micro-api
-Version: 3.5.8
+Version: 3.5.9
 Summary: OARepo REST API microservice
 Home-page: https://github.com/oarepo/oarepo-micro-api
 Author: Miroslav Bauer @ CESNET
 Author-email: bauer@cesnet.cz
 License: MIT
 Keywords: oarepo-micro-api Invenio
 Platform: any
```

### Comparing `oarepo-micro-api-3.5.8/README.md` & `oarepo-micro-api-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/__init__.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/alias_prefix_replacer.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/alias_prefix_replacer.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/cli.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/config.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/signals.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/signals.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/utils.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api/wsgi.py` & `oarepo-micro-api-3.5.9/oarepo_micro_api/wsgi.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/PKG-INFO` & `oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-micro-api
-Version: 3.5.8
+Version: 3.5.9
 Summary: OARepo REST API microservice
 Home-page: https://github.com/oarepo/oarepo-micro-api
 Author: Miroslav Bauer @ CESNET
 Author-email: bauer@cesnet.cz
 License: MIT
 Keywords: oarepo-micro-api Invenio
 Platform: any
```

### Comparing `oarepo-micro-api-3.5.8/oarepo_micro_api.egg-info/SOURCES.txt` & `oarepo-micro-api-3.5.9/oarepo_micro_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/setup.py` & `oarepo-micro-api-3.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import find_packages, setup
 
 readme = open('README.md').read()
 
 packages = find_packages()
 
 DATABASE = "postgresql"
-OAREPO_VERSION = os.environ.get('OAREPO_VERSION', '3.5.12')
+OAREPO_VERSION = os.environ.get('OAREPO_VERSION', '3.5.13')
 
 install_requires = [
     'oarepo~={version}'.format(version=OAREPO_VERSION),
     'oarepo-heartbeat>=1.0.2',
     'importlib_metadata',
     'uwsgi>=2.0',
     'uwsgi-tools>=1.1.1',
```

### Comparing `oarepo-micro-api-3.5.8/tests/api/conftest.py` & `oarepo-micro-api-3.5.9/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/tests/api/test_api_wellknown.py` & `oarepo-micro-api-3.5.9/tests/api/test_api_wellknown.py`

 * *Files identical despite different names*

### Comparing `oarepo-micro-api-3.5.8/tests/api/test_utils.py` & `oarepo-micro-api-3.5.9/tests/api/test_utils.py`

 * *Files identical despite different names*

