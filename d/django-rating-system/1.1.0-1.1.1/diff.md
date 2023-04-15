# Comparing `tmp/django-rating-system-1.1.0.tar.gz` & `tmp/django-rating-system-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rating-system-1.1.0.tar", last modified: Mon Apr 10 08:54:45 2023, max compression
+gzip compressed data, was "django-rating-system-1.1.1.tar", last modified: Sat Apr 15 11:45:51 2023, max compression
```

## Comparing `django-rating-system-1.1.0.tar` & `django-rating-system-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/django_rating_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-10 08:54:45.000000 django-rating-system-1.1.0/django_rating_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/migrations/0002_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.544947 django-rating-system-1.1.0/rating/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.544947 django-rating-system-1.1.0/rating/static/rating/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/static/rating/css/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/css/style.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/static/rating/img/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/img/heart.svg
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/img/star.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/static/rating/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/js/rating.js
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/js/rating.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/templates/rating/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templates/rating/info/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/info/info_base.html
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/info/info_extender.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templates/rating/rating/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/rating/rating.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/rating/rating_info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templates/rating/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/utils/IMPORTS.html
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/utils/SCRIPTS.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templatetags/rating_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.595008 django-rating-system-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-15 11:45:51.595008 django-rating-system-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.595008 django-rating-system-1.1.1/django_rating_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-15 11:45:51.000000 django-rating-system-1.1.1/django_rating_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/migrations/0002_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.587007 django-rating-system-1.1.1/rating/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.587007 django-rating-system-1.1.1/rating/static/rating/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/static/rating/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/static/rating/css/rating.css
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/static/rating/css/rating.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/static/rating/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/static/rating/img/heart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/static/rating/img/star.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/static/rating/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/static/rating/js/rating.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/static/rating/js/rating.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.587007 django-rating-system-1.1.1/rating/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.587007 django-rating-system-1.1.1/rating/templates/rating/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/templates/rating/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templates/rating/info/info_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templates/rating/info/info_extender.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/templates/rating/rating/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templates/rating/rating/rating.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templates/rating/rating/rating_info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.591007 django-rating-system-1.1.1/rating/templates/rating/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templates/rating/utils/IMPORTS.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templates/rating/utils/SCRIPTS.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:51.595008 django-rating-system-1.1.1/rating/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/templatetags/rating_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/rating/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-15 11:45:51.595008 django-rating-system-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 11:45:45.000000 django-rating-system-1.1.1/setup.py
```

### Comparing `django-rating-system-1.1.0/LICENSE` & `django-rating-system-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/PKG-INFO` & `django-rating-system-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rating-system
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django rating System, It can be associated with any given model.
 Home-page: https://github.com/mahyar-amiri/django-rating-system
 Author: Mahyar Amiri
 Author-email: mmaahhyyaarr@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/mahyar-amiri/django-rating-system/README.md
 Project-URL: Source Code, https://github.com/mahyar-amiri/django-rating-system
```

### Comparing `django-rating-system-1.1.0/README.md` & `django-rating-system-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,16 @@
 <details>
 <summary>Static Folder Tree</summary>
 <p>
 
 ```text
 static
    ├── css
-   │    ├── style.css
-   │    └── style.min.css
+   │    ├── rating.css
+   │    └── rating.min.css
    ├── img
    │    ├── heart.svg
    │    └── star.svg
    └── js
         ├── rating.js
         ├── rating.min.js
         └── jquery.min.js
```

### Comparing `django-rating-system-1.1.0/README.rst` & `django-rating-system-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/django_rating_system.egg-info/SOURCES.txt` & `django-rating-system-1.1.1/django_rating_system.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 rating/settings.py
 rating/tests.py
 rating/urls.py
 rating/views.py
 rating/migrations/0001_initial.py
 rating/migrations/0002_config.py
 rating/migrations/__init__.py
-rating/static/rating/css/style.css
-rating/static/rating/css/style.min.css
+rating/static/rating/css/rating.css
+rating/static/rating/css/rating.min.css
 rating/static/rating/img/heart.svg
 rating/static/rating/img/star.svg
 rating/static/rating/js/rating.js
 rating/static/rating/js/rating.min.js
 rating/templates/rating/info/info_base.html
 rating/templates/rating/info/info_extender.html
 rating/templates/rating/rating/rating.html
```

### Comparing `django-rating-system-1.1.0/rating/__init__.py` & `django-rating-system-1.1.1/rating/__init__.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/admin.py` & `django-rating-system-1.1.1/rating/admin.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/migrations/0001_initial.py` & `django-rating-system-1.1.1/rating/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/migrations/0002_config.py` & `django-rating-system-1.1.1/rating/migrations/0002_config.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/models.py` & `django-rating-system-1.1.1/rating/models.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/static/rating/css/style.css` & `django-rating-system-1.1.1/rating/static/rating/css/rating.css`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/static/rating/img/star.svg` & `django-rating-system-1.1.1/rating/static/rating/img/star.svg`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/static/rating/js/rating.js` & `django-rating-system-1.1.1/rating/static/rating/js/rating.js`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/static/rating/js/rating.min.js` & `django-rating-system-1.1.1/rating/static/rating/js/rating.min.js`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/templates/rating/rating/rating.html` & `django-rating-system-1.1.1/rating/templates/rating/rating/rating.html`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/templates/rating/rating/rating_info.html` & `django-rating-system-1.1.1/rating/templates/rating/rating/rating_info.html`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/templatetags/rating_tags.py` & `django-rating-system-1.1.1/rating/templatetags/rating_tags.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/rating/views.py` & `django-rating-system-1.1.1/rating/views.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.1.0/setup.cfg` & `django-rating-system-1.1.1/setup.cfg`

 * *Files identical despite different names*

