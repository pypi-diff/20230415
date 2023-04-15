# Comparing `tmp/poe-web-client-0.0.6.tar.gz` & `tmp/poe-web-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe-web-client-0.0.6.tar", last modified: Tue Apr 11 01:11:21 2023, max compression
+gzip compressed data, was "poe-web-client-0.0.7.tar", last modified: Sat Apr 15 01:54:34 2023, max compression
```

## Comparing `poe-web-client-0.0.6.tar` & `poe-web-client-0.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.945840 poe-web-client-0.0.6/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)    35149 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/LICENSE
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-11 01:11:21.945340 poe-web-client-0.0.6/PKG-INFO
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8459 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/README.md
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.879882 poe-web-client-0.0.6/poe-api/
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.883332 poe-web-client-0.0.6/poe-api/src/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)    12092 2023-04-11 01:10:38.000000 poe-web-client-0.0.6/poe-api/src/poe.py
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.940478 poe-web-client-0.0.6/poe-api/src/poe_graphql/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1093 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      373 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       97 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/BioFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       73 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      100 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     6971 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      686 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      154 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      160 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      123 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      103 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/HandleFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      306 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1885 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      135 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      194 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      145 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      216 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      710 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      263 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      213 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      308 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      159 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      162 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       95 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      147 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      368 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      400 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1038 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      657 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)        0 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/__init__.py
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.944593 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     2035 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)        1 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       46 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/requires.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       16 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/top_level.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       38 2023-04-11 01:11:21.945955 poe-web-client-0.0.6/setup.cfg
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1044 2023-04-11 01:10:03.000000 poe-web-client-0.0.6/setup.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-15 01:54:34.339688 poe-web-client-0.0.7/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)    35149 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/LICENSE
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-15 01:54:34.339062 poe-web-client-0.0.7/PKG-INFO
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8459 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/README.md
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-15 01:54:34.274793 poe-web-client-0.0.7/poe-api/
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-15 01:54:34.277364 poe-web-client-0.0.7/poe-api/src/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)    12521 2023-04-15 01:51:53.000000 poe-web-client-0.0.7/poe-api/src/poe.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-15 01:54:34.323746 poe-web-client-0.0.7/poe-api/src/poe_graphql/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1093 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      373 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       97 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/BioFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       73 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      100 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     6971 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      686 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      154 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      160 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      123 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      103 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      306 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1885 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      135 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      194 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      145 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      216 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      710 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      263 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      213 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      308 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      159 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      162 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       95 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      147 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      368 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      400 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1038 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      657 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)        0 2023-04-09 00:01:12.000000 poe-web-client-0.0.7/poe-api/src/poe_graphql/__init__.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-15 01:54:34.338161 poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-15 01:54:34.000000 poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     2035 2023-04-15 01:54:34.000000 poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)        1 2023-04-15 01:54:34.000000 poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       46 2023-04-15 01:54:34.000000 poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/requires.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       16 2023-04-15 01:54:34.000000 poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/top_level.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       38 2023-04-15 01:54:34.339832 poe-web-client-0.0.7/setup.cfg
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1044 2023-04-15 01:52:42.000000 poe-web-client-0.0.7/setup.py
```

### Comparing `poe-web-client-0.0.6/LICENSE` & `poe-web-client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/PKG-INFO` & `poe-web-client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-web-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api
 Home-page: https://github.com/libaiabcd/poe-api
 Author: libaiabcd
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `poe-web-client-0.0.6/README.md` & `poe-web-client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe.py` & `poe-web-client-0.0.7/poe-api/src/poe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests, re, json, random, logging, time, queue, threading, traceback
+import requests, re, json, random, logging, time, queue, threading, traceback, hashlib
 import websocket
 from pathlib import Path
 from urllib.parse import urlparse
 
 parent_path = Path(__file__).resolve().parent
 queries_path = parent_path / "poe_graphql"
 queries = {}
@@ -37,96 +37,92 @@
   raise RuntimeError(f"Failed to download {url} too many times.")
 
 class Client:
   gql_url = "https://poe.com/api/gql_POST"
   gql_recv_url = "https://poe.com/api/receive_POST"
   home_url = "https://poe.com"
   settings_url = "https://poe.com/api/settings"
-
-  formkey = ""
-  next_data = {}
-  bots = {}
-  active_messages = {}
-  message_queues = {}
-  ws = None
-  ws_connected = False
-
-  token = ""
   
   def __init__(self, token, proxy=None):
     self.proxy = proxy
     self.token = token
     self.session = requests.Session()
         
     if proxy:
       self.session.proxies = {
         "http": self.proxy,
         "https": self.proxy
       }
       logger.info(f"Proxy enabled: {self.proxy}")
 
+    self.active_messages = {}
+    self.message_queues = {}
+
     self.session.cookies.set("p-b", token, domain="poe.com")
     self.headers = {
       "User-Agent": user_agent,
       "Referrer": "https://poe.com/",
       "Origin": "https://poe.com",
     }
     self.ws_domain = f"tch{random.randint(1, 1e6)}"
 
     self.session.headers.update(self.headers)
-    self.next_data = self.get_next_data()
+    self.next_data = self.get_next_data(overwrite_vars=True)
     self.channel = self.get_channel_data()
     self.connect_ws()
-    self.bots = self.get_bots()
+    self.bots = self.get_bots(download_next_data=False)
     self.bot_names = self.get_bot_names()
 
     self.gql_headers = {
       "poe-formkey": self.formkey,
       "poe-tchannel": self.channel["channel"],
     }
     self.gql_headers = {**self.gql_headers, **self.headers}
     self.subscribe()
     
-  def get_next_data(self):
+  def get_next_data(self, overwrite_vars=False):
     logger.info("Downloading next_data...")
     
     r = request_with_retries(self.session.get, self.home_url)
     json_regex = r'<script id="__NEXT_DATA__" type="application\/json">(.+?)</script>'
     json_text = re.search(json_regex, r.text).group(1)
     next_data = json.loads(json_text)
 
-    self.formkey = next_data["props"]["formkey"]
-    self.viewer = next_data["props"]["pageProps"]["payload"]["viewer"]
+    if overwrite_vars:
+      self.formkey = next_data["props"]["formkey"]
+      self.viewer = next_data["props"]["pageProps"]["payload"]["viewer"]
     
     return next_data
   
   def get_bot(self, display_name):
     url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/{display_name}.json'
     logger.info("Downloading "+url)
     
     r = request_with_retries(self.session.get, url)
 
     chat_data = r.json()["pageProps"]["payload"]["chatOfBotDisplayName"]
     return chat_data
     
-
-  def get_bots(self):
-    viewer = self.next_data["props"]["pageProps"]["payload"]["viewer"]
-    if not "availableBots" in viewer:
-      raise RuntimeError("Invalid token.")
-    bot_list = viewer["availableBots"]
+  def get_bots(self, download_next_data=True):
+    if download_next_data:
+      next_data = self.get_next_data()
+    else:
+      next_data = self.next_data
+
+    if not "availableBots" in self.viewer:
+      raise RuntimeError("Invalid token or no bots are available.")
+    bot_list = self.viewer["availableBots"]
 
     bots = {}
     for bot in bot_list:
-      try:
-        chat_data = self.get_bot(bot["displayName"])
-        bots[chat_data["defaultBotObject"]["nickname"]] = chat_data
-      except:
-        pass
-          
+      chat_data = self.get_bot(bot["displayName"])
+      bots[chat_data["defaultBotObject"]["nickname"]] = chat_data
+
+    self.bots = bots
+    self.bot_names = self.get_bot_names()
     return bots
   
   def get_bot_names(self):
     bot_names = {}
     for bot_nickname in self.bots:
       bot_obj = self.bots[bot_nickname]["defaultBotObject"]
       bot_names[bot_nickname] = bot_obj["displayName"]
@@ -144,16 +140,27 @@
     if channel is None:
       channel = self.channel
     query = f'?min_seq={channel["minSeq"]}&channel={channel["channel"]}&hash={channel["channelHash"]}'
     return f'wss://{self.ws_domain}.tch.{channel["baseHost"]}/up/{channel["boxName"]}/updates'+query
 
   def send_query(self, query_name, variables):
     for i in range(20):
-      payload = generate_payload(query_name, variables)
-      r = request_with_retries(self.session.post, self.gql_url, json=payload, headers=self.gql_headers)
+      json_data = generate_payload(query_name, variables)
+      payload = json.dumps(json_data, separators=(',', ':'))
+
+      base_string = payload + self.gql_headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+
+      headers = self.gql_headers | {
+        "content-type": "application/json",
+        "poe-tag-id": hashlib.md5(base_string.encode()).hexdigest()
+      }
+
+      r = request_with_retries(
+        self.session.post, self.gql_url, data=payload, headers=headers)
+
       data = r.json()
       if data["data"] == None:
         logger.warn(f'{query_name} returned an error: {data["errors"][0]["message"]} | Retrying ({i+1}/20)')
         time.sleep(2)
         continue
 
       return r.json()
@@ -184,49 +191,43 @@
         "http_proxy_host": proxy_parsed.hostname,
         "http_proxy_port": proxy_parsed.port
       }
 
     self.ws.run_forever(**kwargs)
 
   def connect_ws(self):
-    tmpurl = self.get_websocket_url()
-    logger.info(f"connect_ws {tmpurl} ")
+    self.ws_connected = False
     self.ws = websocket.WebSocketApp(
-      tmpurl,
+      self.get_websocket_url(),
       header={"User-Agent": user_agent},
       on_message=self.on_message,
       on_open=self.on_ws_connect,
       on_error=self.on_ws_error,
       on_close=self.on_ws_close
     )
     t = threading.Thread(target=self.ws_run_thread, daemon=True)
     t.start()
     while not self.ws_connected:
       time.sleep(0.01)
-    logger.info(f"connect_ws done")
   
   def disconnect_ws(self):
-    logger.info(f"disconnect_ws {self.ws} ")
     if self.ws:
       self.ws.close()
     self.ws_connected = False
   
   def on_ws_connect(self, ws):
-    logger.info(f"on_ws_connect:{ws}")
     self.ws_connected = True
   
   def on_ws_close(self, ws, close_status_code, close_message):
     self.ws_connected = False
     logger.warn(f"Websocket closed with status {close_status_code}: {close_message}")
   
   def on_ws_error(self, ws, error):
-    logger.info(f"on_ws_error:{ws},{error}")
     self.disconnect_ws()
     self.connect_ws()
-    logger.info(f"on_ws_error done:{ws},{error}")
 
   def on_message(self, ws, msg):
     try:
       data = json.loads(msg)
 
       if not "messages" in data:
         return
@@ -323,36 +324,43 @@
       "chatId": self.bots[chatbot]["chatId"]
     })
     return result["data"]["messageBreakCreate"]["message"]
 
   def get_message_history(self, chatbot, count=25, cursor=None):
     logger.info(f"Downloading {count} messages from {chatbot}")
 
+    messages = []
     if cursor == None:
       chat_data = self.get_bot(self.bot_names[chatbot])
       if not chat_data["messagesConnection"]["edges"]:
         return []
-      cursor = chat_data["messagesConnection"]["edges"][-1]["cursor"]
+      messages = chat_data["messagesConnection"]["edges"][:count]
+      cursor = chat_data["messagesConnection"]["pageInfo"]["startCursor"]
+      count -= len(messages)
 
     cursor = str(cursor)
     if count > 50:
-      messages = self.get_message_history(chatbot, count=50, cursor=cursor)
+      messages = self.get_message_history(chatbot, count=50, cursor=cursor) + messages
       while count > 0:
+        count -= 50
         new_cursor = messages[0]["cursor"]
         new_messages = self.get_message_history(chatbot, min(50, count), cursor=new_cursor)
         messages = new_messages + messages
-        count -= 50
       return messages
-      
+    elif count <= 0:
+      return messages
+
     result = self.send_query("ChatListPaginationQuery", {
       "count": count,
       "cursor": cursor,
       "id": self.bots[chatbot]["id"]
     })
-    return result["data"]["node"]["messagesConnection"]["edges"]
+    query_messages = result["data"]["node"]["messagesConnection"]["edges"]
+    messages = query_messages + messages
+    return messages
 
   def delete_message(self, message_ids):
     logger.info(f"Deleting messages: {message_ids}")
     if not type(message_ids) is list:
       message_ids = [int(message_ids)]
 
     result = self.send_query("DeleteMessageMutation", {
```

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatPaginationQuery.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageAddedSubscription.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/SendMessageMutation.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateFragment.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `poe-web-client-0.0.7/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/PKG-INFO` & `poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-web-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api
 Home-page: https://github.com/libaiabcd/poe-api
 Author: libaiabcd
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/SOURCES.txt` & `poe-web-client-0.0.7/poe-api/src/poe_web_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.6/setup.py` & `poe-web-client-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #pip wheel --no-deps -w dist .
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 setuptools.setup(
   name="poe-web-client",
-  version="0.0.6",
+  version="0.0.7",
   author="libaiabcd",
   license="GPLv3",
   description="A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=["poe_graphql"],
   classifiers=[
```

