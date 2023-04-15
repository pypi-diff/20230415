# Comparing `tmp/countrywrangler-0.2.6.tar.gz` & `tmp/countrywrangler-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countrywrangler-0.2.6.tar", last modified: Mon Mar 20 17:03:08 2023, max compression
+gzip compressed data, was "countrywrangler-0.2.7.tar", last modified: Sat Apr 15 14:57:34 2023, max compression
```

## Comparing `countrywrangler-0.2.6.tar` & `countrywrangler-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 17:03:08.765464 countrywrangler-0.2.6/
--rw-rw-rw-   0        0        0     1102 2023-03-17 00:54:45.000000 countrywrangler-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    13437 2023-03-20 17:03:08.764466 countrywrangler-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    12108 2023-03-19 21:16:47.000000 countrywrangler-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 17:03:08.699639 countrywrangler-0.2.6/countrywrangler/
--rw-rw-rw-   0        0        0     1292 2023-03-18 13:55:19.000000 countrywrangler-0.2.6/countrywrangler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:03:08.763497 countrywrangler-0.2.6/countrywrangler/databases/
--rw-rw-rw-   0        0        0     1178 2023-03-17 00:54:45.000000 countrywrangler-0.2.6/countrywrangler/databases/__init__.py
--rw-rw-rw-   0        0        0    12994 2023-03-18 18:20:47.000000 countrywrangler-0.2.6/countrywrangler/databases/codes.py
--rw-rw-rw-   0        0        0    22357 2023-03-19 14:35:52.000000 countrywrangler-0.2.6/countrywrangler/databases/languages.py
--rw-rw-rw-   0        0        0   220939 2023-03-19 20:53:37.000000 countrywrangler-0.2.6/countrywrangler/databases/names.py
--rw-rw-rw-   0        0        0    14097 2023-03-18 18:30:42.000000 countrywrangler-0.2.6/countrywrangler/databases/timezones.py
--rw-rw-rw-   0        0        0     7833 2023-03-17 00:54:45.000000 countrywrangler-0.2.6/countrywrangler/databases/tld.py
--rw-rw-rw-   0        0        0    12129 2023-03-19 21:27:31.000000 countrywrangler-0.2.6/countrywrangler/normalize.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:03:08.718588 countrywrangler-0.2.6/countrywrangler.egg-info/
--rw-rw-rw-   0        0        0    13437 2023-03-20 17:03:08.000000 countrywrangler-0.2.6/countrywrangler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-03-20 17:03:08.000000 countrywrangler-0.2.6/countrywrangler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 17:03:08.000000 countrywrangler-0.2.6/countrywrangler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-20 17:03:08.000000 countrywrangler-0.2.6/countrywrangler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-20 17:03:08.000000 countrywrangler-0.2.6/countrywrangler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 17:03:08.765464 countrywrangler-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1876 2023-03-20 17:01:32.000000 countrywrangler-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:57:34.072539 countrywrangler-0.2.7/
+-rw-rw-rw-   0        0        0     1102 2023-03-17 00:54:45.000000 countrywrangler-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    13437 2023-04-15 14:57:34.071541 countrywrangler-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    12108 2023-03-19 21:16:47.000000 countrywrangler-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 14:57:34.043616 countrywrangler-0.2.7/countrywrangler/
+-rw-rw-rw-   0        0        0     1292 2023-03-18 13:55:19.000000 countrywrangler-0.2.7/countrywrangler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:57:34.070544 countrywrangler-0.2.7/countrywrangler/databases/
+-rw-rw-rw-   0        0        0     1178 2023-03-17 00:54:45.000000 countrywrangler-0.2.7/countrywrangler/databases/__init__.py
+-rw-rw-rw-   0        0        0    12994 2023-03-18 18:20:47.000000 countrywrangler-0.2.7/countrywrangler/databases/codes.py
+-rw-rw-rw-   0        0        0    22357 2023-03-19 14:35:52.000000 countrywrangler-0.2.7/countrywrangler/databases/languages.py
+-rw-rw-rw-   0        0        0   220939 2023-03-19 20:53:37.000000 countrywrangler-0.2.7/countrywrangler/databases/names.py
+-rw-rw-rw-   0        0        0    14097 2023-03-18 18:30:42.000000 countrywrangler-0.2.7/countrywrangler/databases/timezones.py
+-rw-rw-rw-   0        0        0     7833 2023-03-17 00:54:45.000000 countrywrangler-0.2.7/countrywrangler/databases/tld.py
+-rw-rw-rw-   0        0        0    12296 2023-04-15 14:53:15.000000 countrywrangler-0.2.7/countrywrangler/normalize.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:57:34.064560 countrywrangler-0.2.7/countrywrangler.egg-info/
+-rw-rw-rw-   0        0        0    13437 2023-04-15 14:57:34.000000 countrywrangler-0.2.7/countrywrangler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-15 14:57:34.000000 countrywrangler-0.2.7/countrywrangler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 14:57:34.000000 countrywrangler-0.2.7/countrywrangler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-15 14:57:34.000000 countrywrangler-0.2.7/countrywrangler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 14:57:34.000000 countrywrangler-0.2.7/countrywrangler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 14:57:34.072539 countrywrangler-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1876 2023-04-15 14:53:30.000000 countrywrangler-0.2.7/setup.py
```

### Comparing `countrywrangler-0.2.6/LICENSE` & `countrywrangler-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/PKG-INFO` & `countrywrangler-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: countrywrangler
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library that simplifies the handling of country-related data. Easily standardize your data according to ISO 3166-1 and make it consistent across your project.
 Home-page: https://github.com/TheHenryWills/CountryWrangler
