# Comparing `tmp/DjangoKit-0.9.tar.gz` & `tmp/DjangoKit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DjangoKit-0.9.tar", last modified: Sun Feb 20 03:13:29 2022, max compression
+gzip compressed data, was "DjangoKit-0.9.2.tar", last modified: Thu Jun  9 05:02:42 2022, max compression
```

## Comparing `DjangoKit-0.9.tar` & `DjangoKit-0.9.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.548840 DjangoKit-0.9/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       36 2019-12-21 02:47:41.000000 DjangoKit-0.9/AUTHORS
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      319 2019-12-23 03:07:43.000000 DjangoKit-0.9/CONTRIBUTING.rst
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.532840 DjangoKit-0.9/DjangoKit.egg-info/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3053 2022-02-20 03:13:29.000000 DjangoKit-0.9/DjangoKit.egg-info/PKG-INFO
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2056 2022-02-20 03:13:29.000000 DjangoKit-0.9/DjangoKit.egg-info/SOURCES.txt
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        1 2022-02-20 03:13:29.000000 DjangoKit-0.9/DjangoKit.egg-info/dependency_links.txt
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        1 2021-12-14 09:00:11.000000 DjangoKit-0.9/DjangoKit.egg-info/not-zip-safe
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      136 2022-02-20 03:13:29.000000 DjangoKit-0.9/DjangoKit.egg-info/requires.txt
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       10 2022-02-20 03:13:29.000000 DjangoKit-0.9/DjangoKit.egg-info/top_level.txt
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1519 2019-12-21 03:57:54.000000 DjangoKit-0.9/LICENSE
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      166 2021-09-21 07:26:14.000000 DjangoKit-0.9/MANIFEST.in
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3053 2022-02-20 03:13:29.548840 DjangoKit-0.9/PKG-INFO
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1131 2019-12-23 02:34:23.000000 DjangoKit-0.9/README.rst
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.532840 DjangoKit-0.9/djangokit/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      823 2022-02-20 03:10:36.000000 DjangoKit-0.9/djangokit/__init__.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.532840 DjangoKit-0.9/djangokit/access/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      296 2019-12-22 05:56:55.000000 DjangoKit-0.9/djangokit/access/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1006 2019-12-22 05:57:04.000000 DjangoKit-0.9/djangokit/access/decorators.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      913 2019-12-21 08:21:27.000000 DjangoKit-0.9/djangokit/access/functions.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.532840 DjangoKit-0.9/djangokit/db/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9/djangokit/db/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2206 2020-02-22 05:44:03.000000 DjangoKit-0.9/djangokit/db/mixins.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.532840 DjangoKit-0.9/djangokit/db/postgres/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9/djangokit/db/postgres/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      813 2020-09-21 01:05:25.000000 DjangoKit-0.9/djangokit/db/postgres/fields.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.536840 DjangoKit-0.9/djangokit/forms/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9/djangokit/forms/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      846 2020-02-16 11:29:42.000000 DjangoKit-0.9/djangokit/forms/iso.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      746 2020-09-21 01:04:22.000000 DjangoKit-0.9/djangokit/forms/postgres.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.536840 DjangoKit-0.9/djangokit/forms/widgets/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9/djangokit/forms/widgets/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2725 2019-12-23 08:33:06.000000 DjangoKit-0.9/djangokit/forms/widgets/selectize.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.528840 DjangoKit-0.9/djangokit/locale/
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.528840 DjangoKit-0.9/djangokit/locale/en/
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.536840 DjangoKit-0.9/djangokit/locale/en/LC_MESSAGES/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1403 2019-12-23 08:39:37.000000 DjangoKit-0.9/djangokit/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1822 2019-12-23 08:38:57.000000 DjangoKit-0.9/djangokit/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.528840 DjangoKit-0.9/djangokit/locale/ru/
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.536840 DjangoKit-0.9/djangokit/locale/ru/LC_MESSAGES/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1870 2019-12-23 08:39:37.000000 DjangoKit-0.9/djangokit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2295 2019-12-23 08:39:24.000000 DjangoKit-0.9/djangokit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.536840 DjangoKit-0.9/djangokit/logging/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       47 2020-05-28 02:00:24.000000 DjangoKit-0.9/djangokit/logging/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1096 2021-12-14 08:53:13.000000 DjangoKit-0.9/djangokit/logging/formatters.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.536840 DjangoKit-0.9/djangokit/management/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-04-18 12:11:41.000000 DjangoKit-0.9/djangokit/management/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1956 2019-12-22 06:19:40.000000 DjangoKit-0.9/djangokit/management/lock.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3043 2019-12-22 06:18:48.000000 DjangoKit-0.9/djangokit/management/log.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.540840 DjangoKit-0.9/djangokit/middleware/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 05:44:09.000000 DjangoKit-0.9/djangokit/middleware/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3867 2019-12-22 06:04:08.000000 DjangoKit-0.9/djangokit/middleware/access.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1532 2021-12-04 12:35:52.000000 DjangoKit-0.9/djangokit/middleware/sql.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3881 2019-12-22 06:00:39.000000 DjangoKit-0.9/djangokit/middleware/subdomains.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.540840 DjangoKit-0.9/djangokit/serializers/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       67 2019-12-22 06:05:06.000000 DjangoKit-0.9/djangokit/serializers/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     5844 2019-12-21 03:22:15.000000 DjangoKit-0.9/djangokit/serializers/objects.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.528840 DjangoKit-0.9/djangokit/templates/
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.528840 DjangoKit-0.9/djangokit/templates/djangokit/
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.540840 DjangoKit-0.9/djangokit/templates/djangokit/widgets/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      177 2019-11-28 23:49:16.000000 DjangoKit-0.9/djangokit/templates/djangokit/widgets/selectize.html
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      176 2019-12-09 08:37:44.000000 DjangoKit-0.9/djangokit/templates/djangokit/widgets/selectize_multiple.html
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.544840 DjangoKit-0.9/djangokit/templatetags/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9/djangokit/templatetags/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2733 2020-04-30 09:18:05.000000 DjangoKit-0.9/djangokit/templatetags/bootstrap4.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2890 2019-12-22 06:05:54.000000 DjangoKit-0.9/djangokit/templatetags/html.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      554 2021-01-25 04:51:17.000000 DjangoKit-0.9/djangokit/templatetags/json.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2768 2020-02-25 09:17:56.000000 DjangoKit-0.9/djangokit/templatetags/navigation.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      381 2019-12-22 06:05:28.000000 DjangoKit-0.9/djangokit/templatetags/os.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.544840 DjangoKit-0.9/djangokit/utils/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-22 02:18:27.000000 DjangoKit-0.9/djangokit/utils/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1717 2019-12-22 01:03:54.000000 DjangoKit-0.9/djangokit/utils/apps.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3166 2019-12-31 04:43:04.000000 DjangoKit-0.9/djangokit/utils/crypto.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     7063 2020-07-29 12:22:57.000000 DjangoKit-0.9/djangokit/utils/datetimes.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     5051 2019-12-22 03:09:04.000000 DjangoKit-0.9/djangokit/utils/deep.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2235 2019-12-21 04:57:28.000000 DjangoKit-0.9/djangokit/utils/encoders.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1006 2020-10-06 07:09:02.000000 DjangoKit-0.9/djangokit/utils/files.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1503 2021-11-10 11:35:10.000000 DjangoKit-0.9/djangokit/utils/images.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1945 2019-12-21 04:02:33.000000 DjangoKit-0.9/djangokit/utils/markdown.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     7948 2020-06-04 10:10:21.000000 DjangoKit-0.9/djangokit/utils/periods.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2484 2020-06-26 03:06:50.000000 DjangoKit-0.9/djangokit/utils/querysets.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1144 2019-12-21 06:21:47.000000 DjangoKit-0.9/djangokit/utils/requests.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      696 2019-12-22 03:28:35.000000 DjangoKit-0.9/djangokit/utils/responses.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     4454 2019-12-21 06:26:03.000000 DjangoKit-0.9/djangokit/utils/strings.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2484 2021-09-16 02:57:18.000000 DjangoKit-0.9/djangokit/utils/version.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2063 2019-12-23 02:45:12.000000 DjangoKit-0.9/djangokit/validators.py
-drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-02-20 03:13:29.544840 DjangoKit-0.9/djangokit/views/
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      130 2019-12-22 06:06:27.000000 DjangoKit-0.9/djangokit/views/__init__.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)    15603 2021-02-08 10:17:35.000000 DjangoKit-0.9/djangokit/views/controller.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     4726 2022-02-20 03:09:16.000000 DjangoKit-0.9/djangokit/views/decorators.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3126 2021-09-21 09:15:07.000000 DjangoKit-0.9/djangokit/views/logreader.py
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       32 2021-09-21 07:23:59.000000 DjangoKit-0.9/requirements-optional.txt
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       80 2021-12-07 02:55:13.000000 DjangoKit-0.9/requirements.txt
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       38 2022-02-20 03:13:29.548840 DjangoKit-0.9/setup.cfg
--rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2704 2021-09-21 11:36:24.000000 DjangoKit-0.9/setup.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.487903 DjangoKit-0.9.2/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       36 2019-12-21 02:47:41.000000 DjangoKit-0.9.2/AUTHORS
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      319 2019-12-23 03:07:43.000000 DjangoKit-0.9.2/CONTRIBUTING.rst
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/DjangoKit.egg-info/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3077 2022-06-09 05:02:42.000000 DjangoKit-0.9.2/DjangoKit.egg-info/PKG-INFO
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2056 2022-06-09 05:02:42.000000 DjangoKit-0.9.2/DjangoKit.egg-info/SOURCES.txt
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        1 2022-06-09 05:02:42.000000 DjangoKit-0.9.2/DjangoKit.egg-info/dependency_links.txt
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        1 2022-06-09 05:02:42.000000 DjangoKit-0.9.2/DjangoKit.egg-info/not-zip-safe
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      120 2022-06-09 05:02:42.000000 DjangoKit-0.9.2/DjangoKit.egg-info/requires.txt
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       10 2022-06-09 05:02:42.000000 DjangoKit-0.9.2/DjangoKit.egg-info/top_level.txt
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1519 2019-12-21 03:57:54.000000 DjangoKit-0.9.2/LICENSE
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      166 2021-09-21 07:26:14.000000 DjangoKit-0.9.2/MANIFEST.in
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3077 2022-06-09 05:02:42.487903 DjangoKit-0.9.2/PKG-INFO
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1131 2019-12-23 02:34:23.000000 DjangoKit-0.9.2/README.rst
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/djangokit/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      823 2022-06-09 04:59:46.000000 DjangoKit-0.9.2/djangokit/__init__.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/access/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      296 2019-12-22 05:56:55.000000 DjangoKit-0.9.2/djangokit/access/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1006 2019-12-22 05:57:04.000000 DjangoKit-0.9.2/djangokit/access/decorators.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      913 2019-12-21 08:21:27.000000 DjangoKit-0.9.2/djangokit/access/functions.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/db/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9.2/djangokit/db/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2206 2020-02-22 05:44:03.000000 DjangoKit-0.9.2/djangokit/db/mixins.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/db/postgres/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9.2/djangokit/db/postgres/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      813 2020-09-21 01:05:25.000000 DjangoKit-0.9.2/djangokit/db/postgres/fields.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/forms/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9.2/djangokit/forms/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      846 2020-02-16 11:29:42.000000 DjangoKit-0.9.2/djangokit/forms/iso.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      746 2020-09-21 01:04:22.000000 DjangoKit-0.9.2/djangokit/forms/postgres.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/forms/widgets/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9.2/djangokit/forms/widgets/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2725 2019-12-23 08:33:06.000000 DjangoKit-0.9.2/djangokit/forms/widgets/selectize.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/djangokit/locale/
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/djangokit/locale/en/
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/locale/en/LC_MESSAGES/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1403 2019-12-23 08:39:37.000000 DjangoKit-0.9.2/djangokit/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1822 2019-12-23 08:38:57.000000 DjangoKit-0.9.2/djangokit/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/djangokit/locale/ru/
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1870 2019-12-23 08:39:37.000000 DjangoKit-0.9.2/djangokit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2295 2019-12-23 08:39:24.000000 DjangoKit-0.9.2/djangokit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/logging/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       47 2020-05-28 02:00:24.000000 DjangoKit-0.9.2/djangokit/logging/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1096 2021-12-14 08:53:13.000000 DjangoKit-0.9.2/djangokit/logging/formatters.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/management/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-04-18 12:11:41.000000 DjangoKit-0.9.2/djangokit/management/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1956 2019-12-22 06:19:40.000000 DjangoKit-0.9.2/djangokit/management/lock.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3043 2019-12-22 06:18:48.000000 DjangoKit-0.9.2/djangokit/management/log.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/middleware/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 05:44:09.000000 DjangoKit-0.9.2/djangokit/middleware/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3867 2019-12-22 06:04:08.000000 DjangoKit-0.9.2/djangokit/middleware/access.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1551 2022-06-09 04:59:56.000000 DjangoKit-0.9.2/djangokit/middleware/sql.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3881 2019-12-22 06:00:39.000000 DjangoKit-0.9.2/djangokit/middleware/subdomains.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.479903 DjangoKit-0.9.2/djangokit/serializers/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       67 2019-12-22 06:05:06.000000 DjangoKit-0.9.2/djangokit/serializers/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     5844 2019-12-21 03:22:15.000000 DjangoKit-0.9.2/djangokit/serializers/objects.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/djangokit/templates/
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.475903 DjangoKit-0.9.2/djangokit/templates/djangokit/
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.483903 DjangoKit-0.9.2/djangokit/templates/djangokit/widgets/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      177 2019-11-28 23:49:16.000000 DjangoKit-0.9.2/djangokit/templates/djangokit/widgets/selectize.html
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      176 2019-12-09 08:37:44.000000 DjangoKit-0.9.2/djangokit/templates/djangokit/widgets/selectize_multiple.html
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.483903 DjangoKit-0.9.2/djangokit/templatetags/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-21 02:50:47.000000 DjangoKit-0.9.2/djangokit/templatetags/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2733 2020-04-30 09:18:05.000000 DjangoKit-0.9.2/djangokit/templatetags/bootstrap4.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2890 2019-12-22 06:05:54.000000 DjangoKit-0.9.2/djangokit/templatetags/html.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      554 2021-01-25 04:51:17.000000 DjangoKit-0.9.2/djangokit/templatetags/json.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2768 2020-02-25 09:17:56.000000 DjangoKit-0.9.2/djangokit/templatetags/navigation.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      381 2019-12-22 06:05:28.000000 DjangoKit-0.9.2/djangokit/templatetags/os.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.483903 DjangoKit-0.9.2/djangokit/utils/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)        0 2019-12-22 02:18:27.000000 DjangoKit-0.9.2/djangokit/utils/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1717 2019-12-22 01:03:54.000000 DjangoKit-0.9.2/djangokit/utils/apps.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3166 2019-12-31 04:43:04.000000 DjangoKit-0.9.2/djangokit/utils/crypto.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     7063 2020-07-29 12:22:57.000000 DjangoKit-0.9.2/djangokit/utils/datetimes.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     5051 2019-12-22 03:09:04.000000 DjangoKit-0.9.2/djangokit/utils/deep.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2235 2019-12-21 04:57:28.000000 DjangoKit-0.9.2/djangokit/utils/encoders.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1006 2020-10-06 07:09:02.000000 DjangoKit-0.9.2/djangokit/utils/files.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1503 2021-11-10 11:35:10.000000 DjangoKit-0.9.2/djangokit/utils/images.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1945 2019-12-21 04:02:33.000000 DjangoKit-0.9.2/djangokit/utils/markdown.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     7948 2020-06-04 10:10:21.000000 DjangoKit-0.9.2/djangokit/utils/periods.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2484 2020-06-26 03:06:50.000000 DjangoKit-0.9.2/djangokit/utils/querysets.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     1144 2019-12-21 06:21:47.000000 DjangoKit-0.9.2/djangokit/utils/requests.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      696 2019-12-22 03:28:35.000000 DjangoKit-0.9.2/djangokit/utils/responses.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     4454 2019-12-21 06:26:03.000000 DjangoKit-0.9.2/djangokit/utils/strings.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2484 2021-09-16 02:57:18.000000 DjangoKit-0.9.2/djangokit/utils/version.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2063 2019-12-23 02:45:12.000000 DjangoKit-0.9.2/djangokit/validators.py
+drwxr-xr-x   0 djbaldey  (1000) djbaldey  (1000)        0 2022-06-09 05:02:42.487903 DjangoKit-0.9.2/djangokit/views/
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)      130 2019-12-22 06:06:27.000000 DjangoKit-0.9.2/djangokit/views/__init__.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)    15603 2021-02-08 10:17:35.000000 DjangoKit-0.9.2/djangokit/views/controller.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     4726 2022-02-20 03:09:16.000000 DjangoKit-0.9.2/djangokit/views/decorators.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     3126 2021-09-21 09:15:07.000000 DjangoKit-0.9.2/djangokit/views/logreader.py
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       32 2021-09-21 07:23:59.000000 DjangoKit-0.9.2/requirements-optional.txt
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       80 2022-02-20 03:20:48.000000 DjangoKit-0.9.2/requirements.txt
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)       38 2022-06-09 05:02:42.487903 DjangoKit-0.9.2/setup.cfg
+-rw-r--r--   0 djbaldey  (1000) djbaldey  (1000)     2530 2022-02-20 03:36:43.000000 DjangoKit-0.9.2/setup.py
```

### Comparing `DjangoKit-0.9/DjangoKit.egg-info/PKG-INFO` & `DjangoKit-0.9.2/DjangoKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjangoKit
-Version: 0.9
+Version: 0.9.2
 Summary: DjangoKit is a set of extensions for Django.
 Home-page: https://gitlab.com/djbaldey/djangokit/
 Author: Grigoriy Kramarenko
 Author-email: root@rosix.ru
 License: BSD License
 Description: =========
         DjangoKit
