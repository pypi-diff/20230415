# Comparing `tmp/django-api-admin-1.0.3.tar.gz` & `tmp/django-api-admin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-admin-1.0.3.tar", last modified: Mon Aug 29 20:29:27 2022, max compression
+gzip compressed data, was "django-api-admin-1.1.0.tar", last modified: Sat Apr 15 17:26:09 2023, max compression
```

## Comparing `django-api-admin-1.0.3.tar` & `django-api-admin-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,23 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 20:29:27.250437 django-api-admin-1.0.3/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1071 2022-08-29 16:54:12.000000 django-api-admin-1.0.3/LICENSE
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       78 2022-08-29 20:12:13.000000 django-api-admin-1.0.3/MANIFEST.in
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2739 2022-08-29 20:29:27.250437 django-api-admin-1.0.3/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2079 2022-08-29 20:17:40.000000 django-api-admin-1.0.3/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 20:29:27.250437 django-api-admin-1.0.3/django_api_admin/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 16:54:12.000000 django-api-admin-1.0.3/django_api_admin/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1771 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/actions.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      162 2022-08-29 17:10:24.000000 django-api-admin-1.0.3/django_api_admin/apps.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 20:29:27.246437 django-api-admin-1.0.3/django_api_admin/locale/
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 20:29:27.246437 django-api-admin-1.0.3/django_api_admin/locale/ar/
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 20:29:27.250437 django-api-admin-1.0.3/django_api_admin/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3093 2022-08-29 16:54:12.000000 django-api-admin-1.0.3/django_api_admin/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3804 2022-08-29 16:54:12.000000 django-api-admin-1.0.3/django_api_admin/locale/ar/LC_MESSAGES/django.po
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11118 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/options.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      548 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/pagination.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      335 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/permissions.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3711 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/serializer_field_attributes.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     5279 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/serializers.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    12837 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/sites.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     5393 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/utils.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    32056 2022-08-29 20:16:56.000000 django-api-admin-1.0.3/django_api_admin/views.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2022-08-29 20:29:27.250437 django-api-admin-1.0.3/django_api_admin.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2739 2022-08-29 20:29:27.000000 django-api-admin-1.0.3/django_api_admin.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      666 2022-08-29 20:29:27.000000 django-api-admin-1.0.3/django_api_admin.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2022-08-29 20:29:27.000000 django-api-admin-1.0.3/django_api_admin.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       27 2022-08-29 20:29:27.000000 django-api-admin-1.0.3/django_api_admin.egg-info/requires.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       17 2022-08-29 20:29:27.000000 django-api-admin-1.0.3/django_api_admin.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2022-08-29 20:29:27.250437 django-api-admin-1.0.3/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1061 2022-08-29 20:24:41.000000 django-api-admin-1.0.3/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1071 2023-03-15 22:10:39.000000 django-api-admin-1.1.0/LICENSE
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       77 2023-04-15 16:55:11.000000 django-api-admin-1.1.0/MANIFEST.in
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2070 2023-04-15 17:16:56.000000 django-api-admin-1.1.0/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 17:26:09.229582 django-api-admin-1.1.0/django_api_admin/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-03-15 22:10:39.000000 django-api-admin-1.1.0/django_api_admin/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1771 2023-03-24 20:07:54.000000 django-api-admin-1.1.0/django_api_admin/actions.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      162 2023-03-24 20:08:37.000000 django-api-admin-1.1.0/django_api_admin/apps.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3726 2023-03-24 20:00:01.000000 django-api-admin-1.1.0/django_api_admin/field_attributes.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11262 2023-04-06 11:43:08.000000 django-api-admin-1.1.0/django_api_admin/options.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      548 2023-03-24 20:11:26.000000 django-api-admin-1.1.0/django_api_admin/pagination.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      335 2023-03-15 22:10:39.000000 django-api-admin-1.1.0/django_api_admin/permissions.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     5255 2023-04-12 08:25:20.000000 django-api-admin-1.1.0/django_api_admin/serializers.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    12838 2023-03-24 20:15:20.000000 django-api-admin-1.1.0/django_api_admin/sites.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/django_api_admin.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      505 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       27 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/requires.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       17 2023-04-15 17:26:09.000000 django-api-admin-1.1.0/django_api_admin.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-04-15 17:26:09.237582 django-api-admin-1.1.0/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1111 2023-04-15 16:56:25.000000 django-api-admin-1.1.0/setup.py
```

### Comparing `django-api-admin-1.0.3/LICENSE` & `django-api-admin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.0.3/PKG-INFO` & `django-api-admin-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.0.3
+Version: 1.1.0
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 
 ## Features ⚡
 
