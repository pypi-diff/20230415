# Comparing `tmp/dauth-0.1.tar.gz` & `tmp/dauth-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauth-0.1.tar", last modified: Sun Apr  9 22:09:50 2023, max compression
+gzip compressed data, was "dauth-0.2.tar", last modified: Sat Apr 15 19:59:07 2023, max compression
```

## Comparing `dauth-0.1.tar` & `dauth-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 22:09:50.048246 dauth-0.1/
--rw-r--r--   0 vvelikovich (161766200) 593637566     1623 2023-04-09 22:09:50.048132 dauth-0.1/PKG-INFO
--rw-r--r--   0 vvelikovich (161766200) 593637566     1487 2023-04-09 21:37:25.000000 dauth-0.1/README.md
--rw-r--r--   0 vvelikovich (161766200) 593637566       38 2023-04-09 22:09:50.048279 dauth-0.1/setup.cfg
--rw-r--r--   0 vvelikovich (161766200) 593637566      600 2023-04-09 22:09:09.000000 dauth-0.1/setup.py
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 22:09:50.046793 dauth-0.1/src/
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 22:09:50.047346 dauth-0.1/src/dauth/
--rw-r--r--   0 vvelikovich (161766200) 593637566      149 2023-04-09 20:57:55.000000 dauth-0.1/src/dauth/__init__.py
--rw-r--r--   0 vvelikovich (161766200) 593637566      601 2023-04-09 21:17:50.000000 dauth-0.1/src/dauth/auth.py
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 22:09:50.047986 dauth-0.1/src/dauth.egg-info/
--rw-r--r--   0 vvelikovich (161766200) 593637566     1623 2023-04-09 22:09:50.000000 dauth-0.1/src/dauth.egg-info/PKG-INFO
--rw-r--r--   0 vvelikovich (161766200) 593637566      190 2023-04-09 22:09:50.000000 dauth-0.1/src/dauth.egg-info/SOURCES.txt
--rw-r--r--   0 vvelikovich (161766200) 593637566        1 2023-04-09 22:09:50.000000 dauth-0.1/src/dauth.egg-info/dependency_links.txt
--rw-r--r--   0 vvelikovich (161766200) 593637566        6 2023-04-09 22:09:50.000000 dauth-0.1/src/dauth.egg-info/top_level.txt
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.851535 dauth-0.2/
+-rw-r--r--   0 vvelikovich (161766200) 593637566     2705 2023-04-15 19:59:07.851419 dauth-0.2/PKG-INFO
+-rw-r--r--   0 vvelikovich (161766200) 593637566     2569 2023-04-15 19:57:46.000000 dauth-0.2/README.md
+-rw-r--r--   0 vvelikovich (161766200) 593637566       38 2023-04-15 19:59:07.851567 dauth-0.2/setup.cfg
+-rw-r--r--   0 vvelikovich (161766200) 593637566      600 2023-04-09 22:09:09.000000 dauth-0.2/setup.py
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.850242 dauth-0.2/src/
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.850767 dauth-0.2/src/dauth/
+-rw-r--r--   0 vvelikovich (161766200) 593637566      187 2023-04-15 19:47:47.000000 dauth-0.2/src/dauth/__init__.py
+-rw-r--r--   0 vvelikovich (161766200) 593637566      890 2023-04-15 19:58:38.000000 dauth-0.2/src/dauth/auth.py
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.851284 dauth-0.2/src/dauth.egg-info/
+-rw-r--r--   0 vvelikovich (161766200) 593637566     2705 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/PKG-INFO
+-rw-r--r--   0 vvelikovich (161766200) 593637566      190 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/SOURCES.txt
+-rw-r--r--   0 vvelikovich (161766200) 593637566        1 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/dependency_links.txt
+-rw-r--r--   0 vvelikovich (161766200) 593637566        6 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/top_level.txt
```

### Comparing `dauth-0.1/setup.py` & `dauth-0.2/setup.py`

 * *Files identical despite different names*

