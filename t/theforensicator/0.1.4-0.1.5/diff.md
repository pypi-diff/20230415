# Comparing `tmp/theforensicator-0.1.4.tar.gz` & `tmp/theforensicator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theforensicator-0.1.4.tar", max compression
+gzip compressed data, was "theforensicator-0.1.5.tar", max compression
```

## Comparing `theforensicator-0.1.4.tar` & `theforensicator-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-04-15 15:28:32.600435 theforensicator-0.1.4/LICENSE
--rw-r--r--   0        0        0     1091 2023-04-15 15:28:32.600435 theforensicator-0.1.4/README.md
--rw-r--r--   0        0        0     3100 2023-04-15 15:28:32.600435 theforensicator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-15 15:28:32.600435 theforensicator-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-04-15 15:28:32.600435 theforensicator-0.1.4/tests/test_app.py
--rw-r--r--   0        0        0      145 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/__init__.py
--rw-r--r--   0        0        0     4939 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/app.py
--rw-r--r--   0        0        0      473 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_chrome.yaml
--rw-r--r--   0        0        0      116 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_edge.yaml
--rw-r--r--   0        0        0      668 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_firefox.yaml
--rw-r--r--   0        0        0      467 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/browser_ie.yaml
--rw-r--r--   0        0        0      170 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/events_logs.yaml
--rw-r--r--   0        0        0       97 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/prefetch.yaml
--rw-r--r--   0        0        0      366 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/registry_system.yaml
--rw-r--r--   0        0        0      129 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/artefacts/registry_user.yaml
--rw-r--r--   0        0        0     2156 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/cli.py
--rw-r--r--   0        0        0       30 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/ewf/__init__.py
--rw-r--r--   0        0        0    19995 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/ewf/file_parsing.py
--rw-r--r--   0        0        0       65 2023-04-15 15:28:32.600435 theforensicator-0.1.4/theforensicator/fs/__init__.py
--rw-r--r--   0        0        0    12818 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/defs.py
--rw-r--r--   0        0        0     4929 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/gpt.py
--rw-r--r--   0        0        0     3421 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/mbr.py
--rw-r--r--   0        0        0    34140 2023-04-15 15:28:32.604435 theforensicator-0.1.4/theforensicator/fs/ntfs.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-15 16:44:34.747566 theforensicator-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1091 2023-04-15 16:44:34.747566 theforensicator-0.1.5/README.md
+-rw-r--r--   0        0        0     3100 2023-04-15 16:44:34.747566 theforensicator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-15 16:44:34.747566 theforensicator-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-15 16:44:34.747566 theforensicator-0.1.5/tests/test_app.py
+-rw-r--r--   0        0        0      145 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/__init__.py
+-rw-r--r--   0        0        0     4939 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/app.py
+-rw-r--r--   0        0        0      473 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_chrome.yaml
+-rw-r--r--   0        0        0      116 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_edge.yaml
+-rw-r--r--   0        0        0      668 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_firefox.yaml
+-rw-r--r--   0        0        0      467 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_ie.yaml
+-rw-r--r--   0        0        0      170 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/events_logs.yaml
+-rw-r--r--   0        0        0       97 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/prefetch.yaml
+-rw-r--r--   0        0        0      366 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/registry_system.yaml
+-rw-r--r--   0        0        0      129 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/registry_user.yaml
+-rw-r--r--   0        0        0     2156 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/cli.py
+-rw-r--r--   0        0        0       30 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/ewf/__init__.py
+-rw-r--r--   0        0        0    19995 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/ewf/file_parsing.py
+-rw-r--r--   0        0        0       65 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/__init__.py
+-rw-r--r--   0        0        0    12818 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/defs.py
+-rw-r--r--   0        0        0     4929 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/gpt.py
+-rw-r--r--   0        0        0     3421 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/mbr.py
+-rw-r--r--   0        0        0    35265 2023-04-15 16:44:34.751566 theforensicator-0.1.5/theforensicator/fs/ntfs.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.5/PKG-INFO
```

### Comparing `theforensicator-0.1.4/LICENSE` & `theforensicator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/README.md` & `theforensicator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/pyproject.toml` & `theforensicator-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "theforensicator"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/ValekoZ/theforensicator"
 description = "School project for forensic investigations."
 authors = [
     "Joël RABAH <joel.rabah@ecole2600.com>",
     "Edouard GOUT <edouard.gout@ecole2600.com>",
     "Yann MAJEROWICZ <yann.majerowicz@ecole2600.com>",
     "Bastien WINTER DURENNEL <bastien.winter-durennel@ecole2600.com>",
```

### Comparing `theforensicator-0.1.4/tests/test_app.py` & `theforensicator-0.1.5/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/app.py` & `theforensicator-0.1.5/theforensicator/app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/artefacts/browser_firefox.yaml` & `theforensicator-0.1.5/theforensicator/artefacts/browser_firefox.yaml`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/cli.py` & `theforensicator-0.1.5/theforensicator/cli.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/ewf/file_parsing.py` & `theforensicator-0.1.5/theforensicator/ewf/file_parsing.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/fs/defs.py` & `theforensicator-0.1.5/theforensicator/fs/defs.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/fs/gpt.py` & `theforensicator-0.1.5/theforensicator/fs/gpt.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/fs/mbr.py` & `theforensicator-0.1.5/theforensicator/fs/mbr.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.4/theforensicator/fs/ntfs.py` & `theforensicator-0.1.5/theforensicator/fs/ntfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -567,33 +567,44 @@
         self.verbose = verbose
 
         # mft header fields with their values
         self.mft_parsed = {}
         self.is_valid_entry = True
         self.record = {"is_directory": False, "files": []}
 
-    def _get_datetime(self, windows_time: int):
+    def _get_datetime(self, windows_time: int) -> dict:
         """Convert windows time to datetime
 
         Args:
             windows_time: Time to convert
+
+        Returns:
+            Time in a dict
         """
         seconds = windows_time / 10000000
+        epoch = seconds - 11644473600
         
-        if seconds < 0:
-            seconds = 0
+        if epoch < 0:
+            epoch = 0
         
-        epoch = seconds - 11644473600
         dt = datetime.datetime(2000, 1, 1, 0, 0, 0).fromtimestamp(epoch)
         return {"timestamp": epoch, "date": f"{dt.ctime()}"}
 
     """Attribute type : (0x10) STANDARD_INFORMATION.
     """
 
     def _standard_info_decode(self, attribute: bytes):
+        """Decode STANDARD_INFORMATION attribute
+
+        Args:
+            attribute: Raw attribute to decode
+        
+        Returns:
+            The parsed attribute
+        """
         # not complete but at this time we don't need more
         si_info = {}
 
         si_info["creation_time"] = self._get_datetime(
             unpack_from("<Q", attribute, offset=0x0)[0]
         )
         si_info["last_data_change_time"] = self._get_datetime(
@@ -621,14 +632,22 @@
 
         return si_info
 
     """Attribute type : (0x20) ATTR_LIST_ENTRY.
     """
 
     def _attribute_list_decode(self, attribute: bytes) -> dict:
+        """Decode ATTR_LIST_ENTRY attribute
+
+        Args:
+            attribute: Raw attribute to decode
+        
+        Returns:
+            The parsed attribute
+        """
         attr_list = {}
 
         attr_list["type"] = unpack_from("<I", attribute, offset=0)[0]
         attr_list["length"] = unpack_from("<H", attribute, offset=4)[0]
         attr_list["name_length"] = unpack_from("<B", attribute, offset=6)[0]
         attr_list["name_offset"] = unpack_from("<B", attribute, offset=7)[0]
         attr_list["lowest_vcn"] = unpack_from("<Q", attribute, offset=8)[0]
@@ -641,14 +660,22 @@
         return attr_list
 
     """Attribute type : (0x30) FILE_NAME_ATTR
     A file can be an archive, the flags field tells us if it's the case.
     """
 
     def _file_name_decode(self, attribute: bytes) -> dict:
+        """Decode FILE_NAME_ATTR attribute
+
+        Args:
+            attribute: Raw attribute to decode
+        
+        Returns:
+            The parsed attribute
+        """
         _file_name = {}
 
         # for now there's no check on sequence number, maybe after
         # it's used to know either the file is allocated, deleted or orphan
         # https://usermanual.wiki/Pdf/WpNtOrphanFilesEnUs.1012197800.pdf
         parent_dir = unpack_from("<Q", attribute, offset=0x0)[0]
         _file_name["parent_directory"] = parent_dir & 0xFFFFFFFFFFFF
@@ -720,14 +747,22 @@
 
         return _file_name
 
     """Attribute type : (0x40) OBJECT_ID_ATTR
     """
 
     def _object_id_decode(self, attribute: bytes) -> dict:
+        """Decode OBJECT_ID_ATTR attribute
+
+        Args:
+            attribute: Raw attribute to decode
+        
+        Returns:
+            The parsed attribute
+        """
         _object_id = {}
 
         _object_id["data1"] = unpack_from("<I", attribute, offset=0x0)[0]
         _object_id["data2"] = unpack_from("<H", attribute, offset=0x4)[0]
         _object_id["data3"] = unpack_from("<H", attribute, offset=0x6)[0]
         _object_id["data4"] = unpack_from("<8s", attribute, offset=0x8)[0]
 
@@ -748,15 +783,23 @@
     def _volume_name_decode(self, attribute: bytes):
         # _volume_name = {}
         pass
 
     """Attribute type : (0x80) DATA
     """
 
-    def _data_runs_decode(self, dataruns: bytes):
+    def _data_runs_decode(self, dataruns: bytes) -> list:
+        """Decode DATA attribute
+
+        Args:
+            dataruns: dataruns list
+        
+        Returns:
+            Data of the MFT entry
+        """
         current_datarun = dataruns
         run_header = unpack_from("<B", current_datarun, offset=0)[0]
 
         data = []
 
         size_lcn_nb = run_header & 0xF
         size_lcn_offset = run_header >> 4
@@ -824,14 +867,20 @@
             prev_offset = prev_offset + lcn_offset
             current_datarun = current_datarun[1 + size_lcn_nb + size_lcn_offset :]
             run_header = unpack_from("<B", current_datarun, offset=0)[0]
 
         return data
 
     def _analyze_attribute(self, attr_parsed: dict, raw_attr: bytes):
+        """Analyze and decode an attribute
+
+        Args:
+            attr_parsed: parsed attribute dict
+            raw_attr: raw bytes attribute
+        """
         if attr_parsed["non_resident"]:
             attribute = b""
         else:
             attribute = raw_attr[attr_parsed["value_offset"] :]
 
         if attr_parsed["type"] == AT_STANDARD_INFORMATION:
             si_info = self._standard_info_decode(
@@ -906,14 +955,16 @@
                         "raw_data": data,
                     }
 
     """This function will parse attribute header of an MFT entry.
     """
 
     def parse_attr_header(self):
+        """Parse an attribute
+        """
         attrs_offset = self.mft_parsed["attrs_offset"]
 
         # offset must be aligned on 8 bytes
         if attrs_offset % 8:
             print("Attribute misalignment")
 
         self.attributes = []
```

### Comparing `theforensicator-0.1.4/PKG-INFO` & `theforensicator-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theforensicator
-Version: 0.1.4
+Version: 0.1.5
 Summary: School project for forensic investigations.
 Home-page: https://github.com/ValekoZ/theforensicator
 License: MIT
 Author: Joël RABAH
 Author-email: joel.rabah@ecole2600.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

