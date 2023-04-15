# Comparing `tmp/drs-compliance-1.0.4.tar.gz` & `tmp/drs-compliance-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-1.0.4.tar", last modified: Sat Apr 15 03:46:04 2023, max compression
+gzip compressed data, was "drs-compliance-1.0.5.tar", last modified: Sat Apr 15 03:52:25 2023, max compression
```

## Comparing `drs-compliance-1.0.4.tar` & `drs-compliance-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:46:04.161821 drs-compliance-1.0.4/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.4/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 03:46:04.161461 drs-compliance-1.0.4/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.4/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:46:04.148826 drs-compliance-1.0.4/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6351 2023-04-15 03:08:13.000000 drs-compliance-1.0.4/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-1.0.4/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-1.0.4/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:46:04.150384 drs-compliance-1.0.4/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:46:04.156104 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.4/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:46:04.156941 drs-compliance-1.0.4/compliance_suite/web/
--rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-15 03:17:15.000000 drs-compliance-1.0.4/compliance_suite/web/temp_report.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:46:04.161044 drs-compliance-1.0.4/drs_compliance.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 03:46:04.000000 drs-compliance-1.0.4/drs_compliance.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)      958 2023-04-15 03:46:04.000000 drs-compliance-1.0.4/drs_compliance.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 03:46:04.000000 drs-compliance-1.0.4/drs_compliance.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 03:46:04.000000 drs-compliance-1.0.4/drs_compliance.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 03:46:04.000000 drs-compliance-1.0.4/drs_compliance.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 03:46:04.000000 drs-compliance-1.0.4/drs_compliance.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 03:46:04.162625 drs-compliance-1.0.4/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1306 2023-04-15 03:45:40.000000 drs-compliance-1.0.4/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.210946 drs-compliance-1.0.5/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.5/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 03:52:25.210567 drs-compliance-1.0.5/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.5/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.192625 drs-compliance-1.0.5/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6351 2023-04-15 03:08:13.000000 drs-compliance-1.0.5/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-1.0.5/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-1.0.5/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.195427 drs-compliance-1.0.5/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.202467 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.203178 drs-compliance-1.0.5/compliance_suite/web/
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.205095 drs-compliance-1.0.5/compliance_suite/web/static/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/web/static/style.css
+-rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-15 03:17:15.000000 drs-compliance-1.0.5/compliance_suite/web/temp_report.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.206017 drs-compliance-1.0.5/compliance_suite/web/templates/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-1.0.5/compliance_suite/web/templates/index.html
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:52:25.210050 drs-compliance-1.0.5/drs_compliance.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 03:52:25.000000 drs-compliance-1.0.5/drs_compliance.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1038 2023-04-15 03:52:25.000000 drs-compliance-1.0.5/drs_compliance.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 03:52:25.000000 drs-compliance-1.0.5/drs_compliance.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 03:52:25.000000 drs-compliance-1.0.5/drs_compliance.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 03:52:25.000000 drs-compliance-1.0.5/drs_compliance.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 03:52:25.000000 drs-compliance-1.0.5/drs_compliance.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 03:52:25.211723 drs-compliance-1.0.5/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1341 2023-04-15 03:52:22.000000 drs-compliance-1.0.5/setup.py
```

### Comparing `drs-compliance-1.0.4/LICENSE` & `drs-compliance-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/PKG-INFO` & `drs-compliance-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance
-Version: 1.0.4
+Version: 1.0.5
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drs-compliance-1.0.4/README.md` & `drs-compliance-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/helper.py` & `drs-compliance-1.0.5/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/report_runner.py` & `drs-compliance-1.0.5/compliance_suite/report_runner.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/report_server.py` & `drs-compliance-1.0.5/compliance_suite/report_server.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/service_info.json` & `drs-compliance-1.0.5/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/service_type.json` & `drs-compliance-1.0.5/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-1.0.5/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/validate_drs_object_response.py` & `drs-compliance-1.0.5/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/validate_response.py` & `drs-compliance-1.0.5/compliance_suite/validate_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/compliance_suite/web/temp_report.json` & `drs-compliance-1.0.5/compliance_suite/web/temp_report.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.4/drs_compliance.egg-info/PKG-INFO` & `drs-compliance-1.0.5/drs_compliance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance
-Version: 1.0.4
+Version: 1.0.5
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drs-compliance-1.0.4/drs_compliance.egg-info/SOURCES.txt` & `drs-compliance-1.0.5/drs_compliance.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,13 +14,15 @@
 compliance_suite/schemas/v1.2.0/access_url.json
 compliance_suite/schemas/v1.2.0/checksum.json
 compliance_suite/schemas/v1.2.0/contents_object.json
 compliance_suite/schemas/v1.2.0/drs_bundle.json
 compliance_suite/schemas/v1.2.0/drs_object.json
 compliance_suite/schemas/v1.2.0/error.json
 compliance_suite/web/temp_report.json
+compliance_suite/web/static/style.css
+compliance_suite/web/templates/index.html
 drs_compliance.egg-info/PKG-INFO
 drs_compliance.egg-info/SOURCES.txt
 drs_compliance.egg-info/dependency_links.txt
 drs_compliance.egg-info/entry_points.txt
 drs_compliance.egg-info/requires.txt
 drs_compliance.egg-info/top_level.txt
```

### Comparing `drs-compliance-1.0.4/setup.py` & `drs-compliance-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 SUPPORTED_DRS_VERSIONS = ["1.2.0"]
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance",
-    version="1.0.4",
+    version="1.0.5",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
-    package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*', 'web/*']},
+    package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*', 'web/*', 'web/static/*', 'web/templates/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ga4gh/drs-compliance-suite",
     license='MIT',
     python_requires='>=3.8',
```

