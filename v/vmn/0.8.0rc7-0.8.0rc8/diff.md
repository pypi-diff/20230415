# Comparing `tmp/vmn-0.8.0rc7-py3-none-any.whl.zip` & `tmp/vmn-0.8.0rc8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 42216 bytes, number of entries: 10
+Zip file size: 42228 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      152 b- defN 21-Jul-06 16:25 version_stamp/__init__.py
 -rw-r--r--  2.0 unx    45924 b- defN 23-Feb-25 23:00 version_stamp/stamp_utils.py
--rw-r--r--  2.0 unx       58 b- defN 23-Feb-25 23:03 version_stamp/version.py
--rw-r--r--  2.0 unx    97591 b- defN 23-Feb-25 22:40 version_stamp/vmn.py
--rw-r--r--  2.0 unx    35127 b- defN 23-Feb-25 23:03 vmn-0.8.0rc7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      460 b- defN 23-Feb-25 23:03 vmn-0.8.0rc7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-25 23:03 vmn-0.8.0rc7.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Feb-25 23:03 vmn-0.8.0rc7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Feb-25 23:03 vmn-0.8.0rc7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      803 b- defN 23-Feb-25 23:03 vmn-0.8.0rc7.dist-info/RECORD
-10 files, 180269 bytes uncompressed, 40846 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx       58 b- defN 23-Feb-26 14:20 version_stamp/version.py
+-rw-r--r--  2.0 unx    97730 b- defN 23-Feb-26 08:26 version_stamp/vmn.py
+-rw-r--r--  2.0 unx    35127 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      460 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      803 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/RECORD
+10 files, 180408 bytes uncompressed, 40858 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: version_stamp/version.py
 Comment: 
 
 Filename: version_stamp/vmn.py
 Comment: 
 
-Filename: vmn-0.8.0rc7.dist-info/LICENSE.txt
+Filename: vmn-0.8.0rc8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmn-0.8.0rc7.dist-info/METADATA
+Filename: vmn-0.8.0rc8.dist-info/METADATA
 Comment: 
 
-Filename: vmn-0.8.0rc7.dist-info/WHEEL
+Filename: vmn-0.8.0rc8.dist-info/WHEEL
 Comment: 
 
-Filename: vmn-0.8.0rc7.dist-info/entry_points.txt
+Filename: vmn-0.8.0rc8.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmn-0.8.0rc7.dist-info/top_level.txt
+Filename: vmn-0.8.0rc8.dist-info/top_level.txt
 Comment: 
 
-Filename: vmn-0.8.0rc7.dist-info/RECORD
+Filename: vmn-0.8.0rc8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## version_stamp/version.py

```diff
@@ -1,3 +1,3 @@
 name = "vmn"
-version = "0.8.0-rc7"
-_version = "0.8.0-rc7"
+version = "0.8.0-rc8"
+_version = "0.8.0-rc8"
```

## version_stamp/vmn.py

```diff
@@ -973,14 +973,17 @@
         ] = initial_verstr
         self.current_version_info["stamping"]["app"]["release_mode"] = release_mode
         self.current_version_info["stamping"]["app"]["info"] = copy.deepcopy(info)
         self.current_version_info["stamping"]["app"][
             "stamped_on_branch"
         ] = self.backend.active_branch
         self.current_version_info["stamping"]["app"][
+            "stamped_on_remote_branch"
+        ] = self.backend.remote_active_branch
+        self.current_version_info["stamping"]["app"][
             "prerelease_count"
         ] = copy.deepcopy(prerelease_count)
 
     def stamp_root_app_version(self, override_version=None):
         if self.root_app_name is None:
             return None
```

## Comparing `vmn-0.8.0rc7.dist-info/LICENSE.txt` & `vmn-0.8.0rc8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vmn-0.8.0rc7.dist-info/RECORD` & `vmn-0.8.0rc8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 version_stamp/__init__.py,sha256=p_9bnBNpi1jHdKDsmBM7tN2Da3N-QOYEe8s09k9NIrk,152
 version_stamp/stamp_utils.py,sha256=-yqOtzbUBmZRFrGxkonns4thfDrBPTHxdV0PY69gVa0,45924
-version_stamp/version.py,sha256=HSNA4SRtHIJuCvT8zDpgaMW9fHKuH4nxO6h-MKEU-1M,58
-version_stamp/vmn.py,sha256=SRtVJhlphzhxU4bJgA1KC5eX7NPL11cmFhqrEHNTEwk,97591
-vmn-0.8.0rc7.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
-vmn-0.8.0rc7.dist-info/METADATA,sha256=O6JeKBKa21wbDB4z7keoS8D8e4GWteIHxBNBdSjhJo4,460
-vmn-0.8.0rc7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-vmn-0.8.0rc7.dist-info/entry_points.txt,sha256=1v5GbQiSC3z8ZF_dwxte6MeXbHSvUkBqiSVvXsjfzk0,48
-vmn-0.8.0rc7.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
-vmn-0.8.0rc7.dist-info/RECORD,,
+version_stamp/version.py,sha256=llHIQwq3WAf66Id6B-jEMjkQ091GHyVRvkPvZILhtqY,58
+version_stamp/vmn.py,sha256=wI4D_Om9gw_irb1yChcFJlq62_qM_z4E55j1dHwBqGI,97730
+vmn-0.8.0rc8.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
+vmn-0.8.0rc8.dist-info/METADATA,sha256=Cd8WD1hKl_k0_Yqv8RWEmwGBF5rNm3yis-1oanQ995Y,460
+vmn-0.8.0rc8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+vmn-0.8.0rc8.dist-info/entry_points.txt,sha256=1v5GbQiSC3z8ZF_dwxte6MeXbHSvUkBqiSVvXsjfzk0,48
+vmn-0.8.0rc8.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
+vmn-0.8.0rc8.dist-info/RECORD,,
```

