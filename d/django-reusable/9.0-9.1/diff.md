# Comparing `tmp/django-reusable-9.0.tar.gz` & `tmp/django-reusable-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-reusable-9.0.tar", last modified: Fri Apr  7 23:28:55 2023, max compression
+gzip compressed data, was "dist/django-reusable-9.1.tar", last modified: Fri Apr 14 22:43:26 2023, max compression
```

## Comparing `django-reusable-9.0.tar` & `django-reusable-9.1.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/
--rw-r--r--   0 narangwa   (501) staff       (20)       90 2022-04-27 23:42:19.000000 django-reusable-9.0/AUTHORS
--rw-r--r--   0 narangwa   (501) staff       (20)     2952 2022-04-27 23:43:03.000000 django-reusable-9.0/COPYING
--rw-r--r--   0 narangwa   (501) staff       (20)      121 2022-06-29 20:32:10.000000 django-reusable-9.0/MANIFEST.in
--rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 23:28:55.000000 django-reusable-9.0/PKG-INFO
--rw-r--r--   0 narangwa   (501) staff       (20)      399 2022-05-12 17:29:25.000000 django-reusable-9.0/README.md
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/
--rw-r--r--   0 narangwa   (501) staff       (20)      397 2022-09-19 22:17:44.000000 django-reusable-9.0/django_reusable/__init__.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:06:59.000000 django-reusable-9.0/django_reusable/admin/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1830 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/admin/actions.py
--rw-r--r--   0 narangwa   (501) staff       (20)      613 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/admin/filters.py
--rw-r--r--   0 narangwa   (501) staff       (20)    16960 2023-04-07 23:27:24.000000 django-reusable-9.0/django_reusable/admin/mixins.py
--rw-r--r--   0 narangwa   (501) staff       (20)     5061 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/admin/suit_multi_admin.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-19 22:30:31.000000 django-reusable-9.0/django_reusable/admin/theme.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1820 2022-12-06 18:45:43.000000 django-reusable-9.0/django_reusable/admin/urls.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1136 2022-09-19 20:52:12.000000 django-reusable-9.0/django_reusable/admin/utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)      120 2022-12-21 20:19:38.000000 django-reusable-9.0/django_reusable/constants.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/db/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:18:47.000000 django-reusable-9.0/django_reusable/db/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      125 2023-02-09 20:02:21.000000 django-reusable-9.0/django_reusable/db/query.py
--rw-r--r--   0 narangwa   (501) staff       (20)      827 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/db/queryset.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/django_tables2/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-04-29 02:26:18.000000 django-reusable-9.0/django_reusable/django_tables2/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     4605 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/django_tables2/columns.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2713 2022-09-08 17:23:58.000000 django-reusable-9.0/django_reusable/django_tables2/table_mixins.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/error_tracker/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:09:01.000000 django-reusable-9.0/django_reusable/error_tracker/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)    12001 2022-09-08 21:34:35.000000 django-reusable-9.0/django_reusable/error_tracker/error_tracker.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2085 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/error_tracker/views.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/forms/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:25:55.000000 django-reusable-9.0/django_reusable/forms/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      313 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/forms/fields.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1489 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/forms/forms.py
--rw-r--r--   0 narangwa   (501) staff       (20)      802 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/forms/validators.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3609 2023-02-28 06:04:37.000000 django-reusable-9.0/django_reusable/forms/widgets.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/logging/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:20:29.000000 django-reusable-9.0/django_reusable/logging/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      977 2022-12-17 02:19:01.000000 django-reusable-9.0/django_reusable/logging/loggers.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/middleware/
--rw-r--r--   0 narangwa   (501) staff       (20)       26 2022-09-08 21:25:38.000000 django-reusable-9.0/django_reusable/middleware/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3383 2022-12-21 20:26:26.000000 django-reusable-9.0/django_reusable/middleware/middleware.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/migrations/
--rw-r--r--   0 narangwa   (501) staff       (20)      973 2022-06-29 20:33:31.000000 django-reusable-9.0/django_reusable/migrations/0001_initial.py
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-06-29 17:35:27.000000 django-reusable-9.0/django_reusable/migrations/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     7348 2023-01-08 22:06:09.000000 django-reusable-9.0/django_reusable/models.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)     1960 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/admin/overrides.css
--rw-r--r--   0 narangwa   (501) staff       (20)     1133 2022-09-19 22:23:56.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/admin/theme.css
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/js/
--rw-r--r--   0 narangwa   (501) staff       (20)     4589 2022-05-03 18:09:49.000000 django-reusable-9.0/django_reusable/static/django_reusable/js/dynamic-formsets.js
--rw-r--r--   0 narangwa   (501) staff       (20)     1542 2023-04-07 18:14:43.000000 django-reusable-9.0/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)      942 2022-09-19 21:46:11.000000 django-reusable-9.0/django_reusable/templates/admin/base.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/
--rw-r--r--   0 narangwa   (501) staff       (20)     2338 2022-05-17 23:13:44.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/add_wizard.pug
--rw-r--r--   0 narangwa   (501) staff       (20)     1561 2022-06-20 18:41:42.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/create_or_update.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      702 2022-04-17 01:16:14.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/delete.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      487 2022-09-19 21:02:31.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/index.pug
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/
--rw-r--r--   0 narangwa   (501) staff       (20)     1153 2022-05-17 23:09:53.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/formset.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      312 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      505 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/tabular-row.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      311 2022-05-17 23:09:58.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/tabular-table.pug
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/
--rwxr-xr-x   0 narangwa   (501) staff       (20)     3962 2022-11-27 21:01:44.000000 django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/detail.html
--rwxr-xr-x   0 narangwa   (501) staff       (20)     2663 2022-11-27 21:00:29.000000 django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/list.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/filters/
--rw-r--r--   0 narangwa   (501) staff       (20)      129 2022-07-05 21:52:13.000000 django-reusable-9.0/django_reusable/templates/django_reusable/filters/input-filter.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/
--rw-r--r--   0 narangwa   (501) staff       (20)      715 2019-10-14 17:10:39.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/table_form.html
--rw-r--r--   0 narangwa   (501) staff       (20)      727 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html
--rw-r--r--   0 narangwa   (501) staff       (20)      345 2019-10-14 17:10:39.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_header.html
--rw-r--r--   0 narangwa   (501) staff       (20)      593 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_row.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/tables/
--rw-r--r--   0 narangwa   (501) staff       (20)      867 2022-09-07 19:14:43.000000 django-reusable-9.0/django_reusable/templates/django_reusable/tables/enhanced-table.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templatetags/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2019-10-23 04:20:41.000000 django-reusable-9.0/django_reusable/templatetags/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2539 2022-09-19 22:13:59.000000 django-reusable-9.0/django_reusable/templatetags/template_helpers.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/urls/
--rw-r--r--   0 narangwa   (501) staff       (20)       20 2022-09-08 21:25:04.000000 django-reusable-9.0/django_reusable/urls/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      804 2022-12-21 20:19:38.000000 django-reusable-9.0/django_reusable/urls/urls.py
--rw-r--r--   0 narangwa   (501) staff       (20)      727 2022-12-22 00:17:21.000000 django-reusable-9.0/django_reusable/urls/utils.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/utils/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:28:04.000000 django-reusable-9.0/django_reusable/utils/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     4454 2023-02-20 01:44:34.000000 django-reusable-9.0/django_reusable/utils/date_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2472 2023-02-12 20:30:56.000000 django-reusable-9.0/django_reusable/utils/decorators.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1531 2023-02-01 18:37:30.000000 django-reusable-9.0/django_reusable/utils/export_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-08 20:57:31.000000 django-reusable-9.0/django_reusable/utils/file_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3609 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/utils/user_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)    16117 2023-02-28 06:04:05.000000 django-reusable-9.0/django_reusable/utils/utils.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/views/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-12-21 20:16:59.000000 django-reusable-9.0/django_reusable/views/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)    12338 2022-11-01 19:32:29.000000 django-reusable-9.0/django_reusable/views/mixins.py
--rw-r--r--   0 narangwa   (501) staff       (20)      718 2022-12-21 20:38:18.000000 django-reusable-9.0/django_reusable/views/views.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/
--rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 23:28:54.000000 django-reusable-9.0/django_reusable.egg-info/PKG-INFO
--rw-r--r--   0 narangwa   (501) staff       (20)     3263 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/SOURCES.txt
--rw-r--r--   0 narangwa   (501) staff       (20)        1 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/dependency_links.txt
--rw-r--r--   0 narangwa   (501) staff       (20)       62 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/requires.txt
--rw-r--r--   0 narangwa   (501) staff       (20)       16 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/top_level.txt
--rwxr-xr-x   0 narangwa   (501) staff       (20)      539 2022-06-29 20:32:34.000000 django-reusable-9.0/manage.py
--rw-r--r--   0 narangwa   (501) staff       (20)       38 2023-04-07 23:28:55.000000 django-reusable-9.0/setup.cfg
--rw-r--r--   0 narangwa   (501) staff       (20)     1483 2022-09-19 20:52:10.000000 django-reusable-9.0/setup.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/
+-rw-r--r--   0 narangwa   (501) staff       (20)       90 2022-04-27 23:42:19.000000 django-reusable-9.1/AUTHORS
+-rw-r--r--   0 narangwa   (501) staff       (20)     2952 2022-04-27 23:43:03.000000 django-reusable-9.1/COPYING
+-rw-r--r--   0 narangwa   (501) staff       (20)      121 2022-06-29 20:32:10.000000 django-reusable-9.1/MANIFEST.in
+-rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-14 22:43:26.000000 django-reusable-9.1/PKG-INFO
+-rw-r--r--   0 narangwa   (501) staff       (20)      399 2022-05-12 17:29:25.000000 django-reusable-9.1/README.md
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/
+-rw-r--r--   0 narangwa   (501) staff       (20)      397 2022-09-19 22:17:44.000000 django-reusable-9.1/django_reusable/__init__.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:06:59.000000 django-reusable-9.1/django_reusable/admin/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1830 2022-09-19 20:52:10.000000 django-reusable-9.1/django_reusable/admin/actions.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      613 2022-09-19 20:52:10.000000 django-reusable-9.1/django_reusable/admin/filters.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    17914 2023-04-14 22:38:30.000000 django-reusable-9.1/django_reusable/admin/mixins.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     5061 2022-09-19 20:52:10.000000 django-reusable-9.1/django_reusable/admin/suit_multi_admin.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-19 22:30:31.000000 django-reusable-9.1/django_reusable/admin/theme.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1820 2022-12-06 18:45:43.000000 django-reusable-9.1/django_reusable/admin/urls.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1136 2022-09-19 20:52:12.000000 django-reusable-9.1/django_reusable/admin/utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      120 2022-12-21 20:19:38.000000 django-reusable-9.1/django_reusable/constants.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/db/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:18:47.000000 django-reusable-9.1/django_reusable/db/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      125 2023-02-09 20:02:21.000000 django-reusable-9.1/django_reusable/db/query.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      827 2022-09-19 20:52:10.000000 django-reusable-9.1/django_reusable/db/queryset.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/django_tables2/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-04-29 02:26:18.000000 django-reusable-9.1/django_reusable/django_tables2/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     4605 2022-09-19 20:52:11.000000 django-reusable-9.1/django_reusable/django_tables2/columns.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2713 2022-09-08 17:23:58.000000 django-reusable-9.1/django_reusable/django_tables2/table_mixins.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/error_tracker/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:09:01.000000 django-reusable-9.1/django_reusable/error_tracker/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    12001 2022-09-08 21:34:35.000000 django-reusable-9.1/django_reusable/error_tracker/error_tracker.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2085 2022-09-19 20:52:11.000000 django-reusable-9.1/django_reusable/error_tracker/views.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/forms/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:25:55.000000 django-reusable-9.1/django_reusable/forms/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      313 2022-09-19 20:52:11.000000 django-reusable-9.1/django_reusable/forms/fields.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1489 2022-09-19 20:52:11.000000 django-reusable-9.1/django_reusable/forms/forms.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      802 2022-09-19 20:52:10.000000 django-reusable-9.1/django_reusable/forms/validators.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3609 2023-02-28 06:04:37.000000 django-reusable-9.1/django_reusable/forms/widgets.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/logging/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:20:29.000000 django-reusable-9.1/django_reusable/logging/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      977 2022-12-17 02:19:01.000000 django-reusable-9.1/django_reusable/logging/loggers.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/middleware/
+-rw-r--r--   0 narangwa   (501) staff       (20)       26 2022-09-08 21:25:38.000000 django-reusable-9.1/django_reusable/middleware/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3383 2022-12-21 20:26:26.000000 django-reusable-9.1/django_reusable/middleware/middleware.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/migrations/
+-rw-r--r--   0 narangwa   (501) staff       (20)      973 2022-06-29 20:33:31.000000 django-reusable-9.1/django_reusable/migrations/0001_initial.py
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-06-29 17:35:27.000000 django-reusable-9.1/django_reusable/migrations/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     7348 2023-01-08 22:06:09.000000 django-reusable-9.1/django_reusable/models.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/static/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/static/django_reusable/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/static/django_reusable/css/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/static/django_reusable/css/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1960 2022-09-19 20:52:10.000000 django-reusable-9.1/django_reusable/static/django_reusable/css/admin/overrides.css
+-rw-r--r--   0 narangwa   (501) staff       (20)     1133 2022-09-19 22:23:56.000000 django-reusable-9.1/django_reusable/static/django_reusable/css/admin/theme.css
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/static/django_reusable/js/
+-rw-r--r--   0 narangwa   (501) staff       (20)     4691 2023-04-07 23:35:21.000000 django-reusable-9.1/django_reusable/static/django_reusable/js/dynamic-formsets.js
+-rw-r--r--   0 narangwa   (501) staff       (20)     2619 2023-04-14 00:03:08.000000 django-reusable-9.1/django_reusable/static/django_reusable/js/enhanced-admin-inline.js
+-rw-r--r--   0 narangwa   (501) staff       (20)     2306 2023-04-14 22:37:54.000000 django-reusable-9.1/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)      942 2022-09-19 21:46:11.000000 django-reusable-9.1/django_reusable/templates/admin/base.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/crud/
+-rw-r--r--   0 narangwa   (501) staff       (20)     2338 2022-05-17 23:13:44.000000 django-reusable-9.1/django_reusable/templates/django_reusable/crud/add_wizard.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)     1561 2022-06-20 18:41:42.000000 django-reusable-9.1/django_reusable/templates/django_reusable/crud/create_or_update.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      702 2022-04-17 01:16:14.000000 django-reusable-9.1/django_reusable/templates/django_reusable/crud/delete.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      487 2022-09-19 21:02:31.000000 django-reusable-9.1/django_reusable/templates/django_reusable/crud/index.pug
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/dynamic-formset/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1153 2022-05-17 23:09:53.000000 django-reusable-9.1/django_reusable/templates/django_reusable/dynamic-formset/formset.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      312 2020-04-03 06:54:46.000000 django-reusable-9.1/django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      505 2020-04-03 06:54:46.000000 django-reusable-9.1/django_reusable/templates/django_reusable/dynamic-formset/tabular-row.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      311 2022-05-17 23:09:58.000000 django-reusable-9.1/django_reusable/templates/django_reusable/dynamic-formset/tabular-table.pug
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/error_tracker/
+-rwxr-xr-x   0 narangwa   (501) staff       (20)     3962 2022-11-27 21:01:44.000000 django-reusable-9.1/django_reusable/templates/django_reusable/error_tracker/detail.html
+-rwxr-xr-x   0 narangwa   (501) staff       (20)     2663 2022-11-27 21:00:29.000000 django-reusable-9.1/django_reusable/templates/django_reusable/error_tracker/list.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/filters/
+-rw-r--r--   0 narangwa   (501) staff       (20)      129 2022-07-05 21:52:13.000000 django-reusable-9.1/django_reusable/templates/django_reusable/filters/input-filter.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/forms/
+-rw-r--r--   0 narangwa   (501) staff       (20)      715 2019-10-14 17:10:39.000000 django-reusable-9.1/django_reusable/templates/django_reusable/forms/table_form.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      727 2020-04-03 06:54:46.000000 django-reusable-9.1/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      345 2019-10-14 17:10:39.000000 django-reusable-9.1/django_reusable/templates/django_reusable/forms/tabular_inline_header.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      593 2020-04-03 06:54:46.000000 django-reusable-9.1/django_reusable/templates/django_reusable/forms/tabular_inline_row.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templates/django_reusable/tables/
+-rw-r--r--   0 narangwa   (501) staff       (20)      867 2022-09-07 19:14:43.000000 django-reusable-9.1/django_reusable/templates/django_reusable/tables/enhanced-table.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/templatetags/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2019-10-23 04:20:41.000000 django-reusable-9.1/django_reusable/templatetags/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2539 2022-09-19 22:13:59.000000 django-reusable-9.1/django_reusable/templatetags/template_helpers.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/urls/
+-rw-r--r--   0 narangwa   (501) staff       (20)       20 2022-09-08 21:25:04.000000 django-reusable-9.1/django_reusable/urls/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      804 2022-12-21 20:19:38.000000 django-reusable-9.1/django_reusable/urls/urls.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      727 2022-12-22 00:17:21.000000 django-reusable-9.1/django_reusable/urls/utils.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/utils/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:28:04.000000 django-reusable-9.1/django_reusable/utils/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     4454 2023-02-20 01:44:34.000000 django-reusable-9.1/django_reusable/utils/date_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2472 2023-02-12 20:30:56.000000 django-reusable-9.1/django_reusable/utils/decorators.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1531 2023-02-01 18:37:30.000000 django-reusable-9.1/django_reusable/utils/export_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-08 20:57:31.000000 django-reusable-9.1/django_reusable/utils/file_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3609 2022-09-19 20:52:11.000000 django-reusable-9.1/django_reusable/utils/user_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    16120 2023-04-14 22:39:07.000000 django-reusable-9.1/django_reusable/utils/utils.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable/views/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-12-21 20:16:59.000000 django-reusable-9.1/django_reusable/views/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    12338 2022-11-01 19:32:29.000000 django-reusable-9.1/django_reusable/views/mixins.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      718 2022-12-21 20:38:18.000000 django-reusable-9.1/django_reusable/views/views.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable.egg-info/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-14 22:43:25.000000 django-reusable-9.1/django_reusable.egg-info/PKG-INFO
+-rw-r--r--   0 narangwa   (501) staff       (20)     3330 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable.egg-info/SOURCES.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)        1 2023-04-14 22:43:25.000000 django-reusable-9.1/django_reusable.egg-info/dependency_links.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)       62 2023-04-14 22:43:25.000000 django-reusable-9.1/django_reusable.egg-info/requires.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)       16 2023-04-14 22:43:26.000000 django-reusable-9.1/django_reusable.egg-info/top_level.txt
+-rwxr-xr-x   0 narangwa   (501) staff       (20)      539 2022-06-29 20:32:34.000000 django-reusable-9.1/manage.py
+-rw-r--r--   0 narangwa   (501) staff       (20)       38 2023-04-14 22:43:26.000000 django-reusable-9.1/setup.cfg
+-rw-r--r--   0 narangwa   (501) staff       (20)     1483 2022-09-19 20:52:10.000000 django-reusable-9.1/setup.py
```

### Comparing `django-reusable-9.0/COPYING` & `django-reusable-9.1/COPYING`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/PKG-INFO` & `django-reusable-9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reusable
-Version: 9.0
+Version: 9.1
 Summary: Agnostic and easy to use reusable library for django
 Home-page: https://github.com/navedr/django-reusable
 Author: Naved Rangwala
 Author-email: naved@ecarone.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-reusable-9.0/django_reusable/admin/actions.py` & `django-reusable-9.1/django_reusable/admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/admin/filters.py` & `django-reusable-9.1/django_reusable/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/admin/mixins.py` & `django-reusable-9.1/django_reusable/admin/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from copy import deepcopy
 
 from django.contrib import admin, messages
 from django.contrib.admin.options import BaseModelAdmin, InlineModelAdmin
 from django.core.exceptions import PermissionDenied
-from django.http import HttpResponseRedirect, JsonResponse
+from django.http import HttpResponseRedirect, JsonResponse, HttpResponse
 from django.shortcuts import redirect
 from django.urls import reverse, path
 from django.utils.safestring import mark_safe
 
 from django_reusable.admin.urls import ModelURLs
 from django_reusable.admin.utils import remove_from_fieldsets
 from django_reusable.admin.filters import SearchInFilter
 from django_reusable.constants import URLNames
 from django_reusable.forms.forms import EnhancedBaseInlineFormSet
-from django_reusable.utils import ifilter, CustomEncoder
+from django_reusable.utils import ifilter, CustomEncoder, find
 
 
 class EnhancedAdminInlineMixin(InlineModelAdmin):
+    """
+        Auto update template with all the extras and
+    """
+    auto_update_template = True
     select2_inlines_fields = []
     default_field_queryset = dict()
     limit_field_queryset_model_fields = dict()
     limit_saved_queryset_value_fields = []
     formset = EnhancedBaseInlineFormSet
 
     def get_formset(self, request, obj=None, **kwargs):
@@ -29,88 +33,90 @@
         formset.default_field_queryset = self.default_field_queryset
         formset.limit_field_queryset_model_fields = self.limit_field_queryset_model_fields
         return formset
 
     def formfield_for_dbfield(self, db_field, request, **kwargs):
         field = super().formfield_for_dbfield(db_field, request, **kwargs)
         if db_field.name in self.select2_inlines_fields:
-            field.widget.attrs['class'] = 'inline-select2'
+            field.widget.attrs['class'] = 'inline-select2' if not self.auto_update_template else 'dr-inline-select2'
         return field
 
+    @property
+    def media(self):
+        media = super().media
+        media._js.append('django_reusable/js/enhanced-admin-inline.js')
+        return media
+
 
 class EnhancedBaseAdminMixin(BaseModelAdmin):
     user_field = 'created_by'
     only_delete_owned = False
 
     def has_delete_permission(self, request, obj=None):
         if self.only_delete_owned and not request.user.has_perm('user.is_admin'):
             if not (obj and getattr(obj, self.user_field).id == request.user.id):
                 return False
-        return super(EnhancedBaseAdminMixin, self).has_delete_permission(request, obj)
+        return super().has_delete_permission(request, obj)
 
 
 class AjaxActionMixin:
-    admin_site = None
     """
         List of tuples:
         ('field_name', dict(btn_text, btn_class, additional_html, callback, short_desc))
     """
     ajax_action_fields = []
 
-    def get_readonly_fields(self, request, obj=None):
-        return list(super().get_readonly_fields(request, obj)) + [x[0] for x in self.get_ajax_action_fields()]
-
     def get_ajax_action_fields(self):
         return self.ajax_action_fields
 
     def get_callback_key(self, name):
         return f'{self.__class__.__name__}_{name}'
 
-    def register_callback(self, name, callback):
-        if not hasattr(self.admin_site, 'ajax_handler_callback_params'):
-            self.admin_site.ajax_handler_callback_params = {}
-        param_key = self.get_callback_key(name)
-        if not self.admin_site.ajax_handler_callback_params.get(param_key):
-            self.admin_site.ajax_handler_callback_params[param_key] = (self, callback)
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def ajax_action_callback(self, request, name, object_id=None):
+        match = find(lambda x: x[0] == name, self.get_ajax_action_fields())
+        if match:
+            config = match[1]
+            callback = config.get('callback')
+            if callback:
+                result = callback(self, request, object_id)
+                return HttpResponse(result)
+        return HttpResponse(f'no callback params defined for {name}')
 
+    def _create_ajax_actions_fn(self):
+        info = self.model._meta.app_label, self.model._meta.model_name
         for name, config in self.get_ajax_action_fields():
             btn_text = config.get('btn_text', 'Button')
             btn_class = config.get('btn_class', 'btn btn-warning')
 
             @mark_safe
             def func(instance):
-                if not instance.id:
-                    return ''
-                url = reverse(f'django_reusable:{URLNames.AJAX_CALLBACK_HANDLER}',
-                              args=(instance.pk, self.get_callback_key(name)))
-                return (f'<button class="{btn_class} ajax-action-btn" data-url="{url}">{btn_text}</button>' +
+                url = reverse('admin:%s_%s-dr-ajax-action' % info, args=(name, instance.id))
+                return (f'<button class="{btn_class} dr-ajax-action-btn" data-url="{url}">'
+                        f'{btn_text}</button>' +
                         config.get('additional_html', ''))
 
             func.short_description = config.get('short_desc', btn_text)
             func.__name__ = name
             setattr(self, func.__name__, func)
 
-            self.register_callback(name, config['callback'])
-
 
 class ExtraChangelistLinksMixin:
     """
         List of tuples:
         (url, dict(link_text, link_class, new_tab, user_passes_test))
     """
     extra_changelist_links = []
 
     def _get_applicable_extra_changelist_links(self, request):
         def _add_default_values(config):
-            config['link_class'] = config.get('link_class', 'btn-link')
-            config['link_text'] = config.get('link_text', 'Link')
-            config['new_tab'] = config.get('new_tab', False)
+            config.update(dict(
+                link_class=config.get('link_class', 'btn-link'),
+                link_text=config.get('link_text', 'Link'),
+                new_tab=config.get('new_tab', False)
+            ))
             return config
 
         return [(url, _add_default_values(config)) for (url, config) in self.get_extra_changelist_links(request)
                 if config.get('user_passes_test', lambda u: True)(request.user)]
 
     def _add_extra_changelist_links(self, request, extra_context):
         extra_context.update(
@@ -138,16 +144,18 @@
         List of tuples:
         ('name', dict(btn_text, btn_class, stay_on_page, callback, user_passes_test, pk_passes_test))
     """
     extra_change_form_buttons = []
 
     def _get_applicable_extra_change_form_buttons(self, request, pk):
         def _add_default_values(config):
-            config['btn_class'] = config.get('btn_class', 'btn-primary')
-            config['btn_text'] = config.get('btn_text', 'Button')
+            config.update(dict(
+                btn_class=config.get('btn_class', 'btn-primary'),
+                btn_text=config.get('btn_text', 'Button')
+            ))
             return config
 
         return [
             (name, _add_default_values(config)) for (name, config) in self.extra_change_form_buttons
             if (config.get('user_passes_test', lambda u: True)(request.user) and
                 config.get('pk_passes_test', lambda _pk: True)(pk))
         ]
@@ -182,54 +190,40 @@
             extra_submit_buttons=[
                 dict(name=name, config=config)
                 for (name, config) in self._get_applicable_extra_change_form_buttons(request, object_id)
             ]
         )
 
 
-class EnhancedAdminMixin(admin.ModelAdmin,
-                         EnhancedBaseAdminMixin,
-                         ExtraChangelistLinksMixin,
-                         ExtraChangeFormButtonsMixin):
-    """
-    Auto update template with all the extras and
-    """
-    auto_update_template = True
-    default_filters = []
-    search_in_choices = []
+class CustomFieldsMixin:
     """
         List of tuples:
         ('field_name', lambda instance: instance.field.name, optional short_desc)
     """
     custom_fields = []
-    """
-        List of tuples:
-        ('name', dict(btn_text, btn_class, callback, short_desc, custom_redirect))
-        Note: callback is called with args (instance)
-    """
-    action_links = []
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        if self.search_in_choices:
-            if not ifilter(lambda x: 'SearchInFilter' in str(x), self.list_filter):
-                filter_class = type('%sSearchInFilter' % self.__class__.__name__, (SearchInFilter,),
-                                    {'lookup_choices': sorted(self.search_in_choices, key=lambda x: x[1])})
-                self.list_filter.insert(0, filter_class)
-            self.base_search_fields = map(lambda xy: xy[0], self.search_in_choices)
 
+    def _create_custom_fields_fn(self):
         for f in self.custom_fields:
             func = f[1]
             func.allow_tags = True
             if len(f) > 2:
                 func.short_description = f[2]
             func.__name__ = f[0]
             setattr(self, func.__name__, func)
 
+
+class ActionLinksMixin:
+    """
+        List of tuples:
+        ('name', dict(btn_text, btn_class, callback, short_desc, custom_redirect))
+        Note: callback is called with args (instance)
+    """
+    action_links = []
+
+    def _create_action_links_fn(self):
         def get_action_link_fn(name, attrs):
             func = lambda instance: mark_safe(
                 '<a class="btn {0}" href="{1}">{2}</a>'.format(
                     attrs.get('btn_class', ''),
                     reverse(f'admin:{self.model._meta.app_label}_{self.model._meta.model_name}_action_view_{name}',
                             args=(instance.id,)),
                     attrs.get('btn_text', ''),
@@ -242,14 +236,44 @@
 
         for name, attrs in self.action_links:
             if 'callback' not in attrs:
                 continue
             func = get_action_link_fn(name, attrs)
             setattr(self, func.__name__, func)
 
+
+class EnhancedAdminMixin(admin.ModelAdmin,
+                         EnhancedBaseAdminMixin,
+                         ExtraChangelistLinksMixin,
+                         ExtraChangeFormButtonsMixin,
+                         AjaxActionMixin,
+                         CustomFieldsMixin,
+                         ActionLinksMixin):
+    """
+    Auto update template with all the extras and
+    """
+    auto_update_template = True
+    default_filters = []
+    search_in_choices = []
+
+    def _apply_search_in_choices(self):
+        if self.search_in_choices:
+            if not ifilter(lambda x: 'SearchInFilter' in str(x), self.list_filter):
+                filter_class = type('%sSearchInFilter' % self.__class__.__name__, (SearchInFilter,),
+                                    {'lookup_choices': sorted(self.search_in_choices, key=lambda x: x[1])})
+                self.list_filter.insert(0, filter_class)
+            self.base_search_fields = map(lambda xy: xy[0], self.search_in_choices)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._apply_search_in_choices()
+        self._create_custom_fields_fn()
+        self._create_action_links_fn()
+        self._create_ajax_actions_fn()
+
     def get_search_fields(self, request):
         search_fields = deepcopy(self.search_fields)
         if self.search_in_choices:
             search_fields = [request.GET.get(SearchInFilter.parameter_name)] if request.GET.get(
                 SearchInFilter.parameter_name) else (search_fields or self.base_search_fields)
         return search_fields
 
@@ -265,35 +289,40 @@
 
     def get_changelist_extra_context(self, request):
         return {}
 
     def custom_changelist_actions(self, request):
         pass
 
-    def changelist_view(self, request, extra_context=None):
-        extra_context = extra_context or {}
-        self.custom_changelist_actions(request)
-        if not self.auto_update_template:
-            self._add_extra_changelist_links(request, extra_context)
+    def _get_default_filters_redirect(self, request):
         if self.default_filters:
             try:
                 test = request.META['HTTP_REFERER'].split(request.META['PATH_INFO'])
                 if test and test[-1] and not test[-1].startswith('?'):
                     url = reverse('admin:%s_%s_changelist' % (self.opts.app_label, self.opts.model_name))
                     filters = []
                     for f in self.default_filters:
                         key = f.split('=')[0]
                         if key not in request.GET:
                             filters.append(f)
                     if filters:
                         return HttpResponseRedirect("%s?%s" % (url, "&".join(filters)))
             except:
                 pass
+
+    def changelist_view(self, request, extra_context=None):
+        extra_context = extra_context or {}
+        self.custom_changelist_actions(request)
+        if not self.auto_update_template:
+            self._add_extra_changelist_links(request, extra_context)
+        default_filters_redirect = self._get_default_filters_redirect(request)
+        if default_filters_redirect:
+            return default_filters_redirect
         extra_context.update(self.get_changelist_extra_context(request) or {})
-        return super(EnhancedAdminMixin, self).changelist_view(request, extra_context)
+        return super().changelist_view(request, extra_context)
 
     def change_view(self, request, object_id, form_url='', extra_context=None):
         extra_context = extra_context or {}
         if not self.auto_update_template:
             self._add_extra_change_form_buttons(request, object_id, extra_context)
             extra_context.update(
                 hide_save_buttons=self.hide_save_buttons(request, object_id)
@@ -315,15 +344,16 @@
         for inline in to_remove:
             if inline in inline_instances:
                 inline_instances.remove(inline)
 
     def get_readonly_fields(self, request, obj=None):
         return (list(super().get_readonly_fields(request, obj)) +
                 [x[0] for x in self.custom_fields] +
-                [x[0] for x in self.action_links])
+                [x[0] for x in self.action_links] +
+                [x[0] for x in self.get_ajax_action_fields()])
 
     def get_fieldset_section_exclusions(self, request, obj):
         return []
 
     def get_fieldset_field_exclusions(self, request, obj):
         return []
 
@@ -369,14 +399,17 @@
                  name='%s_%s-dr-admin-mixin-js-data_change' % info),
             path('add/dr-admin-mixin-js-data/',
                  self._change_form_mixin_js_data,
                  name='%s_%s-dr-admin-mixin-js-data_add' % info),
             path('dr-admin-mixin-js-data/',
                  self._changelist_mixin_js_data,
                  name='%s_%s_dr-admin-mixin-js-data-changelist' % info),
+            path('ajax-action/<path:name>/<path:object_id>/',
+                 self.ajax_action_callback,
+                 name='%s_%s-dr-ajax-action' % info),
         ]
 
         def get_action_link_view(_view_name, _attrs):
             def action_link_view(request, pk):
                 obj = self.model.objects.get(id=pk)
                 response = _attrs['callback'](obj)
                 if _attrs.get('custom_redirect'):
```

