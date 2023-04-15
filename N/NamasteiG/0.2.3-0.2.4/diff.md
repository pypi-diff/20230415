# Comparing `tmp/NamasteiG-0.2.3.tar.gz` & `tmp/NamasteiG-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.2.3.tar", last modified: Tue Apr  4 14:41:57 2023, max compression
+gzip compressed data, was "NamasteiG-0.2.4.tar", last modified: Sat Apr 15 13:30:36 2023, max compression
```

## Comparing `NamasteiG-0.2.3.tar` & `NamasteiG-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 14:41:57.247667 NamasteiG-0.2.3/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      838 2023-04-04 14:41:57.246401 NamasteiG-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.3/README.md
--rw-rw-rw-   0        0        0      593 2023-04-04 14:38:50.000000 NamasteiG-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 14:41:57.247667 NamasteiG-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-04 14:41:57.223554 NamasteiG-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 14:41:57.236373 NamasteiG-0.2.3/src/NamasteiG/
--rw-rw-rw-   0        0        0    19996 2023-04-04 14:37:51.000000 NamasteiG-0.2.3/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      499 2022-12-14 18:59:48.000000 NamasteiG-0.2.3/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-04-04 14:41:57.243255 NamasteiG-0.2.3/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-04-04 14:41:57.000000 NamasteiG-0.2.3/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-04 14:41:57.000000 NamasteiG-0.2.3/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 14:41:57.000000 NamasteiG-0.2.3/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-04 14:41:57.000000 NamasteiG-0.2.3/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.050384 NamasteiG-0.2.4/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-04-15 13:30:36.050384 NamasteiG-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.4/README.md
+-rw-rw-rw-   0        0        0      593 2023-04-15 13:26:28.000000 NamasteiG-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 13:30:36.050384 NamasteiG-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.034396 NamasteiG-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.041264 NamasteiG-0.2.4/src/NamasteiG/
+-rw-rw-rw-   0        0        0    19992 2023-04-15 13:26:10.000000 NamasteiG-0.2.4/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      499 2022-12-14 18:59:48.000000 NamasteiG-0.2.4/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:30:36.041264 NamasteiG-0.2.4/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 13:30:36.000000 NamasteiG-0.2.4/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.2.3/LICENSE` & `NamasteiG-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.3/PKG-INFO` & `NamasteiG-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.3
+Version: 0.2.4
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.2.3/pyproject.toml` & `NamasteiG-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.2.3/src/NamasteiG/__init__.py` & `NamasteiG-0.2.4/src/NamasteiG/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         publickeyid.to_bytes(1, byteorder='big'),
         iv,
         size_buffer,
         rsa_encrypted,
         tag,
         aes_encrypted
     ]))
-    return payload.decode()
+    return f'#PWD_INSTAGRAM:4:{timestamp}:{payload.decode()}'
 
 
 
 class Instagram:
 
     def __init__(self,User,Password):
         self.user = User
@@ -116,15 +116,15 @@
         return requests.post('https://b.i.instagram.com/api/v1/launcher/mobileconfig/', headers=headers, data=data).headers['ig-set-x-mid']
 
     def Login(self,PassWordEnc=None):
         mid=self.GetMid()
         if PassWordEnc==None:
             self.datapassword=f'#PWD_INSTAGRAM:0:{round(time.time())}:{self.passw}'
         else:
-            self.datapassword = f'#PWD_INSTAGRAM:4:{round(time.time())}:{password_encrypt(self.passw)}'
+            self.datapassword = f'{password_encrypt(self.passw)}'
         data = urlencode({
             'signed_body': 'SIGNATURE.{"jazoest":"' + str(self.generate_jazoest(
                 str(self.IgFamilyDeviceId))) + '","country_codes":"[{\\"country_code\\":\\"91\\",\\"source\\":[\\"sim\\"]},{\\"country_code\\":\\"1\\",\\"source\\":[\\"default\\"]}]","phone_id":"' + str(
                 self.IgFamilyDeviceId) + '","enc_password":"'+str(self.datapassword) + '","username":"' + str(self.user) + '","adid":"' + str(uuid.uuid4()) + '","guid":"' + str(
                 self.IgDeviceId) + '","device_id":"' + str(
                 self.AndroidID) + '","google_tokens":"[]","login_attempt_count":"0"}',
         })
```

### Comparing `NamasteiG-0.2.3/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.2.4/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.3
+Version: 0.2.4
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

