# Comparing `tmp/otree-6.0.0a4.tar.gz` & `tmp/otree-6.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otree-6.0.0a4.tar", last modified: Fri Mar 24 17:40:32 2023, max compression
+gzip compressed data, was "otree-6.0.0a5.tar", last modified: Fri Apr 14 19:47:21 2023, max compression
```

## Comparing `otree-6.0.0a4.tar` & `otree-6.0.0a5.tar`

### file list

```diff
@@ -1,323 +1,325 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.591268 otree-6.0.0a4/
--rw-rw-rw-   0        0        0     1573 2018-11-23 17:31:44.000000 otree-6.0.0a4/LICENSE
--rw-rw-rw-   0        0        0      390 2021-06-06 11:37:30.000000 otree-6.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     1886 2023-03-24 17:40:32.590150 otree-6.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2022-03-03 11:49:02.000000 otree-6.0.0a4/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.377192 otree-6.0.0a4/otree/
--rw-rw-rw-   0        0        0       91 2023-03-24 17:40:03.000000 otree-6.0.0a4/otree/__init__.py
--rw-rw-rw-   0        0        0      559 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/api.py
--rw-rw-rw-   0        0        0    10085 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/api.pyi
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.392954 otree-6.0.0a4/otree/app_template/
--rw-rw-rw-   0        0        0        0 2018-11-23 17:31:44.000000 otree-6.0.0a4/otree/app_template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.400489 otree-6.0.0a4/otree/app_template/__pycache__/
--rw-rw-rw-   0        0        0      127 2017-10-09 12:58:16.000000 otree-6.0.0a4/otree/app_template/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      131 2019-07-18 16:08:18.000000 otree-6.0.0a4/otree/app_template/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1013 2017-10-09 12:58:16.000000 otree-6.0.0a4/otree/app_template/__pycache__/models.cpython-36.pyc
--rw-rw-rw-   0        0        0     1017 2019-07-18 16:08:18.000000 otree-6.0.0a4/otree/app_template/__pycache__/models.cpython-37.pyc
--rw-rw-rw-   0        0        0      615 2017-10-09 12:58:16.000000 otree-6.0.0a4/otree/app_template/__pycache__/tests.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.401707 otree-6.0.0a4/otree/app_template/_builtin/
--rw-rw-rw-   0        0        0      446 2020-10-07 12:35:10.000000 otree-6.0.0a4/otree/app_template/_builtin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.404188 otree-6.0.0a4/otree/app_template/_builtin/__pycache__/
--rw-rw-rw-   0        0        0     1170 2017-10-09 12:58:16.000000 otree-6.0.0a4/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      871 2019-07-18 16:08:18.000000 otree-6.0.0a4/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      464 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/app_template/models.py
--rw-rw-rw-   0        0        0      297 2020-10-07 12:35:10.000000 otree-6.0.0a4/otree/app_template/pages.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.324360 otree-6.0.0a4/otree/app_template/templates/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.406865 otree-6.0.0a4/otree/app_template/templates/app_name/
--rw-rw-rw-   0        0        0      200 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/app_template/templates/app_name/MyPage.html
--rw-rw-rw-   0        0        0      180 2020-12-11 18:14:00.000000 otree-6.0.0a4/otree/app_template/templates/app_name/Results.html
--rw-rw-rw-   0        0        0      200 2020-03-20 01:44:18.000000 otree-6.0.0a4/otree/app_template/tests.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.409634 otree-6.0.0a4/otree/app_template_lite/
--rw-rw-rw-   0        0        0      137 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/app_template_lite/MyPage.html
--rw-rw-rw-   0        0        0      119 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/app_template_lite/Results.html
--rw-rw-rw-   0        0        0      495 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/app_template_lite/__init__.py
--rw-rw-rw-   0        0        0     2888 2022-03-04 18:20:48.000000 otree-6.0.0a4/otree/asgi.py
--rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/auth.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.414151 otree-6.0.0a4/otree/bots/
--rw-rw-rw-   0        0        0       75 2020-03-20 01:44:18.000000 otree-6.0.0a4/otree/bots/__init__.py
--rw-rw-rw-   0        0        0    18278 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/bots/bot.py
--rw-rw-rw-   0        0        0     4815 2022-12-23 08:54:23.000000 otree-6.0.0a4/otree/bots/browser.py
--rw-rw-rw-   0        0        0    11868 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/bots/browser_launcher.py
--rw-rw-rw-   0        0        0     6713 2022-02-01 22:47:42.000000 otree-6.0.0a4/otree/bots/runner.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.418043 otree-6.0.0a4/otree/channels/
--rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/channels/__init__.py
--rw-rw-rw-   0        0        0    27401 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/channels/consumers.py
--rw-rw-rw-   0        0        0      930 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/channels/routing.py
--rw-rw-rw-   0        0        0     4489 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/channels/utils.py
--rw-rw-rw-   0        0        0     2407 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/chat.py
--rw-rw-rw-   0        0        0    10804 2022-12-23 08:54:35.000000 otree-6.0.0a4/otree/checks.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.437154 otree-6.0.0a4/otree/cli/
--rw-rw-rw-   0        0        0        0 2021-09-07 01:38:00.000000 otree-6.0.0a4/otree/cli/__init__.py
--rw-rw-rw-   0        0        0      841 2021-06-29 10:07:36.000000 otree-6.0.0a4/otree/cli/base.py
--rw-rw-rw-   0        0        0     1846 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/bots.py
--rw-rw-rw-   0        0        0     1072 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/browser_bots.py
--rw-rw-rw-   0        0        0     1337 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/create_session.py
--rw-rw-rw-   0        0        0     3402 2021-09-28 08:02:58.000000 otree-6.0.0a4/otree/cli/devserver.py
--rw-rw-rw-   0        0        0     2051 2021-09-28 08:03:24.000000 otree-6.0.0a4/otree/cli/devserver_inner.py
--rw-rw-rw-   0        0        0       35 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/prodserver.py
--rw-rw-rw-   0        0        0     1766 2021-06-30 10:11:04.000000 otree-6.0.0a4/otree/cli/prodserver1of2.py
--rw-rw-rw-   0        0        0      258 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/prodserver2of2.py
--rw-rw-rw-   0        0        0    14172 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/cli/remove_self.py
--rw-rw-rw-   0        0        0     1981 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/resetdb.py
--rw-rw-rw-   0        0        0     1957 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/cli/startapp.py
--rw-rw-rw-   0        0        0     2796 2022-12-23 08:54:35.000000 otree-6.0.0a4/otree/cli/startproject.py
--rw-rw-rw-   0        0        0      345 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/timeoutsubprocess.py
--rw-rw-rw-   0        0        0     1224 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/cli/unzip.py
--rw-rw-rw-   0        0        0     2290 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/cli/upcase_constants.py
--rw-rw-rw-   0        0        0     7229 2021-06-30 09:55:02.000000 otree-6.0.0a4/otree/cli/update_my_code.py
--rw-rw-rw-   0        0        0     7301 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/cli/zip.py
--rw-rw-rw-   0        0        0     6434 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/cli/zipserver.py
--rw-rw-rw-   0        0        0     7803 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/common.py
--rw-rw-rw-   0        0        0     4046 2021-08-28 09:53:12.000000 otree-6.0.0a4/otree/common2.py
--rw-rw-rw-   0        0        0     2511 2022-11-23 14:41:17.000000 otree-6.0.0a4/otree/constants.py
--rw-rw-rw-   0        0        0     8663 2022-09-17 23:55:17.000000 otree-6.0.0a4/otree/currency.py
--rw-rw-rw-   0        0        0    30887 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/database.py
--rw-rw-rw-   0        0        0     8278 2022-03-04 18:20:48.000000 otree-6.0.0a4/otree/errorpage.py
--rw-rw-rw-   0        0        0    16209 2022-11-23 14:41:17.000000 otree-6.0.0a4/otree/export.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.441078 otree-6.0.0a4/otree/forms/
--rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/forms/__init__.py
--rw-rw-rw-   0        0        0     3620 2022-09-19 10:51:45.000000 otree-6.0.0a4/otree/forms/fields.py
--rw-rw-rw-   0        0        0    10547 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/forms/forms.py
--rw-rw-rw-   0        0        0     7446 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/forms/widgets.py
--rw-rw-rw-   0        0        0     6841 2022-09-19 10:51:45.000000 otree-6.0.0a4/otree/i18n.py
--rw-rw-rw-   0        0        0     3662 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/live.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.441078 otree-6.0.0a4/otree/locale/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.326832 otree-6.0.0a4/otree/locale/ar/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.441078 otree-6.0.0a4/otree/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1532 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/ar/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3986 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/ar/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      120 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/babel.ini
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.327831 otree-6.0.0a4/otree/locale/cs/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.446255 otree-6.0.0a4/otree/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1409 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/cs/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3712 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/cs/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.328448 otree-6.0.0a4/otree/locale/de/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.448007 otree-6.0.0a4/otree/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1762 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3875 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/de/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     3188 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/django.pot
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.328714 otree-6.0.0a4/otree/locale/es/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.449823 otree-6.0.0a4/otree/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1567 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.329409 otree-6.0.0a4/otree/locale/fi/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.451919 otree-6.0.0a4/otree/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      497 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/fi/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3114 2021-11-29 03:59:50.000000 otree-6.0.0a4/otree/locale/fi/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.329881 otree-6.0.0a4/otree/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.453706 otree-6.0.0a4/otree/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1634 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3747 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.330438 otree-6.0.0a4/otree/locale/he/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.455570 otree-6.0.0a4/otree/locale/he/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1652 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/he/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3703 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/he/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.331162 otree-6.0.0a4/otree/locale/hi/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.457391 otree-6.0.0a4/otree/locale/hi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2206 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/hi/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4254 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/hi/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.331682 otree-6.0.0a4/otree/locale/hu/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.459043 otree-6.0.0a4/otree/locale/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1722 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/hu/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3900 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/hu/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.332325 otree-6.0.0a4/otree/locale/id/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.459043 otree-6.0.0a4/otree/locale/id/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1520 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/locale/id/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3605 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/locale/id/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.333040 otree-6.0.0a4/otree/locale/it/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.459043 otree-6.0.0a4/otree/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1620 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/it/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3733 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/it/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.333506 otree-6.0.0a4/otree/locale/ja/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.464703 otree-6.0.0a4/otree/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1747 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3826 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/ja/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.334051 otree-6.0.0a4/otree/locale/ko/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.466808 otree-6.0.0a4/otree/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1783 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/ko/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3917 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/ko/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.334668 otree-6.0.0a4/otree/locale/nb/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.468743 otree-6.0.0a4/otree/locale/nb/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1023 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/nb/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3421 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/nb/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.334940 otree-6.0.0a4/otree/locale/nl/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.470639 otree-6.0.0a4/otree/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1579 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3669 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.335628 otree-6.0.0a4/otree/locale/pl/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.472512 otree-6.0.0a4/otree/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/pl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/pl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.336470 otree-6.0.0a4/otree/locale/pt/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.473352 otree-6.0.0a4/otree/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/pt/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/pt/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.337005 otree-6.0.0a4/otree/locale/ru/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.475978 otree-6.0.0a4/otree/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2047 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4156 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/ru/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.337579 otree-6.0.0a4/otree/locale/tr/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.477628 otree-6.0.0a4/otree/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1537 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/tr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3731 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/tr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.338299 otree-6.0.0a4/otree/locale/zh_Hans/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.479600 otree-6.0.0a4/otree/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1452 2022-04-27 15:07:46.000000 otree-6.0.0a4/otree/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3521 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     2323 2021-08-31 15:42:14.000000 otree-6.0.0a4/otree/lookup.py
--rw-rw-rw-   0        0        0     6971 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/main.py
--rw-rw-rw-   0        0        0     1819 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/middleware.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.484825 otree-6.0.0a4/otree/models/
--rw-rw-rw-   0        0        0      230 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/models/__init__.py
--rw-rw-rw-   0        0        0     4133 2021-11-18 17:14:02.000000 otree-6.0.0a4/otree/models/group.py
--rw-rw-rw-   0        0        0     8714 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/models/participant.py
--rw-rw-rw-   0        0        0     3346 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/models/player.py
--rw-rw-rw-   0        0        0     9750 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/models/session.py
--rw-rw-rw-   0        0        0     9025 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/models/subsession.py
--rw-rw-rw-   0        0        0     1929 2021-08-18 09:23:18.000000 otree-6.0.0a4/otree/models_concrete.py
--rw-rw-rw-   0        0        0     7383 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/mturk_client.py
--rw-rw-rw-   0        0        0     1897 2022-03-04 18:20:48.000000 otree-6.0.0a4/otree/patch.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.489078 otree-6.0.0a4/otree/project_template/
--rw-rw-rw-   0        0        0      133 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/project_template/.gitignore
--rw-rw-rw-   0        0        0       57 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/project_template/Procfile
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.339472 otree-6.0.0a4/otree/project_template/_static/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.489078 otree-6.0.0a4/otree/project_template/_static/global/
--rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/project_template/_static/global/empty.css
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.339972 otree-6.0.0a4/otree/project_template/_templates/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.489078 otree-6.0.0a4/otree/project_template/_templates/global/
--rw-rw-rw-   0        0        0      149 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/project_template/_templates/global/Page.html
--rw-rw-rw-   0        0        0      169 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/project_template/requirements.txt
--rw-rw-rw-   0        0        0     1018 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/project_template/settings.py
--rw-rw-rw-   0        0        0     2567 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/read_csv.py
--rw-rw-rw-   0        0        0     4291 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/room.py
--rw-rw-rw-   0        0        0    15047 2022-12-23 08:54:23.000000 otree-6.0.0a4/otree/session.py
--rw-rw-rw-   0        0        0     2380 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.489078 otree-6.0.0a4/otree/static/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.341235 otree-6.0.0a4/otree/static/bootstrap5/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.489078 otree-6.0.0a4/otree/static/bootstrap5/css/
--rw-rw-rw-   0        0        0   155637 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/bootstrap5/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   429472 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/bootstrap5/css/bootstrap.min.css.map
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.497217 otree-6.0.0a4/otree/static/bootstrap5/js/
--rw-rw-rw-   0        0        0    78754 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/bootstrap5/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   326390 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0      198 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.512304 otree-6.0.0a4/otree/static/glyphicons/
--rw-rw-rw-   0        0        0     1412 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/clock.png
--rw-rw-rw-   0        0        0     1307 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/cloud.png
--rw-rw-rw-   0        0        0     1443 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/cogwheel.png
--rw-rw-rw-   0        0        0     1310 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/delete.png
--rw-rw-rw-   0        0        0     1314 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/download-alt.png
--rw-rw-rw-   0        0        0     1475 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/eye-open.png
--rw-rw-rw-   0        0        0     1243 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/folder-closed.png
--rw-rw-rw-   0        0        0     1436 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/link.png
--rw-rw-rw-   0        0        0     1231 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/list-alt.png
--rw-rw-rw-   0        0        0     1342 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/pencil.png
--rw-rw-rw-   0        0        0     1218 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/plus.png
--rw-rw-rw-   0        0        0     1378 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/pushpin.png
--rw-rw-rw-   0        0        0     1471 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/refresh.png
--rw-rw-rw-   0        0        0     1499 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/stats.png
--rw-rw-rw-   0        0        0     1432 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/glyphicons/usd.png
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.342325 otree-6.0.0a4/otree/static/otree/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.513033 otree-6.0.0a4/otree/static/otree/css/
--rw-rw-rw-   0        0        0      868 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/otree/css/table.css
--rw-rw-rw-   0        0        0     2015 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/otree/css/theme.css
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.527649 otree-6.0.0a4/otree/static/otree/js/
--rw-rw-rw-   0        0        0     1909 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/static/otree/js/common.js
--rw-rw-rw-   0        0        0     1624 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/static/otree/js/formInputs.js
--rw-rw-rw-   0        0        0      504 2020-10-07 12:35:10.000000 otree-6.0.0a4/otree/static/otree/js/internet-explorer.js
--rw-rw-rw-   0        0        0    86663 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/otree/js/jquery-3.2.1.min.js
--rw-rw-rw-   0        0        0     6605 2020-11-23 22:42:18.000000 otree-6.0.0a4/otree/static/otree/js/jquery.color-2.1.2.min.js
--rw-rw-rw-   0        0        0     5360 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/otree/js/jquery.countdown.min.js
--rw-rw-rw-   0        0        0      702 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/otree/js/jquery.timeago.en-short.js
--rw-rw-rw-   0        0        0     7200 2018-12-27 12:55:56.000000 otree-6.0.0a4/otree/static/otree/js/jquery.timeago.js
--rw-rw-rw-   0        0        0      663 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/static/otree/js/live.js
--rw-rw-rw-   0        0        0     4271 2022-11-23 14:41:17.000000 otree-6.0.0a4/otree/static/otree/js/monitor2.js
--rw-rw-rw-   0        0        0      967 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/otree/js/page-websocket-redirect.js
--rw-rw-rw-   0        0        0     8729 2020-03-20 01:44:18.000000 otree-6.0.0a4/otree/static/otree/js/reconnecting-websocket-iife.min.js
--rw-rw-rw-   0        0        0     4837 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/static/otree/js/table-utils.js
--rw-rw-rw-   0        0        0      221 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/static/otree/js/trial.js
--rw-rw-rw-   0        0        0       26 2018-11-23 17:31:48.000000 otree-6.0.0a4/otree/static/robots.txt
--rw-rw-rw-   0        0        0     5360 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/tasks.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.343209 otree-6.0.0a4/otree/templates/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.529299 otree-6.0.0a4/otree/templates/global/
--rw-rw-rw-   0        0        0       33 2020-12-01 22:34:50.000000 otree-6.0.0a4/otree/templates/global/Base.html
--rw-rw-rw-   0        0        0      293 2021-10-18 21:34:16.000000 otree-6.0.0a4/otree/templates/global/Page.html
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.560431 otree-6.0.0a4/otree/templates/otree/
--rw-rw-rw-   0        0        0      881 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/AdminReport.html
--rw-rw-rw-   0        0        0     1659 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/templates/otree/Base.html
--rw-rw-rw-   0        0        0     3065 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/BaseAdmin.html
--rw-rw-rw-   0        0        0     2881 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/CreateDemoSession.html
--rw-rw-rw-   0        0        0      199 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/CreateSession.html
--rw-rw-rw-   0        0        0      955 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/DemoIndex.html
--rw-rw-rw-   0        0        0     5961 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templates/otree/Export.html
--rw-rw-rw-   0        0        0       31 2020-12-01 22:34:50.000000 otree-6.0.0a4/otree/templates/otree/FormPage.html
--rw-rw-rw-   0        0        0     1240 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/Login.html
--rw-rw-rw-   0        0        0     2796 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templates/otree/MTurkCreateHIT.html
--rw-rw-rw-   0        0        0     1214 2020-12-01 22:34:50.000000 otree-6.0.0a4/otree/templates/otree/MTurkHTMLQuestion.html
--rw-rw-rw-   0        0        0     6732 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templates/otree/MTurkSessionPayments.html
--rw-rw-rw-   0        0        0       18 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/OutOfRangeNotification.html
--rw-rw-rw-   0        0        0     2716 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/templates/otree/Page.html
--rw-rw-rw-   0        0        0      911 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/templates/otree/RoomInputLabel.html
--rw-rw-rw-   0        0        0      754 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/RoomWithSession.html
--rw-rw-rw-   0        0        0     4282 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/RoomWithoutSession.html
--rw-rw-rw-   0        0        0      353 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/Rooms.html
--rw-rw-rw-   0        0        0     1784 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templates/otree/ServerCheck.html
--rw-rw-rw-   0        0        0     2532 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/Session.html
--rw-rw-rw-   0        0        0     7856 2021-08-19 09:01:20.000000 otree-6.0.0a4/otree/templates/otree/SessionData.html
--rw-rw-rw-   0        0        0      139 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/SessionDescription.html
--rw-rw-rw-   0        0        0      323 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/SessionEditProperties.html
--rw-rw-rw-   0        0        0     2391 2022-11-23 14:41:17.000000 otree-6.0.0a4/otree/templates/otree/SessionMonitor.html
--rw-rw-rw-   0        0        0     1582 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/SessionPayments.html
--rw-rw-rw-   0        0        0     3329 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/SessionSplitScreen.html
--rw-rw-rw-   0        0        0     4087 2021-09-02 00:40:54.000000 otree-6.0.0a4/otree/templates/otree/SessionStartLinks.html
--rw-rw-rw-   0        0        0     5469 2022-05-14 06:42:33.000000 otree-6.0.0a4/otree/templates/otree/Sessions.html
--rw-rw-rw-   0        0        0     5121 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templates/otree/WaitPage.html
--rw-rw-rw-   0        0        0       37 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/WaitPageRoom.html
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.569383 otree-6.0.0a4/otree/templates/otree/includes/
--rw-rw-rw-   0        0        0     5461 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/CreateSessionForm.html
--rw-rw-rw-   0        0        0     1528 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/RoomParticipantLinks.html
--rw-rw-rw-   0        0        0      402 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/SessionInfo.html
--rw-rw-rw-   0        0        0      213 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/TimeLimit.html
--rw-rw-rw-   0        0        0      997 2022-07-06 11:50:24.000000 otree-6.0.0a4/otree/templates/otree/includes/TimeLimit.js.html
--rw-rw-rw-   0        0        0      969 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/debug_info.html
--rw-rw-rw-   0        0        0     2679 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templates/otree/includes/hidden_form_errors.html
--rw-rw-rw-   0        0        0      244 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/messages.html
--rw-rw-rw-   0        0        0     1368 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templates/otree/includes/mturk_payment_table.html
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.570325 otree-6.0.0a4/otree/templates/otree/tags/
--rw-rw-rw-   0        0        0     3572 2021-09-09 20:27:16.000000 otree-6.0.0a4/otree/templates/otree/tags/chat.html
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.578806 otree-6.0.0a4/otree/templating/
--rw-rw-rw-   0        0        0       70 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templating/__init__.py
--rw-rw-rw-   0        0        0     6993 2021-09-10 18:14:58.000000 otree-6.0.0a4/otree/templating/compiler.py
--rw-rw-rw-   0        0        0     2948 2021-09-23 22:55:28.000000 otree-6.0.0a4/otree/templating/context.py
--rw-rw-rw-   0        0        0     1342 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templating/errors.py
--rw-rw-rw-   0        0        0     2081 2021-08-11 02:49:06.000000 otree-6.0.0a4/otree/templating/filters.py
--rw-rw-rw-   0        0        0     3392 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/templating/loader.py
--rw-rw-rw-   0        0        0    33506 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/templating/nodes.py
--rw-rw-rw-   0        0        0     1495 2021-09-10 17:48:20.000000 otree-6.0.0a4/otree/templating/template.py
--rw-rw-rw-   0        0        0     1836 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/templating/utils.py
--rw-rw-rw-   0        0        0      173 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/test.py
--rw-rw-rw-   0        0        0     3114 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/trial.py
--rw-rw-rw-   0        0        0     1919 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/update.py
--rw-rw-rw-   0        0        0     4635 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.588981 otree-6.0.0a4/otree/views/
--rw-rw-rw-   0        0        0       49 2020-06-23 01:10:42.000000 otree-6.0.0a4/otree/views/__init__.py
--rw-rw-rw-   0        0        0    48941 2023-03-24 17:39:59.000000 otree-6.0.0a4/otree/views/abstract.py
--rw-rw-rw-   0        0        0    19290 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/views/admin.py
--rw-rw-rw-   0        0        0     8261 2022-03-03 11:49:02.000000 otree-6.0.0a4/otree/views/cbv.py
--rw-rw-rw-   0        0        0     1537 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/views/demo.py
--rw-rw-rw-   0        0        0     3722 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/views/export.py
--rw-rw-rw-   0        0        0    14856 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/views/mturk.py
--rw-rw-rw-   0        0        0    12981 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/views/participant.py
--rw-rw-rw-   0        0        0    10004 2023-03-08 18:09:53.000000 otree-6.0.0a4/otree/views/rest.py
--rw-rw-rw-   0        0        0     2523 2021-06-06 11:37:30.000000 otree-6.0.0a4/otree/views/room.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:40:32.388707 otree-6.0.0a4/otree.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-03-24 17:40:32.000000 otree-6.0.0a4/otree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7956 2023-03-24 17:40:32.000000 otree-6.0.0a4/otree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 17:40:32.000000 otree-6.0.0a4/otree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-03-24 17:40:32.000000 otree-6.0.0a4/otree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-11-22 05:26:26.000000 otree-6.0.0a4/otree.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      196 2023-03-24 17:40:32.000000 otree-6.0.0a4/otree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-24 17:40:32.000000 otree-6.0.0a4/otree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      311 2023-03-08 18:09:53.000000 otree-6.0.0a4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 17:40:32.591560 otree-6.0.0a4/setup.cfg
--rw-rw-rw-   0        0        0     2548 2023-03-08 18:09:53.000000 otree-6.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:21.367780 otree-6.0.0a5/
+-rw-rw-rw-   0        0        0     1573 2018-11-23 17:31:44.000000 otree-6.0.0a5/LICENSE
+-rw-rw-rw-   0        0        0      390 2021-06-06 11:37:30.000000 otree-6.0.0a5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1886 2023-04-14 19:47:21.366778 otree-6.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2022-03-03 11:49:02.000000 otree-6.0.0a5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.593481 otree-6.0.0a5/otree/
+-rw-rw-rw-   0        0        0       91 2023-04-14 19:47:13.000000 otree-6.0.0a5/otree/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/api.py
+-rw-rw-rw-   0        0        0    10085 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/api.pyi
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.657820 otree-6.0.0a5/otree/app_template/
+-rw-rw-rw-   0        0        0        0 2018-11-23 17:31:44.000000 otree-6.0.0a5/otree/app_template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.666370 otree-6.0.0a5/otree/app_template/__pycache__/
+-rw-rw-rw-   0        0        0      127 2017-10-09 12:58:16.000000 otree-6.0.0a5/otree/app_template/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      131 2019-07-18 16:08:18.000000 otree-6.0.0a5/otree/app_template/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1013 2017-10-09 12:58:16.000000 otree-6.0.0a5/otree/app_template/__pycache__/models.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1017 2019-07-18 16:08:18.000000 otree-6.0.0a5/otree/app_template/__pycache__/models.cpython-37.pyc
+-rw-rw-rw-   0        0        0      615 2017-10-09 12:58:16.000000 otree-6.0.0a5/otree/app_template/__pycache__/tests.cpython-36.pyc
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.672384 otree-6.0.0a5/otree/app_template/_builtin/
+-rw-rw-rw-   0        0        0      446 2020-10-07 12:35:10.000000 otree-6.0.0a5/otree/app_template/_builtin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.677363 otree-6.0.0a5/otree/app_template/_builtin/__pycache__/
+-rw-rw-rw-   0        0        0     1170 2017-10-09 12:58:16.000000 otree-6.0.0a5/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      871 2019-07-18 16:08:18.000000 otree-6.0.0a5/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      464 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/app_template/models.py
+-rw-rw-rw-   0        0        0      297 2020-10-07 12:35:10.000000 otree-6.0.0a5/otree/app_template/pages.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.328650 otree-6.0.0a5/otree/app_template/templates/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.689215 otree-6.0.0a5/otree/app_template/templates/app_name/
+-rw-rw-rw-   0        0        0      200 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/app_template/templates/app_name/MyPage.html
+-rw-rw-rw-   0        0        0      180 2020-12-11 18:14:00.000000 otree-6.0.0a5/otree/app_template/templates/app_name/Results.html
+-rw-rw-rw-   0        0        0      200 2020-03-20 01:44:18.000000 otree-6.0.0a5/otree/app_template/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.716515 otree-6.0.0a5/otree/app_template_lite/
+-rw-rw-rw-   0        0        0      137 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/app_template_lite/MyPage.html
+-rw-rw-rw-   0        0        0      119 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/app_template_lite/Results.html
+-rw-rw-rw-   0        0        0      495 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/app_template_lite/__init__.py
+-rw-rw-rw-   0        0        0     2888 2022-03-04 18:20:48.000000 otree-6.0.0a5/otree/asgi.py
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/auth.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.769285 otree-6.0.0a5/otree/bots/
+-rw-rw-rw-   0        0        0       75 2020-03-20 01:44:18.000000 otree-6.0.0a5/otree/bots/__init__.py
+-rw-rw-rw-   0        0        0    18278 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/bots/bot.py
+-rw-rw-rw-   0        0        0     4815 2022-12-23 08:54:23.000000 otree-6.0.0a5/otree/bots/browser.py
+-rw-rw-rw-   0        0        0    11868 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/bots/browser_launcher.py
+-rw-rw-rw-   0        0        0     6713 2022-02-01 22:47:42.000000 otree-6.0.0a5/otree/bots/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.794634 otree-6.0.0a5/otree/channels/
+-rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/channels/__init__.py
+-rw-rw-rw-   0        0        0    27401 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/channels/consumers.py
+-rw-rw-rw-   0        0        0      930 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/channels/routing.py
+-rw-rw-rw-   0        0        0     4489 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/channels/utils.py
+-rw-rw-rw-   0        0        0     2407 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/chat.py
+-rw-rw-rw-   0        0        0    10804 2022-12-23 08:54:35.000000 otree-6.0.0a5/otree/checks.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.963417 otree-6.0.0a5/otree/cli/
+-rw-rw-rw-   0        0        0        0 2021-09-07 01:38:00.000000 otree-6.0.0a5/otree/cli/__init__.py
+-rw-rw-rw-   0        0        0      841 2021-06-29 10:07:36.000000 otree-6.0.0a5/otree/cli/base.py
+-rw-rw-rw-   0        0        0     1846 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/bots.py
+-rw-rw-rw-   0        0        0     1072 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/browser_bots.py
+-rw-rw-rw-   0        0        0     1337 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/create_session.py
+-rw-rw-rw-   0        0        0     3402 2021-09-28 08:02:58.000000 otree-6.0.0a5/otree/cli/devserver.py
+-rw-rw-rw-   0        0        0     2051 2021-09-28 08:03:24.000000 otree-6.0.0a5/otree/cli/devserver_inner.py
+-rw-rw-rw-   0        0        0       35 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/prodserver.py
+-rw-rw-rw-   0        0        0     1766 2021-06-30 10:11:04.000000 otree-6.0.0a5/otree/cli/prodserver1of2.py
+-rw-rw-rw-   0        0        0      258 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/prodserver2of2.py
+-rw-rw-rw-   0        0        0    14172 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/cli/remove_self.py
+-rw-rw-rw-   0        0        0     1981 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/resetdb.py
+-rw-rw-rw-   0        0        0     1957 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/cli/startapp.py
+-rw-rw-rw-   0        0        0     2796 2022-12-23 08:54:35.000000 otree-6.0.0a5/otree/cli/startproject.py
+-rw-rw-rw-   0        0        0      345 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/timeoutsubprocess.py
+-rw-rw-rw-   0        0        0     1224 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/cli/unzip.py
+-rw-rw-rw-   0        0        0     2290 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/cli/upcase_constants.py
+-rw-rw-rw-   0        0        0     7229 2021-06-30 09:55:02.000000 otree-6.0.0a5/otree/cli/update_my_code.py
+-rw-rw-rw-   0        0        0     7301 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/cli/zip.py
+-rw-rw-rw-   0        0        0     6434 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/cli/zipserver.py
+-rw-rw-rw-   0        0        0     7803 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/common.py
+-rw-rw-rw-   0        0        0     4046 2021-08-28 09:53:12.000000 otree-6.0.0a5/otree/common2.py
+-rw-rw-rw-   0        0        0     2511 2022-11-23 14:41:17.000000 otree-6.0.0a5/otree/constants.py
+-rw-rw-rw-   0        0        0     8663 2022-09-17 23:55:17.000000 otree-6.0.0a5/otree/currency.py
+-rw-rw-rw-   0        0        0    30887 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/database.py
+-rw-rw-rw-   0        0        0     8278 2022-03-04 18:20:48.000000 otree-6.0.0a5/otree/errorpage.py
+-rw-rw-rw-   0        0        0    16209 2022-11-23 14:41:17.000000 otree-6.0.0a5/otree/export.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.003686 otree-6.0.0a5/otree/forms/
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/forms/__init__.py
+-rw-rw-rw-   0        0        0     3620 2022-09-19 10:51:45.000000 otree-6.0.0a5/otree/forms/fields.py
+-rw-rw-rw-   0        0        0    10547 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/forms/forms.py
+-rw-rw-rw-   0        0        0     7446 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/forms/widgets.py
+-rw-rw-rw-   0        0        0     6841 2022-09-19 10:51:45.000000 otree-6.0.0a5/otree/i18n.py
+-rw-rw-rw-   0        0        0     3662 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/live.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.025193 otree-6.0.0a5/otree/locale/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.331789 otree-6.0.0a5/otree/locale/ar/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.049298 otree-6.0.0a5/otree/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1532 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3986 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/ar/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      120 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/babel.ini
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.333580 otree-6.0.0a5/otree/locale/cs/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.072712 otree-6.0.0a5/otree/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1409 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3712 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/cs/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.333580 otree-6.0.0a5/otree/locale/de/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.090496 otree-6.0.0a5/otree/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1762 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3875 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     3188 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/django.pot
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.334712 otree-6.0.0a5/otree/locale/es/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.108803 otree-6.0.0a5/otree/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1567 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.335712 otree-6.0.0a5/otree/locale/fi/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.128301 otree-6.0.0a5/otree/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      497 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3114 2021-11-29 03:59:50.000000 otree-6.0.0a5/otree/locale/fi/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.336228 otree-6.0.0a5/otree/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.148722 otree-6.0.0a5/otree/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1634 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3747 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.336472 otree-6.0.0a5/otree/locale/he/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.165380 otree-6.0.0a5/otree/locale/he/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1652 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/he/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3703 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/he/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.337763 otree-6.0.0a5/otree/locale/hi/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.181023 otree-6.0.0a5/otree/locale/hi/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2206 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4254 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/hi/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.337763 otree-6.0.0a5/otree/locale/hu/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.197006 otree-6.0.0a5/otree/locale/hu/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1722 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3900 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/hu/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.337763 otree-6.0.0a5/otree/locale/id/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.218375 otree-6.0.0a5/otree/locale/id/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1520 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/locale/id/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3605 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/locale/id/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.339254 otree-6.0.0a5/otree/locale/it/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.237408 otree-6.0.0a5/otree/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1620 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/it/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3733 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/it/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.340533 otree-6.0.0a5/otree/locale/ja/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.259443 otree-6.0.0a5/otree/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1747 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3826 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/ja/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.340533 otree-6.0.0a5/otree/locale/ko/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.277483 otree-6.0.0a5/otree/locale/ko/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1783 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3917 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/ko/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.341566 otree-6.0.0a5/otree/locale/nb/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.299432 otree-6.0.0a5/otree/locale/nb/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1023 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3421 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/nb/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.341566 otree-6.0.0a5/otree/locale/nl/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.320011 otree-6.0.0a5/otree/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1579 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3669 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.342564 otree-6.0.0a5/otree/locale/pl/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.342328 otree-6.0.0a5/otree/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/pl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.342564 otree-6.0.0a5/otree/locale/pt/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.366366 otree-6.0.0a5/otree/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/pt/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.343563 otree-6.0.0a5/otree/locale/ru/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.391284 otree-6.0.0a5/otree/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2047 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4156 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/ru/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.343563 otree-6.0.0a5/otree/locale/tr/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.414540 otree-6.0.0a5/otree/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1537 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3731 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/tr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.344565 otree-6.0.0a5/otree/locale/zh_Hans/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.438681 otree-6.0.0a5/otree/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1452 2022-04-27 15:07:46.000000 otree-6.0.0a5/otree/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3521 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     2323 2021-08-31 15:42:14.000000 otree-6.0.0a5/otree/lookup.py
+-rw-rw-rw-   0        0        0     6971 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/main.py
+-rw-rw-rw-   0        0        0     1819 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.529595 otree-6.0.0a5/otree/models/
+-rw-rw-rw-   0        0        0      230 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/models/__init__.py
+-rw-rw-rw-   0        0        0     4133 2021-11-18 17:14:02.000000 otree-6.0.0a5/otree/models/group.py
+-rw-rw-rw-   0        0        0     8714 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/models/participant.py
+-rw-rw-rw-   0        0        0     3346 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/models/player.py
+-rw-rw-rw-   0        0        0     9750 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/models/session.py
+-rw-rw-rw-   0        0        0     9025 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/models/subsession.py
+-rw-rw-rw-   0        0        0     1929 2021-08-18 09:23:18.000000 otree-6.0.0a5/otree/models_concrete.py
+-rw-rw-rw-   0        0        0     7383 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/mturk_client.py
+-rw-rw-rw-   0        0        0     1897 2022-03-04 18:20:48.000000 otree-6.0.0a5/otree/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.558266 otree-6.0.0a5/otree/project_template/
+-rw-rw-rw-   0        0        0      133 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/project_template/.gitignore
+-rw-rw-rw-   0        0        0       57 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/project_template/Procfile
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.344565 otree-6.0.0a5/otree/project_template/_static/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.560666 otree-6.0.0a5/otree/project_template/_static/global/
+-rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/project_template/_static/global/empty.css
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.345564 otree-6.0.0a5/otree/project_template/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.565672 otree-6.0.0a5/otree/project_template/_templates/global/
+-rw-rw-rw-   0        0        0      149 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/project_template/_templates/global/Page.html
+-rw-rw-rw-   0        0        0      169 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/project_template/requirements.txt
+-rw-rw-rw-   0        0        0     1018 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/project_template/settings.py
+-rw-rw-rw-   0        0        0     2567 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/read_csv.py
+-rw-rw-rw-   0        0        0     4291 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/room.py
+-rw-rw-rw-   0        0        0    15047 2022-12-23 08:54:23.000000 otree-6.0.0a5/otree/session.py
+-rw-rw-rw-   0        0        0     2380 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.572101 otree-6.0.0a5/otree/static/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.345564 otree-6.0.0a5/otree/static/bootstrap5/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.595092 otree-6.0.0a5/otree/static/bootstrap5/css/
+-rw-rw-rw-   0        0        0   155637 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/bootstrap5/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   429472 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/bootstrap5/css/bootstrap.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.604191 otree-6.0.0a5/otree/static/bootstrap5/js/
+-rw-rw-rw-   0        0        0    78754 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/bootstrap5/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   326390 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0      198 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.635307 otree-6.0.0a5/otree/static/glyphicons/
+-rw-rw-rw-   0        0        0     1412 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/clock.png
+-rw-rw-rw-   0        0        0     1307 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/cloud.png
+-rw-rw-rw-   0        0        0     1443 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/cogwheel.png
+-rw-rw-rw-   0        0        0     1310 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/delete.png
+-rw-rw-rw-   0        0        0     1314 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/download-alt.png
+-rw-rw-rw-   0        0        0     1475 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/eye-open.png
+-rw-rw-rw-   0        0        0     1243 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/folder-closed.png
+-rw-rw-rw-   0        0        0     1436 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/link.png
+-rw-rw-rw-   0        0        0     1231 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/list-alt.png
+-rw-rw-rw-   0        0        0     1342 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/pencil.png
+-rw-rw-rw-   0        0        0     1218 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/plus.png
+-rw-rw-rw-   0        0        0     1378 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/pushpin.png
+-rw-rw-rw-   0        0        0     1471 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/refresh.png
+-rw-rw-rw-   0        0        0     1499 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/stats.png
+-rw-rw-rw-   0        0        0     1432 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/glyphicons/usd.png
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.346565 otree-6.0.0a5/otree/static/otree/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.644631 otree-6.0.0a5/otree/static/otree/css/
+-rw-rw-rw-   0        0        0      868 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/otree/css/table.css
+-rw-rw-rw-   0        0        0     2015 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/otree/css/theme.css
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.754442 otree-6.0.0a5/otree/static/otree/js/
+-rw-rw-rw-   0        0        0     1909 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/static/otree/js/common.js
+-rw-rw-rw-   0        0        0     1624 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/static/otree/js/formInputs.js
+-rw-rw-rw-   0        0        0      504 2020-10-07 12:35:10.000000 otree-6.0.0a5/otree/static/otree/js/internet-explorer.js
+-rw-rw-rw-   0        0        0    86663 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/otree/js/jquery-3.2.1.min.js
+-rw-rw-rw-   0        0        0     6605 2020-11-23 22:42:18.000000 otree-6.0.0a5/otree/static/otree/js/jquery.color-2.1.2.min.js
+-rw-rw-rw-   0        0        0     5360 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/otree/js/jquery.countdown.min.js
+-rw-rw-rw-   0        0        0      702 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/otree/js/jquery.timeago.en-short.js
+-rw-rw-rw-   0        0        0     7200 2018-12-27 12:55:56.000000 otree-6.0.0a5/otree/static/otree/js/jquery.timeago.js
+-rw-rw-rw-   0        0        0      663 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/static/otree/js/live.js
+-rw-rw-rw-   0        0        0     4271 2022-11-23 14:41:17.000000 otree-6.0.0a5/otree/static/otree/js/monitor2.js
+-rw-rw-rw-   0        0        0    49487 2023-04-14 19:41:59.000000 otree-6.0.0a5/otree/static/otree/js/otree-front.js
+-rw-rw-rw-   0        0        0      967 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/otree/js/page-websocket-redirect.js
+-rw-rw-rw-   0        0        0     8729 2020-03-20 01:44:18.000000 otree-6.0.0a5/otree/static/otree/js/reconnecting-websocket-iife.min.js
+-rw-rw-rw-   0        0        0     4837 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/static/otree/js/table-utils.js
+-rw-rw-rw-   0        0        0      827 2023-04-14 18:32:21.000000 otree-6.0.0a5/otree/static/otree/js/trial-default.js
+-rw-rw-rw-   0        0        0      221 2023-04-14 15:42:00.000000 otree-6.0.0a5/otree/static/otree/js/trial-setup.js
+-rw-rw-rw-   0        0        0       26 2018-11-23 17:31:48.000000 otree-6.0.0a5/otree/static/robots.txt
+-rw-rw-rw-   0        0        0     5360 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/tasks.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.346565 otree-6.0.0a5/otree/templates/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:20.772048 otree-6.0.0a5/otree/templates/global/
+-rw-rw-rw-   0        0        0       33 2020-12-01 22:34:50.000000 otree-6.0.0a5/otree/templates/global/Base.html
+-rw-rw-rw-   0        0        0      293 2021-10-18 21:34:16.000000 otree-6.0.0a5/otree/templates/global/Page.html
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:21.063680 otree-6.0.0a5/otree/templates/otree/
+-rw-rw-rw-   0        0        0      881 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/AdminReport.html
+-rw-rw-rw-   0        0        0     1659 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/templates/otree/Base.html
+-rw-rw-rw-   0        0        0     3065 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/BaseAdmin.html
+-rw-rw-rw-   0        0        0     2881 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/CreateDemoSession.html
+-rw-rw-rw-   0        0        0      199 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/CreateSession.html
+-rw-rw-rw-   0        0        0      955 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/DemoIndex.html
+-rw-rw-rw-   0        0        0     5961 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templates/otree/Export.html
+-rw-rw-rw-   0        0        0       31 2020-12-01 22:34:50.000000 otree-6.0.0a5/otree/templates/otree/FormPage.html
+-rw-rw-rw-   0        0        0     1240 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/Login.html
+-rw-rw-rw-   0        0        0     2796 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templates/otree/MTurkCreateHIT.html
+-rw-rw-rw-   0        0        0     1214 2020-12-01 22:34:50.000000 otree-6.0.0a5/otree/templates/otree/MTurkHTMLQuestion.html
+-rw-rw-rw-   0        0        0     6732 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templates/otree/MTurkSessionPayments.html
+-rw-rw-rw-   0        0        0       18 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/OutOfRangeNotification.html
+-rw-rw-rw-   0        0        0     2844 2023-04-14 19:03:05.000000 otree-6.0.0a5/otree/templates/otree/Page.html
+-rw-rw-rw-   0        0        0      911 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/templates/otree/RoomInputLabel.html
+-rw-rw-rw-   0        0        0      754 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/RoomWithSession.html
+-rw-rw-rw-   0        0        0     4282 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/RoomWithoutSession.html
+-rw-rw-rw-   0        0        0      353 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/Rooms.html
+-rw-rw-rw-   0        0        0     1784 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templates/otree/ServerCheck.html
+-rw-rw-rw-   0        0        0     2532 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/Session.html
+-rw-rw-rw-   0        0        0     7856 2021-08-19 09:01:20.000000 otree-6.0.0a5/otree/templates/otree/SessionData.html
+-rw-rw-rw-   0        0        0      139 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/SessionDescription.html
+-rw-rw-rw-   0        0        0      323 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/SessionEditProperties.html
+-rw-rw-rw-   0        0        0     2391 2022-11-23 14:41:17.000000 otree-6.0.0a5/otree/templates/otree/SessionMonitor.html
+-rw-rw-rw-   0        0        0     1582 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/SessionPayments.html
+-rw-rw-rw-   0        0        0     3329 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/SessionSplitScreen.html
+-rw-rw-rw-   0        0        0     4087 2021-09-02 00:40:54.000000 otree-6.0.0a5/otree/templates/otree/SessionStartLinks.html
+-rw-rw-rw-   0        0        0     5469 2022-05-14 06:42:33.000000 otree-6.0.0a5/otree/templates/otree/Sessions.html
+-rw-rw-rw-   0        0        0     5121 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templates/otree/WaitPage.html
+-rw-rw-rw-   0        0        0       37 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/WaitPageRoom.html
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:21.149328 otree-6.0.0a5/otree/templates/otree/includes/
+-rw-rw-rw-   0        0        0     5461 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/CreateSessionForm.html
+-rw-rw-rw-   0        0        0     1528 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/RoomParticipantLinks.html
+-rw-rw-rw-   0        0        0      402 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/SessionInfo.html
+-rw-rw-rw-   0        0        0      213 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/TimeLimit.html
+-rw-rw-rw-   0        0        0      997 2022-07-06 11:50:24.000000 otree-6.0.0a5/otree/templates/otree/includes/TimeLimit.js.html
+-rw-rw-rw-   0        0        0      969 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/debug_info.html
+-rw-rw-rw-   0        0        0     2679 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templates/otree/includes/hidden_form_errors.html
+-rw-rw-rw-   0        0        0      244 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/messages.html
+-rw-rw-rw-   0        0        0     1368 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templates/otree/includes/mturk_payment_table.html
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:21.167804 otree-6.0.0a5/otree/templates/otree/tags/
+-rw-rw-rw-   0        0        0     3572 2021-09-09 20:27:16.000000 otree-6.0.0a5/otree/templates/otree/tags/chat.html
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:21.245386 otree-6.0.0a5/otree/templating/
+-rw-rw-rw-   0        0        0       70 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templating/__init__.py
+-rw-rw-rw-   0        0        0     6993 2021-09-10 18:14:58.000000 otree-6.0.0a5/otree/templating/compiler.py
+-rw-rw-rw-   0        0        0     2948 2021-09-23 22:55:28.000000 otree-6.0.0a5/otree/templating/context.py
+-rw-rw-rw-   0        0        0     1342 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templating/errors.py
+-rw-rw-rw-   0        0        0     2081 2021-08-11 02:49:06.000000 otree-6.0.0a5/otree/templating/filters.py
+-rw-rw-rw-   0        0        0     3392 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/templating/loader.py
+-rw-rw-rw-   0        0        0    33506 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/templating/nodes.py
+-rw-rw-rw-   0        0        0     1495 2021-09-10 17:48:20.000000 otree-6.0.0a5/otree/templating/template.py
+-rw-rw-rw-   0        0        0     1836 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/templating/utils.py
+-rw-rw-rw-   0        0        0      173 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/test.py
+-rw-rw-rw-   0        0        0     3108 2023-04-14 19:46:28.000000 otree-6.0.0a5/otree/trial.py
+-rw-rw-rw-   0        0        0     1919 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/update.py
+-rw-rw-rw-   0        0        0     4635 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:21.365896 otree-6.0.0a5/otree/views/
+-rw-rw-rw-   0        0        0       49 2020-06-23 01:10:42.000000 otree-6.0.0a5/otree/views/__init__.py
+-rw-rw-rw-   0        0        0    48941 2023-03-24 17:39:59.000000 otree-6.0.0a5/otree/views/abstract.py
+-rw-rw-rw-   0        0        0    19290 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/views/admin.py
+-rw-rw-rw-   0        0        0     8261 2022-03-03 11:49:02.000000 otree-6.0.0a5/otree/views/cbv.py
+-rw-rw-rw-   0        0        0     1537 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/views/demo.py
+-rw-rw-rw-   0        0        0     3722 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/views/export.py
+-rw-rw-rw-   0        0        0    14856 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/views/mturk.py
+-rw-rw-rw-   0        0        0    12981 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/views/participant.py
+-rw-rw-rw-   0        0        0    10004 2023-03-08 18:09:53.000000 otree-6.0.0a5/otree/views/rest.py
+-rw-rw-rw-   0        0        0     2523 2021-06-06 11:37:30.000000 otree-6.0.0a5/otree/views/room.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:47:19.629253 otree-6.0.0a5/otree.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-04-14 19:47:19.000000 otree-6.0.0a5/otree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8038 2023-04-14 19:47:19.000000 otree-6.0.0a5/otree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 19:47:19.000000 otree-6.0.0a5/otree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-14 19:47:19.000000 otree-6.0.0a5/otree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-11-22 05:26:26.000000 otree-6.0.0a5/otree.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      196 2023-04-14 19:47:19.000000 otree-6.0.0a5/otree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 19:47:19.000000 otree-6.0.0a5/otree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      311 2023-03-08 18:09:53.000000 otree-6.0.0a5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 19:47:21.367780 otree-6.0.0a5/setup.cfg
+-rw-rw-rw-   0        0        0     2548 2023-03-08 18:09:53.000000 otree-6.0.0a5/setup.py
```

### Comparing `otree-6.0.0a4/LICENSE` & `otree-6.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/PKG-INFO` & `otree-6.0.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otree
-Version: 6.0.0a4
+Version: 6.0.0a5
 Summary: Framework for multiplayer strategy games and complex surveys.
 Home-page: http://otree.org/
 Author: chris@otree.org
 Author-email: chris@otree.org
 License: MIT License
 Platform: UNKNOWN
 Provides-Extra: mturk
