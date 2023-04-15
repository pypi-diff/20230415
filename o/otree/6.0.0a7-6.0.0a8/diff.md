# Comparing `tmp/otree-6.0.0a7.tar.gz` & `tmp/otree-6.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otree-6.0.0a7.tar", last modified: Sat Apr 15 17:23:48 2023, max compression
+gzip compressed data, was "otree-6.0.0a8.tar", last modified: Sat Apr 15 18:48:35 2023, max compression
```

## Comparing `otree-6.0.0a7.tar` & `otree-6.0.0a8.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.941174 otree-6.0.0a7/
--rw-rw-rw-   0        0        0     1573 2018-11-23 17:31:44.000000 otree-6.0.0a7/LICENSE
--rw-rw-rw-   0        0        0      390 2021-06-06 11:37:30.000000 otree-6.0.0a7/MANIFEST.in
--rw-rw-rw-   0        0        0     1886 2023-04-15 17:23:48.939239 otree-6.0.0a7/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2022-03-03 11:49:02.000000 otree-6.0.0a7/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.818191 otree-6.0.0a7/otree/
--rw-rw-rw-   0        0        0       91 2023-04-15 16:06:43.000000 otree-6.0.0a7/otree/__init__.py
--rw-rw-rw-   0        0        0      623 2023-04-15 17:12:04.000000 otree-6.0.0a7/otree/api.py
--rw-rw-rw-   0        0        0    10345 2023-04-15 17:17:20.000000 otree-6.0.0a7/otree/api.pyi
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.898122 otree-6.0.0a7/otree/app_template/
--rw-rw-rw-   0        0        0        0 2018-11-23 17:31:44.000000 otree-6.0.0a7/otree/app_template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.909266 otree-6.0.0a7/otree/app_template/__pycache__/
--rw-rw-rw-   0        0        0      127 2017-10-09 12:58:16.000000 otree-6.0.0a7/otree/app_template/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      131 2019-07-18 16:08:18.000000 otree-6.0.0a7/otree/app_template/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1013 2017-10-09 12:58:16.000000 otree-6.0.0a7/otree/app_template/__pycache__/models.cpython-36.pyc
--rw-rw-rw-   0        0        0     1017 2019-07-18 16:08:18.000000 otree-6.0.0a7/otree/app_template/__pycache__/models.cpython-37.pyc
--rw-rw-rw-   0        0        0      615 2017-10-09 12:58:16.000000 otree-6.0.0a7/otree/app_template/__pycache__/tests.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.920272 otree-6.0.0a7/otree/app_template/_builtin/
--rw-rw-rw-   0        0        0      446 2020-10-07 12:35:10.000000 otree-6.0.0a7/otree/app_template/_builtin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.925244 otree-6.0.0a7/otree/app_template/_builtin/__pycache__/
--rw-rw-rw-   0        0        0     1170 2017-10-09 12:58:16.000000 otree-6.0.0a7/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      871 2019-07-18 16:08:18.000000 otree-6.0.0a7/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      464 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/app_template/models.py
--rw-rw-rw-   0        0        0      297 2020-10-07 12:35:10.000000 otree-6.0.0a7/otree/app_template/pages.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.544660 otree-6.0.0a7/otree/app_template/templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.944128 otree-6.0.0a7/otree/app_template/templates/app_name/
--rw-rw-rw-   0        0        0      200 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/app_template/templates/app_name/MyPage.html
--rw-rw-rw-   0        0        0      180 2020-12-11 18:14:00.000000 otree-6.0.0a7/otree/app_template/templates/app_name/Results.html
--rw-rw-rw-   0        0        0      200 2020-03-20 01:44:18.000000 otree-6.0.0a7/otree/app_template/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.976483 otree-6.0.0a7/otree/app_template_lite/
--rw-rw-rw-   0        0        0      137 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/app_template_lite/MyPage.html
--rw-rw-rw-   0        0        0      119 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/app_template_lite/Results.html
--rw-rw-rw-   0        0        0      495 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/app_template_lite/__init__.py
--rw-rw-rw-   0        0        0     2888 2022-03-04 18:20:48.000000 otree-6.0.0a7/otree/asgi.py
--rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/auth.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.054483 otree-6.0.0a7/otree/bots/
--rw-rw-rw-   0        0        0       75 2020-03-20 01:44:18.000000 otree-6.0.0a7/otree/bots/__init__.py
--rw-rw-rw-   0        0        0    18278 2023-04-15 00:24:13.000000 otree-6.0.0a7/otree/bots/bot.py
--rw-rw-rw-   0        0        0     4815 2022-12-23 08:54:23.000000 otree-6.0.0a7/otree/bots/browser.py
--rw-rw-rw-   0        0        0    11868 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/bots/browser_launcher.py
--rw-rw-rw-   0        0        0     6713 2022-02-01 22:47:42.000000 otree-6.0.0a7/otree/bots/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.081932 otree-6.0.0a7/otree/channels/
--rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/channels/__init__.py
--rw-rw-rw-   0        0        0    27401 2023-03-24 17:39:59.000000 otree-6.0.0a7/otree/channels/consumers.py
--rw-rw-rw-   0        0        0      930 2023-03-24 17:39:59.000000 otree-6.0.0a7/otree/channels/routing.py
--rw-rw-rw-   0        0        0     4489 2023-03-24 17:39:59.000000 otree-6.0.0a7/otree/channels/utils.py
--rw-rw-rw-   0        0        0     2407 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/chat.py
--rw-rw-rw-   0        0        0    11062 2023-04-15 16:38:25.000000 otree-6.0.0a7/otree/checks.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.308998 otree-6.0.0a7/otree/cli/
--rw-rw-rw-   0        0        0        0 2021-09-07 01:38:00.000000 otree-6.0.0a7/otree/cli/__init__.py
--rw-rw-rw-   0        0        0      841 2021-06-29 10:07:36.000000 otree-6.0.0a7/otree/cli/base.py
--rw-rw-rw-   0        0        0     1846 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/bots.py
--rw-rw-rw-   0        0        0     1072 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/browser_bots.py
--rw-rw-rw-   0        0        0     1337 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/create_session.py
--rw-rw-rw-   0        0        0     3402 2021-09-28 08:02:58.000000 otree-6.0.0a7/otree/cli/devserver.py
--rw-rw-rw-   0        0        0     2051 2021-09-28 08:03:24.000000 otree-6.0.0a7/otree/cli/devserver_inner.py
--rw-rw-rw-   0        0        0       35 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/prodserver.py
--rw-rw-rw-   0        0        0     1766 2021-06-30 10:11:04.000000 otree-6.0.0a7/otree/cli/prodserver1of2.py
--rw-rw-rw-   0        0        0      258 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/prodserver2of2.py
--rw-rw-rw-   0        0        0    14172 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/cli/remove_self.py
--rw-rw-rw-   0        0        0     1981 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/resetdb.py
--rw-rw-rw-   0        0        0     1957 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/cli/startapp.py
--rw-rw-rw-   0        0        0     2796 2022-12-23 08:54:35.000000 otree-6.0.0a7/otree/cli/startproject.py
--rw-rw-rw-   0        0        0      345 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/timeoutsubprocess.py
--rw-rw-rw-   0        0        0     1224 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/cli/unzip.py
--rw-rw-rw-   0        0        0     2290 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/cli/upcase_constants.py
--rw-rw-rw-   0        0        0     7229 2021-06-30 09:55:02.000000 otree-6.0.0a7/otree/cli/update_my_code.py
--rw-rw-rw-   0        0        0     7301 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/cli/zip.py
--rw-rw-rw-   0        0        0     6434 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/cli/zipserver.py
--rw-rw-rw-   0        0        0     7803 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/common.py
--rw-rw-rw-   0        0        0     5217 2023-04-15 09:44:16.000000 otree-6.0.0a7/otree/common2.py
--rw-rw-rw-   0        0        0     2511 2022-11-23 14:41:17.000000 otree-6.0.0a7/otree/constants.py
--rw-rw-rw-   0        0        0     8663 2022-09-17 23:55:17.000000 otree-6.0.0a7/otree/currency.py
--rw-rw-rw-   0        0        0    30887 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/database.py
--rw-rw-rw-   0        0        0     8278 2022-03-04 18:20:48.000000 otree-6.0.0a7/otree/errorpage.py
--rw-rw-rw-   0        0        0    16209 2022-11-23 14:41:17.000000 otree-6.0.0a7/otree/export.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.340842 otree-6.0.0a7/otree/forms/
--rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/forms/__init__.py
--rw-rw-rw-   0        0        0     3620 2022-09-19 10:51:45.000000 otree-6.0.0a7/otree/forms/fields.py
--rw-rw-rw-   0        0        0    10547 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/forms/forms.py
--rw-rw-rw-   0        0        0     7446 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/forms/widgets.py
--rw-rw-rw-   0        0        0     6841 2022-09-19 10:51:45.000000 otree-6.0.0a7/otree/i18n.py
--rw-rw-rw-   0        0        0     3662 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/live.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.358827 otree-6.0.0a7/otree/locale/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.549000 otree-6.0.0a7/otree/locale/ar/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.377089 otree-6.0.0a7/otree/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1532 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/ar/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3986 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/ar/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      120 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/babel.ini
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.549356 otree-6.0.0a7/otree/locale/cs/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.399524 otree-6.0.0a7/otree/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1409 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/cs/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3712 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/cs/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.550460 otree-6.0.0a7/otree/locale/de/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.424495 otree-6.0.0a7/otree/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1762 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3875 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/de/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     3188 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/django.pot
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.551119 otree-6.0.0a7/otree/locale/es/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.450749 otree-6.0.0a7/otree/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1567 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.552263 otree-6.0.0a7/otree/locale/fi/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.475966 otree-6.0.0a7/otree/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      497 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/fi/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3114 2021-11-29 03:59:50.000000 otree-6.0.0a7/otree/locale/fi/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.552999 otree-6.0.0a7/otree/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.500057 otree-6.0.0a7/otree/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1634 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3747 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.554020 otree-6.0.0a7/otree/locale/he/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.518278 otree-6.0.0a7/otree/locale/he/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1652 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/he/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3703 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/he/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.554878 otree-6.0.0a7/otree/locale/hi/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.534645 otree-6.0.0a7/otree/locale/hi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2206 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/hi/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4254 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/hi/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.555558 otree-6.0.0a7/otree/locale/hu/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.550765 otree-6.0.0a7/otree/locale/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1722 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/hu/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3900 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/hu/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.556848 otree-6.0.0a7/otree/locale/id/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.564492 otree-6.0.0a7/otree/locale/id/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1520 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/locale/id/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3605 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/locale/id/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.557457 otree-6.0.0a7/otree/locale/it/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.589301 otree-6.0.0a7/otree/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1620 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/it/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3733 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/it/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.558412 otree-6.0.0a7/otree/locale/ja/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.609481 otree-6.0.0a7/otree/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1747 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3826 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/ja/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.559013 otree-6.0.0a7/otree/locale/ko/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.627784 otree-6.0.0a7/otree/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1783 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/ko/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3917 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/ko/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.560052 otree-6.0.0a7/otree/locale/nb/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.643653 otree-6.0.0a7/otree/locale/nb/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1023 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/nb/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3421 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/nb/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.560420 otree-6.0.0a7/otree/locale/nl/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.660231 otree-6.0.0a7/otree/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1579 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3669 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.561732 otree-6.0.0a7/otree/locale/pl/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.675304 otree-6.0.0a7/otree/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/pl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/pl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.562490 otree-6.0.0a7/otree/locale/pt/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.691223 otree-6.0.0a7/otree/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/pt/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/pt/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.563413 otree-6.0.0a7/otree/locale/ru/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.708095 otree-6.0.0a7/otree/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2047 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4156 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/ru/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.564171 otree-6.0.0a7/otree/locale/tr/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.721707 otree-6.0.0a7/otree/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1537 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/tr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3731 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/tr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.565018 otree-6.0.0a7/otree/locale/zh_Hans/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.738427 otree-6.0.0a7/otree/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1452 2022-04-27 15:07:46.000000 otree-6.0.0a7/otree/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3521 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     2323 2021-08-31 15:42:14.000000 otree-6.0.0a7/otree/lookup.py
--rw-rw-rw-   0        0        0     6971 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/main.py
--rw-rw-rw-   0        0        0     1819 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.817750 otree-6.0.0a7/otree/models/
--rw-rw-rw-   0        0        0      230 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/models/__init__.py
--rw-rw-rw-   0        0        0     4133 2021-11-18 17:14:02.000000 otree-6.0.0a7/otree/models/group.py
--rw-rw-rw-   0        0        0     8714 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/models/participant.py
--rw-rw-rw-   0        0        0     3346 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/models/player.py
--rw-rw-rw-   0        0        0     9750 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/models/session.py
--rw-rw-rw-   0        0        0     9025 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/models/subsession.py
--rw-rw-rw-   0        0        0     1929 2021-08-18 09:23:18.000000 otree-6.0.0a7/otree/models_concrete.py
--rw-rw-rw-   0        0        0     7383 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/mturk_client.py
--rw-rw-rw-   0        0        0     1897 2022-03-04 18:20:48.000000 otree-6.0.0a7/otree/patch.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.855607 otree-6.0.0a7/otree/project_template/
--rw-rw-rw-   0        0        0      133 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/project_template/.gitignore
--rw-rw-rw-   0        0        0       57 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/project_template/Procfile
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.566969 otree-6.0.0a7/otree/project_template/_static/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.856847 otree-6.0.0a7/otree/project_template/_static/global/
--rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/project_template/_static/global/empty.css
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.567598 otree-6.0.0a7/otree/project_template/_templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.864953 otree-6.0.0a7/otree/project_template/_templates/global/
--rw-rw-rw-   0        0        0      149 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/project_template/_templates/global/Page.html
--rw-rw-rw-   0        0        0      169 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/project_template/requirements.txt
--rw-rw-rw-   0        0        0     1018 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/project_template/settings.py
--rw-rw-rw-   0        0        0     2567 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/read_csv.py
--rw-rw-rw-   0        0        0     4291 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/room.py
--rw-rw-rw-   0        0        0    15047 2022-12-23 08:54:23.000000 otree-6.0.0a7/otree/session.py
--rw-rw-rw-   0        0        0     2380 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.875904 otree-6.0.0a7/otree/static/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.568514 otree-6.0.0a7/otree/static/bootstrap5/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.904463 otree-6.0.0a7/otree/static/bootstrap5/css/
--rw-rw-rw-   0        0        0   155637 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/bootstrap5/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   429472 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/bootstrap5/css/bootstrap.min.css.map
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.914986 otree-6.0.0a7/otree/static/bootstrap5/js/
--rw-rw-rw-   0        0        0    78754 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/bootstrap5/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   326390 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0      198 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.942640 otree-6.0.0a7/otree/static/glyphicons/
--rw-rw-rw-   0        0        0     1412 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/clock.png
--rw-rw-rw-   0        0        0     1307 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/cloud.png
--rw-rw-rw-   0        0        0     1443 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/cogwheel.png
--rw-rw-rw-   0        0        0     1310 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/delete.png
--rw-rw-rw-   0        0        0     1314 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/download-alt.png
--rw-rw-rw-   0        0        0     1475 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/eye-open.png
--rw-rw-rw-   0        0        0     1243 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/folder-closed.png
--rw-rw-rw-   0        0        0     1436 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/link.png
--rw-rw-rw-   0        0        0     1231 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/list-alt.png
--rw-rw-rw-   0        0        0     1342 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/pencil.png
--rw-rw-rw-   0        0        0     1218 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/plus.png
--rw-rw-rw-   0        0        0     1378 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/pushpin.png
--rw-rw-rw-   0        0        0     1471 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/refresh.png
--rw-rw-rw-   0        0        0     1499 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/stats.png
--rw-rw-rw-   0        0        0     1432 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/glyphicons/usd.png
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.570343 otree-6.0.0a7/otree/static/otree/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:47.950699 otree-6.0.0a7/otree/static/otree/css/
--rw-rw-rw-   0        0        0      868 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/otree/css/table.css
--rw-rw-rw-   0        0        0     2015 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/otree/css/theme.css
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.110403 otree-6.0.0a7/otree/static/otree/js/
--rw-rw-rw-   0        0        0     1909 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/static/otree/js/common.js
--rw-rw-rw-   0        0        0     1624 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/static/otree/js/formInputs.js
--rw-rw-rw-   0        0        0      504 2020-10-07 12:35:10.000000 otree-6.0.0a7/otree/static/otree/js/internet-explorer.js
--rw-rw-rw-   0        0        0    86663 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/otree/js/jquery-3.2.1.min.js
--rw-rw-rw-   0        0        0     6605 2020-11-23 22:42:18.000000 otree-6.0.0a7/otree/static/otree/js/jquery.color-2.1.2.min.js
--rw-rw-rw-   0        0        0     5360 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/otree/js/jquery.countdown.min.js
--rw-rw-rw-   0        0        0      702 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/otree/js/jquery.timeago.en-short.js
--rw-rw-rw-   0        0        0     7200 2018-12-27 12:55:56.000000 otree-6.0.0a7/otree/static/otree/js/jquery.timeago.js
--rw-rw-rw-   0        0        0      663 2023-03-24 17:39:59.000000 otree-6.0.0a7/otree/static/otree/js/live.js
--rw-rw-rw-   0        0        0     4271 2022-11-23 14:41:17.000000 otree-6.0.0a7/otree/static/otree/js/monitor2.js
--rw-rw-rw-   0        0        0    49322 2023-04-15 17:21:55.000000 otree-6.0.0a7/otree/static/otree/js/otree-front.js
--rw-rw-rw-   0        0        0      967 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/otree/js/page-websocket-redirect.js
--rw-rw-rw-   0        0        0     8729 2020-03-20 01:44:18.000000 otree-6.0.0a7/otree/static/otree/js/reconnecting-websocket-iife.min.js
--rw-rw-rw-   0        0        0     4837 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/static/otree/js/table-utils.js
--rw-rw-rw-   0        0        0      861 2023-04-15 16:01:01.000000 otree-6.0.0a7/otree/static/otree/js/trial-default.js
--rw-rw-rw-   0        0        0      221 2023-04-15 08:05:11.000000 otree-6.0.0a7/otree/static/otree/js/trial-setup.js
--rw-rw-rw-   0        0        0       26 2018-11-23 17:31:48.000000 otree-6.0.0a7/otree/static/robots.txt
--rw-rw-rw-   0        0        0     5360 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/tasks.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.571443 otree-6.0.0a7/otree/templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.130192 otree-6.0.0a7/otree/templates/global/
--rw-rw-rw-   0        0        0       33 2020-12-01 22:34:50.000000 otree-6.0.0a7/otree/templates/global/Base.html
--rw-rw-rw-   0        0        0      293 2021-10-18 21:34:16.000000 otree-6.0.0a7/otree/templates/global/Page.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.520864 otree-6.0.0a7/otree/templates/otree/
--rw-rw-rw-   0        0        0      881 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/AdminReport.html
--rw-rw-rw-   0        0        0     1768 2023-04-15 08:08:38.000000 otree-6.0.0a7/otree/templates/otree/Base.html
--rw-rw-rw-   0        0        0     3065 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/BaseAdmin.html
--rw-rw-rw-   0        0        0     2881 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/CreateDemoSession.html
--rw-rw-rw-   0        0        0      199 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/CreateSession.html
--rw-rw-rw-   0        0        0      955 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/DemoIndex.html
--rw-rw-rw-   0        0        0     5961 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templates/otree/Export.html
--rw-rw-rw-   0        0        0       31 2020-12-01 22:34:50.000000 otree-6.0.0a7/otree/templates/otree/FormPage.html
--rw-rw-rw-   0        0        0     1240 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/Login.html
--rw-rw-rw-   0        0        0     2796 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templates/otree/MTurkCreateHIT.html
--rw-rw-rw-   0        0        0     1214 2020-12-01 22:34:50.000000 otree-6.0.0a7/otree/templates/otree/MTurkHTMLQuestion.html
--rw-rw-rw-   0        0        0     6732 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templates/otree/MTurkSessionPayments.html
--rw-rw-rw-   0        0        0       18 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/OutOfRangeNotification.html
--rw-rw-rw-   0        0        0     3116 2023-04-15 17:20:30.000000 otree-6.0.0a7/otree/templates/otree/Page.html
--rw-rw-rw-   0        0        0      911 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/templates/otree/RoomInputLabel.html
--rw-rw-rw-   0        0        0      754 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/RoomWithSession.html
--rw-rw-rw-   0        0        0     4282 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/RoomWithoutSession.html
--rw-rw-rw-   0        0        0      353 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/Rooms.html
--rw-rw-rw-   0        0        0     1784 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templates/otree/ServerCheck.html
--rw-rw-rw-   0        0        0     2532 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/Session.html
--rw-rw-rw-   0        0        0     7856 2021-08-19 09:01:20.000000 otree-6.0.0a7/otree/templates/otree/SessionData.html
--rw-rw-rw-   0        0        0      139 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/SessionDescription.html
--rw-rw-rw-   0        0        0      323 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/SessionEditProperties.html
--rw-rw-rw-   0        0        0     2391 2022-11-23 14:41:17.000000 otree-6.0.0a7/otree/templates/otree/SessionMonitor.html
--rw-rw-rw-   0        0        0     1582 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/SessionPayments.html
--rw-rw-rw-   0        0        0     3329 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/SessionSplitScreen.html
--rw-rw-rw-   0        0        0     4087 2021-09-02 00:40:54.000000 otree-6.0.0a7/otree/templates/otree/SessionStartLinks.html
--rw-rw-rw-   0        0        0     5469 2022-05-14 06:42:33.000000 otree-6.0.0a7/otree/templates/otree/Sessions.html
--rw-rw-rw-   0        0        0     5121 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templates/otree/WaitPage.html
--rw-rw-rw-   0        0        0       37 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/WaitPageRoom.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.628783 otree-6.0.0a7/otree/templates/otree/includes/
--rw-rw-rw-   0        0        0     5461 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/CreateSessionForm.html
--rw-rw-rw-   0        0        0     1528 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/RoomParticipantLinks.html
--rw-rw-rw-   0        0        0      402 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/SessionInfo.html
--rw-rw-rw-   0        0        0      213 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/TimeLimit.html
--rw-rw-rw-   0        0        0      997 2022-07-06 11:50:24.000000 otree-6.0.0a7/otree/templates/otree/includes/TimeLimit.js.html
--rw-rw-rw-   0        0        0      969 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/debug_info.html
--rw-rw-rw-   0        0        0     2679 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templates/otree/includes/hidden_form_errors.html
--rw-rw-rw-   0        0        0      244 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/messages.html
--rw-rw-rw-   0        0        0     1368 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templates/otree/includes/mturk_payment_table.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.659203 otree-6.0.0a7/otree/templates/otree/tags/
--rw-rw-rw-   0        0        0     3572 2021-09-09 20:27:16.000000 otree-6.0.0a7/otree/templates/otree/tags/chat.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.797141 otree-6.0.0a7/otree/templating/
--rw-rw-rw-   0        0        0       70 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templating/__init__.py
--rw-rw-rw-   0        0        0     6993 2021-09-10 18:14:58.000000 otree-6.0.0a7/otree/templating/compiler.py
--rw-rw-rw-   0        0        0     2948 2021-09-23 22:55:28.000000 otree-6.0.0a7/otree/templating/context.py
--rw-rw-rw-   0        0        0     1342 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templating/errors.py
--rw-rw-rw-   0        0        0     2081 2021-08-11 02:49:06.000000 otree-6.0.0a7/otree/templating/filters.py
--rw-rw-rw-   0        0        0     3392 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/templating/loader.py
--rw-rw-rw-   0        0        0    33516 2023-04-15 08:53:48.000000 otree-6.0.0a7/otree/templating/nodes.py
--rw-rw-rw-   0        0        0     1495 2021-09-10 17:48:20.000000 otree-6.0.0a7/otree/templating/template.py
--rw-rw-rw-   0        0        0     1836 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/templating/utils.py
--rw-rw-rw-   0        0        0      173 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/test.py
--rw-rw-rw-   0        0        0     4683 2023-04-15 17:04:58.000000 otree-6.0.0a7/otree/trial.py
--rw-rw-rw-   0        0        0     1919 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/update.py
--rw-rw-rw-   0        0        0     4635 2023-03-24 17:39:59.000000 otree-6.0.0a7/otree/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:48.935331 otree-6.0.0a7/otree/views/
--rw-rw-rw-   0        0        0       49 2020-06-23 01:10:42.000000 otree-6.0.0a7/otree/views/__init__.py
--rw-rw-rw-   0        0        0    49935 2023-04-15 09:49:30.000000 otree-6.0.0a7/otree/views/abstract.py
--rw-rw-rw-   0        0        0    19290 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/views/admin.py
--rw-rw-rw-   0        0        0     8261 2022-03-03 11:49:02.000000 otree-6.0.0a7/otree/views/cbv.py
--rw-rw-rw-   0        0        0     1537 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/views/demo.py
--rw-rw-rw-   0        0        0     3722 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/views/export.py
--rw-rw-rw-   0        0        0    14856 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/views/mturk.py
--rw-rw-rw-   0        0        0    12981 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/views/participant.py
--rw-rw-rw-   0        0        0    10004 2023-03-08 18:09:53.000000 otree-6.0.0a7/otree/views/rest.py
--rw-rw-rw-   0        0        0     2523 2021-06-06 11:37:30.000000 otree-6.0.0a7/otree/views/room.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:23:46.863992 otree-6.0.0a7/otree.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-04-15 17:23:46.000000 otree-6.0.0a7/otree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8038 2023-04-15 17:23:46.000000 otree-6.0.0a7/otree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:23:46.000000 otree-6.0.0a7/otree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-15 17:23:46.000000 otree-6.0.0a7/otree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-11-22 05:26:26.000000 otree-6.0.0a7/otree.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      196 2023-04-15 17:23:46.000000 otree-6.0.0a7/otree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 17:23:46.000000 otree-6.0.0a7/otree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      311 2023-03-08 18:09:53.000000 otree-6.0.0a7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 17:23:48.941174 otree-6.0.0a7/setup.cfg
--rw-rw-rw-   0        0        0     2548 2023-03-08 18:09:53.000000 otree-6.0.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.311947 otree-6.0.0a8/
+-rw-rw-rw-   0        0        0     1573 2018-11-23 17:31:44.000000 otree-6.0.0a8/LICENSE
+-rw-rw-rw-   0        0        0      390 2021-06-06 11:37:30.000000 otree-6.0.0a8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1886 2023-04-15 18:48:35.311947 otree-6.0.0a8/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2022-03-03 11:49:02.000000 otree-6.0.0a8/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.075647 otree-6.0.0a8/otree/
+-rw-rw-rw-   0        0        0       91 2023-04-15 18:47:37.000000 otree-6.0.0a8/otree/__init__.py
+-rw-rw-rw-   0        0        0      634 2023-04-15 17:56:00.000000 otree-6.0.0a8/otree/api.py
+-rw-rw-rw-   0        0        0    10444 2023-04-15 18:05:39.000000 otree-6.0.0a8/otree/api.pyi
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.095983 otree-6.0.0a8/otree/app_template/
+-rw-rw-rw-   0        0        0        0 2018-11-23 17:31:44.000000 otree-6.0.0a8/otree/app_template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.104268 otree-6.0.0a8/otree/app_template/__pycache__/
+-rw-rw-rw-   0        0        0      127 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      131 2019-07-18 16:08:18.000000 otree-6.0.0a8/otree/app_template/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1013 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1017 2019-07-18 16:08:18.000000 otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-37.pyc
+-rw-rw-rw-   0        0        0      615 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/__pycache__/tests.cpython-36.pyc
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.105322 otree-6.0.0a8/otree/app_template/_builtin/
+-rw-rw-rw-   0        0        0      446 2020-10-07 12:35:10.000000 otree-6.0.0a8/otree/app_template/_builtin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.107717 otree-6.0.0a8/otree/app_template/_builtin/__pycache__/
+-rw-rw-rw-   0        0        0     1170 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      871 2019-07-18 16:08:18.000000 otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      464 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template/models.py
+-rw-rw-rw-   0        0        0      297 2020-10-07 12:35:10.000000 otree-6.0.0a8/otree/app_template/pages.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.025650 otree-6.0.0a8/otree/app_template/templates/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.109616 otree-6.0.0a8/otree/app_template/templates/app_name/
+-rw-rw-rw-   0        0        0      200 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template/templates/app_name/MyPage.html
+-rw-rw-rw-   0        0        0      180 2020-12-11 18:14:00.000000 otree-6.0.0a8/otree/app_template/templates/app_name/Results.html
+-rw-rw-rw-   0        0        0      200 2020-03-20 01:44:18.000000 otree-6.0.0a8/otree/app_template/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.112511 otree-6.0.0a8/otree/app_template_lite/
+-rw-rw-rw-   0        0        0      137 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template_lite/MyPage.html
+-rw-rw-rw-   0        0        0      119 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template_lite/Results.html
+-rw-rw-rw-   0        0        0      495 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/app_template_lite/__init__.py
+-rw-rw-rw-   0        0        0     2888 2022-03-04 18:20:48.000000 otree-6.0.0a8/otree/asgi.py
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/auth.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.117003 otree-6.0.0a8/otree/bots/
+-rw-rw-rw-   0        0        0       75 2020-03-20 01:44:18.000000 otree-6.0.0a8/otree/bots/__init__.py
+-rw-rw-rw-   0        0        0    18278 2023-04-15 00:24:13.000000 otree-6.0.0a8/otree/bots/bot.py
+-rw-rw-rw-   0        0        0     4815 2022-12-23 08:54:23.000000 otree-6.0.0a8/otree/bots/browser.py
+-rw-rw-rw-   0        0        0    11868 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/bots/browser_launcher.py
+-rw-rw-rw-   0        0        0     6713 2022-02-01 22:47:42.000000 otree-6.0.0a8/otree/bots/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.122230 otree-6.0.0a8/otree/channels/
+-rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/channels/__init__.py
+-rw-rw-rw-   0        0        0    27401 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/channels/consumers.py
+-rw-rw-rw-   0        0        0      930 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/channels/routing.py
+-rw-rw-rw-   0        0        0     4489 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/channels/utils.py
+-rw-rw-rw-   0        0        0     2407 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/chat.py
+-rw-rw-rw-   0        0        0    11062 2023-04-15 16:38:25.000000 otree-6.0.0a8/otree/checks.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.140693 otree-6.0.0a8/otree/cli/
+-rw-rw-rw-   0        0        0        0 2021-09-07 01:38:00.000000 otree-6.0.0a8/otree/cli/__init__.py
+-rw-rw-rw-   0        0        0      841 2021-06-29 10:07:36.000000 otree-6.0.0a8/otree/cli/base.py
+-rw-rw-rw-   0        0        0     1846 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/bots.py
+-rw-rw-rw-   0        0        0     1072 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/browser_bots.py
+-rw-rw-rw-   0        0        0     1337 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/create_session.py
+-rw-rw-rw-   0        0        0     3402 2021-09-28 08:02:58.000000 otree-6.0.0a8/otree/cli/devserver.py
+-rw-rw-rw-   0        0        0     2051 2021-09-28 08:03:24.000000 otree-6.0.0a8/otree/cli/devserver_inner.py
+-rw-rw-rw-   0        0        0       35 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/prodserver.py
+-rw-rw-rw-   0        0        0     1766 2021-06-30 10:11:04.000000 otree-6.0.0a8/otree/cli/prodserver1of2.py
+-rw-rw-rw-   0        0        0      258 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/prodserver2of2.py
+-rw-rw-rw-   0        0        0    14172 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/remove_self.py
+-rw-rw-rw-   0        0        0     1981 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/resetdb.py
+-rw-rw-rw-   0        0        0     1957 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/startapp.py
+-rw-rw-rw-   0        0        0     2796 2022-12-23 08:54:35.000000 otree-6.0.0a8/otree/cli/startproject.py
+-rw-rw-rw-   0        0        0      345 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/timeoutsubprocess.py
+-rw-rw-rw-   0        0        0     1224 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/unzip.py
+-rw-rw-rw-   0        0        0     2290 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/cli/upcase_constants.py
+-rw-rw-rw-   0        0        0     7229 2021-06-30 09:55:02.000000 otree-6.0.0a8/otree/cli/update_my_code.py
+-rw-rw-rw-   0        0        0     7301 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/zip.py
+-rw-rw-rw-   0        0        0     6434 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/zipserver.py
+-rw-rw-rw-   0        0        0     7803 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/common.py
+-rw-rw-rw-   0        0        0     5217 2023-04-15 09:44:16.000000 otree-6.0.0a8/otree/common2.py
+-rw-rw-rw-   0        0        0     2511 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/constants.py
+-rw-rw-rw-   0        0        0     8663 2022-09-17 23:55:17.000000 otree-6.0.0a8/otree/currency.py
+-rw-rw-rw-   0        0        0    33059 2023-04-15 18:40:54.000000 otree-6.0.0a8/otree/database.py
+-rw-rw-rw-   0        0        0     8278 2022-03-04 18:20:48.000000 otree-6.0.0a8/otree/errorpage.py
+-rw-rw-rw-   0        0        0    16209 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/export.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.144818 otree-6.0.0a8/otree/forms/
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/forms/__init__.py
+-rw-rw-rw-   0        0        0     3620 2022-09-19 10:51:45.000000 otree-6.0.0a8/otree/forms/fields.py
+-rw-rw-rw-   0        0        0    10547 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/forms/forms.py
+-rw-rw-rw-   0        0        0     7446 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/forms/widgets.py
+-rw-rw-rw-   0        0        0     6841 2022-09-19 10:51:45.000000 otree-6.0.0a8/otree/i18n.py
+-rw-rw-rw-   0        0        0     3662 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/live.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.145865 otree-6.0.0a8/otree/locale/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.030486 otree-6.0.0a8/otree/locale/ar/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.147971 otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1532 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3986 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      120 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/babel.ini
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.030486 otree-6.0.0a8/otree/locale/cs/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.150098 otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1409 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3712 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.031755 otree-6.0.0a8/otree/locale/de/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.153630 otree-6.0.0a8/otree/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1762 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3875 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     3188 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/django.pot
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.032501 otree-6.0.0a8/otree/locale/es/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.154757 otree-6.0.0a8/otree/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1567 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.033278 otree-6.0.0a8/otree/locale/fi/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.156462 otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      497 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3114 2021-11-29 03:59:50.000000 otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.033278 otree-6.0.0a8/otree/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.158309 otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1634 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3747 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.034294 otree-6.0.0a8/otree/locale/he/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.160303 otree-6.0.0a8/otree/locale/he/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1652 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3703 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.035291 otree-6.0.0a8/otree/locale/hi/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.162082 otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2206 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4254 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.036289 otree-6.0.0a8/otree/locale/hu/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.163946 otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1722 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3900 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.037289 otree-6.0.0a8/otree/locale/id/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.166149 otree-6.0.0a8/otree/locale/id/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1520 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3605 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.038289 otree-6.0.0a8/otree/locale/it/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.169209 otree-6.0.0a8/otree/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1620 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3733 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.038289 otree-6.0.0a8/otree/locale/ja/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.170373 otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1747 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3826 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.039291 otree-6.0.0a8/otree/locale/ko/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.172393 otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1783 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3917 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.040289 otree-6.0.0a8/otree/locale/nb/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.174069 otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1023 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3421 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.040289 otree-6.0.0a8/otree/locale/nl/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.176060 otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1579 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3669 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.041355 otree-6.0.0a8/otree/locale/pl/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.178069 otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.041355 otree-6.0.0a8/otree/locale/pt/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.179864 otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.042405 otree-6.0.0a8/otree/locale/ru/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.181652 otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2047 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4156 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.042405 otree-6.0.0a8/otree/locale/tr/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.185052 otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1537 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3731 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.043402 otree-6.0.0a8/otree/locale/zh_Hans/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.186842 otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1452 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3521 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     2323 2021-08-31 15:42:14.000000 otree-6.0.0a8/otree/lookup.py
+-rw-rw-rw-   0        0        0     6971 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/main.py
+-rw-rw-rw-   0        0        0     1819 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.192719 otree-6.0.0a8/otree/models/
+-rw-rw-rw-   0        0        0      230 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/models/__init__.py
+-rw-rw-rw-   0        0        0     4133 2021-11-18 17:14:02.000000 otree-6.0.0a8/otree/models/group.py
+-rw-rw-rw-   0        0        0     8714 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/models/participant.py
+-rw-rw-rw-   0        0        0     3346 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/models/player.py
+-rw-rw-rw-   0        0        0     9750 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/models/session.py
+-rw-rw-rw-   0        0        0     9025 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/models/subsession.py
+-rw-rw-rw-   0        0        0     1929 2021-08-18 09:23:18.000000 otree-6.0.0a8/otree/models_concrete.py
+-rw-rw-rw-   0        0        0     7383 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/mturk_client.py
+-rw-rw-rw-   0        0        0     1897 2022-03-04 18:20:48.000000 otree-6.0.0a8/otree/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.197107 otree-6.0.0a8/otree/project_template/
+-rw-rw-rw-   0        0        0      133 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/project_template/.gitignore
+-rw-rw-rw-   0        0        0       57 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/project_template/Procfile
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.044414 otree-6.0.0a8/otree/project_template/_static/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.198029 otree-6.0.0a8/otree/project_template/_static/global/
+-rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/project_template/_static/global/empty.css
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.045402 otree-6.0.0a8/otree/project_template/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.199071 otree-6.0.0a8/otree/project_template/_templates/global/
+-rw-rw-rw-   0        0        0      149 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/project_template/_templates/global/Page.html
+-rw-rw-rw-   0        0        0      169 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/project_template/requirements.txt
+-rw-rw-rw-   0        0        0     1018 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/project_template/settings.py
+-rw-rw-rw-   0        0        0     2567 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/read_csv.py
+-rw-rw-rw-   0        0        0     4291 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/room.py
+-rw-rw-rw-   0        0        0    15047 2022-12-23 08:54:23.000000 otree-6.0.0a8/otree/session.py
+-rw-rw-rw-   0        0        0     2380 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.201847 otree-6.0.0a8/otree/static/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.046402 otree-6.0.0a8/otree/static/bootstrap5/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.203816 otree-6.0.0a8/otree/static/bootstrap5/css/
+-rw-rw-rw-   0        0        0   155637 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   429472 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.205822 otree-6.0.0a8/otree/static/bootstrap5/js/
+-rw-rw-rw-   0        0        0    78754 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   326390 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0      198 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.221932 otree-6.0.0a8/otree/static/glyphicons/
+-rw-rw-rw-   0        0        0     1412 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/clock.png
+-rw-rw-rw-   0        0        0     1307 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/cloud.png
+-rw-rw-rw-   0        0        0     1443 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/cogwheel.png
+-rw-rw-rw-   0        0        0     1310 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/delete.png
+-rw-rw-rw-   0        0        0     1314 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/download-alt.png
+-rw-rw-rw-   0        0        0     1475 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/eye-open.png
+-rw-rw-rw-   0        0        0     1243 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/folder-closed.png
+-rw-rw-rw-   0        0        0     1436 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/link.png
+-rw-rw-rw-   0        0        0     1231 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/list-alt.png
+-rw-rw-rw-   0        0        0     1342 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/pencil.png
+-rw-rw-rw-   0        0        0     1218 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/plus.png
+-rw-rw-rw-   0        0        0     1378 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/pushpin.png
+-rw-rw-rw-   0        0        0     1471 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/refresh.png
+-rw-rw-rw-   0        0        0     1499 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/stats.png
+-rw-rw-rw-   0        0        0     1432 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/usd.png
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.046402 otree-6.0.0a8/otree/static/otree/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.223786 otree-6.0.0a8/otree/static/otree/css/
+-rw-rw-rw-   0        0        0      868 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/css/table.css
+-rw-rw-rw-   0        0        0     2015 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/css/theme.css
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.241020 otree-6.0.0a8/otree/static/otree/js/
+-rw-rw-rw-   0        0        0     1909 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/static/otree/js/common.js
+-rw-rw-rw-   0        0        0     1624 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/static/otree/js/formInputs.js
+-rw-rw-rw-   0        0        0      504 2020-10-07 12:35:10.000000 otree-6.0.0a8/otree/static/otree/js/internet-explorer.js
+-rw-rw-rw-   0        0        0    86663 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/js/jquery-3.2.1.min.js
+-rw-rw-rw-   0        0        0     6605 2020-11-23 22:42:18.000000 otree-6.0.0a8/otree/static/otree/js/jquery.color-2.1.2.min.js
+-rw-rw-rw-   0        0        0     5360 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/js/jquery.countdown.min.js
+-rw-rw-rw-   0        0        0      702 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/js/jquery.timeago.en-short.js
+-rw-rw-rw-   0        0        0     7200 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/js/jquery.timeago.js
+-rw-rw-rw-   0        0        0      663 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/static/otree/js/live.js
+-rw-rw-rw-   0        0        0     4271 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/static/otree/js/monitor2.js
+-rw-rw-rw-   0        0        0    49322 2023-04-15 17:21:55.000000 otree-6.0.0a8/otree/static/otree/js/otree-front.js
+-rw-rw-rw-   0        0        0      967 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/js/page-websocket-redirect.js
+-rw-rw-rw-   0        0        0     8729 2020-03-20 01:44:18.000000 otree-6.0.0a8/otree/static/otree/js/reconnecting-websocket-iife.min.js
+-rw-rw-rw-   0        0        0     4837 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/js/table-utils.js
+-rw-rw-rw-   0        0        0      861 2023-04-15 16:01:01.000000 otree-6.0.0a8/otree/static/otree/js/trial-default.js
+-rw-rw-rw-   0        0        0      221 2023-04-15 08:05:11.000000 otree-6.0.0a8/otree/static/otree/js/trial-setup.js
+-rw-rw-rw-   0        0        0       26 2018-11-23 17:31:48.000000 otree-6.0.0a8/otree/static/robots.txt
+-rw-rw-rw-   0        0        0     5360 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/tasks.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.047402 otree-6.0.0a8/otree/templates/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.243353 otree-6.0.0a8/otree/templates/global/
+-rw-rw-rw-   0        0        0       33 2020-12-01 22:34:50.000000 otree-6.0.0a8/otree/templates/global/Base.html
+-rw-rw-rw-   0        0        0      293 2021-10-18 21:34:16.000000 otree-6.0.0a8/otree/templates/global/Page.html
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.274743 otree-6.0.0a8/otree/templates/otree/
+-rw-rw-rw-   0        0        0      881 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/AdminReport.html
+-rw-rw-rw-   0        0        0     1768 2023-04-15 08:08:38.000000 otree-6.0.0a8/otree/templates/otree/Base.html
+-rw-rw-rw-   0        0        0     3065 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/BaseAdmin.html
+-rw-rw-rw-   0        0        0     2881 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/CreateDemoSession.html
+-rw-rw-rw-   0        0        0      199 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/CreateSession.html
+-rw-rw-rw-   0        0        0      955 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/DemoIndex.html
+-rw-rw-rw-   0        0        0     5961 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/Export.html
+-rw-rw-rw-   0        0        0       31 2020-12-01 22:34:50.000000 otree-6.0.0a8/otree/templates/otree/FormPage.html
+-rw-rw-rw-   0        0        0     1240 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/Login.html
+-rw-rw-rw-   0        0        0     2796 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/MTurkCreateHIT.html
+-rw-rw-rw-   0        0        0     1214 2020-12-01 22:34:50.000000 otree-6.0.0a8/otree/templates/otree/MTurkHTMLQuestion.html
+-rw-rw-rw-   0        0        0     6732 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/MTurkSessionPayments.html
+-rw-rw-rw-   0        0        0       18 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/OutOfRangeNotification.html
+-rw-rw-rw-   0        0        0     3116 2023-04-15 17:20:30.000000 otree-6.0.0a8/otree/templates/otree/Page.html
+-rw-rw-rw-   0        0        0      911 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/templates/otree/RoomInputLabel.html
+-rw-rw-rw-   0        0        0      754 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/RoomWithSession.html
+-rw-rw-rw-   0        0        0     4282 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/RoomWithoutSession.html
+-rw-rw-rw-   0        0        0      353 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/Rooms.html
+-rw-rw-rw-   0        0        0     1784 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/ServerCheck.html
+-rw-rw-rw-   0        0        0     2532 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/Session.html
+-rw-rw-rw-   0        0        0     7856 2021-08-19 09:01:20.000000 otree-6.0.0a8/otree/templates/otree/SessionData.html
+-rw-rw-rw-   0        0        0      139 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionDescription.html
+-rw-rw-rw-   0        0        0      323 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionEditProperties.html
+-rw-rw-rw-   0        0        0     2391 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/templates/otree/SessionMonitor.html
+-rw-rw-rw-   0        0        0     1582 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionPayments.html
+-rw-rw-rw-   0        0        0     3329 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionSplitScreen.html
+-rw-rw-rw-   0        0        0     4087 2021-09-02 00:40:54.000000 otree-6.0.0a8/otree/templates/otree/SessionStartLinks.html
+-rw-rw-rw-   0        0        0     5469 2022-05-14 06:42:33.000000 otree-6.0.0a8/otree/templates/otree/Sessions.html
+-rw-rw-rw-   0        0        0     5121 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/WaitPage.html
+-rw-rw-rw-   0        0        0       37 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/WaitPageRoom.html
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.286472 otree-6.0.0a8/otree/templates/otree/includes/
+-rw-rw-rw-   0        0        0     5461 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/CreateSessionForm.html
+-rw-rw-rw-   0        0        0     1528 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/RoomParticipantLinks.html
+-rw-rw-rw-   0        0        0      402 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/SessionInfo.html
+-rw-rw-rw-   0        0        0      213 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/TimeLimit.html
+-rw-rw-rw-   0        0        0      997 2022-07-06 11:50:24.000000 otree-6.0.0a8/otree/templates/otree/includes/TimeLimit.js.html
+-rw-rw-rw-   0        0        0      969 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/debug_info.html
+-rw-rw-rw-   0        0        0     2679 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/includes/hidden_form_errors.html
+-rw-rw-rw-   0        0        0      244 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/messages.html
+-rw-rw-rw-   0        0        0     1368 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/mturk_payment_table.html
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.287651 otree-6.0.0a8/otree/templates/otree/tags/
+-rw-rw-rw-   0        0        0     3572 2021-09-09 20:27:16.000000 otree-6.0.0a8/otree/templates/otree/tags/chat.html
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.297592 otree-6.0.0a8/otree/templating/
+-rw-rw-rw-   0        0        0       70 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templating/__init__.py
+-rw-rw-rw-   0        0        0     6993 2021-09-10 18:14:58.000000 otree-6.0.0a8/otree/templating/compiler.py
+-rw-rw-rw-   0        0        0     2948 2021-09-23 22:55:28.000000 otree-6.0.0a8/otree/templating/context.py
+-rw-rw-rw-   0        0        0     1342 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templating/errors.py
+-rw-rw-rw-   0        0        0     2081 2021-08-11 02:49:06.000000 otree-6.0.0a8/otree/templating/filters.py
+-rw-rw-rw-   0        0        0     3392 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templating/loader.py
+-rw-rw-rw-   0        0        0    33516 2023-04-15 08:53:48.000000 otree-6.0.0a8/otree/templating/nodes.py
+-rw-rw-rw-   0        0        0     1495 2021-09-10 17:48:20.000000 otree-6.0.0a8/otree/templating/template.py
+-rw-rw-rw-   0        0        0     1836 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templating/utils.py
+-rw-rw-rw-   0        0        0      173 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/test.py
+-rw-rw-rw-   0        0        0     4850 2023-04-15 18:39:16.000000 otree-6.0.0a8/otree/trial.py
+-rw-rw-rw-   0        0        0     1919 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/update.py
+-rw-rw-rw-   0        0        0     4635 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.310293 otree-6.0.0a8/otree/views/
+-rw-rw-rw-   0        0        0       49 2020-06-23 01:10:42.000000 otree-6.0.0a8/otree/views/__init__.py
+-rw-rw-rw-   0        0        0    49935 2023-04-15 09:49:30.000000 otree-6.0.0a8/otree/views/abstract.py
+-rw-rw-rw-   0        0        0    19290 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/admin.py
+-rw-rw-rw-   0        0        0     8261 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/views/cbv.py
+-rw-rw-rw-   0        0        0     1537 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/views/demo.py
+-rw-rw-rw-   0        0        0     3722 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/export.py
+-rw-rw-rw-   0        0        0    14856 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/mturk.py
+-rw-rw-rw-   0        0        0    12981 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/participant.py
+-rw-rw-rw-   0        0        0    10004 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/rest.py
+-rw-rw-rw-   0        0        0     2523 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/views/room.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.092073 otree-6.0.0a8/otree.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8038 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-11-22 05:26:26.000000 otree-6.0.0a8/otree.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      196 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      311 2023-03-08 18:09:53.000000 otree-6.0.0a8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:48:35.311947 otree-6.0.0a8/setup.cfg
+-rw-rw-rw-   0        0        0     2548 2023-03-08 18:09:53.000000 otree-6.0.0a8/setup.py
```

### Comparing `otree-6.0.0a7/LICENSE` & `otree-6.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/PKG-INFO` & `otree-6.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otree
-Version: 6.0.0a7
+Version: 6.0.0a8
 Summary: Framework for multiplayer strategy games and complex surveys.
 Home-page: http://otree.org/
 Author: chris@otree.org
 Author-email: chris@otree.org
 License: MIT License
 Platform: UNKNOWN
 Provides-Extra: mturk
