# Comparing `tmp/airunner-1.8.17.tar.gz` & `tmp/airunner-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.8.17.tar", last modified: Fri Mar 31 17:01:00 2023, max compression
+gzip compressed data, was "airunner-1.9.0.tar", last modified: Sat Apr 15 20:46:32 2023, max compression
```

## Comparing `airunner-1.8.17.tar` & `airunner-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:01:00.784565 airunner-1.8.17/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 17:00:45.000000 airunner-1.8.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-31 17:01:00.784565 airunner-1.8.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-03-31 17:00:45.000000 airunner-1.8.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 17:01:00.784565 airunner-1.8.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-31 17:00:45.000000 airunner-1.8.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:01:00.780565 airunner-1.8.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:01:00.784565 airunner-1.8.17/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-31 17:01:00.000000 airunner-1.8.17/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-31 17:01:00.000000 airunner-1.8.17/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:01:00.000000 airunner-1.8.17/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-31 17:01:00.000000 airunner-1.8.17/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:01:00.000000 airunner-1.8.17/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.199985 airunner-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 20:46:20.000000 airunner-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-15 20:46:32.199985 airunner-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-15 20:46:20.000000 airunner-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:46:32.199985 airunner-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 20:46:20.000000 airunner-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.195985 airunner-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.199985 airunner-1.9.0/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16605 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62388 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/qtcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/settingsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-15 20:46:21.000000 airunner-1.9.0/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.199985 airunner-1.9.0/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.8.17/LICENSE` & `airunner-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.8.17/setup.py` & `airunner-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version='1.8.17',
+    version="1.9.0",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.8.19",
+        "aihandler==1.9.0",
     ]
 )
```

