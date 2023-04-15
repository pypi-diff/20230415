# Comparing `tmp/django-direct-cloud-upload-0.2.5.tar.gz` & `tmp/django-direct-cloud-upload-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-direct-cloud-upload-0.2.5.tar", last modified: Tue Oct 20 13:09:37 2020, max compression
+gzip compressed data, was "django-direct-cloud-upload-0.2.6.tar", last modified: Sat Apr 15 08:39:33 2023, max compression
```

## Comparing `django-direct-cloud-upload-0.2.5.tar` & `django-direct-cloud-upload-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.256239 django-direct-cloud-upload-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (116)     1498 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      177 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7205 2020-10-20 13:09:37.256239 django-direct-cloud-upload-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5136 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.252239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/
--rw-r--r--   0 runner    (1001) docker     (116)      421 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      221 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/admin.py
--rw-r--r--   0 runner    (1001) docker     (116)      144 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)      222 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/bucket_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.244239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.248239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.252239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      744 2020-10-20 13:09:35.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)     1215 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.248239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.256239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/static/direct_cloud_upload/
--rw-r--r--   0 runner    (1001) docker     (116)      840 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/static/direct_cloud_upload/cloud_file_widget.css
--rw-r--r--   0 runner    (1001) docker     (116)     3668 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/static/direct_cloud_upload/ddcu_upload.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.256239 django-direct-cloud-upload-0.2.5/direct_cloud_upload/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/templates/cloud_file_widget.html
--rw-r--r--   0 runner    (1001) docker     (116)     1930 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/views.py
--rw-r--r--   0 runner    (1001) docker     (116)     1601 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/direct_cloud_upload/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 13:09:37.256239 django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7205 2020-10-20 13:09:36.000000 django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      773 2020-10-20 13:09:37.000000 django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-20 13:09:36.000000 django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-10-20 13:09:36.000000 django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2020-10-20 13:09:36.000000 django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1095 2020-10-20 13:09:37.256239 django-direct-cloud-upload-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       37 2020-10-20 13:09:07.000000 django-direct-cloud-upload-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/bucket_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.144302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.144302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-15 08:39:31.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.144302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/static/direct_cloud_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/static/direct_cloud_upload/cloud_file_widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/static/direct_cloud_upload/ddcu_upload.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/direct_cloud_upload/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/templates/cloud_file_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/direct_cloud_upload/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:39:33.148302 django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-15 08:39:33.000000 django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 08:39:33.000000 django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:39:33.000000 django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 08:39:33.000000 django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 08:39:33.000000 django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-15 08:39:33.152302 django-direct-cloud-upload-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 08:38:40.000000 django-direct-cloud-upload-0.2.6/setup.py
```

### Comparing `django-direct-cloud-upload-0.2.5/LICENSE` & `django-direct-cloud-upload-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-direct-cloud-upload-0.2.5/PKG-INFO` & `django-direct-cloud-upload-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,165 @@
 Metadata-Version: 2.1
 Name: django-direct-cloud-upload
-Version: 0.2.5
+Version: 0.2.6
 Summary: Widget for uploading files from the client directly to a cloud storage bucket.
 Home-page: https://github.com/koendewit/django-direct-cloud-upload
 Author: Koen De Wit
 Author-email: koendewit@gmail.com
 License: BSD-3-Clause
