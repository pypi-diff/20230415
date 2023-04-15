# Comparing `tmp/django_model_privacy_mixin-0.2.tar.gz` & `tmp/django_model_privacy_mixin-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_model_privacy_mixin-0.2.tar", last modified: Mon Mar 13 10:26:43 2023, max compression
+gzip compressed data, was "django_model_privacy_mixin-0.3.tar", last modified: Sat Apr 15 03:04:01 2023, max compression
```

## Comparing `django_model_privacy_mixin-0.2.tar` & `django_model_privacy_mixin-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-03-13 10:26:43.362538 django_model_privacy_mixin-0.2/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_model_privacy_mixin-0.2/LICENSE.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-03-13 10:26:43.362538 django_model_privacy_mixin-0.2/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    13691 2023-03-13 10:24:23.000000 django_model_privacy_mixin-0.2/README.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_model_privacy_mixin-0.2/pyproject.toml
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      947 2023-03-13 10:26:43.362538 django_model_privacy_mixin-0.2/setup.cfg
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-03-13 10:26:43.362538 django_model_privacy_mixin-0.2/src/
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-03-13 10:26:43.362538 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin/
--rw-r--r--   0 bernd     (1000) bernd     (1000)    12330 2023-03-13 10:21:49.000000 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin/__init__.py
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-03-13 10:26:43.362538 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-03-13 10:26:43.000000 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      357 2023-03-13 10:26:43.000000 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/SOURCES.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2023-03-13 10:26:43.000000 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/dependency_links.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       49 2023-03-13 10:26:43.000000 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/requires.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       27 2023-03-13 10:26:43.000000 django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/top_level.txt
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_model_privacy_mixin-0.3/LICENSE.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    13691 2023-03-13 10:24:23.000000 django_model_privacy_mixin-0.3/README.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_model_privacy_mixin-0.3/pyproject.toml
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      935 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/setup.cfg
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.523549 django_model_privacy_mixin-0.3/src/
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.523549 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin/
+-rw-r--r--   0 bernd     (1000) bernd     (1000)    12480 2023-04-15 02:57:57.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin/__init__.py
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      357 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       39 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/requires.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       27 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/top_level.txt
```

### Comparing `django_model_privacy_mixin-0.2/LICENSE.md` & `django_model_privacy_mixin-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_model_privacy_mixin-0.2/PKG-INFO` & `django_model_privacy_mixin-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django_model_privacy_mixin
-Version: 0.2
+Version: 0.3
 Summary: Django Model MixIn providing flexible field privacy control
 Home-page: https://github.com/bernd-wechner/django-model-privacy-mixin
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-model-privacy-mixin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django Model Privacy MixIn
```

### Comparing `django_model_privacy_mixin-0.2/README.md` & `django_model_privacy_mixin-0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_model_privacy_mixin-0.2/setup.cfg` & `django_model_privacy_mixin-0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = django_model_privacy_mixin
-version = 0.2
+version = 0.3
 author = Bernd Wechner
 author_email = bwechner@yahoo.com
 description = Django Model MixIn providing flexible field privacy control
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bernd-wechner/django-model-privacy-mixin
 project_urls = 
 	Bug Tracker = https://github.com/bernd-wechner/django-model-privacy-mixin/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Freely Distributable
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
 	Intended Audience :: System Administrators
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 install_requires = 
-	django-currentuser >= 0.5.3
+	django-crequest
 	django-bitfield >= 2.0.1
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
```

### Comparing `django_model_privacy_mixin-0.2/src/django_model_privacy_mixin/__init__.py` & `django_model_privacy_mixin-0.3/src/django_model_privacy_mixin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 '''
 Created on 8 Mar.,2018
 
 @author: Bernd Wechner
 @status: Beta - works and is in use on a dedicated project.
 
+In your Dango settings.py make sure to cilude 'crequest.middleware.CrequestMiddleware' in the MIDDDLEWARE list.
+
 Provides one class PrivacyMixIn which adds Privacy support for model fields in a Django model.
 '''
 
 from django.core.exceptions import PermissionDenied
 from django.forms.models import fields_for_model
 from django.utils.safestring import mark_safe
 
-from django_currentuser.middleware import get_current_user
+from crequest.middleware import CrequestMiddleware
 
 class PrivacyMixIn():
     '''
     A MixIn that adds database load overrides which populates the "hidden" attribute of
     an object with the names of fields that should be hidden. It is up to the other
     methods in the model to implement this hiding where desired.
     '''
@@ -237,15 +239,16 @@
         Override the from_db method.
         Runs the standard model from_db() then checks for and enforces privacy constraints.
 
         This is the central pinch point for database access and all requests for objects come
         through this method.
         '''
         obj = super().from_db(db, field_names, values)
-        user = get_current_user()
+        request = CrequestMiddleware.get_request()
+        user = request.user
         obj.hidden = obj.fields_to_hide(user)
         if obj.hidden:
             for f in obj.hidden:
                 val = getattr(obj, f, None)
                 if cls.HIDE_EMPTY_FIELD or not (val is None or str(val) == ""):
                     if callable(getattr(obj, cls.HIDE_METHOD, None)):
                         setattr(obj, f, getattr(obj, cls.HIDE_METHOD)(cls._meta.get_field(f)))
```

### Comparing `django_model_privacy_mixin-0.2/src/django_model_privacy_mixin.egg-info/PKG-INFO` & `django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-model-privacy-mixin
-Version: 0.2
+Version: 0.3
 Summary: Django Model MixIn providing flexible field privacy control
 Home-page: https://github.com/bernd-wechner/django-model-privacy-mixin
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-model-privacy-mixin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django Model Privacy MixIn
```

