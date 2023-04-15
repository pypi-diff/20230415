# Comparing `tmp/admin-form-image-preivew-1.4.tar.gz` & `tmp/admin-form-image-preivew-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin-form-image-preivew-1.4.tar", last modified: Tue Apr 11 11:30:34 2023, max compression
+gzip compressed data, was "admin-form-image-preivew-1.5.tar", last modified: Sat Apr 15 08:01:01 2023, max compression
```

## Comparing `admin-form-image-preivew-1.4.tar` & `admin-form-image-preivew-1.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.771909 admin-form-image-preivew-1.4/
--rw-rw-r--   0 sami      (1000) sami      (1000)      419 2023-04-11 05:45:07.000000 admin-form-image-preivew-1.4/.gitignore
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.4/CHANGES.rst
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.4/LICENSE.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)     1911 2023-04-11 11:30:34.771909 admin-form-image-preivew-1.4/PKG-INFO
--rw-rw-r--   0 sami      (1000) sami      (1000)     1114 2023-04-11 11:29:43.000000 admin-form-image-preivew-1.4/README.md
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.759909 admin-form-image-preivew-1.4/admin_form_image_preivew/
--rw-rw-r--   0 sami      (1000) sami      (1000)       22 2023-04-01 14:28:33.000000 admin-form-image-preivew-1.4/admin_form_image_preivew/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     3845 2023-04-08 06:36:12.000000 admin-form-image-preivew-1.4/admin_form_image_preivew/settings.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      185 2023-04-01 14:28:25.000000 admin-form-image-preivew-1.4/admin_form_image_preivew/wsgi.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.759909 admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/
--rw-rw-r--   0 sami      (1000) sami      (1000)     1911 2023-04-11 11:30:34.000000 admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/PKG-INFO
--rw-rw-r--   0 sami      (1000) sami      (1000)     1564 2023-04-11 11:30:34.000000 admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/SOURCES.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)        1 2023-04-11 11:30:34.000000 admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/dependency_links.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)      159 2023-04-11 11:30:34.000000 admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/requires.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)       20 2023-04-11 11:30:34.000000 admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/top_level.txt
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.763909 admin-form-image-preivew-1.4/admin_image_preview/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.4/admin_image_preview/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      168 2023-04-08 06:26:54.000000 admin-form-image-preivew-1.4/admin_image_preview/apps.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.763909 admin-form-image-preivew-1.4/admin_image_preview/migrations/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.4/admin_image_preview/migrations/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      293 2023-04-07 14:30:35.000000 admin-form-image-preivew-1.4/admin_image_preview/models.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     1767 2023-04-10 12:09:04.000000 admin-form-image-preivew-1.4/admin_image_preview/readme.md
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.747909 admin-form-image-preivew-1.4/admin_image_preview/static/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.763909 admin-form-image-preivew-1.4/admin_image_preview/static/admin_image_preview/
--rw-rw-r--   0 sami      (1000) sami      (1000)     3872 2023-04-11 04:52:02.000000 admin-form-image-preivew-1.4/admin_image_preview/static/admin_image_preview/image_preview.js
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.747909 admin-form-image-preivew-1.4/admin_image_preview/templates/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.763909 admin-form-image-preivew-1.4/admin_image_preview/templates/admin/
--rw-rw-r--   0 sami      (1000) sami      (1000)      213 2023-04-10 12:05:52.000000 admin-form-image-preivew-1.4/admin_image_preview/templates/admin/change_form.html
--rw-rw-r--   0 sami      (1000) sami      (1000)     3804 2023-04-10 08:30:05.000000 admin-form-image-preivew-1.4/admin_image_preview/templates/admin/original_change_form.html
--rw-rw-r--   0 sami      (1000) sami      (1000)     1113 2023-04-08 07:03:57.000000 admin-form-image-preivew-1.4/del.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.763909 admin-form-image-preivew-1.4/docs/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.4/docs/index.rst
--rw-rw-r--   0 sami      (1000) sami      (1000)     1348 2023-04-11 11:30:19.000000 admin-form-image-preivew-1.4/docs/make_pip.md
--rw-rw-r--   0 sami      (1000) sami      (1000)     1096 2023-04-10 12:10:33.000000 admin-form-image-preivew-1.4/pyproject.toml
--rw-rw-r--   0 sami      (1000) sami      (1000)       74 2023-04-11 06:04:33.000000 admin-form-image-preivew-1.4/requirements.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)      230 2023-04-11 08:00:45.000000 admin-form-image-preivew-1.4/sample_pypirc_test.txt
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.767909 admin-form-image-preivew-1.4/sample_usage/
--rw-r--r--   0 sami      (1000) sami      (1000)    90636 2023-04-01 08:16:18.000000 admin-form-image-preivew-1.4/sample_usage/92news-logo.png
--rw-rw-r--   0 sami      (1000) sami      (1000)     1121 2023-04-10 07:55:08.000000 admin-form-image-preivew-1.4/sample_usage/del.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     1413 2023-04-11 11:30:17.000000 admin-form-image-preivew-1.4/sample_usage/fixtures.json
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.747909 admin-form-image-preivew-1.4/sample_usage/initsql/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.767909 admin-form-image-preivew-1.4/sample_usage/initsql/fixtures/
--rw-rw-r--   0 sami      (1000) sami      (1000)     1165 2023-04-10 12:21:32.000000 admin-form-image-preivew-1.4/sample_usage/initsql/fixtures/auth.json
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.747909 admin-form-image-preivew-1.4/sample_usage/initsql/management/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.767909 admin-form-image-preivew-1.4/sample_usage/initsql/management/commands/
--rwxrwxr-x   0 sami      (1000) sami      (1000)     1791 2023-04-10 08:05:37.000000 admin-form-image-preivew-1.4/sample_usage/initsql/management/commands/initsql.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.767909 admin-form-image-preivew-1.4/sample_usage/main_app/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 11:55:49.000000 admin-form-image-preivew-1.4/sample_usage/main_app/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:24:35.000000 admin-form-image-preivew-1.4/sample_usage/main_app/asgi.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     3453 2023-04-10 12:18:16.000000 admin-form-image-preivew-1.4/sample_usage/main_app/settings.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      814 2023-04-10 12:02:30.000000 admin-form-image-preivew-1.4/sample_usage/main_app/urls.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:25:37.000000 admin-form-image-preivew-1.4/sample_usage/main_app/wsgi.py
--rwxrwxr-x   0 sami      (1000) sami      (1000)      664 2023-04-08 06:24:26.000000 admin-form-image-preivew-1.4/sample_usage/manage.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.767909 admin-form-image-preivew-1.4/sample_usage/media/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-03 15:01:56.000000 admin-form-image-preivew-1.4/sample_usage/media/init.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)       56 2023-04-11 06:04:53.000000 admin-form-image-preivew-1.4/sample_usage/requirements.txt
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.771909 admin-form-image-preivew-1.4/sample_usage/sample_app/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 14:38:44.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-01 08:12:10.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/admin.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      151 2023-04-08 06:33:58.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/apps.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.771909 admin-form-image-preivew-1.4/sample_usage/sample_app/migrations/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/migrations/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      194 2023-04-01 08:46:06.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/models.py
--rw-rw-r--   0 sami      (1000) sami      (1000)       60 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/tests.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      191 2023-04-01 08:08:31.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/urls.py
--rw-rw-r--   0 sami      (1000) sami      (1000)       63 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.4/sample_usage/sample_app/views.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      144 2023-04-11 11:30:34.771909 admin-form-image-preivew-1.4/setup.cfg
--rwxrwxr-x   0 sami      (1000) sami      (1000)     1852 2023-04-11 06:00:12.000000 admin-form-image-preivew-1.4/setup.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:30:34.771909 admin-form-image-preivew-1.4/test/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.4/test/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-10 12:08:38.000000 admin-form-image-preivew-1.4/towncrier.toml
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.724178 admin-form-image-preivew-1.5/
+-rw-rw-r--   0 sami      (1000) sami      (1000)      419 2023-04-11 05:45:07.000000 admin-form-image-preivew-1.5/.gitignore
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.5/CHANGES.rst
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.5/LICENSE.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1911 2023-04-15 08:01:01.724178 admin-form-image-preivew-1.5/PKG-INFO
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1114 2023-04-11 11:29:43.000000 admin-form-image-preivew-1.5/README.md
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.708178 admin-form-image-preivew-1.5/admin_form_image_preivew/
+-rw-rw-r--   0 sami      (1000) sami      (1000)       22 2023-04-01 14:28:33.000000 admin-form-image-preivew-1.5/admin_form_image_preivew/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3845 2023-04-08 06:36:12.000000 admin-form-image-preivew-1.5/admin_form_image_preivew/settings.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      185 2023-04-01 14:28:25.000000 admin-form-image-preivew-1.5/admin_form_image_preivew/wsgi.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.712178 admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1911 2023-04-15 08:01:01.000000 admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/PKG-INFO
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1564 2023-04-15 08:01:01.000000 admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/SOURCES.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)        1 2023-04-15 08:01:01.000000 admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/dependency_links.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)      159 2023-04-15 08:01:01.000000 admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/requires.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)       20 2023-04-15 08:01:01.000000 admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/top_level.txt
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.712178 admin-form-image-preivew-1.5/admin_image_preview/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.5/admin_image_preview/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      168 2023-04-08 06:26:54.000000 admin-form-image-preivew-1.5/admin_image_preview/apps.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.712178 admin-form-image-preivew-1.5/admin_image_preview/migrations/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.5/admin_image_preview/migrations/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      293 2023-04-07 14:30:35.000000 admin-form-image-preivew-1.5/admin_image_preview/models.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1767 2023-04-10 12:09:04.000000 admin-form-image-preivew-1.5/admin_image_preview/readme.md
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.704178 admin-form-image-preivew-1.5/admin_image_preview/static/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.712178 admin-form-image-preivew-1.5/admin_image_preview/static/admin_image_preview/
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3872 2023-04-11 04:52:02.000000 admin-form-image-preivew-1.5/admin_image_preview/static/admin_image_preview/image_preview.js
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.704178 admin-form-image-preivew-1.5/admin_image_preview/templates/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.712178 admin-form-image-preivew-1.5/admin_image_preview/templates/admin/
+-rw-rw-r--   0 sami      (1000) sami      (1000)      213 2023-04-10 12:05:52.000000 admin-form-image-preivew-1.5/admin_image_preview/templates/admin/change_form.html
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3804 2023-04-10 08:30:05.000000 admin-form-image-preivew-1.5/admin_image_preview/templates/admin/original_change_form.html
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1113 2023-04-08 07:03:57.000000 admin-form-image-preivew-1.5/del.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.712178 admin-form-image-preivew-1.5/docs/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.5/docs/index.rst
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1348 2023-04-15 08:00:33.000000 admin-form-image-preivew-1.5/docs/make_pip.md
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1096 2023-04-10 12:10:33.000000 admin-form-image-preivew-1.5/pyproject.toml
+-rw-rw-r--   0 sami      (1000) sami      (1000)       72 2023-04-15 07:58:45.000000 admin-form-image-preivew-1.5/requirements.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)      230 2023-04-11 08:00:45.000000 admin-form-image-preivew-1.5/sample_pypirc_test.txt
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.716178 admin-form-image-preivew-1.5/sample_usage/
+-rw-r--r--   0 sami      (1000) sami      (1000)    90636 2023-04-01 08:16:18.000000 admin-form-image-preivew-1.5/sample_usage/92news-logo.png
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1121 2023-04-10 07:55:08.000000 admin-form-image-preivew-1.5/sample_usage/del.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1413 2023-04-11 11:30:17.000000 admin-form-image-preivew-1.5/sample_usage/fixtures.json
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.704178 admin-form-image-preivew-1.5/sample_usage/initsql/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.716178 admin-form-image-preivew-1.5/sample_usage/initsql/fixtures/
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1165 2023-04-10 12:21:32.000000 admin-form-image-preivew-1.5/sample_usage/initsql/fixtures/auth.json
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.704178 admin-form-image-preivew-1.5/sample_usage/initsql/management/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.716178 admin-form-image-preivew-1.5/sample_usage/initsql/management/commands/
+-rwxrwxr-x   0 sami      (1000) sami      (1000)     1791 2023-04-10 08:05:37.000000 admin-form-image-preivew-1.5/sample_usage/initsql/management/commands/initsql.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.720178 admin-form-image-preivew-1.5/sample_usage/main_app/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 11:55:49.000000 admin-form-image-preivew-1.5/sample_usage/main_app/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:24:35.000000 admin-form-image-preivew-1.5/sample_usage/main_app/asgi.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3453 2023-04-10 12:18:16.000000 admin-form-image-preivew-1.5/sample_usage/main_app/settings.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      814 2023-04-10 12:02:30.000000 admin-form-image-preivew-1.5/sample_usage/main_app/urls.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:25:37.000000 admin-form-image-preivew-1.5/sample_usage/main_app/wsgi.py
+-rwxrwxr-x   0 sami      (1000) sami      (1000)      664 2023-04-08 06:24:26.000000 admin-form-image-preivew-1.5/sample_usage/manage.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.720178 admin-form-image-preivew-1.5/sample_usage/media/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-03 15:01:56.000000 admin-form-image-preivew-1.5/sample_usage/media/init.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)       54 2023-04-15 07:59:39.000000 admin-form-image-preivew-1.5/sample_usage/requirements.txt
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.720178 admin-form-image-preivew-1.5/sample_usage/sample_app/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 14:38:44.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-01 08:12:10.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/admin.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      151 2023-04-08 06:33:58.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/apps.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.720178 admin-form-image-preivew-1.5/sample_usage/sample_app/migrations/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/migrations/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      194 2023-04-01 08:46:06.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/models.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)       60 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/tests.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      191 2023-04-01 08:08:31.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/urls.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)       63 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.5/sample_usage/sample_app/views.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      144 2023-04-15 08:01:01.724178 admin-form-image-preivew-1.5/setup.cfg
+-rwxrwxr-x   0 sami      (1000) sami      (1000)     1852 2023-04-15 07:58:45.000000 admin-form-image-preivew-1.5/setup.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-15 08:01:01.724178 admin-form-image-preivew-1.5/test/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.5/test/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-10 12:08:38.000000 admin-form-image-preivew-1.5/towncrier.toml
```

### Comparing `admin-form-image-preivew-1.4/PKG-INFO` & `admin-form-image-preivew-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin-form-image-preivew
-Version: 1.4
+Version: 1.5
 Summary: Sami Test Pip
 Home-page: https://github.com/humblesami/admin_form_image_preivew.git
 Author: Sami Akram
 Author-email: Sami Akram <samiakram@live.com>
 Maintainer-email: Sami Akram <samiakram@live.com>
 Project-URL: Changelog, https://github.com/humblesami/admin_form_image_preivew/CHANGES.rst
 Project-URL: Code, https://github.com/humblesami/admin_form_image_preivew
