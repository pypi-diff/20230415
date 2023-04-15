# Comparing `tmp/wtfutil-1.0.8.tar.gz` & `tmp/wtfutil-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtfutil-1.0.8.tar", last modified: Fri Feb 24 17:14:11 2023, max compression
+gzip compressed data, was "wtfutil-1.0.9.tar", last modified: Sat Mar 11 15:09:38 2023, max compression
```

## Comparing `wtfutil-1.0.8.tar` & `wtfutil-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 17:14:11.355732 wtfutil-1.0.8/
--rw-rw-rw-   0        0        0       55 2023-02-24 15:22:26.000000 wtfutil-1.0.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1489 2023-02-24 15:22:26.000000 wtfutil-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      126 2023-02-24 15:22:26.000000 wtfutil-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2118 2023-02-24 17:14:11.355732 wtfutil-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-02-24 15:22:26.000000 wtfutil-1.0.8/README.md
--rw-rw-rw-   0        0        0       14 2023-02-24 15:22:26.000000 wtfutil-1.0.8/TODO.rst
--rw-rw-rw-   0        0        0      107 2023-02-24 17:14:11.357724 wtfutil-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3575 2023-02-24 17:13:55.000000 wtfutil-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 17:14:11.346754 wtfutil-1.0.8/wtfutil/
--rw-rw-rw-   0        0        0        0 2023-02-24 15:22:26.000000 wtfutil-1.0.8/wtfutil/__init__.py
--rw-rw-rw-   0        0        0     2851 2023-02-24 15:22:26.000000 wtfutil-1.0.8/wtfutil/notifyutil.py
--rw-rw-rw-   0        0        0    21949 2023-02-24 15:22:26.000000 wtfutil-1.0.8/wtfutil/sqlutil.py
--rw-rw-rw-   0        0        0    17254 2023-02-24 15:23:52.000000 wtfutil-1.0.8/wtfutil/util.py
-drwxrwxrwx   0        0        0        0 2023-02-24 17:14:11.354733 wtfutil-1.0.8/wtfutil.egg-info/
--rw-rw-rw-   0        0        0     2118 2023-02-24 17:14:10.000000 wtfutil-1.0.8/wtfutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-02-24 17:14:10.000000 wtfutil-1.0.8/wtfutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 17:14:10.000000 wtfutil-1.0.8/wtfutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-24 17:14:10.000000 wtfutil-1.0.8/wtfutil.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-02-24 17:14:10.000000 wtfutil-1.0.8/wtfutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-24 17:14:10.000000 wtfutil-1.0.8/wtfutil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-11 15:09:38.042157 wtfutil-1.0.9/
+-rw-rw-rw-   0        0        0       55 2023-02-24 15:22:26.000000 wtfutil-1.0.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1489 2023-02-24 15:22:26.000000 wtfutil-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-02-24 15:22:26.000000 wtfutil-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2118 2023-03-11 15:09:38.042157 wtfutil-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-02-24 15:22:26.000000 wtfutil-1.0.9/README.md
+-rw-rw-rw-   0        0        0       14 2023-02-24 15:22:26.000000 wtfutil-1.0.9/TODO.rst
+-rw-rw-rw-   0        0        0      107 2023-03-11 15:09:38.042157 wtfutil-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2023-03-11 15:08:33.000000 wtfutil-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-11 15:09:37.995282 wtfutil-1.0.9/wtfutil/
+-rw-rw-rw-   0        0        0        0 2023-02-24 15:22:26.000000 wtfutil-1.0.9/wtfutil/__init__.py
+-rw-rw-rw-   0        0        0     2851 2023-02-24 15:22:26.000000 wtfutil-1.0.9/wtfutil/notifyutil.py
+-rw-rw-rw-   0        0        0    21949 2023-02-24 15:22:26.000000 wtfutil-1.0.9/wtfutil/sqlutil.py
+-rw-rw-rw-   0        0        0    17524 2023-03-11 15:07:44.000000 wtfutil-1.0.9/wtfutil/util.py
+drwxrwxrwx   0        0        0        0 2023-03-11 15:09:38.041160 wtfutil-1.0.9/wtfutil.egg-info/
+-rw-rw-rw-   0        0        0     2118 2023-03-11 15:09:37.000000 wtfutil-1.0.9/wtfutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-03-11 15:09:37.000000 wtfutil-1.0.9/wtfutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-11 15:09:37.000000 wtfutil-1.0.9/wtfutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-24 17:14:10.000000 wtfutil-1.0.9/wtfutil.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2023-03-11 15:09:37.000000 wtfutil-1.0.9/wtfutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-03-11 15:09:37.000000 wtfutil-1.0.9/wtfutil.egg-info/top_level.txt
```

### Comparing `wtfutil-1.0.8/LICENSE` & `wtfutil-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfutil-1.0.8/PKG-INFO` & `wtfutil-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtfutil
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python utility.
 Home-page: https://github.com/vicrack
 Author: vicrack
 Author-email: 18179821+ViCrack@users.noreply.github.com
 Platform: any
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wtfutil Version: 1.0.8 Summary: A Python utility.
+Metadata-Version: 2.1 Name: wtfutil Version: 1.0.9 Summary: A Python utility.
 Home-page: https://github.com/vicrack Author: vicrack Author-email:
 18179821+ViCrack@users.noreply.github.com Platform: any Classifier: Topic ::
 Utilities Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: BSD License Classifier: Topic :: Software Development ::
 Libraries Classifier: Development Status :: 5 - Production/Stable Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 2 Classifier: Programming Language :: Python :: 2.6 Classifier: Programming
