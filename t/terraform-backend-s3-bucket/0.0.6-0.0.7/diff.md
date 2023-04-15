# Comparing `tmp/terraform-backend-s3-bucket-0.0.6.tar.gz` & `tmp/terraform-backend-s3-bucket-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraform-backend-s3-bucket-0.0.6.tar", last modified: Mon Apr 10 04:15:41 2023, max compression
+gzip compressed data, was "terraform-backend-s3-bucket-0.0.7.tar", last modified: Sat Apr 15 07:43:41 2023, max compression
```

## Comparing `terraform-backend-s3-bucket-0.0.6.tar` & `terraform-backend-s3-bucket-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17889 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:15:27.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:15:41.334872 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 04:15:41.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-10 04:15:41.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:15:41.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 04:15:41.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 04:15:41.000000 terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:43:41.351889 terraform-backend-s3-bucket-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-15 07:43:41.351889 terraform-backend-s3-bucket-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:43:41.351889 terraform-backend-s3-bucket-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:43:41.347889 terraform-backend-s3-bucket-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:43:41.351889 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:43:41.351889 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:43:29.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:43:41.351889 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-15 07:43:41.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-15 07:43:41.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:43:41.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 07:43:41.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 07:43:41.000000 terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/top_level.txt
```

### Comparing `terraform-backend-s3-bucket-0.0.6/LICENSE` & `terraform-backend-s3-bucket-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-0.0.6/PKG-INFO` & `terraform-backend-s3-bucket-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 0.0.6
-Summary: terraform-backend-s3-bucket
+Version: 0.0.7
+Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `terraform-backend-s3-bucket-0.0.6/README.md` & `terraform-backend-s3-bucket-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-0.0.6/setup.py` & `terraform-backend-s3-bucket-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "terraform-backend-s3-bucket",
-    "version": "0.0.6",
-    "description": "terraform-backend-s3-bucket",
+    "version": "0.0.7",
+    "description": "Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/terraform-backend-s3-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,23 +22,23 @@
     },
     "packages": [
         "terraform_backend_s3_bucket",
         "terraform_backend_s3_bucket._jsii"
     ],
     "package_data": {
         "terraform_backend_s3_bucket._jsii": [
-            "terraform-backend-s3-bucket@0.0.6.jsii.tgz"
+            "terraform-backend-s3-bucket@0.0.7.jsii.tgz"
         ],
         "terraform_backend_s3_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.70.0, <3.0.0",
+        "aws-cdk-lib>=2.74.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket/__init__.py` & `terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/PKG-INFO` & `terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 0.0.6
-Summary: terraform-backend-s3-bucket
+Version: 0.0.7
+Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `terraform-backend-s3-bucket-0.0.6/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt` & `terraform-backend-s3-bucket-0.0.7/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/terraform_backend_s3_bucket/py.typed
 src/terraform_backend_s3_bucket.egg-info/PKG-INFO
 src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
 src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
 src/terraform_backend_s3_bucket.egg-info/requires.txt
 src/terraform_backend_s3_bucket.egg-info/top_level.txt
 src/terraform_backend_s3_bucket/_jsii/__init__.py
-src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.6.jsii.tgz
+src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@0.0.7.jsii.tgz
```