```

### Comparing `admin-form-image-preivew-1.4/README.md` & `admin-form-image-preivew-1.5/README.md`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/admin_form_image_preivew/settings.py` & `admin-form-image-preivew-1.5/admin_form_image_preivew/settings.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/PKG-INFO` & `admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin-form-image-preivew
-Version: 1.4
+Version: 1.5
 Summary: Sami Test Pip
 Home-page: https://github.com/humblesami/admin_form_image_preivew.git
 Author: Sami Akram
 Author-email: Sami Akram <samiakram@live.com>
 Maintainer-email: Sami Akram <samiakram@live.com>
 Project-URL: Changelog, https://github.com/humblesami/admin_form_image_preivew/CHANGES.rst
 Project-URL: Code, https://github.com/humblesami/admin_form_image_preivew
```

### Comparing `admin-form-image-preivew-1.4/admin_form_image_preivew.egg-info/SOURCES.txt` & `admin-form-image-preivew-1.5/admin_form_image_preivew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/admin_image_preview/readme.md` & `admin-form-image-preivew-1.5/admin_image_preview/readme.md`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/admin_image_preview/static/admin_image_preview/image_preview.js` & `admin-form-image-preivew-1.5/admin_image_preview/static/admin_image_preview/image_preview.js`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/admin_image_preview/templates/admin/original_change_form.html` & `admin-form-image-preivew-1.5/admin_image_preview/templates/admin/original_change_form.html`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/del.py` & `admin-form-image-preivew-1.5/del.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/docs/make_pip.md` & `admin-form-image-preivew-1.5/docs/make_pip.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 `sudo apt-get install twine`
 
 6. Make your build
 
     `rm -r dist/*`
     `rm -r build/*`
     `python setup.py clean --all`