```

### Comparing `otree-6.0.0a7/README.rst` & `otree-6.0.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/api.py` & `otree-6.0.0a8/otree/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from otree.constants import BaseConstants  # noqa
 from otree.views import Page, WaitPage  # noqa
 from otree.currency import Currency, currency_range, safe_json  # noqa
 from otree.bots import Bot, Submission, SubmissionMustFail, expect  # noqa
 from otree import database as models  # noqa
 from otree.forms import widgets  # noqa
 from otree.i18n import extract_otreetemplate  # noqa
-from otree.database import ExtraModel  # noqa
+from otree.database import ExtraModel, BaseTrial  # noqa
 from otree.read_csv import read_csv  # noqa
 from otree.common2 import url_of_static_file  # noqa
 
 cu = Currency
```

### Comparing `otree-6.0.0a7/otree/api.pyi` & `otree-6.0.0a8/otree/api.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,19 @@
 
     @classmethod
     def create(cls: Type[T_extramodel], **kwargs) -> T_extramodel:
         pass
 
     id: int
 
+class BaseTrial(ExtraModel):
+    player: PlayerTV
+    queue_position: int
+
+
 class WaitPage:
     wait_for_all_groups = False
     group_by_arrival_time = False
     title_text: str
     body_text: str
     template_name: str
 