-Description: # django-direct-cloud-upload (DDCU)
-        Widget for uploading files from the client directly to a cloud storage bucket. Currently only supports [Google Cloud Storage](https://cloud.google.com/storage/).
-        
-        Works with Internet Explorer 11, Google Chrome, Mozilla Firefox and Apple Safari.
-        
-        ## Installation and setup
-        
-        Install DDCU using pip :
-        
-            pip install django-direct-cloud-upload
-        
-        Make sure that `'django.contrib.staticfiles'` is [set up properly](https://docs.djangoproject.com/en/stable/howto/static-files/) and add `'direct_cloud_upload'` to your `INSTALLED_APPS` setting :
-        
-            INSTALLED_APPS = [
-                # ...
-                'django.contrib.staticfiles',
-                # ...
-                'direct_cloud_upload',
-            ]
-            
-            STATIC_URL = '/static/'
-            
-        DDCU provides a view that will generate a 'signed URL' for uploading a file. To enable this view, include DDCU's `urlpatterns` to your project's URLconf :
-        
-            import direct_cloud_upload
-            
-            urlpatterns = [
-                # ...
-                path('direct_cloud_upload/', include(direct_cloud_upload.urlpatterns)),
-            ]
-            
-        _Note_: It is not mandatory to choose `direct_cloud_upload/` as the path, you are free to set any path.
-        
-        ## Configuring the GCS bucket
-        
-        If you don't have a GCS bucket yet, [create one](https://cloud.google.com/storage/docs/creating-buckets) first.
-        
-        [Configure CORS](https://cloud.google.com/storage/docs/configuring-cors) on your bucket to allow uploads from your website. Configuring CORS for GCS buckets is done by creating a JSON-file describing the CORS policy and uploading the JSON file with `gsutil`.
-        
-        Example JSON file containing a CORS policy:
-        
-            [
-                {
-                    "origin": [
-                        "https://example-app.com",
-                        "https://www.example-app.com",
-                        "http://localhost:8000"
-                    ],
-                    "responseHeader": ["Content-Type"],
-                    "method": ["GET", "HEAD", "PUT"],
-                    "maxAgeSeconds": 3600
-                }
-            ]
-            
-        Upload the JSON file with the `gsutil cors set` command:
-        
-            gsutil cors set cors-json-file.json gs://example-bucket
-        
-        ## Usage
-        
-        Create a `Bucket` instance and register it with DDCU :
-        
-            import google.cloud.storage
-            import direct_cloud_upload
-            
-            client = google.cloud.storage.Client()
-            gcs_bucket = client.get_bucket('bucket-id-here')
-            ddcu_bucket_identifier = direct_cloud_upload.register_gcs_bucket(gcs_bucket)
-            
-        Creating the `Client` can be a bit more complicated if you need to authenticate, see the [GCS Python client documentation](https://googleapis.dev/python/storage/latest/client.html).
-        
-        Now you can use the `CloudFileWidget` for any `django.forms.CharField` in a Form :
-        
-            from direct_cloud_upload import CloudFileWidget
-        
-            class EbookForm(forms.ModelForm):
-                class Meta:
-                    model = Ebook
-                    fields = ['title', 'pdf_file']
-                    widgets = {
-                        'pdf_file': CloudFileWidget(
-                            bucket_identifier = ddcu_bucket_identifier,
-                            path_prefix = "ebook_pdf/",
-                        )
-                    }
-                    
-        `CloudFileWidget` has one required parameter:
-        
-        * `bucket_identifier` (string): identifier retrieved when registering the bucket with DDCU.
-        
-        `CloudFileWidget` has some optional parameters:
-        
-        * `path_prefix` (string): Will be prepended automatically to the path of each file. This is useful for collecting all files uploaded via this widget into one directory.
-        * `include_timestamp` (bool) : Determines if a timestamp will be added to the path. Defaults to `True`.
-        * `submit_timeout` (int) : Timeout (in seconds) for uploading the form. Defaults to 129600 (36 hours).
-        * `clearable` (bool) : Add a "Delete file" button to the widget. Defaults to `True`.
-        * `immediate_submit` (bool) : Immediately submit the form once the user selected a file. Defaults to `False`. _Warning:_ This is probably only useful if the file input is the only field in a form, because the user will not be able to input data in the other fields after selecting a file.
-        
-        When the form is being submitted, the field will contain the path in the bucket where the file has been uploaded to.
-        
-        ## Including static JS and CSS files
-        
-        DDCU needs a Javascript and CSS file to function. If you use the widget in a django-admin site, you can use the first method to include these files. For all other sites, you should read the "For generic forms" section below.
-        
-        ### For admin sites
-        
-        Let your Admin classes inherit from `DdcuAdminMixin`, which will instruct the admin interface to include the necessary files:
-        
-            from direct_cloud_upload import DdcuAdminMixin
-            
-            class EbookAdmin(admin.ModelAdmin, DdcuAdminMixin):
-                form = EbookForm
-        
-        ### For generic forms
-        
-        Every page containing a `CloudFileWidget` should include jQuery 1.9 (or newer) and the JS and CSS file in the `head` section:
-        
-            {% load static %}
-            
-            <head>
-                <link rel="stylesheet" href="{% static "direct_cloud_upload/cloud_file_widget.css" %}">
-                <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
-                <script src="{% static "direct_cloud_upload/ddcu_upload.js" %}"></script>
-            </head>
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-direct-cloud-upload (DDCU)
+Widget for uploading files from the client directly to a cloud storage bucket. Currently only supports [Google Cloud Storage](https://cloud.google.com/storage/).
+
+Works with Internet Explorer 11, Google Chrome, Mozilla Firefox and Apple Safari.
+
+After submitting a form containing this widget, the value of the widget will be the path of the file in the cloud bucket, not the file itself. Therefore, you cannot use this widget for a `FileField`. Use a `django.db.models.TextField` (for models) or `django.forms.CharField` (for forms) instead.
+
+## Installation and setup
+
+Install DDCU using pip :
+
+    pip install django-direct-cloud-upload
+
+Make sure that `'django.contrib.staticfiles'` is [set up properly](https://docs.djangoproject.com/en/stable/howto/static-files/) and add `'direct_cloud_upload'` to your `INSTALLED_APPS` setting :
+
+    INSTALLED_APPS = [
+        # ...
+        'django.contrib.staticfiles',
+        # ...
+        'direct_cloud_upload',
+    ]
+    
+    STATIC_URL = '/static/'
+    
+DDCU provides a view that will generate a 'signed URL' for uploading a file. To enable this view, include DDCU's `urlpatterns` to your project's URLconf :
+
+    import direct_cloud_upload
+    
+    urlpatterns = [
+        # ...
+        path('direct_cloud_upload/', include(direct_cloud_upload.urlpatterns)),
+    ]
+    
+_Note_: It is not mandatory to choose `direct_cloud_upload/` as the path, you are free to set any path.
+
+## Configuring the GCS bucket
+
+If you don't have a GCS bucket yet, [create one](https://cloud.google.com/storage/docs/creating-buckets) first.
+
+[Configure CORS](https://cloud.google.com/storage/docs/configuring-cors) on your bucket to allow uploads from your website. Configuring CORS for GCS buckets is done by creating a JSON-file describing the CORS policy and uploading the JSON file with `gsutil`.
+
+Example JSON file containing a CORS policy:
+
+    [
+        {
+            "origin": [
+                "https://example-app.com",
+                "https://www.example-app.com",
+                "http://localhost:8000"
+            ],
+            "responseHeader": ["Content-Type"],
+            "method": ["GET", "HEAD", "PUT"],
+            "maxAgeSeconds": 3600
+        }
+    ]
+    
+Upload the JSON file with the `gsutil cors set` command:
+
+    gsutil cors set cors-json-file.json gs://example-bucket
+
+## Usage
+
+Create a `Bucket` instance and register it with DDCU :
+
+    import google.cloud.storage
+    import direct_cloud_upload
+    
+    client = google.cloud.storage.Client()
+    gcs_bucket = client.get_bucket('bucket-id-here')
+    ddcu_bucket_identifier = direct_cloud_upload.register_gcs_bucket(gcs_bucket)
+    
+Creating the `Client` can be a bit more complicated if you need to authenticate, see the [GCS Python client documentation](https://googleapis.dev/python/storage/latest/client.html).
+
+Now you can use the `CloudFileWidget` for any `django.forms.CharField` in a Form :
+
+    from direct_cloud_upload import CloudFileWidget
+
+    class EbookForm(forms.ModelForm):
+        class Meta:
+            model = Ebook
+            fields = ['title', 'pdf_file']
+            widgets = {
+                'pdf_file': CloudFileWidget(
+                    bucket_identifier = ddcu_bucket_identifier,
+                    path_prefix = "ebook_pdf/",
+                )
+            }
+            
+`CloudFileWidget` has one required parameter:
+
+* `bucket_identifier` (string): identifier retrieved when registering the bucket with DDCU.
+
+`CloudFileWidget` has some optional parameters:
+
+* `path_prefix` (string): Will be prepended automatically to the path of each file. This is useful for collecting all files uploaded via this widget into one directory.
+* `include_timestamp` (bool) : Determines if a timestamp will be added to the path. Defaults to `True`.
+* `submit_timeout` (int) : Timeout (in seconds) for uploading the form. Defaults to 129600 (36 hours).
+* `clearable` (bool) : Add a "Delete file" button to the widget. Defaults to `True`.
+* `immediate_submit` (bool) : Immediately submit the form once the user selected a file. Defaults to `False`. _Warning:_ This is probably only useful if the file input is the only field in a form, because the user will not be able to input data in the other fields after selecting a file.
+* `show_replace_button` (bool) : Add a "Choose other file" button to the widget if the field contains a file. Defaults to `True`. _Warning:_ `clearable` and `show_replace_button` should not both be set to False, otherwise the user has no way to change the file.
+
+When the form is being submitted, the field will contain the path in the bucket where the file has been uploaded to.
+
+## Including static JS and CSS files
+
+DDCU needs a Javascript and CSS file to function. If you use the widget in a django-admin site, you can use the first method to include these files. For all other sites, you should read the "For generic forms" section below.
+
+### For admin sites
+
+Let your Admin classes inherit from `DdcuAdminMixin`, which will instruct the admin interface to include the necessary files:
+
+    from direct_cloud_upload import DdcuAdminMixin
+    
+    class EbookAdmin(DdcuAdminMixin):
+        form = EbookForm
+
+### For generic forms
+
+Every page containing a `CloudFileWidget` should include jQuery 1.9 (or newer) and the JS and CSS file in the `head` section:
+
+    {% load static %}
+    
+    <head>
+        <link rel="stylesheet" href="{% static "direct_cloud_upload/cloud_file_widget.css" %}">
+        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
+        <script src="{% static "direct_cloud_upload/ddcu_upload.js" %}"></script>
+    </head>
+
+## Troubleshooting
+
+### Error "No file was submitted. Check the encoding type on the form."
+
+If you get this error when submitting a form containing a `CloudFileWidget`, the widget is probably attached to a `FileField`. Use a `django.db.models.TextField` (for models) or `django.forms.CharField` (for forms) instead.
```

### Comparing `django-direct-cloud-upload-0.2.5/README.md` & `django-direct-cloud-upload-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # django-direct-cloud-upload (DDCU)
 Widget for uploading files from the client directly to a cloud storage bucket. Currently only supports [Google Cloud Storage](https://cloud.google.com/storage/).
 
 Works with Internet Explorer 11, Google Chrome, Mozilla Firefox and Apple Safari.
 
+After submitting a form containing this widget, the value of the widget will be the path of the file in the cloud bucket, not the file itself. Therefore, you cannot use this widget for a `FileField`. Use a `django.db.models.TextField` (for models) or `django.forms.CharField` (for forms) instead.
+
 ## Installation and setup
 
 Install DDCU using pip :
 
     pip install django-direct-cloud-upload
 
 Make sure that `'django.contrib.staticfiles'` is [set up properly](https://docs.djangoproject.com/en/stable/howto/static-files/) and add `'direct_cloud_upload'` to your `INSTALLED_APPS` setting :
@@ -91,34 +93,41 @@
 `CloudFileWidget` has some optional parameters:
 
 * `path_prefix` (string): Will be prepended automatically to the path of each file. This is useful for collecting all files uploaded via this widget into one directory.
 * `include_timestamp` (bool) : Determines if a timestamp will be added to the path. Defaults to `True`.
 * `submit_timeout` (int) : Timeout (in seconds) for uploading the form. Defaults to 129600 (36 hours).
 * `clearable` (bool) : Add a "Delete file" button to the widget. Defaults to `True`.
 * `immediate_submit` (bool) : Immediately submit the form once the user selected a file. Defaults to `False`. _Warning:_ This is probably only useful if the file input is the only field in a form, because the user will not be able to input data in the other fields after selecting a file.
+* `show_replace_button` (bool) : Add a "Choose other file" button to the widget if the field contains a file. Defaults to `True`. _Warning:_ `clearable` and `show_replace_button` should not both be set to False, otherwise the user has no way to change the file.
 
 When the form is being submitted, the field will contain the path in the bucket where the file has been uploaded to.
 
 ## Including static JS and CSS files
 
 DDCU needs a Javascript and CSS file to function. If you use the widget in a django-admin site, you can use the first method to include these files. For all other sites, you should read the "For generic forms" section below.
 
 ### For admin sites
 
 Let your Admin classes inherit from `DdcuAdminMixin`, which will instruct the admin interface to include the necessary files:
 
     from direct_cloud_upload import DdcuAdminMixin
     
-    class EbookAdmin(admin.ModelAdmin, DdcuAdminMixin):
+    class EbookAdmin(DdcuAdminMixin):
         form = EbookForm
 
 ### For generic forms
 
 Every page containing a `CloudFileWidget` should include jQuery 1.9 (or newer) and the JS and CSS file in the `head` section:
 
     {% load static %}
     
     <head>
         <link rel="stylesheet" href="{% static "direct_cloud_upload/cloud_file_widget.css" %}">
         <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
         <script src="{% static "direct_cloud_upload/ddcu_upload.js" %}"></script>
-    </head>
+    </head>
+
+## Troubleshooting
+
+### Error "No file was submitted. Check the encoding type on the form."
+
+If you get this error when submitting a form containing a `CloudFileWidget`, the widget is probably attached to a `FileField`. Use a `django.db.models.TextField` (for models) or `django.forms.CharField` (for forms) instead.
```

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/nl/LC_MESSAGES/django.mo` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/locale/nl/LC_MESSAGES/django.po` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/static/direct_cloud_upload/cloud_file_widget.css` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/static/direct_cloud_upload/cloud_file_widget.css`

 * *Files identical despite different names*

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/static/direct_cloud_upload/ddcu_upload.js` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/static/direct_cloud_upload/ddcu_upload.js`

 * *Files identical despite different names*

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/templates/cloud_file_widget.html` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/templates/cloud_file_widget.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,13 +5,15 @@
         type="hidden" name="{{ widget.name }}"
         {% if widget.value != None %} value="{{ widget.value|stringformat:'s' }}"{% endif %}
         {% include "django/forms/widgets/attrs.html" %}
     >
     <span class="ddcu_current_file_name">{{ current_file_name }}</span>
     <label>
         <span class="ddcu_choose_file">{% if ddcu_image %}{% trans "Choose image" %}{% else %}{% trans "Choose file" %}{% endif %}</span>
-        <span class="ddcu_choose_other_file">{% if ddcu_image %}{% trans "Choose other image" %}{% else %}{% trans "Choose other file" %}<{% endif %}/span>
+        {% if show_replace_button %}
+            <span class="ddcu_choose_other_file">{% if ddcu_image %}{% trans "Choose other image" %}{% else %}{% trans "Choose other file" %}{% endif %}</span>
+        {% endif %}
         <input type="file" class="ddcu_file_input" {% if ddcu_image %}accept="image/*"{% endif %}/>
     </label>
     {% if input_clearable %}<span class="ddcu_delete_file">{% if ddcu_image %}{% trans "Delete image" %}{% else %}{% trans "Delete file" %}{% endif %}</span>{% endif %}
 </div>
 <div class="ddcu_overlay"><p class="ddcu_overlay_text">{% trans "Uploading file, please wait..." %}</p></div>
```

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/views.py` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/views.py`

 * *Files identical despite different names*

### Comparing `django-direct-cloud-upload-0.2.5/direct_cloud_upload/widgets.py` & `django-direct-cloud-upload-0.2.6/direct_cloud_upload/widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,27 +12,30 @@
     def __init__(self,
                  bucket_identifier: str,
                  path_prefix: str = "",
                  include_timestamp: bool = True,
                  submit_timeout: int = 36 * 3600,
                  clearable = True,
                  immediate_submit = False,
+                 show_replace_button = True,
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.bucket_identifier = bucket_identifier
         self.path_prefix = path_prefix
         self.include_timestamp = include_timestamp
         self.submit_timeout = submit_timeout
         self.clearable = clearable
         self.immediate_submit = immediate_submit
+        self.show_replace_button = show_replace_button
 
     def get_context(self, name, value, attrs):
         context = super(CloudFileWidget, self).get_context(name, value, attrs)
         include_timestamp_indicator = '1' if self.include_timestamp else '0'
         valid_until = baseconv.base62.encode(int(time.time()) + self.submit_timeout)
         to_sign = f"{self.bucket_identifier}/{self.path_prefix}:{include_timestamp_indicator}:{valid_until}"
         context['ddcu_token'] = signer.sign(to_sign)
         context['guu_path'] = reverse('ddcu-get-upload-url')
         context['current_file_name'] = value.rsplit('/', 1)[-1] if value else ""
         context['input_clearable'] = self.clearable
         context['immediate_submit'] = self.immediate_submit
+        context['show_replace_button'] = self.show_replace_button
         return context
```

### Comparing `django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/PKG-INFO` & `django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,165 @@
 Metadata-Version: 2.1
 Name: django-direct-cloud-upload
-Version: 0.2.5
+Version: 0.2.6
 Summary: Widget for uploading files from the client directly to a cloud storage bucket.
 Home-page: https://github.com/koendewit/django-direct-cloud-upload
 Author: Koen De Wit
 Author-email: koendewit@gmail.com
 License: BSD-3-Clause
-Description: # django-direct-cloud-upload (DDCU)
-        Widget for uploading files from the client directly to a cloud storage bucket. Currently only supports [Google Cloud Storage](https://cloud.google.com/storage/).
-        
-        Works with Internet Explorer 11, Google Chrome, Mozilla Firefox and Apple Safari.
-        
-        ## Installation and setup
-        
-        Install DDCU using pip :
-        
-            pip install django-direct-cloud-upload
-        
-        Make sure that `'django.contrib.staticfiles'` is [set up properly](https://docs.djangoproject.com/en/stable/howto/static-files/) and add `'direct_cloud_upload'` to your `INSTALLED_APPS` setting :
-        
-            INSTALLED_APPS = [
-                # ...
-                'django.contrib.staticfiles',
-                # ...
-                'direct_cloud_upload',
-            ]
-            
-            STATIC_URL = '/static/'
-            
-        DDCU provides a view that will generate a 'signed URL' for uploading a file. To enable this view, include DDCU's `urlpatterns` to your project's URLconf :
-        
-            import direct_cloud_upload
-            
-            urlpatterns = [
-                # ...
-                path('direct_cloud_upload/', include(direct_cloud_upload.urlpatterns)),
-            ]
-            
-        _Note_: It is not mandatory to choose `direct_cloud_upload/` as the path, you are free to set any path.
-        
-        ## Configuring the GCS bucket
-        
-        If you don't have a GCS bucket yet, [create one](https://cloud.google.com/storage/docs/creating-buckets) first.
-        
-        [Configure CORS](https://cloud.google.com/storage/docs/configuring-cors) on your bucket to allow uploads from your website. Configuring CORS for GCS buckets is done by creating a JSON-file describing the CORS policy and uploading the JSON file with `gsutil`.
-        
-        Example JSON file containing a CORS policy:
-        
-            [
-                {
-                    "origin": [
-                        "https://example-app.com",
-                        "https://www.example-app.com",
-                        "http://localhost:8000"
-                    ],
-                    "responseHeader": ["Content-Type"],
-                    "method": ["GET", "HEAD", "PUT"],
-                    "maxAgeSeconds": 3600
-                }
-            ]
-            
-        Upload the JSON file with the `gsutil cors set` command:
-        
-            gsutil cors set cors-json-file.json gs://example-bucket
-        
-        ## Usage
-        
-        Create a `Bucket` instance and register it with DDCU :
-        
-            import google.cloud.storage
-            import direct_cloud_upload
-            
-            client = google.cloud.storage.Client()
-            gcs_bucket = client.get_bucket('bucket-id-here')
-            ddcu_bucket_identifier = direct_cloud_upload.register_gcs_bucket(gcs_bucket)
-            
-        Creating the `Client` can be a bit more complicated if you need to authenticate, see the [GCS Python client documentation](https://googleapis.dev/python/storage/latest/client.html).
-        
-        Now you can use the `CloudFileWidget` for any `django.forms.CharField` in a Form :
-        
-            from direct_cloud_upload import CloudFileWidget
-        
-            class EbookForm(forms.ModelForm):
-                class Meta:
-                    model = Ebook
-                    fields = ['title', 'pdf_file']
-                    widgets = {
-                        'pdf_file': CloudFileWidget(
-                            bucket_identifier = ddcu_bucket_identifier,
-                            path_prefix = "ebook_pdf/",
-                        )
-                    }
-                    
-        `CloudFileWidget` has one required parameter:
-        
-        * `bucket_identifier` (string): identifier retrieved when registering the bucket with DDCU.
-        
-        `CloudFileWidget` has some optional parameters:
-        
-        * `path_prefix` (string): Will be prepended automatically to the path of each file. This is useful for collecting all files uploaded via this widget into one directory.
-        * `include_timestamp` (bool) : Determines if a timestamp will be added to the path. Defaults to `True`.
-        * `submit_timeout` (int) : Timeout (in seconds) for uploading the form. Defaults to 129600 (36 hours).
-        * `clearable` (bool) : Add a "Delete file" button to the widget. Defaults to `True`.
-        * `immediate_submit` (bool) : Immediately submit the form once the user selected a file. Defaults to `False`. _Warning:_ This is probably only useful if the file input is the only field in a form, because the user will not be able to input data in the other fields after selecting a file.
-        
-        When the form is being submitted, the field will contain the path in the bucket where the file has been uploaded to.
-        
-        ## Including static JS and CSS files
-        
-        DDCU needs a Javascript and CSS file to function. If you use the widget in a django-admin site, you can use the first method to include these files. For all other sites, you should read the "For generic forms" section below.
-        
-        ### For admin sites
-        
-        Let your Admin classes inherit from `DdcuAdminMixin`, which will instruct the admin interface to include the necessary files:
-        
-            from direct_cloud_upload import DdcuAdminMixin
-            
-            class EbookAdmin(admin.ModelAdmin, DdcuAdminMixin):
-                form = EbookForm
-        
-        ### For generic forms
-        
-        Every page containing a `CloudFileWidget` should include jQuery 1.9 (or newer) and the JS and CSS file in the `head` section:
-        
-            {% load static %}
-            
-            <head>
-                <link rel="stylesheet" href="{% static "direct_cloud_upload/cloud_file_widget.css" %}">
-                <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
-                <script src="{% static "direct_cloud_upload/ddcu_upload.js" %}"></script>
-            </head>
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-direct-cloud-upload (DDCU)
+Widget for uploading files from the client directly to a cloud storage bucket. Currently only supports [Google Cloud Storage](https://cloud.google.com/storage/).
+
+Works with Internet Explorer 11, Google Chrome, Mozilla Firefox and Apple Safari.
+
+After submitting a form containing this widget, the value of the widget will be the path of the file in the cloud bucket, not the file itself. Therefore, you cannot use this widget for a `FileField`. Use a `django.db.models.TextField` (for models) or `django.forms.CharField` (for forms) instead.
+
+## Installation and setup
+
+Install DDCU using pip :
+
+    pip install django-direct-cloud-upload
+
+Make sure that `'django.contrib.staticfiles'` is [set up properly](https://docs.djangoproject.com/en/stable/howto/static-files/) and add `'direct_cloud_upload'` to your `INSTALLED_APPS` setting :
+
+    INSTALLED_APPS = [
+        # ...
+        'django.contrib.staticfiles',
+        # ...
+        'direct_cloud_upload',
+    ]
+    
+    STATIC_URL = '/static/'
+    
+DDCU provides a view that will generate a 'signed URL' for uploading a file. To enable this view, include DDCU's `urlpatterns` to your project's URLconf :
+
+    import direct_cloud_upload
+    
+    urlpatterns = [
+        # ...
+        path('direct_cloud_upload/', include(direct_cloud_upload.urlpatterns)),
+    ]
+    
+_Note_: It is not mandatory to choose `direct_cloud_upload/` as the path, you are free to set any path.
+
+## Configuring the GCS bucket
+
+If you don't have a GCS bucket yet, [create one](https://cloud.google.com/storage/docs/creating-buckets) first.
+
+[Configure CORS](https://cloud.google.com/storage/docs/configuring-cors) on your bucket to allow uploads from your website. Configuring CORS for GCS buckets is done by creating a JSON-file describing the CORS policy and uploading the JSON file with `gsutil`.
+
+Example JSON file containing a CORS policy:
+
+    [
+        {
+            "origin": [
+                "https://example-app.com",
+                "https://www.example-app.com",
+                "http://localhost:8000"
+            ],
+            "responseHeader": ["Content-Type"],
+            "method": ["GET", "HEAD", "PUT"],
+            "maxAgeSeconds": 3600
+        }
+    ]
+    
+Upload the JSON file with the `gsutil cors set` command:
+
+    gsutil cors set cors-json-file.json gs://example-bucket
+
+## Usage
+
+Create a `Bucket` instance and register it with DDCU :
+
+    import google.cloud.storage
+    import direct_cloud_upload
+    
+    client = google.cloud.storage.Client()
+    gcs_bucket = client.get_bucket('bucket-id-here')
+    ddcu_bucket_identifier = direct_cloud_upload.register_gcs_bucket(gcs_bucket)
+    
+Creating the `Client` can be a bit more complicated if you need to authenticate, see the [GCS Python client documentation](https://googleapis.dev/python/storage/latest/client.html).
+
+Now you can use the `CloudFileWidget` for any `django.forms.CharField` in a Form :
+
+    from direct_cloud_upload import CloudFileWidget
+
+    class EbookForm(forms.ModelForm):
+        class Meta:
+            model = Ebook
+            fields = ['title', 'pdf_file']
+            widgets = {
+                'pdf_file': CloudFileWidget(
+                    bucket_identifier = ddcu_bucket_identifier,
+                    path_prefix = "ebook_pdf/",
+                )
+            }
+            
+`CloudFileWidget` has one required parameter:
+
+* `bucket_identifier` (string): identifier retrieved when registering the bucket with DDCU.
+
+`CloudFileWidget` has some optional parameters:
+
+* `path_prefix` (string): Will be prepended automatically to the path of each file. This is useful for collecting all files uploaded via this widget into one directory.
+* `include_timestamp` (bool) : Determines if a timestamp will be added to the path. Defaults to `True`.
+* `submit_timeout` (int) : Timeout (in seconds) for uploading the form. Defaults to 129600 (36 hours).
+* `clearable` (bool) : Add a "Delete file" button to the widget. Defaults to `True`.
+* `immediate_submit` (bool) : Immediately submit the form once the user selected a file. Defaults to `False`. _Warning:_ This is probably only useful if the file input is the only field in a form, because the user will not be able to input data in the other fields after selecting a file.
+* `show_replace_button` (bool) : Add a "Choose other file" button to the widget if the field contains a file. Defaults to `True`. _Warning:_ `clearable` and `show_replace_button` should not both be set to False, otherwise the user has no way to change the file.
+
+When the form is being submitted, the field will contain the path in the bucket where the file has been uploaded to.
+
+## Including static JS and CSS files
+
+DDCU needs a Javascript and CSS file to function. If you use the widget in a django-admin site, you can use the first method to include these files. For all other sites, you should read the "For generic forms" section below.
+
+### For admin sites
+
+Let your Admin classes inherit from `DdcuAdminMixin`, which will instruct the admin interface to include the necessary files:
+
+    from direct_cloud_upload import DdcuAdminMixin
+    
+    class EbookAdmin(DdcuAdminMixin):
+        form = EbookForm
+
+### For generic forms
+
+Every page containing a `CloudFileWidget` should include jQuery 1.9 (or newer) and the JS and CSS file in the `head` section:
+
+    {% load static %}
+    
+    <head>
+        <link rel="stylesheet" href="{% static "direct_cloud_upload/cloud_file_widget.css" %}">
+        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
+        <script src="{% static "direct_cloud_upload/ddcu_upload.js" %}"></script>
+    </head>
+
+## Troubleshooting
+
+### Error "No file was submitted. Check the encoding type on the form."
+
+If you get this error when submitting a form containing a `CloudFileWidget`, the widget is probably attached to a `FileField`. Use a `django.db.models.TextField` (for models) or `django.forms.CharField` (for forms) instead.
```

### Comparing `django-direct-cloud-upload-0.2.5/django_direct_cloud_upload.egg-info/SOURCES.txt` & `django-direct-cloud-upload-0.2.6/django_direct_cloud_upload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