-* Expose all django.contrib.admin views as a restful api.
-* Similar to django.contrib.admin.
-* Customizable AdminSite and ModelAdmin.
-* Supports InlineModelAdmins.
-* Provides data to dynamically create forms on clients from serializers.
-* Supports Arabic Language.
-* Extensively tested
+- [x] Expose all django.contrib.admin views as a restful api.
+- [x] Similar to django.contrib.admin.
+- [x] Customizable AdminSite and ModelAdmin.
+- [x] Supports InlineModelAdmins and bulk edits.
+- [x] Provides data to dynamically create forms on clients from serializers.
+- [x] Extensively tested
+
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
 <p>This package depends on</p>
 <ul>
     <li><a href="https://github.com/encode/django-rest-framework">django-rest-framework</a></li>
@@ -106,15 +106,11 @@
 <p>4. run your development server.</p>
 
 ```bash
 $ python manage.py runsever
 ```
 
 visit your <a href="http://127.0.0.1:8000/api_admin">localhost</a> to see the browsable api.
-<<<<<<< HEAD
-=======
 
 ## Screenshots 🖼
 
 <img src="screenshots/browsable_api_root.png" alt="browsable_api_root"/>
-
-
```

### Comparing `django-api-admin-1.0.3/README.md` & `django-api-admin-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 
 ## Features ⚡
 
-* Expose all django.contrib.admin views as a restful api.
-* Similar to django.contrib.admin.
-* Customizable AdminSite and ModelAdmin.
-* Supports InlineModelAdmins.
-* Provides data to dynamically create forms on clients from serializers.
-* Supports Arabic Language.
-* Extensively tested
+- [x] Expose all django.contrib.admin views as a restful api.
+- [x] Similar to django.contrib.admin.
+- [x] Customizable AdminSite and ModelAdmin.
+- [x] Supports InlineModelAdmins and bulk edits.
+- [x] Provides data to dynamically create forms on clients from serializers.
+- [x] Extensively tested
+
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
 <p>This package depends on</p>
 <ul>
     <li><a href="https://github.com/encode/django-rest-framework">django-rest-framework</a></li>
@@ -89,13 +89,11 @@
 <p>4. run your development server.</p>
 
 ```bash
 $ python manage.py runsever
 ```
 
 visit your <a href="http://127.0.0.1:8000/api_admin">localhost</a> to see the browsable api.
-<<<<<<< HEAD
-=======
 
 ## Screenshots 🖼
 
 <img src="screenshots/browsable_api_root.png" alt="browsable_api_root"/>
```

### Comparing `django-api-admin-1.0.3/django_api_admin/actions.py` & `django-api-admin-1.1.0/django_api_admin/actions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.contrib.admin import action
 from django.contrib.admin.utils import model_ngettext
 from django.utils.translation import gettext_lazy, gettext as _
+
 from rest_framework import status
 from rest_framework.exceptions import PermissionDenied
-
 from rest_framework.response import Response
 
 
 @action(
     permissions=['delete'],
     description=gettext_lazy('Delete selected %(verbose_name_plural)s')
 )
```

### Comparing `django-api-admin-1.0.3/django_api_admin/options.py` & `django-api-admin-1.1.0/django_api_admin/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+"""
+API model admin.
+"""
+
 from django.contrib.admin.options import InlineModelAdmin, ModelAdmin
 from django.contrib.admin.utils import flatten_fieldsets
 from django.contrib.auth import get_permission_codename
 from django.db import router, transaction
 from rest_framework import serializers
 
-from . import views as api_views
+from .views import admin_views
 from .serializers import ActionSerializer
 
 
 class BaseAPIModelAdmin:
     """
     Shared behavior between APIModelAdmin, APIInlineModelAdmin.
     """
@@ -33,14 +37,15 @@
         excluded = self.get_exclude(request, obj)
         exclude = list(excluded) if excluded is not None else []
         # get read only fields
         readonly_fields = self.get_readonly_fields(request, obj)
         # subtract excluded fields from fieldsets_fields
         fields = [field for field in fieldsets_fields if field not in exclude]
 
