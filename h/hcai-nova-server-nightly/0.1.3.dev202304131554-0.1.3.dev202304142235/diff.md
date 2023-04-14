# Comparing `tmp/hcai-nova-server-nightly-0.1.3.dev202304131554.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.3.dev202304142235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202304131554.tar", last modified: Thu Apr 13 15:54:21 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202304142235.tar", last modified: Fri Apr 14 22:35:23 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554.tar` & `hcai-nova-server-nightly-0.1.3.dev202304142235.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.112242 hcai-nova-server-nightly-0.1.3.dev202304131554/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-04-13 15:54:21.112242 hcai-nova-server-nightly-0.1.3.dev202304131554/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.108242 hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-04-13 15:54:21.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-13 15:54:21.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 15:54:21.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-13 15:54:21.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-13 15:54:21.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.108242 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.108242 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/logs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.108242 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     6548 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.108242 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:21.112242 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 15:54:21.112242 hcai-nova-server-nightly-0.1.3.dev202304131554/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-13 15:54:13.000000 hcai-nova-server-nightly-0.1.3.dev202304131554/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-04-14 22:35:23.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-14 22:35:23.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 22:35:23.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-14 22:35:23.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-14 22:35:23.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/logs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8547 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7845 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10762 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 22:35:23.573400 hcai-nova-server-nightly-0.1.3.dev202304142235/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-14 22:35:14.000000 hcai-nova-server-nightly-0.1.3.dev202304142235/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202304142235/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202304131554
+Version: 0.1.3.dev202304142235
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/README.md` & `hcai-nova-server-nightly-0.1.3.dev202304142235/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202304131554
+Version: 0.1.3.dev202304142235
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.3.dev202304142235/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/nova_backend.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -155,26 +155,31 @@
                 if not extractor.chainable:
                     raise AssertionError(
                         "Extraction module does not not support further chaining but is not the last link in chain."
                     )
 
                 # TODO implement nova data types in the server module
                 # TODO process data and write tmp session files to disk if necessary
+                logger.info("Extract data...")
                 data = extractor.process_data(ds_iter)
                 ds_iter = extractor.to_ds_iterable(data)
+                logger.info("...done")
 
             # Last element of chain
             else:
+                logger.info("Extract data...")
                 data = extractor.process_data(ds_iter)
                 stream_dict = extractor.to_stream(data)
+                logger.info("...done")
 
                 # Write to disk
                 if not stream_dict:
                     raise ValueError("Stream data is none")
                 else:
+                    logger.info("Write data to disk...")
                     for stream_id, (data_type, sr, data) in stream_dict.items():
 
                         out_path = Path(ds_iter.nova_data_dir) / ds_iter.dataset / ds_iter.sessions[0] / stream_id
 
                         # SSI-Stream
                         if data_type == DataTypes.FEATURE:
                             ftype = FileTypes.BINARY
@@ -203,10 +208,14 @@
                         # Video Data
                         elif data_type == DataTypes.VIDEO:
                             raise NotImplementedError()
 
                         # Annotations
                         elif data_type in AnnoTypes:
                             raise NotImplementedError()