-Download-URL: https://github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.6.tar.gz
+Download-URL: https://github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.7.tar.gz
 Author: Henry Wills
 Author-email: hello@henrywills.com
 License: MIT
 Project-URL: Documentation, https://countrywrangler.readthedocs.io/en/latest/
 Project-URL: Linktree, https://linktr.ee/thehenrywills
 Keywords: iso-3166,iso-3166-1 ,normalize, countries-data,country,data-normalization,data-cleaning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: countrywrangler Version: 0.2.6 Summary: A library
+Metadata-Version: 2.1 Name: countrywrangler Version: 0.2.7 Summary: A library
 that simplifies the handling of country-related data. Easily standardize your
 data according to ISO 3166-1 and make it consistent across your project. Home-
 page: https://github.com/TheHenryWills/CountryWrangler Download-URL: https://
-github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.6.tar.gz
+github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.7.tar.gz
 Author: Henry Wills Author-email: hello@henrywills.com License: MIT Project-
 URL: Documentation, https://countrywrangler.readthedocs.io/en/latest/ Project-
 URL: Linktree, https://linktr.ee/thehenrywills Keywords: iso-3166,iso-3166-
 1 ,normalize, countries-data,country,data-normalization,data-cleaning
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

### Comparing `countrywrangler-0.2.6/README.md` & `countrywrangler-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/__init__.py` & `countrywrangler-0.2.7/countrywrangler/__init__.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/databases/__init__.py` & `countrywrangler-0.2.7/countrywrangler/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/databases/codes.py` & `countrywrangler-0.2.7/countrywrangler/databases/codes.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/databases/languages.py` & `countrywrangler-0.2.7/countrywrangler/databases/languages.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/databases/names.py` & `countrywrangler-0.2.7/countrywrangler/databases/names.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/databases/timezones.py` & `countrywrangler-0.2.7/countrywrangler/databases/timezones.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/databases/tld.py` & `countrywrangler-0.2.7/countrywrangler/databases/tld.py`

 * *Files identical despite different names*

### Comparing `countrywrangler-0.2.6/countrywrangler/normalize.py` & `countrywrangler-0.2.7/countrywrangler/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
                 return names[text]
             else:
                 return None
         else:
             # Exclude known edge cases from fuzzy search
             if text == "howland island" or text == "baker island":    # Would become IS for Iceland
                 return "US"
+            elif text == "united states" or text == "united states of america": # Would become UM for United States Minor Outlying Islands
+                return "US"
             elif text == "netherlands antilles": # Would become NL for Netherlands
                 return "AN"
             elif text == "juan de nova island" or text == "europa island": # Would become IS for Iceland
                 return "TF"
             elif text == "christmas island" or text == "norfolk island": # Would become IS for Iceland
                 return "AU"
```

### Comparing `countrywrangler-0.2.6/countrywrangler.egg-info/PKG-INFO` & `countrywrangler-0.2.7/countrywrangler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: countrywrangler
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library that simplifies the handling of country-related data. Easily standardize your data according to ISO 3166-1 and make it consistent across your project.
 Home-page: https://github.com/TheHenryWills/CountryWrangler
-Download-URL: https://github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.6.tar.gz
+Download-URL: https://github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.7.tar.gz
 Author: Henry Wills
 Author-email: hello@henrywills.com
 License: MIT
 Project-URL: Documentation, https://countrywrangler.readthedocs.io/en/latest/
 Project-URL: Linktree, https://linktr.ee/thehenrywills
 Keywords: iso-3166,iso-3166-1 ,normalize, countries-data,country,data-normalization,data-cleaning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: countrywrangler Version: 0.2.6 Summary: A library
+Metadata-Version: 2.1 Name: countrywrangler Version: 0.2.7 Summary: A library
 that simplifies the handling of country-related data. Easily standardize your
 data according to ISO 3166-1 and make it consistent across your project. Home-
 page: https://github.com/TheHenryWills/CountryWrangler Download-URL: https://
-github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.6.tar.gz
+github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.7.tar.gz
 Author: Henry Wills Author-email: hello@henrywills.com License: MIT Project-
 URL: Documentation, https://countrywrangler.readthedocs.io/en/latest/ Project-
 URL: Linktree, https://linktr.ee/thehenrywills Keywords: iso-3166,iso-3166-
 1 ,normalize, countries-data,country,data-normalization,data-cleaning
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

### Comparing `countrywrangler-0.2.6/setup.py` & `countrywrangler-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     with open(os.path.join(os.path.dirname(__file__), filename), encoding="utf-8") as file:
         return file.read()
 
 
 setup(
   name = 'countrywrangler',        
   packages = ['countrywrangler', 'countrywrangler.databases'],  
-  version = '0.2.6',     
+  version = '0.2.7',     
   license='MIT',       
   description = 'A library that simplifies the handling of country-related data. Easily standardize your data according to ISO 3166-1 and make it consistent across your project.', 
   long_description=read_file('README.md'),
   long_description_content_type='text/markdown',
   author = 'Henry Wills',                   
   author_email = 'hello@henrywills.com',      
   url = 'https://github.com/TheHenryWills/CountryWrangler', 
-  download_url = 'https://github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.6.tar.gz', 
+  download_url = 'https://github.com/TheHenryWills/CountryWrangler/archive/refs/tags/v_0.2.7.tar.gz', 
   keywords = ['iso-3166', 'iso-3166-1 ', 'normalize', ' countries-data', 'country', 'data-normalization', 'data-cleaning'],  
   install_requires=[           
           'phone_iso3166', 'fuzzywuzzy'
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