-    `python setup.py sdist bdist_wheel -v=1.4`
+    `python setup.py sdist bdist_wheel -v=1.5`
 
 **Install and test locally**
 `pip uninstall admin-form-image-preivew`
-`pip install dist/your_module_name-1.4-py3-none-any.whl`
+`pip install dist/your_module_name-1.5-py3-none-any.whl`
 
 
 **Upload your pip**
 
 https://twine.readthedocs.io/en/stable/
 
 `pip install twine`
```

### Comparing `admin-form-image-preivew-1.4/pyproject.toml` & `admin-form-image-preivew-1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/92news-logo.png` & `admin-form-image-preivew-1.5/sample_usage/92news-logo.png`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/del.py` & `admin-form-image-preivew-1.5/sample_usage/del.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/fixtures.json` & `admin-form-image-preivew-1.5/sample_usage/fixtures.json`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/initsql/fixtures/auth.json` & `admin-form-image-preivew-1.5/sample_usage/initsql/fixtures/auth.json`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/initsql/management/commands/initsql.py` & `admin-form-image-preivew-1.5/sample_usage/initsql/management/commands/initsql.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/main_app/settings.py` & `admin-form-image-preivew-1.5/sample_usage/main_app/settings.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/main_app/urls.py` & `admin-form-image-preivew-1.5/sample_usage/main_app/urls.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/sample_usage/manage.py` & `admin-form-image-preivew-1.5/sample_usage/manage.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.4/setup.py` & `admin-form-image-preivew-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from setuptools import find_namespace_packages, setup
 
 def main(vv):
 
     install_requires = [
         "Django>=3",
-        "Pillow>=9"
+        "Pillow>=8"
     ]
 
     deploy_requires = [
         "bump2version",
         "readme_renderer[md]",
         "git-changelog",
     ]
```