@@ -373,14 +378,15 @@
     "models",
     "widgets",
     "BaseConstants",
     "BaseSubsession",
     "BaseGroup",
     "BasePlayer",
     "ExtraModel",
+    "BaseTrial",
     "WaitPage",
     "Page",
     "Bot",
     "Submission",
     "SubmissionMustFail",
     "expect",
     "read_csv",
```

### Comparing `otree-6.0.0a7/otree/app_template/__pycache__/models.cpython-36.pyc` & `otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/app_template/__pycache__/models.cpython-37.pyc` & `otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/app_template/__pycache__/tests.cpython-36.pyc` & `otree-6.0.0a8/otree/app_template/__pycache__/tests.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc` & `otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc` & `otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/asgi.py` & `otree-6.0.0a8/otree/asgi.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/bots/bot.py` & `otree-6.0.0a8/otree/bots/bot.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/bots/browser.py` & `otree-6.0.0a8/otree/bots/browser.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/bots/browser_launcher.py` & `otree-6.0.0a8/otree/bots/browser_launcher.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/bots/runner.py` & `otree-6.0.0a8/otree/bots/runner.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/channels/consumers.py` & `otree-6.0.0a8/otree/channels/consumers.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/channels/routing.py` & `otree-6.0.0a8/otree/channels/routing.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/channels/utils.py` & `otree-6.0.0a8/otree/channels/utils.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/chat.py` & `otree-6.0.0a8/otree/chat.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/checks.py` & `otree-6.0.0a8/otree/checks.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/base.py` & `otree-6.0.0a8/otree/cli/base.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/bots.py` & `otree-6.0.0a8/otree/cli/bots.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/browser_bots.py` & `otree-6.0.0a8/otree/cli/browser_bots.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/create_session.py` & `otree-6.0.0a8/otree/cli/create_session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/devserver.py` & `otree-6.0.0a8/otree/cli/devserver.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/devserver_inner.py` & `otree-6.0.0a8/otree/cli/devserver_inner.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/prodserver1of2.py` & `otree-6.0.0a8/otree/cli/prodserver1of2.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/remove_self.py` & `otree-6.0.0a8/otree/cli/remove_self.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/resetdb.py` & `otree-6.0.0a8/otree/cli/resetdb.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/startapp.py` & `otree-6.0.0a8/otree/cli/startapp.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/startproject.py` & `otree-6.0.0a8/otree/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/unzip.py` & `otree-6.0.0a8/otree/cli/unzip.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/upcase_constants.py` & `otree-6.0.0a8/otree/cli/upcase_constants.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/update_my_code.py` & `otree-6.0.0a8/otree/cli/update_my_code.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/zip.py` & `otree-6.0.0a8/otree/cli/zip.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/cli/zipserver.py` & `otree-6.0.0a8/otree/cli/zipserver.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/common.py` & `otree-6.0.0a8/otree/common.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/common2.py` & `otree-6.0.0a8/otree/common2.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/constants.py` & `otree-6.0.0a8/otree/constants.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/currency.py` & `otree-6.0.0a8/otree/currency.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/database.py` & `otree-6.0.0a8/otree/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.ext.mutable import Mutable
 from sqlalchemy.orm import (
     mapper,
     relationship,
 )
