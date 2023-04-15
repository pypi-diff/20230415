# Comparing `tmp/credentials-manager-client-0.0.1.tar.gz` & `tmp/credentials_manager_client-0.1a-.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credentials-manager-client-0.0.1.tar", last modified: Sat Apr 15 10:26:16 2023, max compression
+gzip compressed data, was "credentials_manager_client-0.1a-.tar", last modified: Sat Apr 15 10:05:36 2023, max compression
```

## Comparing `credentials-manager-client-0.0.1.tar` & `credentials_manager_client-0.1a-.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.700683 credentials-manager-client-0.0.1/
--rw-r--r--   0 tof        (501) staff       (20)     1092 2023-04-15 10:22:31.000000 credentials-manager-client-0.0.1/LICENSE
--rw-r--r--   0 tof        (501) staff       (20)     1777 2023-04-15 10:26:16.700540 credentials-manager-client-0.0.1/PKG-INFO
--rw-r--r--   0 tof        (501) staff       (20)       14 2023-04-15 10:21:24.000000 credentials-manager-client-0.0.1/README.md
--rw-r--r--   0 tof        (501) staff       (20)      944 2023-04-15 10:25:27.000000 credentials-manager-client-0.0.1/pyproject.toml
--rw-r--r--   0 tof        (501) staff       (20)       38 2023-04-15 10:26:16.700731 credentials-manager-client-0.0.1/setup.cfg
--rw-r--r--   0 tof        (501) staff       (20)     1020 2023-04-15 10:15:38.000000 credentials-manager-client-0.0.1/setup.py
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.697002 credentials-manager-client-0.0.1/src/
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.698104 credentials-manager-client-0.0.1/src/credentials_manager_client/
--rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 10:15:38.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/__init__.py
--rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 10:15:38.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/app.py
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.699321 credentials-manager-client-0.0.1/src/credentials_manager_client/apps/
--rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 10:15:38.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/apps/__init__.py
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.699879 credentials-manager-client-0.0.1/src/credentials_manager_client/apps/auth/
--rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 10:15:38.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/apps/auth/__init__.py
--rw-r--r--   0 tof        (501) staff       (20)      501 2023-04-15 10:24:23.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/apps/auth/abstract_models.py
--rw-r--r--   0 tof        (501) staff       (20)     2005 2023-04-15 10:15:52.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/apps/auth/models.py
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.700311 credentials-manager-client-0.0.1/src/credentials_manager_client/db/
--rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 10:15:52.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/db/__init__.py
--rw-r--r--   0 tof        (501) staff       (20)     1251 2023-04-15 10:15:52.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/db/base_model.py
--rw-r--r--   0 tof        (501) staff       (20)       35 2023-04-15 10:15:38.000000 credentials-manager-client-0.0.1/src/credentials_manager_client/main.py
-drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:26:16.699185 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/
--rw-r--r--   0 tof        (501) staff       (20)     1777 2023-04-15 10:26:16.000000 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/PKG-INFO
--rw-r--r--   0 tof        (501) staff       (20)      793 2023-04-15 10:26:16.000000 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/SOURCES.txt
--rw-r--r--   0 tof        (501) staff       (20)        1 2023-04-15 10:26:16.000000 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/dependency_links.txt
--rw-r--r--   0 tof        (501) staff       (20)       71 2023-04-15 10:26:16.000000 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/entry_points.txt
--rw-r--r--   0 tof        (501) staff       (20)      124 2023-04-15 10:26:16.000000 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/requires.txt
--rw-r--r--   0 tof        (501) staff       (20)       27 2023-04-15 10:26:16.000000 credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/top_level.txt
+drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:05:36.849824 credentials_manager_client-0.1a-/
+-rw-r--r--   0 tof        (501) staff       (20)      182 2023-04-15 10:05:36.849521 credentials_manager_client-0.1a-/PKG-INFO
+-rw-r--r--   0 tof        (501) staff       (20)       21 2023-04-15 09:06:43.000000 credentials_manager_client-0.1a-/README.md
+-rw-r--r--   0 tof        (501) staff       (20)       38 2023-04-15 10:05:36.849990 credentials_manager_client-0.1a-/setup.cfg
+-rw-r--r--   0 tof        (501) staff       (20)     1027 2023-04-15 10:01:25.000000 credentials_manager_client-0.1a-/setup.py
+drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:05:36.828142 credentials_manager_client-0.1a-/src/
+drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:05:36.837299 credentials_manager_client-0.1a-/src/credentials_manager_client/
+-rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 09:06:43.000000 credentials_manager_client-0.1a-/src/credentials_manager_client/__init__.py
+-rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 09:06:43.000000 credentials_manager_client-0.1a-/src/credentials_manager_client/app.py
+drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:05:36.849035 credentials_manager_client-0.1a-/src/credentials_manager_client/apps/
+-rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 09:06:43.000000 credentials_manager_client-0.1a-/src/credentials_manager_client/apps/__init__.py
+drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:05:36.849189 credentials_manager_client-0.1a-/src/credentials_manager_client/apps/auth/
+-rw-r--r--   0 tof        (501) staff       (20)        0 2023-04-15 09:06:43.000000 credentials_manager_client-0.1a-/src/credentials_manager_client/apps/auth/__init__.py
+-rw-r--r--   0 tof        (501) staff       (20)       35 2023-04-15 09:06:43.000000 credentials_manager_client-0.1a-/src/credentials_manager_client/main.py
+drwxr-xr-x   0 tof        (501) staff       (20)        0 2023-04-15 10:05:36.839993 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/
+-rw-r--r--   0 tof        (501) staff       (20)      182 2023-04-15 10:05:36.000000 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/PKG-INFO
+-rw-r--r--   0 tof        (501) staff       (20)      565 2023-04-15 10:05:36.000000 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tof        (501) staff       (20)        1 2023-04-15 10:05:36.000000 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tof        (501) staff       (20)       80 2023-04-15 10:05:36.000000 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/entry_points.txt
+-rw-r--r--   0 tof        (501) staff       (20)      119 2023-04-15 10:05:36.000000 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/requires.txt
+-rw-r--r--   0 tof        (501) staff       (20)       27 2023-04-15 10:05:36.000000 credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/top_level.txt
```

### Comparing `credentials-manager-client-0.0.1/setup.py` & `credentials_manager_client-0.1a-/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ('environs', '9.5.0'),
     ('psutil', '5.9.4'),
     ('fastapi', '0.85.0'),
     ('pydantic', '1.9.2'),
     ('SQLAlchemy', '1.4.36'),
 ]
 
