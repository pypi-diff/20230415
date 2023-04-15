# Comparing `tmp/drs-compliance-1.0.7.tar.gz` & `tmp/drs-compliance-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-1.0.7.tar", last modified: Sat Apr 15 04:17:38 2023, max compression
+gzip compressed data, was "drs-compliance-1.0.8.tar", last modified: Sat Apr 15 04:34:31 2023, max compression
```

## Comparing `drs-compliance-1.0.7.tar` & `drs-compliance-1.0.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.810333 drs-compliance-1.0.7/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.7/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 04:17:38.809808 drs-compliance-1.0.7/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.7/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.795040 drs-compliance-1.0.7/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6351 2023-04-15 03:08:13.000000 drs-compliance-1.0.7/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17209 2023-04-15 04:16:58.000000 drs-compliance-1.0.7/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-15 04:16:57.000000 drs-compliance-1.0.7/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.796777 drs-compliance-1.0.7/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.802823 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.803587 drs-compliance-1.0.7/compliance_suite/web/
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.804686 drs-compliance-1.0.7/compliance_suite/web/static/
--rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/web/static/style.css
--rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-15 03:17:15.000000 drs-compliance-1.0.7/compliance_suite/web/temp_report.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.805360 drs-compliance-1.0.7/compliance_suite/web/templates/
--rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/web/templates/index.html
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.809288 drs-compliance-1.0.7/drs_compliance.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     1038 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 04:17:38.812365 drs-compliance-1.0.7/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1341 2023-04-15 04:17:36.000000 drs-compliance-1.0.7/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.433166 drs-compliance-1.0.8/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.8/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 04:34:31.432842 drs-compliance-1.0.8/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.8/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.418414 drs-compliance-1.0.8/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6351 2023-04-15 03:08:13.000000 drs-compliance-1.0.8/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17203 2023-04-15 04:34:29.000000 drs-compliance-1.0.8/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-15 04:16:57.000000 drs-compliance-1.0.8/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.420553 drs-compliance-1.0.8/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.426161 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3643 2023-04-15 04:34:29.000000 drs-compliance-1.0.8/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.427109 drs-compliance-1.0.8/compliance_suite/web/
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.428638 drs-compliance-1.0.8/compliance_suite/web/static/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/web/static/style.css
+-rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-15 03:17:15.000000 drs-compliance-1.0.8/compliance_suite/web/temp_report.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.429637 drs-compliance-1.0.8/compliance_suite/web/templates/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-1.0.8/compliance_suite/web/templates/index.html
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:34:31.432424 drs-compliance-1.0.8/drs_compliance.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 04:34:31.000000 drs-compliance-1.0.8/drs_compliance.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1038 2023-04-15 04:34:31.000000 drs-compliance-1.0.8/drs_compliance.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 04:34:31.000000 drs-compliance-1.0.8/drs_compliance.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 04:34:31.000000 drs-compliance-1.0.8/drs_compliance.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 04:34:31.000000 drs-compliance-1.0.8/drs_compliance.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 04:34:31.000000 drs-compliance-1.0.8/drs_compliance.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 04:34:31.434016 drs-compliance-1.0.8/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1341 2023-04-15 04:34:29.000000 drs-compliance-1.0.8/setup.py
```

### Comparing `drs-compliance-1.0.7/LICENSE` & `drs-compliance-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/PKG-INFO` & `drs-compliance-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance
-Version: 1.0.7
+Version: 1.0.8
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drs-compliance-1.0.7/README.md` & `drs-compliance-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/helper.py` & `drs-compliance-1.0.8/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/report_runner.py` & `drs-compliance-1.0.8/compliance_suite/report_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         schema_file = SERVICE_INFO_SCHEMA,
         expected_status_code = "200",
         expected_content_type = "application/json")
 
     service_info_phase.set_end_time_now()
 
     # TODO : Add a test case to check that drs version from service-info == drs_version provided.
-    schema_dir = "v" + drs_version + "/"
+    schema_dir = "v" + drs_version
 
     # TODO: extend support to DRS v1.3.0 -
     #  1. make a json map of endpoints per each DRS version
     #  using which phases are created and added to the report object
     #  2. schema_dir should take care of pulling the right schema for validation
     #  3. Add the version to supported_drs_versions
     #  4. add any version specific test cases
```

### Comparing `drs-compliance-1.0.7/compliance_suite/report_server.py` & `drs-compliance-1.0.8/compliance_suite/report_server.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/service_info.json` & `drs-compliance-1.0.8/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/service_type.json` & `drs-compliance-1.0.8/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-1.0.8/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/validate_drs_object_response.py` & `drs-compliance-1.0.8/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/validate_response.py` & `drs-compliance-1.0.8/compliance_suite/validate_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,16 @@
             schema = json.load(file)
         return schema
 
     def validate_response_schema(self):
         if self.case.get_status() == Status.SKIP:
             self.case.set_end_time_now()
             return
+
+        # schema_dir_path = os.path.join(os.path.dirname(__file__), 'schemas')
         expected_schema_file_path = os.path.join(SCHEMA_DIR, self.response_schema_file)
         expected_schema = self.get_schema(expected_schema_file_path)
         absolute_schema_file_path = os.path.dirname(os.path.abspath(expected_schema_file_path))
         reference_resolver = jsonschema.RefResolver(base_uri=f"file://{absolute_schema_file_path}/", referrer=None)
         try:
             validate(instance=self.actual_response.json(), resolver=reference_resolver, schema=expected_schema)
             self.case.set_message("Schema Validation Successful")
```

### Comparing `drs-compliance-1.0.7/compliance_suite/web/static/style.css` & `drs-compliance-1.0.8/compliance_suite/web/static/style.css`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/web/temp_report.json` & `drs-compliance-1.0.8/compliance_suite/web/temp_report.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/compliance_suite/web/templates/index.html` & `drs-compliance-1.0.8/compliance_suite/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/drs_compliance.egg-info/PKG-INFO` & `drs-compliance-1.0.8/drs_compliance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance
-Version: 1.0.7
+Version: 1.0.8
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drs-compliance-1.0.7/drs_compliance.egg-info/SOURCES.txt` & `drs-compliance-1.0.8/drs_compliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.7/setup.py` & `drs-compliance-1.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SUPPORTED_DRS_VERSIONS = ["1.2.0"]
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance",
-    version="1.0.7",
+    version="1.0.8",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
     package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*', 'web/*', 'web/static/*', 'web/templates/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
     long_description=long_description,
```