```

### Comparing `wtfutil-1.0.8/README.md` & `wtfutil-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wtfutil-1.0.8/setup.py` & `wtfutil-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 import io
 import os
 import sys
 from codecs import open
 from shutil import rmtree
 
 __author__ = 'vicrack'
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 __contact__ = '18179821+ViCrack@users.noreply.github.com'
 __url__ = 'https://github.com/vicrack'
 __license__ = 'BSD'
 requires = [
     'pymysql',
     'faker',
     'requests',
     'cacheout',
     'requests_cache',
+    'tldextract',
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
```

### Comparing `wtfutil-1.0.8/wtfutil/notifyutil.py` & `wtfutil-1.0.9/wtfutil/notifyutil.py`

 * *Files identical despite different names*

### Comparing `wtfutil-1.0.8/wtfutil/sqlutil.py` & `wtfutil-1.0.9/wtfutil/sqlutil.py`

 * *Files identical despite different names*

### Comparing `wtfutil-1.0.8/wtfutil/util.py` & `wtfutil-1.0.9/wtfutil/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import re
 import ssl
 from io import BytesIO
 from socket import gethostbyname
 from typing import Any
 from urllib.parse import unquote, quote, urljoin
 from urllib.parse import urlparse
+import tldextract
 
 import faker
 import requests
 import urllib3
 from requests_cache import CachedSession
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.ssl_ import create_urllib3_context
@@ -539,7 +540,17 @@
 
 def get_resource(filename):
     resource_path = get_resource_dir(sys._getframe(1).f_code.co_filename) + "/" + filename
     if Path(resource_path).exists():
         return str(Path(resource_path).absolute())
     if Path(filename).expanduser().exists():
         return str(Path(filename).expanduser().absolute())
+
+
+def get_maindomain(subdomain):
+    # get the main domain from subdomain
+    tld = tldextract.extract(subdomain)
+    if tld.suffix != '':
+        domain = f'{tld.domain}.{tld.suffix}'
+    else:
+        domain = tld.domain
+    return domain
```

### Comparing `wtfutil-1.0.8/wtfutil.egg-info/PKG-INFO` & `wtfutil-1.0.9/wtfutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtfutil
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python utility.
 Home-page: https://github.com/vicrack
 Author: vicrack
 Author-email: 18179821+ViCrack@users.noreply.github.com
 Platform: any
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wtfutil Version: 1.0.8 Summary: A Python utility.
+Metadata-Version: 2.1 Name: wtfutil Version: 1.0.9 Summary: A Python utility.
 Home-page: https://github.com/vicrack Author: vicrack Author-email:
 18179821+ViCrack@users.noreply.github.com Platform: any Classifier: Topic ::
 Utilities Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: BSD License Classifier: Topic :: Software Development ::
 Libraries Classifier: Development Status :: 5 - Production/Stable Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 2 Classifier: Programming Language :: Python :: 2.6 Classifier: Programming
```

