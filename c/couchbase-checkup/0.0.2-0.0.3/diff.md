# Comparing `tmp/couchbase-checkup-0.0.2.tar.gz` & `tmp/couchbase_checkup-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbase-checkup-0.0.2.tar", last modified: Sat Apr 15 08:50:09 2023, max compression
+gzip compressed data, was "couchbase_checkup-0.0.3.tar", last modified: Sat Apr 15 09:30:29 2023, max compression
```

## Comparing `couchbase-checkup-0.0.2.tar` & `couchbase_checkup-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:50:09.348320 couchbase-checkup-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-10 05:47:09.000000 couchbase-checkup-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-15 08:50:09.348320 couchbase-checkup-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5486 2023-04-12 09:21:36.000000 couchbase-checkup-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:50:09.348320 couchbase-checkup-0.0.2/couchbase_checkup.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-15 08:50:09.000000 couchbase-checkup-0.0.2/couchbase_checkup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-15 08:50:09.000000 couchbase-checkup-0.0.2/couchbase_checkup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 08:50:09.000000 couchbase-checkup-0.0.2/couchbase_checkup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-15 08:50:09.000000 couchbase-checkup-0.0.2/couchbase_checkup.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 08:50:09.000000 couchbase-checkup-0.0.2/couchbase_checkup.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 08:50:09.348320 couchbase-checkup-0.0.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      443 2023-04-15 08:50:07.000000 couchbase-checkup-0.0.2/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 09:30:29.275955 couchbase_checkup-0.0.3/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      746 2023-04-15 09:30:29.275955 couchbase_checkup-0.0.3/PKG-INFO
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 09:30:29.275955 couchbase_checkup-0.0.3/couchbase_checkup.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      746 2023-04-15 09:30:29.000000 couchbase_checkup-0.0.3/couchbase_checkup.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      212 2023-04-15 09:30:29.000000 couchbase_checkup-0.0.3/couchbase_checkup.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 09:30:29.000000 couchbase_checkup-0.0.3/couchbase_checkup.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       25 2023-04-15 09:30:29.000000 couchbase_checkup-0.0.3/couchbase_checkup.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 09:30:29.000000 couchbase_checkup-0.0.3/couchbase_checkup.egg-info/top_level.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       38 2023-04-15 09:30:29.275955 couchbase_checkup-0.0.3/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)      909 2023-04-15 09:25:01.000000 couchbase_checkup-0.0.3/setup.py
```