```

### Comparing `otree-6.0.0a4/README.rst` & `otree-6.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/api.py` & `otree-6.0.0a5/otree/api.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/api.pyi` & `otree-6.0.0a5/otree/api.pyi`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/app_template/__pycache__/models.cpython-36.pyc` & `otree-6.0.0a5/otree/app_template/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/app_template/__pycache__/models.cpython-37.pyc` & `otree-6.0.0a5/otree/app_template/__pycache__/models.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/app_template/__pycache__/tests.cpython-36.pyc` & `otree-6.0.0a5/otree/app_template/__pycache__/tests.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc` & `otree-6.0.0a5/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc` & `otree-6.0.0a5/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/asgi.py` & `otree-6.0.0a5/otree/asgi.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/bots/bot.py` & `otree-6.0.0a5/otree/bots/bot.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/bots/browser.py` & `otree-6.0.0a5/otree/bots/browser.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/bots/browser_launcher.py` & `otree-6.0.0a5/otree/bots/browser_launcher.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/bots/runner.py` & `otree-6.0.0a5/otree/bots/runner.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/channels/consumers.py` & `otree-6.0.0a5/otree/channels/consumers.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/channels/routing.py` & `otree-6.0.0a5/otree/channels/routing.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/channels/utils.py` & `otree-6.0.0a5/otree/channels/utils.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/chat.py` & `otree-6.0.0a5/otree/chat.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/checks.py` & `otree-6.0.0a5/otree/checks.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/base.py` & `otree-6.0.0a5/otree/cli/base.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/bots.py` & `otree-6.0.0a5/otree/cli/bots.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/browser_bots.py` & `otree-6.0.0a5/otree/cli/browser_bots.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/create_session.py` & `otree-6.0.0a5/otree/cli/create_session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/devserver.py` & `otree-6.0.0a5/otree/cli/devserver.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/devserver_inner.py` & `otree-6.0.0a5/otree/cli/devserver_inner.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/prodserver1of2.py` & `otree-6.0.0a5/otree/cli/prodserver1of2.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/remove_self.py` & `otree-6.0.0a5/otree/cli/remove_self.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/resetdb.py` & `otree-6.0.0a5/otree/cli/resetdb.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/startapp.py` & `otree-6.0.0a5/otree/cli/startapp.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/startproject.py` & `otree-6.0.0a5/otree/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/unzip.py` & `otree-6.0.0a5/otree/cli/unzip.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/upcase_constants.py` & `otree-6.0.0a5/otree/cli/upcase_constants.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/update_my_code.py` & `otree-6.0.0a5/otree/cli/update_my_code.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/zip.py` & `otree-6.0.0a5/otree/cli/zip.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/cli/zipserver.py` & `otree-6.0.0a5/otree/cli/zipserver.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/common.py` & `otree-6.0.0a5/otree/common.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/common2.py` & `otree-6.0.0a5/otree/common2.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/constants.py` & `otree-6.0.0a5/otree/constants.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/currency.py` & `otree-6.0.0a5/otree/currency.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/database.py` & `otree-6.0.0a5/otree/database.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/errorpage.py` & `otree-6.0.0a5/otree/errorpage.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/export.py` & `otree-6.0.0a5/otree/export.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/forms/fields.py` & `otree-6.0.0a5/otree/forms/fields.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/forms/forms.py` & `otree-6.0.0a5/otree/forms/forms.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/forms/widgets.py` & `otree-6.0.0a5/otree/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/i18n.py` & `otree-6.0.0a5/otree/i18n.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/live.py` & `otree-6.0.0a5/otree/live.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ar/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ar/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/cs/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/cs/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/de/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/de/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/django.pot` & `otree-6.0.0a5/otree/locale/django.pot`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/es/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/es/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/fi/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/fr/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/fr/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/he/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/he/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/hi/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/hi/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/hu/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/hu/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/id/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/id/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/it/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/it/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ja/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ja/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ko/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ko/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/nb/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/nb/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/nl/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/nl/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/pl/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/pl/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/pt/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/pt/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ru/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/ru/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/tr/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/tr/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/zh_Hans/LC_MESSAGES/django.mo` & `otree-6.0.0a5/otree/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/locale/zh_Hans/LC_MESSAGES/django.po` & `otree-6.0.0a5/otree/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/lookup.py` & `otree-6.0.0a5/otree/lookup.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/main.py` & `otree-6.0.0a5/otree/main.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/middleware.py` & `otree-6.0.0a5/otree/middleware.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/models/group.py` & `otree-6.0.0a5/otree/models/group.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/models/participant.py` & `otree-6.0.0a5/otree/models/participant.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/models/player.py` & `otree-6.0.0a5/otree/models/player.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/models/session.py` & `otree-6.0.0a5/otree/models/session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/models/subsession.py` & `otree-6.0.0a5/otree/models/subsession.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/models_concrete.py` & `otree-6.0.0a5/otree/models_concrete.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/mturk_client.py` & `otree-6.0.0a5/otree/mturk_client.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/patch.py` & `otree-6.0.0a5/otree/patch.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/project_template/settings.py` & `otree-6.0.0a5/otree/project_template/settings.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/read_csv.py` & `otree-6.0.0a5/otree/read_csv.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/room.py` & `otree-6.0.0a5/otree/room.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/session.py` & `otree-6.0.0a5/otree/session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/settings.py` & `otree-6.0.0a5/otree/settings.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/bootstrap5/css/bootstrap.min.css` & `otree-6.0.0a5/otree/static/bootstrap5/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/bootstrap5/css/bootstrap.min.css.map` & `otree-6.0.0a5/otree/static/bootstrap5/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/bootstrap5/js/bootstrap.bundle.min.js` & `otree-6.0.0a5/otree/static/bootstrap5/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map` & `otree-6.0.0a5/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/clock.png` & `otree-6.0.0a5/otree/static/glyphicons/clock.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/cloud.png` & `otree-6.0.0a5/otree/static/glyphicons/cloud.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/cogwheel.png` & `otree-6.0.0a5/otree/static/glyphicons/cogwheel.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/delete.png` & `otree-6.0.0a5/otree/static/glyphicons/delete.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/download-alt.png` & `otree-6.0.0a5/otree/static/glyphicons/download-alt.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/eye-open.png` & `otree-6.0.0a5/otree/static/glyphicons/eye-open.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/folder-closed.png` & `otree-6.0.0a5/otree/static/glyphicons/folder-closed.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/link.png` & `otree-6.0.0a5/otree/static/glyphicons/link.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/list-alt.png` & `otree-6.0.0a5/otree/static/glyphicons/list-alt.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/pencil.png` & `otree-6.0.0a5/otree/static/glyphicons/pencil.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/plus.png` & `otree-6.0.0a5/otree/static/glyphicons/plus.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/pushpin.png` & `otree-6.0.0a5/otree/static/glyphicons/pushpin.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/refresh.png` & `otree-6.0.0a5/otree/static/glyphicons/refresh.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/stats.png` & `otree-6.0.0a5/otree/static/glyphicons/stats.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/glyphicons/usd.png` & `otree-6.0.0a5/otree/static/glyphicons/usd.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/css/table.css` & `otree-6.0.0a5/otree/static/otree/css/table.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/css/theme.css` & `otree-6.0.0a5/otree/static/otree/css/theme.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/common.js` & `otree-6.0.0a5/otree/static/otree/js/common.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/formInputs.js` & `otree-6.0.0a5/otree/static/otree/js/formInputs.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/jquery-3.2.1.min.js` & `otree-6.0.0a5/otree/static/otree/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/jquery.color-2.1.2.min.js` & `otree-6.0.0a5/otree/static/otree/js/jquery.color-2.1.2.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/jquery.countdown.min.js` & `otree-6.0.0a5/otree/static/otree/js/jquery.countdown.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/jquery.timeago.en-short.js` & `otree-6.0.0a5/otree/static/otree/js/jquery.timeago.en-short.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/jquery.timeago.js` & `otree-6.0.0a5/otree/static/otree/js/jquery.timeago.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/live.js` & `otree-6.0.0a5/otree/static/otree/js/live.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/monitor2.js` & `otree-6.0.0a5/otree/static/otree/js/monitor2.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/page-websocket-redirect.js` & `otree-6.0.0a5/otree/static/otree/js/page-websocket-redirect.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/reconnecting-websocket-iife.min.js` & `otree-6.0.0a5/otree/static/otree/js/reconnecting-websocket-iife.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/static/otree/js/table-utils.js` & `otree-6.0.0a5/otree/static/otree/js/table-utils.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/tasks.py` & `otree-6.0.0a5/otree/tasks.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/AdminReport.html` & `otree-6.0.0a5/otree/templates/otree/AdminReport.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/Base.html` & `otree-6.0.0a5/otree/templates/otree/Base.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/BaseAdmin.html` & `otree-6.0.0a5/otree/templates/otree/BaseAdmin.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/CreateDemoSession.html` & `otree-6.0.0a5/otree/templates/otree/CreateDemoSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/DemoIndex.html` & `otree-6.0.0a5/otree/templates/otree/DemoIndex.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/Export.html` & `otree-6.0.0a5/otree/templates/otree/Export.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/Login.html` & `otree-6.0.0a5/otree/templates/otree/Login.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/MTurkCreateHIT.html` & `otree-6.0.0a5/otree/templates/otree/MTurkCreateHIT.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/MTurkHTMLQuestion.html` & `otree-6.0.0a5/otree/templates/otree/MTurkHTMLQuestion.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/MTurkSessionPayments.html` & `otree-6.0.0a5/otree/templates/otree/MTurkSessionPayments.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/Page.html` & `otree-6.0.0a5/otree/templates/otree/Page.html`

 * *Files 6% similar despite different names*

```diff
@@ -57,11 +57,13 @@
     <script src="{% static 'otree/js/live.js' %}" id="otree-live" data-socket-url="{{ view.live_url() }}"></script>
   {% endif %}
 {% endblock %}
 
 
 {% block trial %}
   {% if has_trial %}
