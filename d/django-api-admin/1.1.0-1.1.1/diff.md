# Comparing `tmp/django-api-admin-1.1.0.tar.gz` & `tmp/django-api-admin-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-admin-1.1.0.tar", last modified: Sat Apr 15 17:26:09 2023, max compression
+gzip compressed data, was "django-api-admin-1.1.1.tar", last modified: Sat Apr 15 21:03:51 2023, max compression
```

## Comparing `django-api-admin-1.1.0.tar` & `django-api-admin-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,40 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1071 2023-03-15 22:10:39.000000 django-api-admin-1.1.0/LICENSE
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       77 2023-04-15 16:55:11.000000 django-api-admin-1.1.0/MANIFEST.in
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2070 2023-04-15 17:16:56.000000 django-api-admin-1.1.0/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 17:26:09.229582 django-api-admin-1.1.0/django_api_admin/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-03-15 22:10:39.000000 django-api-admin-1.1.0/django_api_admin/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1771 2023-03-24 20:07:54.000000 django-api-admin-1.1.0/django_api_admin/actions.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      162 2023-03-24 20:08:37.000000 django-api-admin-1.1.0/django_api_admin/apps.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3726 2023-03-24 20:00:01.000000 django-api-admin-1.1.0/django_api_admin/field_attributes.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11262 2023-04-06 11:43:08.000000 django-api-admin-1.1.0/django_api_admin/options.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      548 2023-03-24 20:11:26.000000 django-api-admin-1.1.0/django_api_admin/pagination.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      335 2023-03-15 22:10:39.000000 django-api-admin-1.1.0/django_api_admin/permissions.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     5255 2023-04-12 08:25:20.000000 django-api-admin-1.1.0/django_api_admin/serializers.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    12838 2023-03-24 20:15:20.000000 django-api-admin-1.1.0/django_api_admin/sites.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/django_api_admin.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      505 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       27 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/requires.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       17 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1111 2023-04-15 16:56:25.000000 django-api-admin-1.1.0/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1071 2023-03-15 22:10:39.000000 django-api-admin-1.1.1/LICENSE
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       90 2023-04-15 20:58:20.000000 django-api-admin-1.1.1/MANIFEST.in
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2070 2023-04-15 20:39:35.000000 django-api-admin-1.1.1/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.414317 django-api-admin-1.1.1/django_api_admin/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-03-15 22:10:39.000000 django-api-admin-1.1.1/django_api_admin/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1771 2023-03-24 20:07:54.000000 django-api-admin-1.1.1/django_api_admin/actions.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.422317 django-api-admin-1.1.1/django_api_admin/declarations/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/declarations/__init__.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.426317 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      186 2023-04-15 19:12:35.000000 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2319 2023-04-13 19:27:34.000000 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/classes.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     6903 2023-04-15 13:54:24.000000 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/functions.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1324 2023-04-13 10:53:41.000000 django-api-admin-1.1.1/django_api_admin/declarations/classes.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    13151 2023-04-15 13:54:21.000000 django-api-admin-1.1.1/django_api_admin/declarations/functions.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3726 2023-03-24 20:00:01.000000 django-api-admin-1.1.1/django_api_admin/field_attributes.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11294 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/options.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      548 2023-03-24 20:11:26.000000 django-api-admin-1.1.1/django_api_admin/pagination.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      335 2023-03-15 22:10:39.000000 django-api-admin-1.1.1/django_api_admin/permissions.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     5255 2023-04-12 08:25:20.000000 django-api-admin-1.1.1/django_api_admin/serializers.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    12948 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/sites.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.430317 django-api-admin-1.1.1/django_api_admin/views/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/views/__init__.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/django_api_admin/views/__pycache__/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      179 2023-04-15 18:52:38.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    17641 2023-04-15 16:51:31.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/admin_views.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     7747 2023-04-14 11:41:03.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/fields_test_views.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     8325 2023-04-14 11:40:18.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/site_views.cpython-310.pyc
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    25791 2023-04-15 16:51:29.000000 django-api-admin-1.1.1/django_api_admin/views/admin_views.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11410 2023-04-14 11:40:59.000000 django-api-admin-1.1.1/django_api_admin/views/fields_test_views.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     8166 2023-04-14 11:40:16.000000 django-api-admin-1.1.1/django_api_admin/views/site_views.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.418317 django-api-admin-1.1.1/django_api_admin.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1215 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       27 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/requires.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       17 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1111 2023-04-15 21:03:11.000000 django-api-admin-1.1.1/setup.py
```

### Comparing `django-api-admin-1.1.0/LICENSE` & `django-api-admin-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.0/PKG-INFO` & `django-api-admin-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.0
+Version: 1.1.1
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-api-admin-1.1.0/README.md` & `django-api-admin-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.0/django_api_admin/actions.py` & `django-api-admin-1.1.1/django_api_admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.0/django_api_admin/field_attributes.py` & `django-api-admin-1.1.1/django_api_admin/field_attributes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.0/django_api_admin/options.py` & `django-api-admin-1.1.1/django_api_admin/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from django.contrib.admin.options import InlineModelAdmin, ModelAdmin
 from django.contrib.admin.utils import flatten_fieldsets
 from django.contrib.auth import get_permission_codename
 from django.db import router, transaction
 from rest_framework import serializers
 