+        # if it's a changelist include all the fields because the hiding happens in the changelist view
         if changelist:
             fields = '__all__'
 
         # dynamically construct a model serializer
         return type('%sSerializer' % self.model.__name__, (serializers.ModelSerializer,), {
             'Meta': type('Meta', (object,), {
                 'model': self.model,
@@ -98,45 +103,45 @@
         return isinstance(self, InlineModelAdmin)
 
     def list_view(self, request):
         defaults = {
             'serializer_class': self.get_serializer_class(request),
             'permission_classes': self.admin_site.default_permission_classes,
         }
-        return api_views.ListView.as_view(**defaults)(request, self)
+        return admin_views.ListView.as_view(**defaults)(request, self)
 
     def detail_view(self, request, object_id):
         defaults = {
             'serializer_class': self.get_serializer_class(request),
             'permission_classes': self.admin_site.default_permission_classes,
         }
-        return api_views.DetailView.as_view(**defaults)(request, object_id, self)
+        return admin_views.DetailView.as_view(**defaults)(request, object_id, self)
 
     def add_view(self, request, **kwargs):
         defaults = {
             'serializer_class': self.get_serializer_class(request),
             'permission_classes': self.admin_site.default_permission_classes,
         }
         with transaction.atomic(using=router.db_for_write(self.model)):
-            return api_views.AddView.as_view(**defaults)(request, self, **kwargs)
+            return admin_views.AddView.as_view(**defaults)(request, self, **kwargs)
 
     def change_view(self, request, object_id, **kwargs):
         defaults = {
             'serializer_class': self.get_serializer_class(request),
             'permission_classes': self.admin_site.default_permission_classes,
         }
         with transaction.atomic(using=router.db_for_write(self.model)):
-            return api_views.ChangeView.as_view(**defaults)(request, object_id, self, **kwargs)
+            return admin_views.ChangeView.as_view(**defaults)(request, object_id, self, **kwargs)
 
     def delete_view(self, request, object_id, **kwargs):
         defaults = {
             'permission_classes': self.admin_site.default_permission_classes
         }
         with transaction.atomic(using=router.db_for_write(self.model)):
-            return api_views.DeleteView.as_view(**defaults)(request, object_id, self, **kwargs)
+            return admin_views.DeleteView.as_view(**defaults)(request, object_id, self, **kwargs)
 
 
 class APIModelAdmin(BaseAPIModelAdmin, ModelAdmin):
     """
     exposes django.contrib.admin.options.ModelAdmin as a restful api.
     everything that is ui specific is handled by the ui
     filtering is also handled by the ui
@@ -211,29 +216,29 @@
             ])
         return urlpatterns
 
     def changelist_view(self, request, **kwargs):
         defaults = {
             'permission_classes': self.admin_site.default_permission_classes
         }
-        return api_views.ChangeListView.as_view(**defaults)(request, self)
+        return admin_views.ChangeListView.as_view(**defaults)(request, self)
 
     def handle_action_view(self, request):
         defaults = {
             'permission_classes': self.admin_site.default_permission_classes,
             'serializer_class': self.get_action_serializer(request)
         }
-        return api_views.HandleActionView.as_view(**defaults)(request, self)
+        return admin_views.HandleActionView.as_view(**defaults)(request, self)
 
     def history_view(self, request, object_id, extra_context=None):
         defaults = {
             'permission_classes': self.admin_site.default_permission_classes,
             'serializer_class': self.admin_site.log_entry_serializer,
         }
-        return api_views.HistoryView.as_view(**defaults)(request, object_id, self)
+        return admin_views.HistoryView.as_view(**defaults)(request, object_id, self)
 
 
 class InlineAPIModelAdmin(BaseAPIModelAdmin, InlineModelAdmin):
     """
     Edit models connected with a relationship in one page
     """
     admin_style = None
```

### Comparing `django-api-admin-1.0.3/django_api_admin/pagination.py` & `django-api-admin-1.1.0/django_api_admin/pagination.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.0.3/django_api_admin/serializer_field_attributes.py` & `django-api-admin-1.1.0/django_api_admin/field_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Django rest framework serializer fields attributes.
+"""
+
 shared_attributes = [
     'read_only', 'write_only', 'required', 'default',
     'allow_blank', 'allow_null', 'style', 'label',
     'help_text', 'initial',
 ]
 
 shared_string_fields_attributes = [
@@ -21,15 +25,14 @@
 shared_relationship_fields_attributes = [
     'choices', 'many', 'html_cutoff', 'html_cutoff_text',
 ]
 
 field_attributes = {
     # boolean fields attributes
     'BooleanField': {*shared_attributes},
-    'NullBooleanField': {*shared_attributes},
 
     # String fields attributes
     'CharField': [*shared_attributes, *shared_string_fields_attributes],
     'EmailField': [*shared_attributes, *shared_string_fields_attributes],
     'RegexField': [*shared_attributes, *shared_string_fields_attributes, 'regex'],
     'SlugField': [*shared_attributes, *shared_string_fields_attributes, 'allow_unicode'],
     'URLField': [*shared_attributes, *shared_string_fields_attributes],
```

### Comparing `django-api-admin-1.0.3/django_api_admin/serializers.py` & `django-api-admin-1.1.0/django_api_admin/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.admin.models import LogEntry
 from django.contrib.auth import get_user_model, authenticate
 from django.utils.translation import gettext_lazy as _
 from rest_framework import serializers
-from pathlib import Path
+
 
 UserModel = get_user_model()
 
 
 class UserSerializer(serializers.ModelSerializer):
     class Meta:
         model = UserModel
```

### Comparing `django-api-admin-1.0.3/django_api_admin/sites.py` & `django-api-admin-1.1.0/django_api_admin/sites.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+"""
+API admin site.
+"""
+
 from functools import update_wrapper
 
 from django.apps import apps
 from django.contrib.admin import AdminSite
 from django.contrib.admin.sites import AlreadyRegistered
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models.base import ModelBase
 from django.urls import NoReverseMatch, reverse
 from django.utils.text import capfirst
 from django.views.decorators.cache import never_cache
 from django.views.decorators.csrf import csrf_protect
-from rest_framework import filters
 
 from . import actions
 from . import serializers as api_serializers
-from . import views as api_views
+from .views import site_views 
 from .options import APIModelAdmin
 from .pagination import AdminLogPagination, AdminResultsListPagination
 from .permissions import IsAdminUser
 
 UserModel = get_user_model()
 
 
@@ -149,15 +152,15 @@
         # add api_root for browsable api.
         if self.include_root_view:
             # remove detail, redirect urls and urls with no names
             excluded_url_names = ['app_list',
                                   'view_on_site', 'language_catalog']
             root_urls = [url for url in urlpatterns if
                          isinstance(url, URLPattern) and url.name and url.name not in excluded_url_names]
-            root_view = api_views.AdminAPIRootView.as_view(root_urls=root_urls)
+            root_view = site_views.AdminAPIRootView.as_view(root_urls=root_urls)
             urlpatterns.append(path('', root_view, name='api-root'))
         return urlpatterns
 
     @property
     def urls(self):
         return self.get_urls(), self.name, self.name
 
@@ -248,80 +251,80 @@
             'user': self.user_serializer(read_only=True),
         })
 
     def index(self, request, extra_context=None):
         defaults = {
             'permission_classes': self.default_permission_classes,
         }
-        return api_views.IndexView.as_view(**defaults)(request, admin_site=self)
+        return site_views.IndexView.as_view(**defaults)(request, admin_site=self)
 
     def app_index(self, request, app_label, extra_context=None):
         defaults = {
             'permission_classes': self.default_permission_classes,
         }
-        return api_views.AppIndexView.as_view(**defaults)(request, app_label=app_label, admin_site=self)
+        return site_views.AppIndexView.as_view(**defaults)(request, app_label=app_label, admin_site=self)
 
     def login(self, request, extra_context=None):
         defaults = {
             'permission_classes': [],
             'serializer_class': self.login_serializer,
         }
 
         if request.method == 'GET':
-            return api_views.LoginView.as_view(**defaults)(request, self)
+            return site_views.LoginView.as_view(**defaults)(request, self)
 
-        return api_views.LoginView.as_view(**defaults)(request, self)
+        return site_views.LoginView.as_view(**defaults)(request, self)
 
     def logout(self, request, extra_context=None):
         defaults = {
             'permission_classes': self.default_permission_classes,
         }
-        return api_views.LogoutView.as_view(**defaults)(request)
+        return site_views.LogoutView.as_view(**defaults)(request)
 
     def password_change(self, request, extra_context=None):
         defaults = {
             'permission_classes': self.default_permission_classes,
             'serializer_class': self.password_change_serializer,
         }
-        return api_views.PasswordChangeView.as_view(**defaults)(request)
+        return site_views.PasswordChangeView.as_view(**defaults)(request)
 
     def i18n_javascript(self, request, extra_context=None):
         defaults = {
             'permission_classes': self.default_permission_classes,
         }
-        return api_views.LanguageCatalogView.as_view(**defaults)(request)
+        return site_views.LanguageCatalogView.as_view(**defaults)(request)
 
     def autocomplete_view(self, request):
         defaults = {
             'permission_classes': self.default_permission_classes,
         }
-        return api_views.AutoCompleteView.as_view(**defaults)(request, admin_site=self)
+        return site_views.AutoCompleteView.as_view(**defaults)(request, admin_site=self)
 
     def site_context_view(self, request):
         defaults = {
             'permission_classes': self.default_permission_classes,
         }
-        return api_views.SiteContextView.as_view(**defaults)(request, admin_site=self)
+        return site_views.SiteContextView.as_view(**defaults)(request, admin_site=self)
 
     def admin_log_view(self, request):
         defaults = {
             'permission_classes': self.default_permission_classes,
             'pagination_class': self.default_log_pagination_class,
             'serializer_class': self.get_log_entry_serializer(),
         }
-        return api_views.AdminLogView.as_view(**defaults)(request, self)
+        return site_views.AdminLogView.as_view(**defaults)(request, self)
 
     def csrf_view(self, request, extra_context=None):
         defaults = {
             'permission_classes': [],
         }
-        return api_views.CsrfTokenView.as_view(**defaults)(request)
+        return site_views.CsrfTokenView.as_view(**defaults)(request)
 
     def user_info_view(self, request):
         defaults = {
             'permission_classes': self.default_permission_classes,
             'serializer_class': self.user_serializer
         }
-        return api_views.UserInformation.as_view(**defaults)(request)
+        return site_views.UserInformation.as_view(**defaults)(request)
 
 
 site = APIAdminSite(name='api_admin', include_auth=True)
```

### Comparing `django-api-admin-1.0.3/django_api_admin.egg-info/PKG-INFO` & `django-api-admin-1.1.0/django_api_admin.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.0.3
+Version: 1.1.0
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 
 ## Features ⚡
 
-* Expose all django.contrib.admin views as a restful api.
-* Similar to django.contrib.admin.
-* Customizable AdminSite and ModelAdmin.
-* Supports InlineModelAdmins.
-* Provides data to dynamically create forms on clients from serializers.
-* Supports Arabic Language.
-* Extensively tested
+- [x] Expose all django.contrib.admin views as a restful api.
+- [x] Similar to django.contrib.admin.
+- [x] Customizable AdminSite and ModelAdmin.
+- [x] Supports InlineModelAdmins and bulk edits.
+- [x] Provides data to dynamically create forms on clients from serializers.
+- [x] Extensively tested
+
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
 <p>This package depends on</p>
 <ul>
     <li><a href="https://github.com/encode/django-rest-framework">django-rest-framework</a></li>
@@ -106,15 +106,11 @@
 <p>4. run your development server.</p>
 
 ```bash
 $ python manage.py runsever
 ```
 
 visit your <a href="http://127.0.0.1:8000/api_admin">localhost</a> to see the browsable api.
-<<<<<<< HEAD
-=======
 
 ## Screenshots 🖼
 
 <img src="screenshots/browsable_api_root.png" alt="browsable_api_root"/>
-
-
```

### Comparing `django-api-admin-1.0.3/setup.py` & `django-api-admin-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-api-admin",
-    version="1.0.3",
+    version="1.1.0",
     description="Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MuhammadSalahAli/django-api-admin",
     author="Muhammad Salah",
     author_email="msmainacc0unt@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     packages=["django_api_admin"],
     include_package_data=True,
     install_requires=["django", "djangorestframework"],
 )
```

