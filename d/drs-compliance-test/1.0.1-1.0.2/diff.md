# Comparing `tmp/drs-compliance-test-1.0.1.tar.gz` & `tmp/drs-compliance-test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-test-1.0.1.tar", last modified: Sat Apr 15 02:43:19 2023, max compression
+gzip compressed data, was "drs-compliance-test-1.0.2.tar", last modified: Sat Apr 15 02:56:38 2023, max compression
```

## Comparing `drs-compliance-test-1.0.1.tar` & `drs-compliance-test-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:43:19.108393 drs-compliance-test-1.0.1/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-test-1.0.1/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)      414 2023-04-15 02:43:19.107732 drs-compliance-test-1.0.1/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-test-1.0.1/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:43:19.090811 drs-compliance-test-1.0.1/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-12 18:19:20.000000 drs-compliance-test-1.0.1/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-test-1.0.1/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-test-1.0.1/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:43:19.093551 drs-compliance-test-1.0.1/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:43:19.101584 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.1/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:43:19.106740 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)      414 2023-04-15 02:43:18.000000 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)      950 2023-04-15 02:43:19.000000 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 02:43:18.000000 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 02:43:18.000000 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 02:43:18.000000 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 02:43:18.000000 drs-compliance-test-1.0.1/drs_compliance_test.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 02:43:19.110123 drs-compliance-test-1.0.1/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1292 2023-04-15 02:42:17.000000 drs-compliance-test-1.0.1/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:56:38.506677 drs-compliance-test-1.0.2/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-test-1.0.2/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)      414 2023-04-15 02:56:38.505893 drs-compliance-test-1.0.2/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-test-1.0.2/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:56:38.486052 drs-compliance-test-1.0.2/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-12 18:19:20.000000 drs-compliance-test-1.0.2/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-test-1.0.2/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-test-1.0.2/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:56:38.489515 drs-compliance-test-1.0.2/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:56:38.499456 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-test-1.0.2/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 02:56:38.505078 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)      414 2023-04-15 02:56:38.000000 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)      950 2023-04-15 02:56:38.000000 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 02:56:38.000000 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 02:56:38.000000 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 02:56:38.000000 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 02:56:38.000000 drs-compliance-test-1.0.2/drs_compliance_test.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 02:56:38.509266 drs-compliance-test-1.0.2/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1292 2023-04-15 02:56:32.000000 drs-compliance-test-1.0.2/setup.py
```

### Comparing `drs-compliance-test-1.0.1/LICENSE` & `drs-compliance-test-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/README.md` & `drs-compliance-test-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/helper.py` & `drs-compliance-test-1.0.2/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/report_runner.py` & `drs-compliance-test-1.0.2/compliance_suite/report_runner.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/report_server.py` & `drs-compliance-test-1.0.2/compliance_suite/report_server.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/service_info.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/service_type.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-test-1.0.2/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/validate_drs_object_response.py` & `drs-compliance-test-1.0.2/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/compliance_suite/validate_response.py` & `drs-compliance-test-1.0.2/compliance_suite/validate_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/drs_compliance_test.egg-info/SOURCES.txt` & `drs-compliance-test-1.0.2/drs_compliance_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drs-compliance-test-1.0.1/setup.py` & `drs-compliance-test-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SUPPORTED_DRS_VERSIONS = ["1.2.0"]
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance-test",
-    version="1.0.1",
+    version="1.0.2",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
     package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
     long_description="test",
```

