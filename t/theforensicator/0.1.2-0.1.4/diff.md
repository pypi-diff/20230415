# Comparing `tmp/theforensicator-0.1.2.tar.gz` & `tmp/theforensicator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theforensicator-0.1.2.tar", max compression
+gzip compressed data, was "theforensicator-0.1.4.tar", max compression
```

## Comparing `theforensicator-0.1.2.tar` & `theforensicator-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-04-14 20:25:49.052108 theforensicator-0.1.2/LICENSE
--rw-r--r--   0        0        0     1091 2023-04-14 20:25:49.052108 theforensicator-0.1.2/README.md
--rw-r--r--   0        0        0     3100 2023-04-14 20:25:49.056108 theforensicator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-14 20:25:49.056108 theforensicator-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-04-14 20:25:49.056108 theforensicator-0.1.2/tests/test_app.py
--rw-r--r--   0        0        0      145 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/__init__.py
--rw-r--r--   0        0        0     4939 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/app.py
--rw-r--r--   0        0        0      473 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_chrome.yaml
--rw-r--r--   0        0        0      116 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_edge.yaml
--rw-r--r--   0        0        0      668 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_firefox.yaml
--rw-r--r--   0        0        0      467 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_ie.yaml
--rw-r--r--   0        0        0      170 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/events_logs.yaml
--rw-r--r--   0        0        0       97 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/prefetch.yaml
--rw-r--r--   0        0        0      366 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/registry_system.yaml
--rw-r--r--   0        0        0      129 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/registry_user.yaml
--rw-r--r--   0        0        0     2156 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/cli.py
--rw-r--r--   0        0        0       30 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/ewf/__init__.py
--rw-r--r--   0        0        0    19995 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/ewf/file_parsing.py
--rw-r--r--   0        0        0       65 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/__init__.py
--rw-r--r--   0        0        0    12818 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/defs.py
--rw-r--r--   0        0        0     4929 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/gpt.py
--rw-r--r--   0        0        0     3421 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/mbr.py
--rw-r--r--   0        0        0    34074 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/ntfs.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-15 15:28:32.600435 theforensicator-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1091 2023-04-15 15:28:32.600435 theforensicator-0.1.4/README.md
+-rw-r--r--   0        0        0     3100 2023-04-15 15:28:32.600435 theforensicator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-15 15:28:32.600435 theforensicator-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-15 15:28:32.600435 theforensicator-0.1.4/tests/test_app.py
+-rw-r--r--   0        0        0      145 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/__init__.py
+-rw-r--r--   0        0        0     4939 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/app.py
+-rw-r--r--   0        0        0      473 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_chrome.yaml
+-rw-r--r--   0        0        0      116 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_edge.yaml
+-rw-r--r--   0        0        0      668 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_firefox.yaml
+-rw-r--r--   0        0        0      467 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_ie.yaml
+-rw-r--r--   0        0        0      170 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/events_logs.yaml
+-rw-r--r--   0        0        0       97 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/prefetch.yaml
+-rw-r--r--   0        0        0      366 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/registry_system.yaml
+-rw-r--r--   0        0        0      129 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/registry_user.yaml
+-rw-r--r--   0        0        0     2156 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/cli.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/ewf/__init__.py
+-rw-r--r--   0        0        0    19995 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/ewf/file_parsing.py
+-rw-r--r--   0        0        0       65 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/fs/__init__.py
+-rw-r--r--   0        0        0    12818 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/defs.py
+-rw-r--r--   0        0        0     4929 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/gpt.py
+-rw-r--r--   0        0        0     3421 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/mbr.py
+-rw-r--r--   0        0        0    34140 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/ntfs.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.4/PKG-INFO
```

### Comparing `theforensicator-0.1.2/LICENSE` & `theforensicator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/README.md` & `theforensicator-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 ## Features
 
 * [X] Read a EWF file
 * [X] Extract MBR from NTFS partitions
 * [X] Resolve paths of files from NTFS partitions
 * [X] Extract files from NTFS partitions
-* [ ] Extract list of files from NFTS partitons using yaml file as a list
+* [X] Extract list of files from NFTS partitons using yaml file as a list
 
 ## Credits
 
 This package was created with the [ppw](https://zillionare.github.io/python-project-wizard) tool. For more information, please visit the [project page](https://zillionare.github.io/python-project-wizard/).
```

### Comparing `theforensicator-0.1.2/pyproject.toml` & `theforensicator-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "theforensicator"
-version = "0.1.2"
+version = "0.1.4"
 homepage = "https://github.com/ValekoZ/theforensicator"
 description = "School project for forensic investigations."
 authors = [
     "Joël RABAH <joel.rabah@ecole2600.com>",
     "Edouard GOUT <edouard.gout@ecole2600.com>",
     "Yann MAJEROWICZ <yann.majerowicz@ecole2600.com>",
     "Bastien WINTER DURENNEL <bastien.winter-durennel@ecole2600.com>",
```

### Comparing `theforensicator-0.1.2/tests/test_app.py` & `theforensicator-0.1.4/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/app.py` & `theforensicator-0.1.4/theforensicator/app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/artefacts/browser_firefox.yaml` & `theforensicator-0.1.4/theforensicator/artefacts/browser_firefox.yaml`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/cli.py` & `theforensicator-0.1.4/theforensicator/cli.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/ewf/file_parsing.py` & `theforensicator-0.1.4/theforensicator/ewf/file_parsing.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/fs/defs.py` & `theforensicator-0.1.4/theforensicator/fs/defs.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/fs/gpt.py` & `theforensicator-0.1.4/theforensicator/fs/gpt.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/fs/mbr.py` & `theforensicator-0.1.4/theforensicator/fs/mbr.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.2/theforensicator/fs/ntfs.py` & `theforensicator-0.1.4/theforensicator/fs/ntfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,14 +574,18 @@
     def _get_datetime(self, windows_time: int):
         """Convert windows time to datetime
 
         Args:
             windows_time: Time to convert
         """
         seconds = windows_time / 10000000
+        
+        if seconds < 0:
+            seconds = 0
+        
         epoch = seconds - 11644473600
         dt = datetime.datetime(2000, 1, 1, 0, 0, 0).fromtimestamp(epoch)
         return {"timestamp": epoch, "date": f"{dt.ctime()}"}
 
     """Attribute type : (0x10) STANDARD_INFORMATION.
     """
```

### Comparing `theforensicator-0.1.2/PKG-INFO` & `theforensicator-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theforensicator
-Version: 0.1.2
+Version: 0.1.4
 Summary: School project for forensic investigations.
 Home-page: https://github.com/ValekoZ/theforensicator
 License: MIT
 Author: Joël RABAH
 Author-email: joel.rabah@ecole2600.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -67,13 +67,13 @@
 
 ## Features
 
 * [X] Read a EWF file
 * [X] Extract MBR from NTFS partitions
 * [X] Resolve paths of files from NTFS partitions
 * [X] Extract files from NTFS partitions
-* [ ] Extract list of files from NFTS partitons using yaml file as a list
+* [X] Extract list of files from NFTS partitons using yaml file as a list
 
 ## Credits
 
 This package was created with the [ppw](https://zillionare.github.io/python-project-wizard) tool. For more information, please visit the [project page](https://zillionare.github.io/python-project-wizard/).
```