### Comparing `django-reusable-9.0/django_reusable/admin/suit_multi_admin.py` & `django-reusable-9.1/django_reusable/admin/suit_multi_admin.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/admin/theme.py` & `django-reusable-9.1/django_reusable/admin/theme.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/admin/urls.py` & `django-reusable-9.1/django_reusable/admin/urls.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/admin/utils.py` & `django-reusable-9.1/django_reusable/admin/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/db/queryset.py` & `django-reusable-9.1/django_reusable/db/queryset.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/django_tables2/columns.py` & `django-reusable-9.1/django_reusable/django_tables2/columns.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/django_tables2/table_mixins.py` & `django-reusable-9.1/django_reusable/django_tables2/table_mixins.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/error_tracker/error_tracker.py` & `django-reusable-9.1/django_reusable/error_tracker/error_tracker.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/error_tracker/views.py` & `django-reusable-9.1/django_reusable/error_tracker/views.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/forms/forms.py` & `django-reusable-9.1/django_reusable/forms/forms.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/forms/validators.py` & `django-reusable-9.1/django_reusable/forms/validators.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/forms/widgets.py` & `django-reusable-9.1/django_reusable/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/logging/loggers.py` & `django-reusable-9.1/django_reusable/logging/loggers.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/middleware/middleware.py` & `django-reusable-9.1/django_reusable/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/migrations/0001_initial.py` & `django-reusable-9.1/django_reusable/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/models.py` & `django-reusable-9.1/django_reusable/models.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/static/django_reusable/css/admin/overrides.css` & `django-reusable-9.1/django_reusable/static/django_reusable/css/admin/overrides.css`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/static/django_reusable/css/admin/theme.css` & `django-reusable-9.1/django_reusable/static/django_reusable/css/admin/theme.css`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/static/django_reusable/js/dynamic-formsets.js` & `django-reusable-9.1/django_reusable/static/django_reusable/js/dynamic-formsets.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,58 +1,57 @@
-const formClassName = '.dynamic-form-row';
-const formsContainer = '.formset-forms';
-const addBtnClassName = '.add-form-row';
-const removeBtnClassName = '.remove-form-row';
-const prefixAttrs = ['name', 'id', 'for'];
-const serialNoClassName = '.serial-no';
-const emptyFormDataAttr = '[data-empty-form]';
+const formClassName = ".dynamic-form-row";
+const formsContainer = ".formset-forms";
+const addBtnClassName = ".add-form-row";
+const removeBtnClassName = ".remove-form-row";
+const prefixAttrs = ["name", "id", "for"];
+const serialNoClassName = ".serial-no";
+const emptyFormDataAttr = "[data-empty-form]";
 
 (function($) {
-
     $.fn.extend({
         dynamicFormSet: function(options) {
             options = $.extend({}, $.DynamicFormSet.defaults, options);
 
             this.each(function() {
                 new $.DynamicFormSet(this, options);
             });
 
             return this;
-        }
+        },
     });
 
     // ctl is the element, options is the set of defaults + user options
     $.DynamicFormSet = function(ctl, options) {
         const $el = $(ctl);
         const $total = $(`#id_${options.prefix}-TOTAL_FORMS`);
 
         function bindEvents() {
-            $($el).on('click', addBtnClassName, function(e) {
+            $($el).on("click", addBtnClassName, function(e) {
                 e.preventDefault();
                 const total = parseInt($total.val());
                 if (total < options.maxNum) {
                     addForm();
                 }
                 e.stopPropagation();
                 return false;
             });
 
-            $($el).on('click', removeBtnClassName, function(e) {
+            $($el).on("click", removeBtnClassName, function(e) {
                 e.preventDefault();
                 deleteForm($(this));
                 e.stopPropagation();
                 return false;
             });
             toggleAddButton();
             limitDeleteButtons();
         }
 
         function updateElementIndex(el, ndx) {
-            const id_regex = new RegExp('(' + options.prefix + '-\\d+)');
-            const replacement = options.prefix + '-' + ndx;
+            const id_regex = new RegExp("(" + options.prefix + "-\\d+)");
+            const replacement = options.prefix + "-" + ndx;
             if ($(el).attr("for")) $(el).attr("for", $(el).attr("for").replace(id_regex, replacement));
             if (el.id) el.id = el.id.replace(id_regex, replacement);
             if (el.name) el.name = el.name.replace(id_regex, replacement);
         }
 
         function addForm() {
             const $form = $($el.find(emptyFormDataAttr).html().replace("<\\/script>", "</script>"));
@@ -63,54 +62,58 @@
             updateSerialNo();
             limitDeleteButtons();
             return false;
         }
 
         function updatedPrefixes($form) {
             const total = $total.val();
-            const prefixSelector = prefixAttrs.map(attr => `[${attr}*="__prefix__"]`).join(', ');
+            const prefixSelector = prefixAttrs.map(attr => `[${attr}*="__prefix__"]`).join(", ");
             const $prefixEl = $form.find(prefixSelector);
             $prefixEl.each((i, el) => {
                 const $pe = $(el);
                 prefixAttrs.forEach(attr => {
                     const value = $pe.attr(attr);
-                    if (value && value.match('__prefix__')) {
-                        $pe.attr(attr, value.replace('__prefix__', total));
+                    if (value && value.match("__prefix__")) {
+                        $pe.attr(attr, value.replace("__prefix__", total));
                     }
                 });
             });
-            $form.html($form.html().replace('__prefix__', total))
+            $form.html($form.html().replace("__prefix__", total));
         }
 
         function deleteForm(btn) {
             const total = parseInt($total.val());
             if (total > options.minNum) {
                 btn.closest(formClassName).remove();
                 const $forms = $el.find(formClassName);
                 $total.val($forms.length);
                 for (let i = 0, formCount = $forms.length; i < formCount; i++) {
-                    $($forms.get(i)).find(':input').each(function() {
-                        updateElementIndex(this, i);
-                    });
+                    $($forms.get(i))
+                        .find(":input")
+                        .each(function() {
+                            updateElementIndex(this, i);
+                        });
                 }
             }
             toggleAddButton();
             updateSerialNo();
             limitDeleteButtons();
             return false;
         }
 
         function toggleAddButton() {
             const total = parseInt($total.val());
-            $el.find(addBtnClassName).toggleClass('hide', total === options.maxNum);
+            $el.find(addBtnClassName).toggleClass("hide", total === options.maxNum);
         }
 
         function updateSerialNo() {
             $.each($el.find(formClassName), (i, el) => {
-                $(el).find(serialNoClassName).html(`# ${i + 1}`);
+                $(el)
+                    .find(serialNoClassName)
+                    .html(`# ${i + 1}`);
             });
         }
 
         function limitDeleteButtons() {
             if (options.minNum) {
                 $.each($el.find(formClassName), (i, el) => {
                     if (i < options.minNum) {
@@ -122,14 +125,13 @@
 
         bindEvents();
         return this;
     };
 
     // option defaults
     $.DynamicFormSet.defaults = {
-        prefix: 'form',
+        prefix: "form",
         minNum: undefined,
         maxNum: undefined,
-        canDelete: true
+        canDelete: true,
     };
-
 })(jQuery);
```

### Comparing `django-reusable-9.0/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js` & `django-reusable-9.1/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,58 +1,83 @@
 const EnhancedAdminMixin = {
-    init: function() {
+    init: function({
+        isChangelist,
+        isChangeForm
+    }) {
         $.ajax({
             url: `${location.pathname}dr-admin-mixin-js-data`,
             success: $.proxy(function(data) {
-                console.log(data)
                 if (!data.enabled) {
                     return;
                 }
-                if ($("#changelist").size()) {
+                $("body").addClass("enhanced-admin");
+                if (isChangelist) {
                     this.initChangelist(data);
-                } else if ($("body").hasClass("change-form")) {
+                } else if (isChangeForm) {
                     this.initChangeForm(data);
                 }
-            }, this)
-        })
+                this.handleAjaxFields();
+            }, this),
+        });
     },
     initChangelist: function(data) {
         data.extra_links.forEach(({
             url,
             config: {
                 link_class,
                 new_tab,
                 link_text
             }
         }) => {
             $("ul.breadcrumb").append(
                 `<li>
                     <span class="divider">|</span>
-                    <a href="${url}" class="btn ${link_class}" target="${new_tab ? '_blank' : ''}">${link_text}</a>
-                </li>`
-            )
+                    <a href="${url}" class="btn ${link_class}" target="${new_tab ? "_blank" : ""}">${link_text}</a>
+                </li>`,
+            );
         });
     },
     initChangeForm: function(data) {
         if (data.hide_save_buttons) {
             $(".submit-row").remove();
         } else {
             data.extra_submit_buttons.forEach(({
                 name,
                 config: {
                     btn_text,
                     btn_class
                 }
             }) => {
                 $(".submit-row").append(
-                    `<button name="__${name}" type="submit" class="btn ${btn_class}">${btn_text}</button>`
-                )
+                    `<button name="__${name}" type="submit" class="btn ${btn_class}">${btn_text}</button>`,
+                );
             });
         }
-    }
+    },
+    handleAjaxFields: function() {
+        $(".dr-ajax-action-btn").click(function(e) {
+            console.log($(e.currentTarget));
+            $.ajax({
+                url: $(e.currentTarget).data("url"),
+                success: function(response) {
+                    alert(response);
+                },
+                error: function(response) {
+                    console.log(response);
+                    alert("Error while performing this action!");
+                },
+            });
+            return false;
+        });
+    },
 };
 
 $(document).ready(function() {
-    if ($("#changelist").size() || $("body").hasClass("change-form")) {
-        EnhancedAdminMixin.init();
+    const isChangelist = !!$("#changelist").size();
+    const isChangeForm = $("body").hasClass("change-form");
+    if (isChangelist || isChangeForm) {
+        EnhancedAdminMixin.init({
+            isChangelist,
+            isChangeForm,
+        });
     }
 });
```

### Comparing `django-reusable-9.0/django_reusable/templates/admin/base.html` & `django-reusable-9.1/django_reusable/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/crud/add_wizard.pug` & `django-reusable-9.1/django_reusable/templates/django_reusable/crud/add_wizard.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/crud/create_or_update.pug` & `django-reusable-9.1/django_reusable/templates/django_reusable/crud/create_or_update.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/crud/delete.pug` & `django-reusable-9.1/django_reusable/templates/django_reusable/crud/delete.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/formset.pug` & `django-reusable-9.1/django_reusable/templates/django_reusable/dynamic-formset/formset.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/detail.html` & `django-reusable-9.1/django_reusable/templates/django_reusable/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/list.html` & `django-reusable-9.1/django_reusable/templates/django_reusable/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/forms/table_form.html` & `django-reusable-9.1/django_reusable/templates/django_reusable/forms/table_form.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html` & `django-reusable-9.1/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_row.html` & `django-reusable-9.1/django_reusable/templates/django_reusable/forms/tabular_inline_row.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templates/django_reusable/tables/enhanced-table.html` & `django-reusable-9.1/django_reusable/templates/django_reusable/tables/enhanced-table.html`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/templatetags/template_helpers.py` & `django-reusable-9.1/django_reusable/templatetags/template_helpers.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/urls/urls.py` & `django-reusable-9.1/django_reusable/urls/urls.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/urls/utils.py` & `django-reusable-9.1/django_reusable/urls/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/utils/date_utils.py` & `django-reusable-9.1/django_reusable/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/utils/decorators.py` & `django-reusable-9.1/django_reusable/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/utils/export_utils.py` & `django-reusable-9.1/django_reusable/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/utils/file_utils.py` & `django-reusable-9.1/django_reusable/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/utils/user_utils.py` & `django-reusable-9.1/django_reusable/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/utils/utils.py` & `django-reusable-9.1/django_reusable/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,13 +545,13 @@
 
 
 def omit(input_dict: dict, keys_to_omit: []):
     return dict((k, v) for (k, v) in input_dict.items() if k not in keys_to_omit)
 
 
 def find(fn, iterable):
-    filtered = imap(fn, iterable)
+    filtered = ifilter(fn, iterable)
     return filtered[0] if filtered else None
 
 
 def get_offset_range(minus=0, plus=0):
     return list(reversed([x*-1 for x in range(1, minus + 1)])) + [0] + list(range(1, plus + 1))
```

### Comparing `django-reusable-9.0/django_reusable/views/mixins.py` & `django-reusable-9.1/django_reusable/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable/views/views.py` & `django-reusable-9.1/django_reusable/views/views.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/django_reusable.egg-info/PKG-INFO` & `django-reusable-9.1/django_reusable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reusable
-Version: 9.0
+Version: 9.1
 Summary: Agnostic and easy to use reusable library for django
 Home-page: https://github.com/navedr/django-reusable
 Author: Naved Rangwala
 Author-email: naved@ecarone.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-reusable-9.0/django_reusable.egg-info/SOURCES.txt` & `django-reusable-9.1/django_reusable.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 django_reusable/middleware/__init__.py
 django_reusable/middleware/middleware.py
 django_reusable/migrations/0001_initial.py
 django_reusable/migrations/__init__.py
 django_reusable/static/django_reusable/css/admin/overrides.css
 django_reusable/static/django_reusable/css/admin/theme.css
 django_reusable/static/django_reusable/js/dynamic-formsets.js
+django_reusable/static/django_reusable/js/enhanced-admin-inline.js
 django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
 django_reusable/templates/admin/base.html
 django_reusable/templates/django_reusable/crud/add_wizard.pug
 django_reusable/templates/django_reusable/crud/create_or_update.pug
 django_reusable/templates/django_reusable/crud/delete.pug
 django_reusable/templates/django_reusable/crud/index.pug
 django_reusable/templates/django_reusable/dynamic-formset/formset.pug
```

### Comparing `django-reusable-9.0/manage.py` & `django-reusable-9.1/manage.py`

 * *Files identical despite different names*

### Comparing `django-reusable-9.0/setup.py` & `django-reusable-9.1/setup.py`

 * *Files identical despite different names*