+                    logger.info("...done")
+
+        logger.info("Extraction completed!")
+        status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
         logger.info("Action 'Extract' finished.")
         # TODO: Start legacy ssi chain support
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/predict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This file contains the general logic for predicting annotations to the nova database"""
-
+import copy
 import os
 from pathlib import Path, PureWindowsPath
 from nova_server.utils import db_utils
 from flask import Blueprint, request, jsonify
 from nova_utils.ssi_utils.ssi_xml_utils import Trainer
 from importlib.machinery import SourceFileLoader
 from nova_server.utils.thread_utils import THREADS
@@ -12,14 +12,18 @@
 from nova_server.utils import (
     thread_utils,
     status_utils,
     log_utils,
     dataset_utils,
     import_utils,
 )
+from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import (
+    HcaiNovaDynamicIterable,
+)
+from nova_utils.interfaces.server_module import Trainer as iTrainer
 from flask import current_app
 
 predict = Blueprint("predict", __name__)
 
 
 @predict.route("/predict", methods=["POST"])
 def predict_thread():
@@ -37,15 +41,17 @@
 @thread_utils.ml_thread_wrapper
 def predict_data(request_form, app_context):
     key = get_key_from_request_form(request_form)
     logger = log_utils.get_logger_for_thread(key)
     cml_dir = app_context.config["CML_DIR"]
     data_dir = app_context.config["DATA_DIR"]
 
-    # try:
+    log_conform_request = dict(request_form)
+    log_conform_request["password"] = "---"
+
     logger.info("Action 'Predict' started.")
     status_utils.update_status(key, status_utils.JobStatus.RUNNING)
     sessions = request_form["sessions"].split(";")
     roles = request_form["roles"].split(";")
     trainer_file_path = Path(cml_dir).joinpath(
         PureWindowsPath(request_form["trainerFilePath"])
     )
@@ -60,110 +66,146 @@
         logger.info("Trainer successfully loaded.")
 
     if not trainer.model_script_path:
         logger.error('Trainer has no attribute "script" in model tag.')
         status_utils.update_status(key, status_utils.JobStatus.ERROR)
         return None
 
-    model_script = None
+    # TODO: Integrate multi_role_input attribute in xml trainer files
+    multi_role_input = True
 
-    # Load Data
-    for session in sessions:
-        request_form[
-            "sessions"
-        ] = session  # overwrite so we handle each session seperatly..
-        for role in roles:
-            try:
-                update_progress(key, "Data loading")
-                request_form["roles"] = role
-                ds_iter = dataset_utils.dataset_from_request_form(
-                    request_form, data_dir
+    # Load data
+    try:
+        update_progress(key, "Data loading")
+        sessions = request_form.pop("sessions").split(";")
+        roles = request_form.pop("roles").split(";")
+        iterators = []
+        for session in sessions:
+            request_form["sessions"] = session
+            if multi_role_input:
+                request_form["roles"] = ";".join(roles)
+                iterators.append(
+                    dataset_utils.dataset_from_request_form(request_form, data_dir)
                 )
-                logger.info("Prediction data successfully loaded.")
-            except ValueError:
-                log_utils.remove_log_from_dict(key)
-                logger.error("Not able to load the data from the database!")
-                status_utils.update_status(key, status_utils.JobStatus.ERROR)
-                return
-
-            # Load the model_script only once
-            if model_script is None:
-                # Load Trainer
-                model_script_path = trainer_file_path.parent / trainer.model_script_path
-                source = SourceFileLoader(
-                    "model_script", str(model_script_path)
-                ).load_module()
-                import_utils.assert_or_install_dependencies(
-                    source.REQUIREMENTS, Path(model_script_path).stem
-                )
-                model_script = source.TrainerClass(ds_iter, logger, request_form)
+            else:
+                for role in roles:
+                    request_form["roles"] = role
+                    iterators.append(
+                        dataset_utils.dataset_from_request_form(request_form, data_dir)
+                    )
+
+        logger.info("Data iterators initialized.")
+    except ValueError as e:
+        print(e)
+        log_utils.remove_log_from_dict(key)
+        logger.error("Not able to load the data from the database!")
+        status_utils.update_status(key, status_utils.JobStatus.ERROR)
+        return None
+
+
+    # Load Trainer
+    model_script_path = trainer_file_path.parent / trainer.model_script_path
+    source = SourceFileLoader(
+        "ns_tr_" + model_script_path.stem, str(model_script_path)
+    ).load_module()
+    import_utils.assert_or_install_dependencies(
+        source.REQUIREMENTS, Path(model_script_path).stem
+    )
+    logger.info(f"Trainer module {Path(model_script_path).name} loaded")
+    trainer_class = getattr(source, trainer.model_create)
+    predictor = trainer_class(logger, log_conform_request)
+    logger.info(f"Model {trainer.model_create} created")
+    #model_script = source.TrainerClass(ds_iter, logger, request_form)
+
+    # Set Options
+    logger.info("Setting options...")
+    if not request_form["optStr"] == "":
+        for k, v in dict(
+            option.split("=")
+            for option in request_form["optStr"].split(";")
+        ).items():
+            if v in ("True", "False"):
+                predictor.OPTIONS[k] = True if v == "True" else False
+            elif v == "None":
+                predictor.OPTIONS[k] = True if v == "True" else False
+            else:
+                predictor.OPTIONS[k] = v
+            logger.info(k + "=" + v)
+    logger.info("...done.")
+
+
+    # If the module implements the Trainer interface load weights
+    if isinstance(predictor, iTrainer):
+
+        # Load Model
+        model_weight_path = (
+                trainer_file_path.parent / trainer.model_weights_path
+        )
+        logger.info(f"Loading weights from {model_weight_path}")
+        predictor.load(model_weight_path)
+        logger.info("Model loaded.")
+
+    # Iterate over all sessions
+    ds_iter: HcaiNovaDynamicIterable
+    for ds_iter in iterators:
+
+        # TODO: Remove prior creation of separate iterators to reduce redundancy
+        ss_ds_iter = ds_iter.to_single_session_iterator()
+
+        logger.info("Predict data...")
+        data = predictor.process_data(ss_ds_iter)
+        annos = predictor.to_anno(data)
+        logger.info("...done")
+
+        logger.info("Saving predictions to database...")
+        # TODO: Refactor to not use request form in upload
+        request_form_copy = copy.copy(request_form)
+        request_form_copy['sessions'] = session
+        db_utils.write_annotation_to_db(request_form_copy, annos, logger)
+        logger.info("...done")
+
+    logger.info("Prediction completed!")
+    status_utils.update_status(key, status_utils.JobStatus.FINISHED)
+
+        # model_script.ds_iter = ds_iter
+        # model_script.request_form["sessions"] = session
+        # model_script.request_form["roles"] = role
+        #
+        # logger.info("Execute preprocessing.")
+        # model_script.preprocess()
+        # logger.info("Preprocessing done.")
+        #
+        # logger.info("Execute prediction.")
+        # model_script.predict()
+        # logger.info("Prediction done.")
+        #
+        # logger.info("Execute postprocessing.")
+        # results = model_script.postprocess()
+        # logger.info("Postprocessing done.")
+        #
+        # logger.info("Execute saving process.")
+        # db_utils.write_annotation_to_db(request_form, results, logger)
+        # logger.info("Saving process done.")
+
+        # 5. In CML case, delete temporary files..
+        # if request_form["deleteFiles"] == "True":
+        #     trainer_name = request_form["trainerName"]
+        #     logger.info("Deleting temporary CML files...")
+        #     out_dir = Path(cml_dir).joinpath(
+        #         PureWindowsPath(request_form["trainerOutputDirectory"])
+        #     )
+        #     os.remove(out_dir / trainer.model_weights_path)
+        #     os.remove(out_dir / trainer.model_script_path)
+        #     for f in model_script.DEPENDENCIES:
+        #         os.remove(trainer_file_path.parent / f)
+        #     trainer_fullname = trainer_name + ".trainer"
+        #     os.remove(out_dir / trainer_fullname)
+        #     logger.info("...done")
 
-                # Set Options
-                logger.info("Setting options...")
-                if not request_form["OptStr"] == "":
-                    for k, v in dict(
-                        option.split("=")
-                        for option in request_form["OptStr"].split(";")
-                    ).items():
-                        if v in ("True", "False"):
-                            model_script.OPTIONS[k] = True if v == "True" else False
-                        elif v == "None":
-                            model_script.OPTIONS[k] = True if v == "True" else False
-                        else:
-                            model_script.OPTIONS[k] = v
-                        logger.info(k + "=" + v)
-                logger.info("...done.")
-
-                # Load Model
-                model_weight_path = (
-                    trainer_file_path.parent / trainer.model_weights_path
-                )
-                logger.info("Loading model.")
-                model_script.load(model_weight_path)
-                logger.info("Model loaded.")
-
-            # Load the model only one time as well
-
-            model_script.ds_iter = ds_iter
-            model_script.request_form["sessions"] = session
-            model_script.request_form["roles"] = role
-
-            logger.info("Execute preprocessing.")
-            model_script.preprocess()
-            logger.info("Preprocessing done.")
-
-            logger.info("Execute prediction.")
-            model_script.predict()
-            logger.info("Prediction done.")
-
-            logger.info("Execute postprocessing.")
-            results = model_script.postprocess()
-            logger.info("Postprocessing done.")
-
-            logger.info("Execute saving process.")
-            db_utils.write_annotation_to_db(request_form, results, logger)
-            logger.info("Saving process done.")
-
-            # 5. In CML case, delete temporary files..
-        if request_form["deleteFiles"] == "True":
-            trainer_name = request_form["trainerName"]
-            logger.info("Deleting temporary CML files...")
-            out_dir = Path(cml_dir).joinpath(
-                PureWindowsPath(request_form["trainerOutputDirectory"])
-            )
-            os.remove(out_dir / trainer.model_weights_path)
-            os.remove(out_dir / trainer.model_script_path)
-            for f in model_script.DEPENDENCIES:
-                os.remove(trainer_file_path.parent / f)
-            trainer_fullname = trainer_name + ".trainer"
-            os.remove(out_dir / trainer_fullname)
-            logger.info("...done")
 
-        logger.info("Prediction completed!")
-        status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
 
 # except Exception as e:
 # logger.error('Error:' + str(e))
 #   status_utils.update_status(key, status_utils.JobStatus.ERROR)
 # finally:
 #    del results, ds_iter, ds_iter_pp, model, model_script, model_script_path, model_weight_path, spec
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/dataset_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,60 @@
-from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import HcaiNovaDynamicIterable
+from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import (
+    HcaiNovaDynamicIterable,
+)
+
 
 def dataset_from_request_form(request_form, data_dir):
     """
     Creates a tensorflow dataset from nova dynamically
     :param request_form: the requestform that specifices the parameters of the dataset
     """
     db_config_dict = {
-        'ip': request_form["server"].split(':')[0],
-        'port': int(request_form["server"].split(':')[1]),
-        'user': request_form["username"],
-        'password': request_form["password"]
+        "ip": request_form["server"].split(":")[0],
+        "port": int(request_form["server"].split(":")[1]),
+        "user": request_form["username"],
+        "password": request_form["password"],
     }
 
     flattenSamples = False
     if request_form["flattenSamples"] == "true":
         flattenSamples = True
 
     ds_iter = HcaiNovaDynamicIterable(
         # Database Config
         db_config_path=None,  # os.path.join(os.path.dirname(os.path.abspath(__file__)), 'db.cfg'),
         db_config_dict=db_config_dict,
-
         # Dataset Config
         dataset=request_form.get("database"),
         nova_data_dir=data_dir,
-        sessions=request_form.get("sessions").split(';') if request_form.get("sessions") else None,
-        roles=request_form.get("roles", '').split(';') if request_form.get("roles") else None,
-        schemes=request_form.get("scheme", '').split(';') if request_form.get("scheme") else None,
+        sessions=request_form.get("sessions").split(";")
+        if request_form.get("sessions")
+        else None,
+        roles=request_form.get("roles", "").split(";")
+        if request_form.get("roles")
+        else None,
+        schemes=request_form.get("scheme", "").split(";")
+        if request_form.get("scheme")
+        else None,
         annotator=request_form.get("annotator"),
-        data_streams=request_form.get("streamName", '').split(' ') if request_form.get("streamName") else None,
-
+        data_streams=request_form.get("streamName", "").split(" ")
+        if request_form.get("streamName")
+        else None,
         # Sample Config
         frame_size=request_form.get("frameSize"),
         stride=request_form.get("stride"),
         left_context=request_form.get("leftContext"),
         right_context=request_form.get("rightContext"),
         start=request_form.get("startTime"),
         end=request_form.get("endTime"),
-
-        #TODO: This does not work with pytorch bridge when set to true because the data field does not contain the role anymore<.
+        # TODO: This does not work with pytorch bridge when set to true because the data field does not contain the role anymore<.
         # transformation cannot be applied. fix it!
         flatten_samples=flattenSamples,
-        supervised_keys=[request_form["streamName"].split(' ')[0],
-                         request_form["scheme"].split(';')[0]],
-
+        supervised_keys=[
+            request_form.get("streamName", "").split(" ")[0],
+            request_form.get("scheme", "").split(";")[0],
+        ],
         # Additional Config
         clear_cache=True,
     )
 
     return ds_iter
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,30 @@
     elif request_form["schemeType"] == "POINT":
         pass  # todo
     elif request_form["schemeType"] == "DISCRETE_POLYGON" or request_form["schemeType"] == "POLYGON":
         write_polygons_to_db(request_form, results, db_handler, logger)
 
 
 def write_freeform_to_db(request_form, results: dict, db_handler, logger):
+    '''
+    Args:
+        request_form ():
+        results (dict): {
+            'from_to' : {
+                <role>.<stream>: {
+                    'name': <text>, 'conf': <confidence>
+                }
+            }
+        }
+        db_handler ():
+        logger ():
+
+    Returns:
+
+    '''
     annotations = {}
     """Temp fix"""
     results.pop('values', None)
     results.pop('confidences', None)
 
     for frame, results in results.items():
         frame_info = frame.split('_')
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304131554/setup.py` & `hcai-nova-server-nightly-0.1.3.dev202304142235/setup.py`

 * *Files identical despite different names*