-    <script>var _TRIALS = {{ trials_json }}; var _trials_use_roundtrip_mode = {{ _trials_use_roundtrip_mode }}</script>
-    <script src="{% static 'otree/js/trial.js' %}" id="otree-trial" data-socket-url="{{ view.trial_url() }}"></script>
+    <script>var TRIALS = {{ trials_json }}; var _TRIALS_SSE = {{ _trials_use_roundtrip_mode }}</script>
+    <script src="{% static 'otree/js/trial-setup.js' %}" id="otree-trial" data-socket-url="{{ view.trial_url() }}"></script>
+    <script src="{% static 'otree/js/otree-front.js' %}"></script>
+    <script src="{% static 'otree/js/trial-default.js' %}"></script>
   {% endif %}
 {% endblock %}
```

### Comparing `otree-6.0.0a4/otree/templates/otree/RoomInputLabel.html` & `otree-6.0.0a5/otree/templates/otree/RoomInputLabel.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/RoomWithSession.html` & `otree-6.0.0a5/otree/templates/otree/RoomWithSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/RoomWithoutSession.html` & `otree-6.0.0a5/otree/templates/otree/RoomWithoutSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/ServerCheck.html` & `otree-6.0.0a5/otree/templates/otree/ServerCheck.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/Session.html` & `otree-6.0.0a5/otree/templates/otree/Session.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/SessionData.html` & `otree-6.0.0a5/otree/templates/otree/SessionData.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/SessionMonitor.html` & `otree-6.0.0a5/otree/templates/otree/SessionMonitor.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/SessionPayments.html` & `otree-6.0.0a5/otree/templates/otree/SessionPayments.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/SessionSplitScreen.html` & `otree-6.0.0a5/otree/templates/otree/SessionSplitScreen.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/SessionStartLinks.html` & `otree-6.0.0a5/otree/templates/otree/SessionStartLinks.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/Sessions.html` & `otree-6.0.0a5/otree/templates/otree/Sessions.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/WaitPage.html` & `otree-6.0.0a5/otree/templates/otree/WaitPage.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/includes/CreateSessionForm.html` & `otree-6.0.0a5/otree/templates/otree/includes/CreateSessionForm.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/includes/RoomParticipantLinks.html` & `otree-6.0.0a5/otree/templates/otree/includes/RoomParticipantLinks.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/includes/TimeLimit.js.html` & `otree-6.0.0a5/otree/templates/otree/includes/TimeLimit.js.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/includes/debug_info.html` & `otree-6.0.0a5/otree/templates/otree/includes/debug_info.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/includes/hidden_form_errors.html` & `otree-6.0.0a5/otree/templates/otree/includes/hidden_form_errors.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/includes/mturk_payment_table.html` & `otree-6.0.0a5/otree/templates/otree/includes/mturk_payment_table.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templates/otree/tags/chat.html` & `otree-6.0.0a5/otree/templates/otree/tags/chat.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/compiler.py` & `otree-6.0.0a5/otree/templating/compiler.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/context.py` & `otree-6.0.0a5/otree/templating/context.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/errors.py` & `otree-6.0.0a5/otree/templating/errors.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/filters.py` & `otree-6.0.0a5/otree/templating/filters.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/loader.py` & `otree-6.0.0a5/otree/templating/loader.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/nodes.py` & `otree-6.0.0a5/otree/templating/nodes.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/template.py` & `otree-6.0.0a5/otree/templating/template.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/templating/utils.py` & `otree-6.0.0a5/otree/templating/utils.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/trial.py` & `otree-6.0.0a5/otree/trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import logging
 from otree.database import NoResultFound
 
 logger = logging.getLogger(__name__)
 
 
 async def trial_payload_function(participant_code, page_name, msg):