@@ -66,16 +66,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
-Provides-Extra: markdown
-Provides-Extra: pygments
+Provides-Extra: full
```

### Comparing `DjangoKit-0.9/DjangoKit.egg-info/SOURCES.txt` & `DjangoKit-0.9.2/DjangoKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/LICENSE` & `DjangoKit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/PKG-INFO` & `DjangoKit-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjangoKit
-Version: 0.9
+Version: 0.9.2
 Summary: DjangoKit is a set of extensions for Django.
 Home-page: https://gitlab.com/djbaldey/djangokit/
 Author: Grigoriy Kramarenko
 Author-email: root@rosix.ru
 License: BSD License
 Description: =========
         DjangoKit
@@ -66,16 +66,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
-Provides-Extra: markdown
-Provides-Extra: pygments
+Provides-Extra: full
```

### Comparing `DjangoKit-0.9/README.rst` & `DjangoKit-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/__init__.py` & `DjangoKit-0.9.2/djangokit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # The version (X, Y, Z, R, N) builds by next rules:
 # Variables X, Y, Z & N must be integers. R - can be 'alpha', 'beta' 'rc' or
 # 'final' string. R == 'alpha' and N > 0 it is pre-alpha release.
 # version = X.Y[.Z]
 # subversion = .devN - for pre-alpha releases
 #            | {a|b|c}N - for 'alpha', 'beta' and 'rc' releases
 # subversion is not exists for 'final' release.
