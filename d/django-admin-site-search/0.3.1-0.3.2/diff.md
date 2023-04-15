# Comparing `tmp/django-admin-site-search-0.3.1.tar.gz` & `tmp/django-admin-site-search-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-site-search-0.3.1.tar", last modified: Mon Apr  3 09:43:34 2023, max compression
+gzip compressed data, was "django-admin-site-search-0.3.2.tar", last modified: Sat Apr 15 13:40:38 2023, max compression
```

## Comparing `django-admin-site-search-0.3.1.tar` & `django-admin-site-search-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.655974 django-admin-site-search-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-03 09:43:34.655974 django-admin-site-search-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.647974 django-admin-site-search-0.3.1/admin_site_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.643974 django-admin-site-search-0.3.1/admin_site_search/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.647974 django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.651975 django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/alpinejs/
--rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.643974 django-admin-site-search-0.3.1/admin_site_search/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.651975 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/button.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/head.html
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/input.html
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/results.html
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/spinner.html
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/admin_site_search/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:43:34.655974 django-admin-site-search-0.3.1/django_admin_site_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-03 09:43:34.000000 django-admin-site-search-0.3.1/django_admin_site_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-03 09:43:34.000000 django-admin-site-search-0.3.1/django_admin_site_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 09:43:34.000000 django-admin-site-search-0.3.1/django_admin_site_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 09:43:34.000000 django-admin-site-search-0.3.1/django_admin_site_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-03 09:43:34.000000 django-admin-site-search-0.3.1/django_admin_site_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-03 09:43:34.655974 django-admin-site-search-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 09:43:18.000000 django-admin-site-search-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/admin_site_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.812678 django-admin-site-search-0.3.2/admin_site_search/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/alpinejs/
+-rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.812678 django-admin-site-search-0.3.2/admin_site_search/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/input.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/spinner.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/admin_site_search/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/django_admin_site_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-15 13:40:38.000000 django-admin-site-search-0.3.2/django_admin_site_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-15 13:40:38.000000 django-admin-site-search-0.3.2/django_admin_site_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:40:38.000000 django-admin-site-search-0.3.2/django_admin_site_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 13:40:38.000000 django-admin-site-search-0.3.2/django_admin_site_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 13:40:38.000000 django-admin-site-search-0.3.2/django_admin_site_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-15 13:40:38.816678 django-admin-site-search-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:40:25.000000 django-admin-site-search-0.3.2/setup.py
```

### Comparing `django-admin-site-search-0.3.1/LICENSE` & `django-admin-site-search-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/PKG-INFO` & `django-admin-site-search-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-site-search
-Version: 0.3.1
+Version: 0.3.2
 Summary: A search (cmd+k) modal, for the Django admin UI, that searches your entire site.
 Home-page: https://github.com/ahmedaljawahiry/django-admin-site-search/
 Author: Ahmed Al-Jawahiry
 Author-email: ahmedaljawahiry@gmail.com
 License: MIT
 Project-URL: Maintainer, https://ahmedaljawahiry.com
 Keywords: Django
```

### Comparing `django-admin-site-search-0.3.1/README.md` & `django-admin-site-search-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js` & `django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/alpinejs/3-12-0.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js` & `django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/alpinejs/focus-3-12-0.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/search.js` & `django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -32,15 +32,15 @@
     }
 
     /**
      * State/functions for performing searches.
      */
     Alpine.data('siteSearch', () => {
         const adminPath = window.location.pathname.split('/')[1] || '';
-        const adminSearchPath = adminPath ? `/${adminPath}/search/` : '/search';
+        const adminSearchPath = adminPath ? `/${adminPath}/search/` : '/search/';
         const minChars = 2;
         const resultsEmpty = {
             apps: []
         };
 
         return {
             /**
```

### Comparing `django-admin-site-search-0.3.1/admin_site_search/static/admin_site_search/style.css` & `django-admin-site-search-0.3.2/admin_site_search/static/admin_site_search/style.css`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/button.html` & `django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/button.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/head.html` & `django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/input.html` & `django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/input.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/modal.html` & `django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/modal.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/templates/admin_site_search/results.html` & `django-admin-site-search-0.3.2/admin_site_search/templates/admin_site_search/results.html`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/admin_site_search/views.py` & `django-admin-site-search-0.3.2/admin_site_search/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/django_admin_site_search.egg-info/PKG-INFO` & `django-admin-site-search-0.3.2/django_admin_site_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-site-search
-Version: 0.3.1
+Version: 0.3.2
 Summary: A search (cmd+k) modal, for the Django admin UI, that searches your entire site.
 Home-page: https://github.com/ahmedaljawahiry/django-admin-site-search/
 Author: Ahmed Al-Jawahiry
 Author-email: ahmedaljawahiry@gmail.com
 License: MIT
 Project-URL: Maintainer, https://ahmedaljawahiry.com
 Keywords: Django
```

### Comparing `django-admin-site-search-0.3.1/django_admin_site_search.egg-info/SOURCES.txt` & `django-admin-site-search-0.3.2/django_admin_site_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-site-search-0.3.1/setup.cfg` & `django-admin-site-search-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-admin-site-search
-version = 0.3.1
+version = 0.3.2
 description = A search (cmd+k) modal, for the Django admin UI, that searches your entire site.
 long_description = file: README.md
 long_description_content_type = text/markdown
 readme = "README.md"
 url = https://github.com/ahmedaljawahiry/django-admin-site-search/
 author = Ahmed Al-Jawahiry
 author_email = ahmedaljawahiry@gmail.com
```