-
     try:
         participant = Participant.objects_get(code=participant_code)
     except NoResultFound:
         logger.warning(f'Participant not found: {participant_code}')
         return
     lookup = get_page_lookup(participant._session_code, participant._index_in_pages)
     app_name = lookup.app_name
@@ -27,15 +26,14 @@
         return
 
     player = models_module.Player.objects_get(
         round_number=lookup.round_number, participant=participant
     )
     Trial = PageClass.trial_model
     trial = get_current_trial(Trial, player)
-
     resp = dict(is_page_load=msg['type'] == 'load')
     if trial and msg['type'] == 'response':
         assert trial.id == msg['trial_id']
         response = msg['response']
         if hasattr(PageClass, 'evaluate_trial'):
             feedback = PageClass.evaluate_trial(trial, response)
         else:
@@ -48,15 +46,14 @@
         resp.update(feedback=feedback)
         trial = get_current_trial(Trial, player)
     if trial:
         resp.update(trial=encode_trial(trial, PageClass.trial_stimulus_fields))
     else:
         resp.update(trial=None)
     resp.update(progress=get_progress(Trial, player))
-
     await _send_back(
         participant.code,
         participant._index_in_pages,
         resp,
     )
```

### Comparing `otree-6.0.0a4/otree/update.py` & `otree-6.0.0a5/otree/update.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/urls.py` & `otree-6.0.0a5/otree/urls.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/abstract.py` & `otree-6.0.0a5/otree/views/abstract.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/admin.py` & `otree-6.0.0a5/otree/views/admin.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/cbv.py` & `otree-6.0.0a5/otree/views/cbv.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/demo.py` & `otree-6.0.0a5/otree/views/demo.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/export.py` & `otree-6.0.0a5/otree/views/export.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/mturk.py` & `otree-6.0.0a5/otree/views/mturk.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/participant.py` & `otree-6.0.0a5/otree/views/participant.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/rest.py` & `otree-6.0.0a5/otree/views/rest.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree/views/room.py` & `otree-6.0.0a5/otree/views/room.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a4/otree.egg-info/PKG-INFO` & `otree-6.0.0a5/otree.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otree
-Version: 6.0.0a4
+Version: 6.0.0a5
 Summary: Framework for multiplayer strategy games and complex surveys.
 Home-page: http://otree.org/
 Author: chris@otree.org
 Author-email: chris@otree.org
 License: MIT License
 Platform: UNKNOWN
 Provides-Extra: mturk
