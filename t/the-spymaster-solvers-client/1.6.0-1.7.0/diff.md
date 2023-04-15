# Comparing `tmp/the-spymaster-solvers-client-1.6.0.tar.gz` & `tmp/the-spymaster-solvers-client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-spymaster-solvers-client-1.6.0.tar", last modified: Sat Apr  8 20:43:30 2023, max compression
+gzip compressed data, was "the-spymaster-solvers-client-1.7.0.tar", last modified: Sat Apr 15 12:55:24 2023, max compression
```

## Comparing `the-spymaster-solvers-client-1.6.0.tar` & `the-spymaster-solvers-client-1.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/
--rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      492 2023-04-08 20:40:54.000000 the-spymaster-solvers-client-1.6.0/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/
--rw-rw-r--   0 akali     (1000) akali     (1000)       60 2022-06-26 22:20:09.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1517 2023-01-27 16:28:55.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/client.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/
--rw-rw-r--   0 akali     (1000) akali     (1000)       93 2022-06-26 22:01:46.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      708 2022-06-26 22:42:36.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      156 2023-02-10 18:30:33.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/errors.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1263 2023-04-08 20:41:50.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/requests.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      740 2023-04-08 20:41:50.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/responses.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      597 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       68 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       29 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/top_level.txt
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 12:55:24.407241 the-spymaster-solvers-client-1.7.0/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-04-15 12:55:24.407241 the-spymaster-solvers-client-1.7.0/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-15 12:55:24.407241 the-spymaster-solvers-client-1.7.0/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      492 2023-04-15 12:54:44.000000 the-spymaster-solvers-client-1.7.0/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 12:55:24.403233 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       60 2022-06-26 22:20:09.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1517 2023-01-27 16:28:55.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/client.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 12:55:24.407241 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       93 2022-06-26 22:01:46.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      724 2023-04-15 12:48:54.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/base.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      156 2023-02-10 18:30:33.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/errors.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1263 2023-04-08 20:41:50.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/requests.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      740 2023-04-08 20:41:50.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/responses.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 12:55:24.407241 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-04-15 12:55:24.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      597 2023-04-15 12:55:24.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-15 12:55:24.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       68 2023-04-15 12:55:24.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       29 2023-04-15 12:55:24.000000 the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/top_level.txt
```

### Comparing `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/client.py` & `the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/client.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/base.py` & `the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pydantic import BaseModel
 
 
 class Solver(str, Enum):
     NAIVE = "naive"
     OLYMPIC = "olympic"
     SNA = "sna"
+    GPT = "gpt"
 
 
 class Difficulty(str, Enum):
     EASY = "easy"
     MEDIUM = "medium"
     HARD = "hard"
```

### Comparing `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/requests.py` & `the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/requests.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/responses.py` & `the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client/structs/responses.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/SOURCES.txt` & `the-spymaster-solvers-client-1.7.0/the_spymaster_solvers_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