-VERSION = (0, 9, 0, 'final', 0)
+VERSION = (0, 9, 2, 'final', 0)
 
 
 def get_version():
     path = os.path.dirname(os.path.abspath(__file__))
     return version.get_version(VERSION, path)
```

### Comparing `DjangoKit-0.9/djangokit/access/decorators.py` & `DjangoKit-0.9.2/djangokit/access/decorators.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/access/functions.py` & `DjangoKit-0.9.2/djangokit/access/functions.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/db/mixins.py` & `DjangoKit-0.9.2/djangokit/db/mixins.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/db/postgres/fields.py` & `DjangoKit-0.9.2/djangokit/db/postgres/fields.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/forms/iso.py` & `DjangoKit-0.9.2/djangokit/forms/iso.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/forms/postgres.py` & `DjangoKit-0.9.2/djangokit/forms/postgres.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/forms/widgets/selectize.py` & `DjangoKit-0.9.2/djangokit/forms/widgets/selectize.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/locale/en/LC_MESSAGES/django.mo` & `DjangoKit-0.9.2/djangokit/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/locale/en/LC_MESSAGES/django.po` & `DjangoKit-0.9.2/djangokit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/locale/ru/LC_MESSAGES/django.mo` & `DjangoKit-0.9.2/djangokit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/locale/ru/LC_MESSAGES/django.po` & `DjangoKit-0.9.2/djangokit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/logging/formatters.py` & `DjangoKit-0.9.2/djangokit/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/management/lock.py` & `DjangoKit-0.9.2/djangokit/management/lock.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/management/log.py` & `DjangoKit-0.9.2/djangokit/management/log.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/middleware/access.py` & `DjangoKit-0.9.2/djangokit/middleware/access.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/middleware/sql.py` & `DjangoKit-0.9.2/djangokit/middleware/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 # Copyright (c) 2021, Grigoriy Kramarenko
 # All rights reserved.
 # This file is distributed under the BSD 3-Clause License.
 #
 import logging
 from sqlparse import format