```

### Comparing `otree-6.0.0a4/otree.egg-info/SOURCES.txt` & `otree-6.0.0a5/otree.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -174,18 +174,20 @@
 otree/static/otree/js/jquery-3.2.1.min.js
 otree/static/otree/js/jquery.color-2.1.2.min.js
 otree/static/otree/js/jquery.countdown.min.js
 otree/static/otree/js/jquery.timeago.en-short.js
 otree/static/otree/js/jquery.timeago.js
 otree/static/otree/js/live.js
 otree/static/otree/js/monitor2.js
+otree/static/otree/js/otree-front.js
 otree/static/otree/js/page-websocket-redirect.js
 otree/static/otree/js/reconnecting-websocket-iife.min.js
 otree/static/otree/js/table-utils.js
-otree/static/otree/js/trial.js
+otree/static/otree/js/trial-default.js
+otree/static/otree/js/trial-setup.js
 otree/templates/global/Base.html
 otree/templates/global/Page.html
 otree/templates/otree/AdminReport.html
 otree/templates/otree/Base.html
 otree/templates/otree/BaseAdmin.html
 otree/templates/otree/CreateDemoSession.html
 otree/templates/otree/CreateSession.html
```

### Comparing `otree-6.0.0a4/setup.py` & `otree-6.0.0a5/setup.py`

 * *Files identical despite different names*