+from sqlalchemy.sql.functions import func
 from sqlalchemy.orm import sessionmaker, configure_mappers
 from sqlalchemy.orm.exc import NoResultFound  # noqa
 from sqlalchemy.sql import sqltypes as st
 from starlette.exceptions import HTTPException
 
 from otree import __version__
 from otree import common
@@ -924,14 +925,66 @@
             name = col.name
             if not (col.primary_key or col.foreign_keys):
                 # this could be huge, maybe should truncate
                 items.append((name, repr(getattr(self, name))))
         return dict(items)
 
 
+class BaseTrial(ExtraModel):
+    """
+    We should have a class for this because:
+    - makes it easier to enforce correctness
+    - we may need to add stuff to it in the future.
+    - less code to loop and create trials in the regular case
+    - if someone forgets to assign queue_positions, then all queue positions will be None
+      and it will skip right past the trials page, which will be confusing.
+    - if doing infinite iteration, the trials will not all be created at the same time.
+      therefore, it's hard to know what the previous queue_position was.
+      need to store it somewhere, which is a pain.
+    """
+
+    __abstract__ = True
+
+    # can't use autoincrement=True because that only has an effect
+    # if the field is part of the primary key.
+    queue_position = Column(st.Integer)
+
+    @declared_attr
+    def player_id(cls):
+        app_name = cls.get_folder_name()
+        # needs to be nullable so re-grouping can happen
+        return Column(st.Integer, ForeignKey(f'{app_name}_player.id'), nullable=True)
+
+    @declared_attr
+    def player(cls):
+        # back_populates=f'{cls.__name__}_set'
+        return relationship(
+            f'{cls.__module__}.Player',
+        )
+
+    @classmethod
+    def create(cls, **kwargs):
+        if 'queue_position' not in kwargs:
+            global _incrementing_queue_position
+            if _incrementing_queue_position is None:
+                _incrementing_queue_position = (
+                    dbq(func.max(cls.queue_position)).scalar() or 0
+                )
+            _incrementing_queue_position += 1
+            kwargs['queue_position'] = _incrementing_queue_position
+        return super().create(**kwargs)
+
+
+# queue position doesn't need to always contain the global max, but it must consistently increment
+# for a given player, even between server restarts (because you might create trials on the fly).
+# it's OK if 1 app passes queue_position explicitly, and another app auto-increments.
+# because those queue positions will never get compared to each other.
+_incrementing_queue_position = None
+
+
 @event.listens_for(mapper, "instrument_class")
 def prevent_forbidden_colnames(mapper, cls):
     forbidden_list = ['order', 'index']
     if cls.__name__ == 'Player':
         forbidden_list += ['payoff', 'role']
 
     columns = list(cls.__table__.columns)