-from time import time
 
 from django.conf import settings
 from django.db import connection, reset_queries
 
 
 def logging_queries(get_response):
     """
@@ -22,35 +21,36 @@
     def pretty_sql(sql):
         return format(sql, reindent=REINDENT, keyword_case='upper')
 
     def middleware(request):
         if settings.DEBUG:
             reset_queries()
             start_queries = len(connection.queries)
-            start_time = time()
 
             response = get_response(request)
 
-            end_time = time()
             end_queries = len(connection.queries)
 
-            queries = ''
+            queries = []
+            total_time = 0
             for i, query in enumerate(connection.queries):
-                queries += (
-                    f"\nQUERY #{i + 1}. {query['time']} seconds:\n"
-                    f"{pretty_sql(query['sql'])}\n"
+                time = query['time']
+                total_time += float(time)
+                queries.append(
+                    f"QUERY #{i + 1}. {time} seconds:\n"
+                    f"{pretty_sql(query['sql'])}"
                 )
 
             logger.debug(
-                '%s %s -- %d database queries at %f seconds. %s',
+                '%s %s -- %d database queries at %f seconds.\n\n%s\n',
                 request.method,
                 request.path,
                 end_queries - start_queries,
-                end_time - start_time,
-                queries
+                total_time,
+                '\n\n'.join(queries)
             )
         else:
             response = get_response(request)
 
         return response
 
     return middleware
```

### Comparing `DjangoKit-0.9/djangokit/middleware/subdomains.py` & `DjangoKit-0.9.2/djangokit/middleware/subdomains.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/serializers/objects.py` & `DjangoKit-0.9.2/djangokit/serializers/objects.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/templatetags/bootstrap4.py` & `DjangoKit-0.9.2/djangokit/templatetags/bootstrap4.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/templatetags/html.py` & `DjangoKit-0.9.2/djangokit/templatetags/html.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/templatetags/json.py` & `DjangoKit-0.9.2/djangokit/templatetags/json.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/templatetags/navigation.py` & `DjangoKit-0.9.2/djangokit/templatetags/navigation.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/apps.py` & `DjangoKit-0.9.2/djangokit/utils/apps.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/crypto.py` & `DjangoKit-0.9.2/djangokit/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/datetimes.py` & `DjangoKit-0.9.2/djangokit/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/deep.py` & `DjangoKit-0.9.2/djangokit/utils/deep.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/encoders.py` & `DjangoKit-0.9.2/djangokit/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/files.py` & `DjangoKit-0.9.2/djangokit/utils/files.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/images.py` & `DjangoKit-0.9.2/djangokit/utils/images.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/markdown.py` & `DjangoKit-0.9.2/djangokit/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/periods.py` & `DjangoKit-0.9.2/djangokit/utils/periods.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/querysets.py` & `DjangoKit-0.9.2/djangokit/utils/querysets.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/requests.py` & `DjangoKit-0.9.2/djangokit/utils/requests.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/responses.py` & `DjangoKit-0.9.2/djangokit/utils/responses.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/strings.py` & `DjangoKit-0.9.2/djangokit/utils/strings.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/utils/version.py` & `DjangoKit-0.9.2/djangokit/utils/version.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/validators.py` & `DjangoKit-0.9.2/djangokit/validators.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/views/controller.py` & `DjangoKit-0.9.2/djangokit/views/controller.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/views/decorators.py` & `DjangoKit-0.9.2/djangokit/views/decorators.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/djangokit/views/logreader.py` & `DjangoKit-0.9.2/djangokit/views/logreader.py`

 * *Files identical despite different names*

### Comparing `DjangoKit-0.9/setup.py` & `DjangoKit-0.9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,37 +20,29 @@
 with open('requirements-optional.txt') as f:
     optional_requirements = [
         line.split('#', 1)[0].strip() for line in f.read().splitlines()
         if not line.strip().startswith('#')
     ]
 
 
-def option(package):
-    for line in optional_requirements:
-        if line.startswith(package):
-            return line
-    raise ValueError('Package %r not found.' % package)
-
-
 setup(
     name="DjangoKit",
     version=version,
     author="Grigoriy Kramarenko",
     author_email="root@rosix.ru",
     description=("DjangoKit is a set of extensions for Django."),
     long_description=long_description,
     url="https://gitlab.com/djbaldey/djangokit/",
     license="BSD License",
     zip_safe=False,
     packages=['djangokit'],
     include_package_data=True,
     install_requires=requirements,
     extras_require={
-        'markdown': [option('markdown')],
-        'pygments': [option('pygments')],
+        'full': optional_requirements,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
@@ -65,14 +57,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