-from .views import admin_views
-from .serializers import ActionSerializer
+from django_api_admin.views import admin_views
+from django_api_admin.serializers import ActionSerializer
 
 
 class BaseAPIModelAdmin:
     """
     Shared behavior between APIModelAdmin, APIInlineModelAdmin.
     """
     # these are the options used in the change/add forms
```

### Comparing `django-api-admin-1.1.0/django_api_admin/pagination.py` & `django-api-admin-1.1.1/django_api_admin/pagination.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.0/django_api_admin/serializers.py` & `django-api-admin-1.1.1/django_api_admin/serializers.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.0/django_api_admin/sites.py` & `django-api-admin-1.1.1/django_api_admin/sites.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models.base import ModelBase
 from django.urls import NoReverseMatch, reverse
 from django.utils.text import capfirst
 from django.views.decorators.cache import never_cache
 from django.views.decorators.csrf import csrf_protect
 
-from . import actions
-from . import serializers as api_serializers
-from .views import site_views 
-from .options import APIModelAdmin
-from .pagination import AdminLogPagination, AdminResultsListPagination
-from .permissions import IsAdminUser
+from django_api_admin import actions
+from django_api_admin import serializers as api_serializers
+from django_api_admin.views import site_views
+from django_api_admin.options import APIModelAdmin
+from django_api_admin.pagination import AdminLogPagination, AdminResultsListPagination
+from django_api_admin.permissions import IsAdminUser
 
 UserModel = get_user_model()
 
 
 class APIAdminSite(AdminSite):
     """
     Encapsulates an instance of the django admin application.
@@ -152,15 +152,16 @@
         # add api_root for browsable api.
         if self.include_root_view:
             # remove detail, redirect urls and urls with no names
             excluded_url_names = ['app_list',
                                   'view_on_site', 'language_catalog']
             root_urls = [url for url in urlpatterns if
                          isinstance(url, URLPattern) and url.name and url.name not in excluded_url_names]
-            root_view = site_views.AdminAPIRootView.as_view(root_urls=root_urls)
+            root_view = site_views.AdminAPIRootView.as_view(
+                root_urls=root_urls)
             urlpatterns.append(path('', root_view, name='api-root'))
         return urlpatterns
 
     @property
     def urls(self):
         return self.get_urls(), self.name, self.name
```

### Comparing `django-api-admin-1.1.0/django_api_admin.egg-info/PKG-INFO` & `django-api-admin-1.1.1/django_api_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.0
+Version: 1.1.1
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-api-admin-1.1.0/setup.py` & `django-api-admin-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-api-admin",
-    version="1.1.0",
+    version="1.1.1",
     description="Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MuhammadSalahAli/django-api-admin",
     author="Muhammad Salah",
     author_email="msmainacc0unt@gmail.com",
     license="MIT",
```

