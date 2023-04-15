# Comparing `tmp/drs-compliance-1.0.6.tar.gz` & `tmp/drs-compliance-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-1.0.6.tar", last modified: Sat Apr 15 03:55:31 2023, max compression
+gzip compressed data, was "drs-compliance-1.0.7.tar", last modified: Sat Apr 15 04:17:38 2023, max compression
```

## Comparing `drs-compliance-1.0.6.tar` & `drs-compliance-1.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.461048 drs-compliance-1.0.6/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.6/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 03:55:31.460575 drs-compliance-1.0.6/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.6/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.447904 drs-compliance-1.0.6/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6351 2023-04-15 03:08:13.000000 drs-compliance-1.0.6/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-1.0.6/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-1.0.6/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.449345 drs-compliance-1.0.6/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.453839 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.454535 drs-compliance-1.0.6/compliance_suite/web/
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.455598 drs-compliance-1.0.6/compliance_suite/web/static/
--rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/web/static/style.css
--rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-15 03:17:15.000000 drs-compliance-1.0.6/compliance_suite/web/temp_report.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.456268 drs-compliance-1.0.6/compliance_suite/web/templates/
--rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-1.0.6/compliance_suite/web/templates/index.html
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 03:55:31.460032 drs-compliance-1.0.6/drs_compliance.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 03:55:31.000000 drs-compliance-1.0.6/drs_compliance.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     1038 2023-04-15 03:55:31.000000 drs-compliance-1.0.6/drs_compliance.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 03:55:31.000000 drs-compliance-1.0.6/drs_compliance.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 03:55:31.000000 drs-compliance-1.0.6/drs_compliance.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 03:55:31.000000 drs-compliance-1.0.6/drs_compliance.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 03:55:31.000000 drs-compliance-1.0.6/drs_compliance.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 03:55:31.462258 drs-compliance-1.0.6/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1341 2023-04-15 03:55:18.000000 drs-compliance-1.0.6/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.810333 drs-compliance-1.0.7/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.7/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 04:17:38.809808 drs-compliance-1.0.7/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.7/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.795040 drs-compliance-1.0.7/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6351 2023-04-15 03:08:13.000000 drs-compliance-1.0.7/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17209 2023-04-15 04:16:58.000000 drs-compliance-1.0.7/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-15 04:16:57.000000 drs-compliance-1.0.7/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.796777 drs-compliance-1.0.7/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.802823 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.803587 drs-compliance-1.0.7/compliance_suite/web/
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.804686 drs-compliance-1.0.7/compliance_suite/web/static/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/web/static/style.css
+-rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-15 03:17:15.000000 drs-compliance-1.0.7/compliance_suite/web/temp_report.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.805360 drs-compliance-1.0.7/compliance_suite/web/templates/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-1.0.7/compliance_suite/web/templates/index.html
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-15 04:17:38.809288 drs-compliance-1.0.7/drs_compliance.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1038 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-15 04:17:38.000000 drs-compliance-1.0.7/drs_compliance.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-15 04:17:38.812365 drs-compliance-1.0.7/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1341 2023-04-15 04:17:36.000000 drs-compliance-1.0.7/setup.py
```

### Comparing `drs-compliance-1.0.6/LICENSE` & `drs-compliance-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/PKG-INFO` & `drs-compliance-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance
-Version: 1.0.6
+Version: 1.0.7
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drs-compliance-1.0.6/README.md` & `drs-compliance-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/helper.py` & `drs-compliance-1.0.7/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/report_runner.py` & `drs-compliance-1.0.7/compliance_suite/report_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,14 +442,16 @@
     if not os.path.exists("./output"):
         os.makedirs("./output")
 
     # write output report to file
     with open(args.report_path, 'w', encoding='utf-8') as f:
         json.dump(output_report_json, f, ensure_ascii=False, indent=4)
 
+    web_dir_path = os.path.join(os.path.dirname(__file__), 'web')
+
     if (args.serve):
-        with open("./compliance_suite/web/temp_report.json", 'w', encoding='utf-8') as f:
+        with open(web_dir_path+"/temp_report.json", 'w', encoding='utf-8') as f:
             json.dump(output_report_json, f, ensure_ascii=False, indent=4)
         start_mock_server(args.serve_port)
 
 if __name__=="__main__":
     main()
```

### Comparing `drs-compliance-1.0.6/compliance_suite/report_server.py` & `drs-compliance-1.0.7/compliance_suite/report_server.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/service_info.json` & `drs-compliance-1.0.7/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/service_type.json` & `drs-compliance-1.0.7/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-1.0.7/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/validate_drs_object_response.py` & `drs-compliance-1.0.7/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/validate_response.py` & `drs-compliance-1.0.7/compliance_suite/validate_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/web/static/style.css` & `drs-compliance-1.0.7/compliance_suite/web/static/style.css`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/web/temp_report.json` & `drs-compliance-1.0.7/compliance_suite/web/temp_report.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/compliance_suite/web/templates/index.html` & `drs-compliance-1.0.7/compliance_suite/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/drs_compliance.egg-info/PKG-INFO` & `drs-compliance-1.0.7/drs_compliance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance
-Version: 1.0.6
+Version: 1.0.7
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drs-compliance-1.0.6/drs_compliance.egg-info/SOURCES.txt` & `drs-compliance-1.0.7/drs_compliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.6/setup.py` & `drs-compliance-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SUPPORTED_DRS_VERSIONS = ["1.2.0"]
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance",
-    version="1.0.6",
+    version="1.0.7",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
     package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*', 'web/*', 'web/static/*', 'web/templates/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
     long_description=long_description,
```

