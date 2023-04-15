# Comparing `tmp/searchlix-1.0.4.tar.gz` & `tmp/searchlix-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\searchlix-1.0.4.tar", last modified: Fri Apr 14 20:50:57 2023, max compression
+gzip compressed data, was "dist\searchlix-1.0.5.tar", last modified: Sat Apr 15 19:50:02 2023, max compression
```

## Comparing `searchlix-1.0.4.tar` & `searchlix-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:50:57.000000 searchlix-1.0.4/
--rw-rw-rw-   0        0        0     2162 2023-04-14 20:50:57.000000 searchlix-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1298 2023-04-14 20:50:21.000000 searchlix-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix/
--rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.4/searchlix/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-04-14 19:50:21.000000 searchlix-1.0.4/searchlix/searchlix.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/
--rw-rw-rw-   0        0        0     2162 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 20:50:57.000000 searchlix-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-14 20:50:48.000000 searchlix-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:50:02.000000 searchlix-1.0.5/
+-rw-rw-rw-   0        0        0     2465 2023-04-15 19:50:02.000000 searchlix-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1545 2023-04-15 19:49:33.000000 searchlix-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix/
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.5/searchlix/__init__.py
+-rw-rw-rw-   0        0        0     3559 2023-04-15 19:48:19.000000 searchlix-1.0.5/searchlix/searchlix.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/
+-rw-rw-rw-   0        0        0     2465 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:50:02.000000 searchlix-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-15 19:49:39.000000 searchlix-1.0.5/setup.py
```

### Comparing `searchlix-1.0.4/PKG-INFO` & `searchlix-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: searchlix
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for extract data from websites and text
 Home-page: UNKNOWN
 Author: Hashem
 Author-email: hashem.a.muhammad@gmail.com
 License: UNKNOWN
 Description: # Searchlix
         ## _powerful python pakage to search in text and websites_
         
         
         
         ## Features
         
-        - Find emails in text / Email validation
-        - Find emails in website page
-        - Find phone number in text / Phone number validation
-        - Find phone number in website page
-        - Pattern search in text
         - Search for page name in website
+        - Extract emails from website page
+        - Extract phone number from website page
+        - check if domain has a valid mail server
+        - check if domain is valid
+        - Pattern search in text
+        - Search for word in text
+        - Extract phone number in text / Phone number validation
+        - Extract emails in text / Email validation
+        
+        
         
         
         
         
         ## Installation
         
         python 3.6+
@@ -39,14 +44,16 @@
         | ------ | ------ |
         | Find emails in text / Email validation | find_email(text) |
         | Find emails in website page | extract_email_from_link(url) |
         | Find phone number in text / Phone number validation | find_phone_number(text) |
         | Find phone number in website page | extract_phone_from_link(url) |
         | Pattern search in text | pattern_search(text, pattern) |
         | Search for page name in website | extract_page_url(url, page_name) |
+        | check if domain has a valid mail server | check_mail_server(domain) |
+        | check if domain is valid | is_valid_domian(domain) |
         
         ## Import
         
         
         
         
         ```sh
```

### Comparing `searchlix-1.0.4/searchlix/searchlix.py` & `searchlix-1.0.5/searchlix/searchlix.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import re
 from bs4 import BeautifulSoup
-
+import dns.resolver
 
 requests.packages.urllib3.disable_warnings(
     requests.packages.urllib3.exceptions.InsecureRequestWarning)
 
 
 def find_phone_number(text):
     phone_pattern = r'\(?\d{3}\)?[-.\s]?\d{3}[-.\s]?\d{4}'
@@ -90,8 +90,40 @@
     for link in links:
         result = pattern_search(link, page_name)
         if result:
             if link in url_found:
                 url_found[link] += 1
             else:
                 url_found[link] = 1
-    return url_found
+    return url_found
+
+
+def check_mail_server(domain):
+    domain = re.sub(r'(www\.|http(s)*://)', '', domain)
+    try:
+        result = dns.resolver.resolve(domain, 'MX')
+        for exdata in result:
+            if exdata:
+                return True
+            return False
+    except dns.resolver.NXDOMAIN:
+        return False
+    except dns.resolver.Timeout:
+        return "Timed out while resolving"
+
+
+def is_valid_domian(domain):
+    domain = re.sub(r'(www\.|http(s)*://)', '', domain)
+    try:
+        result = dns.resolver.resolve(domain, 'A')
+        for ip in result:
+            if ip:
+                return True
+            return False
+    except dns.resolver.NXDOMAIN:
+        return False
+    except dns.resolver.Timeout:
+        return "Timed out while resolving"
+    
+
+t = check_mail_server('https://www.domains.tm')
+print(t)
```

### Comparing `searchlix-1.0.4/searchlix.egg-info/PKG-INFO` & `searchlix-1.0.5/searchlix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: searchlix
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for extract data from websites and text
 Home-page: UNKNOWN
 Author: Hashem
 Author-email: hashem.a.muhammad@gmail.com
 License: UNKNOWN
 Description: # Searchlix
         ## _powerful python pakage to search in text and websites_
         
         
         
         ## Features
         
-        - Find emails in text / Email validation
-        - Find emails in website page
-        - Find phone number in text / Phone number validation
-        - Find phone number in website page
-        - Pattern search in text
         - Search for page name in website
+        - Extract emails from website page
+        - Extract phone number from website page
+        - check if domain has a valid mail server
+        - check if domain is valid
+        - Pattern search in text
+        - Search for word in text
+        - Extract phone number in text / Phone number validation
+        - Extract emails in text / Email validation
+        
+        
         
         
         
         
         ## Installation
         
         python 3.6+
@@ -39,14 +44,16 @@
         | ------ | ------ |
         | Find emails in text / Email validation | find_email(text) |
         | Find emails in website page | extract_email_from_link(url) |
         | Find phone number in text / Phone number validation | find_phone_number(text) |
         | Find phone number in website page | extract_phone_from_link(url) |
         | Pattern search in text | pattern_search(text, pattern) |
         | Search for page name in website | extract_page_url(url, page_name) |
+        | check if domain has a valid mail server | check_mail_server(domain) |
+        | check if domain is valid | is_valid_domian(domain) |
         
         ## Import
         
         
         
         
         ```sh
```

### Comparing `searchlix-1.0.4/setup.py` & `searchlix-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='searchlix',
-    version='1.0.4',
+    version='1.0.5',
     description='A package for extract data from websites and text',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hashem',
     author_email='hashem.a.muhammad@gmail.com',
     packages=find_packages(),
     install_requires=[
```

