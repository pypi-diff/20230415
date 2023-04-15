# Comparing `tmp/drs-compliance-1.0.1.tar.gz` & `tmp/drs-compliance-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-1.0.1.tar", last modified: Fri Apr 14 18:10:23 2023, max compression
+gzip compressed data, was "drs-compliance-1.0.2.tar", last modified: Sat Apr 15 03:04:06 2023, max compression
```

## Comparing `drs-compliance-1.0.1.tar` & `drs-compliance-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.493146 drs-compliance-1.0.1/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.1/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-14 18:10:23.492486 drs-compliance-1.0.1/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.1/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.471738 drs-compliance-1.0.1/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-12 18:19:20.000000 drs-compliance-1.0.1/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-1.0.1/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-1.0.1/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.474266 drs-compliance-1.0.1/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.483430 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.491534 drs-compliance-1.0.1/drs_compliance.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)      920 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-14 18:10:23.494885 drs-compliance-1.0.1/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1259 2023-04-14 18:07:14.000000 drs-compliance-1.0.1/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:04:06.509205 drs-compliance-1.0.2/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.2/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)      409 2023-04-15 03:04:06.508637 drs-compliance-1.0.2/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.2/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:04:06.488375 drs-compliance-1.0.2/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-12 18:19:20.000000 drs-compliance-1.0.2/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-1.0.2/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-1.0.2/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:04:06.491154 drs-compliance-1.0.2/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:04:06.500170 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.2/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:04:06.507787 drs-compliance-1.0.2/drs_compliance.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)      409 2023-04-15 03:04:06.000000 drs-compliance-1.0.2/drs_compliance.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)      920 2023-04-15 03:04:06.000000 drs-compliance-1.0.2/drs_compliance.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 03:04:06.000000 drs-compliance-1.0.2/drs_compliance.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 03:04:06.000000 drs-compliance-1.0.2/drs_compliance.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 03:04:06.000000 drs-compliance-1.0.2/drs_compliance.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 03:04:06.000000 drs-compliance-1.0.2/drs_compliance.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 03:04:06.510611 drs-compliance-1.0.2/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1287 2023-04-15 03:03:59.000000 drs-compliance-1.0.2/setup.py
```

### Comparing `drs-compliance-1.0.1/LICENSE` & `drs-compliance-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/PKG-INFO` & `drs-compliance-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: drs-compliance
-Version: 1.0.1
-Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
-Home-page: https://github.com/ga4gh/drs-compliance-suite
-Author: Yash Puligundla
-Author-email: yasasvini.puligundla@ga4gh.org
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # drs-compliance-suite
 Tests to verify the compliance of a DRS implementation with GA4GH Data Repository Service (DRS) specification. 
 This compliance suite currently supports the following DRS versions and will aim to support more versions of DRS in the future.
 * DRS 1.2.0
 
 ## Installations
 - [Python 3.x](https://www.python.org/downloads/) is required to run DRS Compliance Suite natively or using PyPI package.
@@ -141,8 +129,8 @@
 
 ## Changelog
 ### v1.0.1
 * Fixed a bug in the docker deployment of DRS Compliance Suite 
 * Update README documentation
 
 ### v1.0.0
-* DRS Compliance Suite for [Data Repository Service v1.2.0](https://ga4gh.github.io/data-repository-service-schemas/preview/release/drs-1.2.0/docs/)
+* DRS Compliance Suite for [Data Repository Service v1.2.0](https://ga4gh.github.io/data-repository-service-schemas/preview/release/drs-1.2.0/docs/)
```

### Comparing `drs-compliance-1.0.1/compliance_suite/helper.py` & `drs-compliance-1.0.2/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/report_runner.py` & `drs-compliance-1.0.2/compliance_suite/report_runner.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/report_server.py` & `drs-compliance-1.0.2/compliance_suite/report_server.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/service_info.json` & `drs-compliance-1.0.2/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/service_type.json` & `drs-compliance-1.0.2/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-1.0.2/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/validate_drs_object_response.py` & `drs-compliance-1.0.2/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/compliance_suite/validate_response.py` & `drs-compliance-1.0.2/compliance_suite/validate_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/drs_compliance.egg-info/SOURCES.txt` & `drs-compliance-1.0.2/drs_compliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.1/setup.py` & `drs-compliance-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import setuptools
-from supported_drs_versions import SUPPORTED_DRS_VERSIONS
+# from supported_drs_versions import SUPPORTED_DRS_VERSIONS
+
+SUPPORTED_DRS_VERSIONS = ["1.2.0"]
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance",
-    version="1.0.1",
+    version="1.0.2",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
     package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
-    long_description=long_description,
+    long_description="test",
     long_description_content_type="text/markdown",
     url="https://github.com/ga4gh/drs-compliance-suite",
     license='MIT',
     python_requires='>=3.8',
     install_requires=['python-json-logger==2.0.4',
                       'structlog==21.5.0',
                       'requests==2.28.1',
```