```

### Comparing `otree-6.0.0a7/otree/errorpage.py` & `otree-6.0.0a8/otree/errorpage.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/export.py` & `otree-6.0.0a8/otree/export.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/forms/fields.py` & `otree-6.0.0a8/otree/forms/fields.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/forms/forms.py` & `otree-6.0.0a8/otree/forms/forms.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/forms/widgets.py` & `otree-6.0.0a8/otree/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/i18n.py` & `otree-6.0.0a8/otree/i18n.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/live.py` & `otree-6.0.0a8/otree/live.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ar/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ar/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/cs/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/cs/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/de/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/de/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/django.pot` & `otree-6.0.0a8/otree/locale/django.pot`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/es/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/es/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/fi/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/fr/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/fr/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/he/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/he/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/hi/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/hi/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/hu/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/hu/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/id/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/id/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/it/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/it/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ja/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ja/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ko/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ko/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/nb/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/nb/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/nl/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/nl/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/pl/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/pl/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/pt/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/pt/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ru/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/ru/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/tr/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/tr/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/zh_Hans/LC_MESSAGES/django.mo` & `otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/locale/zh_Hans/LC_MESSAGES/django.po` & `otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/lookup.py` & `otree-6.0.0a8/otree/lookup.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/main.py` & `otree-6.0.0a8/otree/main.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/middleware.py` & `otree-6.0.0a8/otree/middleware.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/models/group.py` & `otree-6.0.0a8/otree/models/group.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/models/participant.py` & `otree-6.0.0a8/otree/models/participant.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/models/player.py` & `otree-6.0.0a8/otree/models/player.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/models/session.py` & `otree-6.0.0a8/otree/models/session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/models/subsession.py` & `otree-6.0.0a8/otree/models/subsession.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/models_concrete.py` & `otree-6.0.0a8/otree/models_concrete.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/mturk_client.py` & `otree-6.0.0a8/otree/mturk_client.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/patch.py` & `otree-6.0.0a8/otree/patch.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/project_template/settings.py` & `otree-6.0.0a8/otree/project_template/settings.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/read_csv.py` & `otree-6.0.0a8/otree/read_csv.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/room.py` & `otree-6.0.0a8/otree/room.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/session.py` & `otree-6.0.0a8/otree/session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/settings.py` & `otree-6.0.0a8/otree/settings.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/bootstrap5/css/bootstrap.min.css` & `otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/bootstrap5/css/bootstrap.min.css.map` & `otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/bootstrap5/js/bootstrap.bundle.min.js` & `otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map` & `otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/clock.png` & `otree-6.0.0a8/otree/static/glyphicons/clock.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/cloud.png` & `otree-6.0.0a8/otree/static/glyphicons/cloud.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/cogwheel.png` & `otree-6.0.0a8/otree/static/glyphicons/cogwheel.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/delete.png` & `otree-6.0.0a8/otree/static/glyphicons/delete.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/download-alt.png` & `otree-6.0.0a8/otree/static/glyphicons/download-alt.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/eye-open.png` & `otree-6.0.0a8/otree/static/glyphicons/eye-open.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/folder-closed.png` & `otree-6.0.0a8/otree/static/glyphicons/folder-closed.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/link.png` & `otree-6.0.0a8/otree/static/glyphicons/link.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/list-alt.png` & `otree-6.0.0a8/otree/static/glyphicons/list-alt.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/pencil.png` & `otree-6.0.0a8/otree/static/glyphicons/pencil.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/plus.png` & `otree-6.0.0a8/otree/static/glyphicons/plus.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/pushpin.png` & `otree-6.0.0a8/otree/static/glyphicons/pushpin.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/refresh.png` & `otree-6.0.0a8/otree/static/glyphicons/refresh.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/stats.png` & `otree-6.0.0a8/otree/static/glyphicons/stats.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/glyphicons/usd.png` & `otree-6.0.0a8/otree/static/glyphicons/usd.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/css/table.css` & `otree-6.0.0a8/otree/static/otree/css/table.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/css/theme.css` & `otree-6.0.0a8/otree/static/otree/css/theme.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/common.js` & `otree-6.0.0a8/otree/static/otree/js/common.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/formInputs.js` & `otree-6.0.0a8/otree/static/otree/js/formInputs.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/jquery-3.2.1.min.js` & `otree-6.0.0a8/otree/static/otree/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/jquery.color-2.1.2.min.js` & `otree-6.0.0a8/otree/static/otree/js/jquery.color-2.1.2.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/jquery.countdown.min.js` & `otree-6.0.0a8/otree/static/otree/js/jquery.countdown.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/jquery.timeago.en-short.js` & `otree-6.0.0a8/otree/static/otree/js/jquery.timeago.en-short.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/jquery.timeago.js` & `otree-6.0.0a8/otree/static/otree/js/jquery.timeago.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/live.js` & `otree-6.0.0a8/otree/static/otree/js/live.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/monitor2.js` & `otree-6.0.0a8/otree/static/otree/js/monitor2.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/otree-front.js` & `otree-6.0.0a8/otree/static/otree/js/otree-front.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/page-websocket-redirect.js` & `otree-6.0.0a8/otree/static/otree/js/page-websocket-redirect.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/reconnecting-websocket-iife.min.js` & `otree-6.0.0a8/otree/static/otree/js/reconnecting-websocket-iife.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/table-utils.js` & `otree-6.0.0a8/otree/static/otree/js/table-utils.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/static/otree/js/trial-default.js` & `otree-6.0.0a8/otree/static/otree/js/trial-default.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/tasks.py` & `otree-6.0.0a8/otree/tasks.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/AdminReport.html` & `otree-6.0.0a8/otree/templates/otree/AdminReport.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/Base.html` & `otree-6.0.0a8/otree/templates/otree/Base.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/BaseAdmin.html` & `otree-6.0.0a8/otree/templates/otree/BaseAdmin.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/CreateDemoSession.html` & `otree-6.0.0a8/otree/templates/otree/CreateDemoSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/DemoIndex.html` & `otree-6.0.0a8/otree/templates/otree/DemoIndex.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/Export.html` & `otree-6.0.0a8/otree/templates/otree/Export.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/Login.html` & `otree-6.0.0a8/otree/templates/otree/Login.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/MTurkCreateHIT.html` & `otree-6.0.0a8/otree/templates/otree/MTurkCreateHIT.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/MTurkHTMLQuestion.html` & `otree-6.0.0a8/otree/templates/otree/MTurkHTMLQuestion.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/MTurkSessionPayments.html` & `otree-6.0.0a8/otree/templates/otree/MTurkSessionPayments.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/Page.html` & `otree-6.0.0a8/otree/templates/otree/Page.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/RoomInputLabel.html` & `otree-6.0.0a8/otree/templates/otree/RoomInputLabel.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/RoomWithSession.html` & `otree-6.0.0a8/otree/templates/otree/RoomWithSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/RoomWithoutSession.html` & `otree-6.0.0a8/otree/templates/otree/RoomWithoutSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/ServerCheck.html` & `otree-6.0.0a8/otree/templates/otree/ServerCheck.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/Session.html` & `otree-6.0.0a8/otree/templates/otree/Session.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/SessionData.html` & `otree-6.0.0a8/otree/templates/otree/SessionData.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/SessionMonitor.html` & `otree-6.0.0a8/otree/templates/otree/SessionMonitor.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/SessionPayments.html` & `otree-6.0.0a8/otree/templates/otree/SessionPayments.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/SessionSplitScreen.html` & `otree-6.0.0a8/otree/templates/otree/SessionSplitScreen.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/SessionStartLinks.html` & `otree-6.0.0a8/otree/templates/otree/SessionStartLinks.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/Sessions.html` & `otree-6.0.0a8/otree/templates/otree/Sessions.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/WaitPage.html` & `otree-6.0.0a8/otree/templates/otree/WaitPage.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/includes/CreateSessionForm.html` & `otree-6.0.0a8/otree/templates/otree/includes/CreateSessionForm.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/includes/RoomParticipantLinks.html` & `otree-6.0.0a8/otree/templates/otree/includes/RoomParticipantLinks.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/includes/TimeLimit.js.html` & `otree-6.0.0a8/otree/templates/otree/includes/TimeLimit.js.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/includes/debug_info.html` & `otree-6.0.0a8/otree/templates/otree/includes/debug_info.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/includes/hidden_form_errors.html` & `otree-6.0.0a8/otree/templates/otree/includes/hidden_form_errors.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/includes/mturk_payment_table.html` & `otree-6.0.0a8/otree/templates/otree/includes/mturk_payment_table.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templates/otree/tags/chat.html` & `otree-6.0.0a8/otree/templates/otree/tags/chat.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/compiler.py` & `otree-6.0.0a8/otree/templating/compiler.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/context.py` & `otree-6.0.0a8/otree/templating/context.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/errors.py` & `otree-6.0.0a8/otree/templating/errors.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/filters.py` & `otree-6.0.0a8/otree/templating/filters.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/loader.py` & `otree-6.0.0a8/otree/templating/loader.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/nodes.py` & `otree-6.0.0a8/otree/templating/nodes.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/template.py` & `otree-6.0.0a8/otree/templating/template.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/templating/utils.py` & `otree-6.0.0a8/otree/templating/utils.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/trial.py` & `otree-6.0.0a8/otree/trial.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,80 +12,84 @@
 
     # print('in trial_payload_function', msg)
     try:
         participant = Participant.objects_get(code=participant_code)
     except NoResultFound:
         logger.warning(f'Participant not found: {participant_code}')
         return
-    send_error = _send_back(
-        participant_code,
-        participant._index_in_pages,
-        dict(type='error'),
-    )
+
+    def send_error():
+        """need to put it in a function, otherwise we get a warning
+        that the coroutine wasn't awaited."""
+        return _send_back(
+            participant_code,
+            participant._index_in_pages,
+            dict(type='error'),
+        )
 
     lookup = get_page_lookup(participant._session_code, participant._index_in_pages)
     app_name = lookup.app_name
     models_module = otree.common.get_models_module(app_name)
     PageClass = lookup.page_class
     if page_name != PageClass.__name__:
         logger.warning(
             f'Ignoring message from {participant_code} because '
             f'they are on page {PageClass.__name__}, not {page_name}.'
         )
-        await send_error
+        await send_error()
 
     player = models_module.Player.objects_get(
         round_number=lookup.round_number, participant=participant
     )
     Trial = PageClass.trial_model
     trial = get_current_trial(Trial, player)
     msg_type = msg['type']
     is_page_load = msg_type == 'load'
     resp = dict(is_page_load=is_page_load, type=msg_type)
     if trial and msg_type == 'response':
         if trial.id != msg['trial_id']:
-            await send_error
+            await send_error()
             msg = (
                 "Trials: server and client are out of sync. "
                 "Check if there were any errors earlier."
             )
             raise Exception(msg)
         response: dict = msg['response']
         if hasattr(PageClass, 'evaluate_trial'):
             try:
                 feedback = PageClass.evaluate_trial(trial, response)
             except Exception:
-                await send_error
+                await send_error()
                 raise
         else:
             server_fields = set(PageClass.trial_response_fields)
             client_fields = response.keys()
             server_only = server_fields - client_fields
             if server_only:
-                await send_error
+                await send_error()
                 msg = (
                     "The following fields are in trial_response_fields, "
                     f"but were not sent from sendTrialResponse: {server_only}"
                 )
                 raise Exception(msg)
             client_only = client_fields - server_fields
             if client_only:
-                await send_error
+                await send_error()
                 msg = (
                     "The following fields were sent from the sendTrialResponse, "
                     f"but are not in trial_response_fields: {client_only}"
                 )
                 raise Exception(msg)
             try:
                 # need to do it this way rather than having an overridable evaluate_trial,
                 # because it's a static method, so has no access to trial_response_fields.
                 for attr in PageClass.trial_response_fields:
                     setattr(trial, attr, response[attr])
             except Exception:
-                await send_error
+                await send_error()
                 raise
             trial.queue_position = None
             feedback = {}
         resp.update(feedback=feedback)
         trial = get_current_trial(Trial, player)
     if trial:
         resp.update(trial=encode_trial(trial, PageClass.trial_stimulus_fields))
```

