# Comparing `tmp/ondewo-csi-client-3.0.0.tar.gz` & `tmp/ondewo-csi-client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-csi-client-3.0.0.tar", last modified: Thu Sep 15 10:38:42 2022, max compression
+gzip compressed data, was "ondewo-csi-client-3.0.1.tar", last modified: Sat Apr 15 05:54:29 2023, max compression
```

## Comparing `ondewo-csi-client-3.0.0.tar` & `ondewo-csi-client-3.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3121 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2557 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 10:38:42.132944 ondewo-csi-client-3.0.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/ondewo/csi/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/ondewo/csi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1370 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      872 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/ondewo/csi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3151 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/client/services/conversations.py
--rw-rw-r--   0 root         (0) root         (0)      879 2022-09-15 10:38:08.000000 ondewo-csi-client-3.0.0/ondewo/csi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    16912 2022-09-15 10:38:27.000000 ondewo-csi-client-3.0.0/ondewo/csi/conversation_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    18957 2022-09-15 10:38:27.000000 ondewo-csi-client-3.0.0/ondewo/csi/conversation_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3121 2022-09-15 10:38:42.000000 ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2022-09-15 10:38:42.000000 ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 10:38:42.000000 ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      222 2022-09-15 10:38:42.000000 ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-09-15 10:38:42.000000 ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2022-09-15 10:38:42.136945 ondewo-csi-client-3.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1160 2022-09-15 10:38:27.000000 ondewo-csi-client-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:54:29.440475 ondewo-csi-client-3.0.1/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-04-15 05:54:29.440475 ondewo-csi-client-3.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6526 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:54:29.439475 ondewo-csi-client-3.0.1/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:54:29.439475 ondewo-csi-client-3.0.1/ondewo/csi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:54:29.439475 ondewo-csi-client-3.0.1/ondewo/csi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1370 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      872 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:54:29.440475 ondewo-csi-client-3.0.1/ondewo/csi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3151 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/client/services/conversations.py
+-rw-rw-r--   0 root         (0) root         (0)      879 2023-01-24 18:48:24.000000 ondewo-csi-client-3.0.1/ondewo/csi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    16912 2023-01-24 19:39:47.000000 ondewo-csi-client-3.0.1/ondewo/csi/conversation_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    18957 2023-01-24 19:39:47.000000 ondewo-csi-client-3.0.1/ondewo/csi/conversation_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:54:29.440475 ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-04-15 05:54:29.000000 ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-15 05:54:29.000000 ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 05:54:29.000000 ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-15 05:54:29.000000 ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-15 05:54:29.000000 ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-04-15 05:54:29.440475 ondewo-csi-client-3.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1902 2023-04-15 05:38:27.000000 ondewo-csi-client-3.0.1/setup.py
```

### Comparing `ondewo-csi-client-3.0.0/LICENSE` & `ondewo-csi-client-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo/csi/client/client.py` & `ondewo-csi-client-3.0.1/ondewo/csi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo/csi/client/client_config.py` & `ondewo-csi-client-3.0.1/ondewo/csi/client/client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo/csi/client/services/conversations.py` & `ondewo-csi-client-3.0.1/ondewo/csi/client/services/conversations.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo/csi/client/services_container.py` & `ondewo-csi-client-3.0.1/ondewo/csi/client/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo/csi/conversation_pb2.py` & `ondewo-csi-client-3.0.1/ondewo/csi/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo/csi/conversation_pb2_grpc.py` & `ondewo-csi-client-3.0.1/ondewo/csi/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.0.0/ondewo_csi_client.egg-info/SOURCES.txt` & `ondewo-csi-client-3.0.1/ondewo_csi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

