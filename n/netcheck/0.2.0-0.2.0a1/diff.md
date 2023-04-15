# Comparing `tmp/netcheck-0.2.0.tar.gz` & `tmp/netcheck-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.2.0.tar", max compression
+gzip compressed data, was "netcheck-0.2.0a1.tar", max compression
```

## Comparing `netcheck-0.2.0.tar` & `netcheck-0.2.0a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-15 04:38:02.403201 netcheck-0.2.0/LICENSE
--rw-r--r--   0        0        0     7020 2023-04-15 04:38:02.403201 netcheck-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/__init__.py
--rw-r--r--   0        0        0     5896 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/cli.py
--rw-r--r--   0        0        0     2418 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/dns.py
--rw-r--r--   0        0        0     2192 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/http.py
--rw-r--r--   0        0        0     3406 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/runner.py
--rw-r--r--   0        0        0     1146 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/validation.py
--rw-r--r--   0        0        0      229 2023-04-15 04:38:02.415202 netcheck-0.2.0/netcheck/version.py
--rw-r--r--   0        0        0      850 2023-04-15 04:38:02.423201 netcheck-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 netcheck-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 04:20:27.771741 netcheck-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     7020 2023-04-15 04:20:27.771741 netcheck-0.2.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/__init__.py
+-rw-r--r--   0        0        0     5896 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/cli.py
+-rw-r--r--   0        0        0     2418 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/dns.py
+-rw-r--r--   0        0        0     2192 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/http.py
+-rw-r--r--   0        0        0     3406 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/runner.py
+-rw-r--r--   0        0        0     1146 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/validation.py
+-rw-r--r--   0        0        0      229 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/version.py
+-rw-r--r--   0        0        0      634 2023-04-15 04:20:27.791741 netcheck-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 netcheck-0.2.0a1/PKG-INFO
```

### Comparing `netcheck-0.2.0/LICENSE` & `netcheck-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/README.md` & `netcheck-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/netcheck/cli.py` & `netcheck-0.2.0a1/netcheck/cli.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/netcheck/dns.py` & `netcheck-0.2.0a1/netcheck/dns.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/netcheck/http.py` & `netcheck-0.2.0a1/netcheck/http.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/netcheck/runner.py` & `netcheck-0.2.0a1/netcheck/runner.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/netcheck/validation.py` & `netcheck-0.2.0a1/netcheck/validation.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0/PKG-INFO` & `netcheck-0.2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netcheck
-Version: 0.2.0
-Summary: Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration.
+Version: 0.2.0a1
+Summary: 
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cel-python (>=0.1.5,<0.2.0)
```

