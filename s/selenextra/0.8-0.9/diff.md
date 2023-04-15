# Comparing `tmp/selenextra-0.8.tar.gz` & `tmp/selenextra-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.8.tar", last modified: Sat Apr 15 06:01:36 2023, max compression
+gzip compressed data, was "selenextra-0.9.tar", last modified: Sat Apr 15 06:18:46 2023, max compression
```

## Comparing `selenextra-0.8.tar` & `selenextra-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 06:01:36.560641 selenextra-0.8/
--rw-rw-rw-   0        0        0    35823 2023-04-15 04:40:09.000000 selenextra-0.8/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-15 06:01:36.560641 selenextra-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-15 04:40:09.000000 selenextra-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 06:01:36.553660 selenextra-0.8/selenextra/
--rw-rw-rw-   0        0        0     4609 2023-04-15 06:00:14.000000 selenextra-0.8/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-15 04:40:09.000000 selenextra-0.8/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-15 04:40:09.000000 selenextra-0.8/selenextra/patcher.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:01:36.559644 selenextra-0.8/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 06:01:36.561638 selenextra-0.8/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-15 04:48:37.000000 selenextra-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:18:46.686995 selenextra-0.9/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 04:40:09.000000 selenextra-0.9/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-15 06:18:46.686995 selenextra-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-15 04:40:09.000000 selenextra-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 06:18:46.679014 selenextra-0.9/selenextra/
+-rw-rw-rw-   0        0        0     4629 2023-04-15 06:18:24.000000 selenextra-0.9/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-15 04:40:09.000000 selenextra-0.9/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-15 04:40:09.000000 selenextra-0.9/selenextra/patcher.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:18:46.684998 selenextra-0.9/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 06:18:46.686995 selenextra-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-15 06:18:13.000000 selenextra-0.9/setup.py
```

### Comparing `selenextra-0.8/LICENSE` & `selenextra-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.8/PKG-INFO` & `selenextra-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.8
+Version: 0.9
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.8/selenextra/__init__.py` & `selenextra-0.9/selenextra/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,16 @@
 
         self.custom_patcher.auto()
 
         release = self.custom_patcher.fetch_release_number()
         version = release.version[0]
 
         kwargs['driver_executable_path'] = self.custom_patcher.executable_path
-        kwargs['seleniumwire_options'] = {
-            'mitm_http2': False,
-            'proxy': {
-                'no_proxy': 'localhost,127.0.0.1'
-            }
-
-        }
+        kwargs['seleniumwire_options'] = kwargs.get('seleniumwire_options', {})
+        kwargs['seleniumwire_options']['mitm_http2'] = False
 
         super().__init__(
             version_main=version,
             **kwargs
         )
 
     def get_user_agent(self) -> str:
@@ -118,14 +113,16 @@
         if proxy_type == 'http':
             proxy_dict['http'] = proxy
             proxy_dict['https'] = proxy
         elif proxy_type == 'https':
             proxy_dict['http'] = f'{proxy.replace("https", "http")}'
             proxy_dict['https'] = proxy
 
+        proxy_dict['no_proxy'] = 'localhost,127.0.0.1'
+
         result = (False, None)
 
         try:
             resp = requests.get('https://httpbin.org/ip', proxies=proxy_dict)
             if not resp.status_code == 200:
                 return result
         except:
```

### Comparing `selenextra-0.8/selenextra/patcher.py` & `selenextra-0.9/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.8/selenextra.egg-info/PKG-INFO` & `selenextra-0.9/selenextra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.8
+Version: 0.9
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.8/setup.py` & `selenextra-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.8',
+    version='0.9',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'scipy',
```