### Comparing `otree-6.0.0a7/otree/update.py` & `otree-6.0.0a8/otree/update.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/urls.py` & `otree-6.0.0a8/otree/urls.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/abstract.py` & `otree-6.0.0a8/otree/views/abstract.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/admin.py` & `otree-6.0.0a8/otree/views/admin.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/cbv.py` & `otree-6.0.0a8/otree/views/cbv.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/demo.py` & `otree-6.0.0a8/otree/views/demo.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/export.py` & `otree-6.0.0a8/otree/views/export.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/mturk.py` & `otree-6.0.0a8/otree/views/mturk.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/participant.py` & `otree-6.0.0a8/otree/views/participant.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/rest.py` & `otree-6.0.0a8/otree/views/rest.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree/views/room.py` & `otree-6.0.0a8/otree/views/room.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/otree.egg-info/PKG-INFO` & `otree-6.0.0a8/otree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otree
-Version: 6.0.0a7
+Version: 6.0.0a8
 Summary: Framework for multiplayer strategy games and complex surveys.
 Home-page: http://otree.org/
 Author: chris@otree.org
 Author-email: chris@otree.org
 License: MIT License
 Platform: UNKNOWN
 Provides-Extra: mturk
```

### Comparing `otree-6.0.0a7/otree.egg-info/SOURCES.txt` & `otree-6.0.0a8/otree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a7/setup.py` & `otree-6.0.0a8/setup.py`

 * *Files identical despite different names*