-CI_PROJECT_NAME = os.environ.get("CI_PROJECT_NAME", "credentials_manager")
+CI_PROJECT_NAME = os.environ.get("CI_PROJECT_NAME", "credentials_manager_client")
 ARTIFACT_VERSION = os.environ.get("ARTIFACT_VERSION", "0.1a+")
 CI_PROJECT_TITLE = os.environ.get("CI_PROJECT_TITLE", "Backend service")
 CI_PROJECT_URL = os.environ.get("CI_PROJECT_URL", "https://github.com/makersdevs/credentials_manager")
 
 setup(
     name=CI_PROJECT_NAME,
     version=ARTIFACT_VERSION,
```

### Comparing `credentials-manager-client-0.0.1/src/credentials_manager_client.egg-info/SOURCES.txt` & `credentials_manager_client-0.1a-/src/credentials_manager_client.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-LICENSE
 README.md
-pyproject.toml
 setup.py
 src/credentials_manager_client/__init__.py
 src/credentials_manager_client/app.py
 src/credentials_manager_client/main.py
 src/credentials_manager_client.egg-info/PKG-INFO
 src/credentials_manager_client.egg-info/SOURCES.txt
 src/credentials_manager_client.egg-info/dependency_links.txt
 src/credentials_manager_client.egg-info/entry_points.txt
 src/credentials_manager_client.egg-info/requires.txt
 src/credentials_manager_client.egg-info/top_level.txt
 src/credentials_manager_client/apps/__init__.py
-src/credentials_manager_client/apps/auth/__init__.py
-src/credentials_manager_client/apps/auth/abstract_models.py
-src/credentials_manager_client/apps/auth/models.py
-src/credentials_manager_client/db/__init__.py
-src/credentials_manager_client/db/base_model.py
+src/credentials_manager_client/apps/auth/__init__.py
```

