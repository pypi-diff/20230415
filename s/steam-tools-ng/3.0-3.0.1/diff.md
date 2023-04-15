# Comparing `tmp/steam-tools-ng-3.0.tar.gz` & `tmp/steam-tools-ng-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-tools-ng-3.0.tar", last modified: Tue Apr  4 10:05:58 2023, max compression
+gzip compressed data, was "steam-tools-ng-3.0.1.tar", last modified: Sat Apr 15 21:17:06 2023, max compression
```

## Comparing `steam-tools-ng-3.0.tar` & `steam-tools-ng-3.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.336256 steam-tools-ng-3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-04 10:05:58.332256 steam-tools-ng-3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3419 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.328256 steam-tools-ng-3.0/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/i18n/fr.po
--rwxr-xr-x   0 runner    (1001) docker     (123)    45277 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/i18n/pt_BR.po
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 10:05:58.336256 steam-tools-ng-3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     6250 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.328256 steam-tools-ng-3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.328256 steam-tools-ng-3.0/src/steam_tools_ng/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.328256 steam-tools-ng-3.0/src/steam_tools_ng/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/console/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/console/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/console/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/console/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.332256 steam-tools-ng-3.0/src/steam_tools_ng/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/cardfarming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/confirmations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/coupons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/fakerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/steamgifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/steamguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/steamtrades.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.332256 steam-tools-ng-3.0/src/steam_tools_ng/gtk/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/async_gtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/confirmation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24002 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37846 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gtk/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.332256 steam-tools-ng-3.0/src/steam_tools_ng/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/icons/stng.ico
--rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/icons/stng.png
--rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_console.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_console.png
--rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_nc.ico
--rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_nc.png
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/logger_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/src/steam_tools_ng/steam_api_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.328256 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-04 10:05:58.000000 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-04 10:05:58.000000 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:05:58.000000 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-04 10:05:58.000000 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-04 10:05:58.000000 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 10:05:58.000000 steam-tools-ng-3.0/src/steam_tools_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/steam-tools-ng.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:05:58.332256 steam-tools-ng-3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 10:05:40.000000 steam-tools-ng-3.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/i18n/fr.po
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45277 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/i18n/pt_BR.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6250 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/steam_tools_ng/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/steam_tools_ng/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/src/steam_tools_ng/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/cardfarming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/confirmations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/coupons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/fakerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamgifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamtrades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/async_gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38037 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.png
+-rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.png
+-rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/logger_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/steam_api_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/steam-tools-ng.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/tests/test_placeholder.py
```

### Comparing `steam-tools-ng-3.0/LICENSE` & `steam-tools-ng-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/PKG-INFO` & `steam-tools-ng-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.0
+Version: 3.0.1
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
@@ -56,15 +56,15 @@
 
 * More (**Coming Soon**)
 
 Graphical User Interface
 -------------
 
 ```
-Just run and follow on-screen instructions
+Just run steam-tools-ng-gui and follow on-screen instructions
 ```
 
 Command Line Interface
 -----------------
 ```
 usage: steam-tools-ng [-h] [--reset] [--reset-password] [--add-authenticator] [-v] [<module>]
```

### Comparing `steam-tools-ng-3.0/README.md` & `steam-tools-ng-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 * More (**Coming Soon**)
 
 Graphical User Interface
 -------------
 
 ```
-Just run and follow on-screen instructions
+Just run steam-tools-ng-gui and follow on-screen instructions
 ```
 
 Command Line Interface
 -----------------
 ```
 usage: steam-tools-ng [-h] [--reset] [--reset-password] [--add-authenticator] [-v] [<module>]
```

### Comparing `steam-tools-ng-3.0/i18n/fr.po` & `steam-tools-ng-3.0.1/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/i18n/pt_BR.po` & `steam-tools-ng-3.0.1/i18n/pt_BR.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/pyproject.toml` & `steam-tools-ng-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "certifi", "cx_Freeze; sys_platform == 'win32'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "steam-tools-ng"
-version = "3.0"
+version = "3.0.1"
 description = "Steam Tools NG"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
```

### Comparing `steam-tools-ng-3.0/setup.py` & `steam-tools-ng-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/__init__.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/__main__.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/__main__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/cli.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/cli.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/config.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/config.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/console/authenticator.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/console/authenticator.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/console/cli.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/console/cli.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/console/login.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/console/login.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/console/utils.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/console/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/__init__.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/cardfarming.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/cardfarming.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/confirmations.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/confirmations.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,34 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
+
 import logging
-from typing import AsyncGenerator
+from typing import AsyncGenerator, Callable, Awaitable
+
+import aiohttp
 
 from stlib import login, universe, community
 from . import utils
 from .. import i18n, config
 
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
 
 
-async def main(steamid: universe.SteamId) -> AsyncGenerator[utils.ModuleData, None]:
+async def main(
+        steamid: universe.SteamId,
+        wait_available: Callable[[], Awaitable[None]],
+) -> AsyncGenerator[utils.ModuleData, None]:
+    await wait_available()
+
     identity_secret = config.parser.get("login", "identity_secret")
     session = community.Community.get_session(0)
 
     if not identity_secret:
         config.new("confirmations", "enable", "false")
         module_data = utils.ModuleData(error=_("The current identity secret is invalid."), info=_("Waiting Changes"))
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/coupons.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/coupons.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,34 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
 import asyncio
 import logging
-from typing import AsyncGenerator
+from typing import AsyncGenerator, Callable, Awaitable
+
+import aiohttp
 
 from stlib import universe, community, internals, webapi
 from . import utils
 from .. import i18n, config
 
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
 
 
-async def main(steamid: universe.SteamId, fetch_coupon_event: asyncio.Event) -> AsyncGenerator[utils.ModuleData, None]:
+async def main(
+        steamid: universe.SteamId,
+        fetch_coupon_event: asyncio.Event,
+        wait_available: Callable[[], Awaitable[None]],
+) -> AsyncGenerator[utils.ModuleData, None]:
+    await wait_available()
     await fetch_coupon_event.wait()
 
     community_session = community.Community.get_session(0)
     internals_session = internals.Internals.get_session(0)
     webapi_session = webapi.SteamWebAPI.get_session(0)
     botids = config.parser.get('coupons', 'botids')
     tokens = config.parser.get('coupons', 'tokens')
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/fakerun.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/fakerun.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/steamgifts.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamgifts.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/steamguard.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamguard.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/steamtrades.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamtrades.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/core/utils.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/core/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/__init__.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/about.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/about.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/application.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,17 +195,15 @@
 
                         if module_name in ["steamgifts", "steamtrades"]:
                             plugin = plugins.get_plugin(module_name)
 
                             with contextlib.suppress(IndexError):
                                 await plugin.Main.new_session(0)
 
-                        if module_name == "coupons":
-                            task = asyncio.create_task(module(self.main_window.fetch_coupon_event))
-                        elif module_name == "confirmations":
+                        if module_name in ["coupons", "confirmations"]:
                             task = asyncio.create_task(module())
                         else:
                             self.main_window.set_status(module_name, status=_("Loading"))
                             play_event = self.main_window.get_play_event(module_name)
                             task = asyncio.create_task(module(play_event))
 
                         log.debug(_("Adding a new callback for %s"), task)
@@ -253,26 +251,25 @@
                     await play_event.wait()
 
                     for executor in executors:
                         executor.__init__(executor.appid)
 
     @while_window_realized
     async def run_confirmations(self) -> None:
-        confirmations = core.confirmations.main(self.steamid)
+        wait_available = self.main_window.confirmations_tree.wait_available
+        confirmations = core.confirmations.main(self.steamid, wait_available)
 
         async for module_data in confirmations:
+            await wait_available()
+
             if module_data.error:
                 self.main_window.statusbar.set_critical('confirmations', module_data.error)
             else:
                 self.main_window.statusbar.clear('confirmations')
 
-            if self.main_window.confirmations_tree.lock:
-                await self.main_window.confirmations_tree.wait_available()
-                continue
-
             if module_data.action == "login":
                 await self.do_login(auto=True)
                 continue
 
             if module_data.action == "update":
                 self.main_window.statusbar.set_warning("confirmations", "Updating now!")
                 if module_data.raw_data == self.old_confirmations:
@@ -300,20 +297,23 @@
                         row = ['', '', '', item[0], '-->', item[1] if item[1] else 'Nothing']
                         self.main_window.confirmations_tree.store.append(iter_, row)
 
                 self.old_confirmations = module_data.raw_data
                 self.main_window.statusbar.clear('confirmations')
 
     @while_window_realized
-    async def run_coupons(self, play_event: asyncio.Event) -> None:
-        coupons = core.coupons.main(self.steamid, self.main_window.fetch_coupon_event)
+    async def run_coupons(self) -> None:
+        fetch_coupon_event = self.main_window.fetch_coupon_event
+        wait_available = self.main_window.coupons_tree.wait_available
+        coupons = core.coupons.main(self.steamid, fetch_coupon_event, wait_available)
 
         async for module_data in coupons:
             self.main_window.statusbar.clear("coupons")
-            await play_event.wait()
+            await wait_available()
+            await fetch_coupon_event.wait()
 
             if module_data.error:
                 self.main_window.statusbar.set_critical("coupons", module_data.error)
 
             if module_data.info:
                 self.main_window.statusbar.set_warning("coupons", module_data.info)
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/async_gtk.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/async_gtk.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/authenticator.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/authenticator.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/confirmation.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/confirmation.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         self.content_area.set_margin_end(10)
         self.content_area.set_margin_top(10)
         self.content_area.set_margin_bottom(10)
 
         self.status = utils.SimpleStatus()
         self.content_area.append(self.status)
 
+        self.progress = Gtk.LevelBar()
+        self.content_area.append(self.progress)
+
         self.yes_button = Gtk.Button()
         self.yes_button.set_label(_("Continue"))
         self.yes_button.connect("clicked", self.on_yes_button_clicked)
         self.header_bar.pack_end(self.yes_button)
 
         self.no_button = Gtk.Button()
         self.no_button.set_label(_("Cancel"))
@@ -101,15 +104,15 @@
             self.content_area.append(self.give_label)
 
             self.receive_label = Gtk.Label()
             self.content_area.append(self.receive_label)
 
             self.give_label.set_markup(
                 utils.markup(
-                    _("You are trading the following items with {}:").format(self.model[self.iter][4]),
+                    _("You are trading the following items with {}:").format(utils.unmarkup(self.model[self.iter][4])),
                     color='blue',
                 )
             )
 
             self.status.info(_("Do you really want to {} that?\nIt can't be undone!").format(self.action.upper()))
 
             self.grid = Gtk.Grid()
@@ -129,28 +132,25 @@
             utils.copy_childrens(self.model, self.receive_tree.store, self.iter, 5)
 
         self.connect('response', lambda dialog, response_id: self.destroy())
 
     def on_yes_button_clicked(self, button: Gtk.Button) -> None:
         button.hide()
         self.no_button.hide()
-
-        with contextlib.suppress(AttributeError):
-            self.give_label.hide()
-            self.give_tree.hide()
-            self.arrow.hide()
-            self.receive_tree.hide()
-
-        self.set_size_request(0, 0)
+        self.set_size_request(300, 60)
         self.header_bar.set_show_title_buttons(False)
         self.parent_window.confirmations_tree.lock = True
+
         loop = asyncio.get_event_loop()
         task: asyncio.Task[Union[Dict[str, Any], List[Tuple[Gtk.TreeIter, Dict[str, Any]]]]]
 
         if self.iter:
+            self.content_area.remove(self.grid)
+            self.content_area.remove(self.give_label)
+            self.content_area.remove(self.receive_label)
             task = loop.create_task(self.finalize())
         else:
             task = loop.create_task(self.batch_finalize())
 
         task.add_done_callback(self.on_task_finish)
 
     def on_task_finish(self, task: asyncio.Task[Any]) -> None:
@@ -188,14 +188,15 @@
             steamid = universe.generate_steamid(steamid_raw)
         except ValueError:
             self.status.info(_("Your steam is invalid. (are you logged in?)"))
             await asyncio.sleep(5)
             return {}
 
         self.status.info(_("Waiting Steam Server (OP: {})").format(self.model[self.iter][1]))
+        result: Dict[str, Any] = {}
 
         # steam confirmation server isn't reliable
         for i in range(2):
             result = await self.community_session.send_confirmation(
                 identity_secret,
                 steamid,
                 deviceid,
@@ -207,35 +208,27 @@
 
         if not keep_iter:
             try:
                 self.model.remove(self.iter)
             except IndexError:
                 log.debug(_("Unable to remove tree path %s (already removed?). Ignoring."), self.iter)
 
-        # noinspection PyUnboundLocalVariable
         assert isinstance(result, dict)
         return result
 
     async def batch_finalize(self) -> List[Tuple[Gtk.TreeIter, Dict[str, Any]]]:
         results = []
         self.status.info(_("Waiting Steam Server response"))
-        progress = Gtk.LevelBar()
-        self.content_area.append(progress)
-
         confirmation_count = len(self.model)
 
         for index in range(confirmation_count):
             self.iter = self.model[index].iter
 
-            try:
-                progress.set_value(index)
-                progress.set_max_value(confirmation_count)
-            except KeyError:
-                progress.set_value(0)
-                progress.set_max_value(0)
+            self.progress.set_value(index)
+            self.progress.set_max_value(confirmation_count)
 
             result = await self.finalize(True)
             results.append((self.iter, result))
 
         self.status.info(_("Updating tree"))
         for iter_, result in results:
             self.model.remove(iter_)
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/coupon.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/coupon.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 import asyncio
 import logging
 import time
-from gi.repository import Gtk
 from typing import Union, Optional, Any
 
+from gi.repository import Gtk
+
 from stlib import community
 from stlib import universe
 from . import utils, confirmation
 from .. import config, i18n
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/login.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/login.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/settings.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/settings.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/utils.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
             if fixed_width:
                 column.set_fixed_width(fixed_width)
 
             self._view.append_column(column)
 
     async def wait_available(self) -> None:
-        while self.lock:
+        while self.lock or self.disabled:
             await asyncio.sleep(1)
 
     @property
     def lock(self) -> bool:
         return self._lock
 
     @lock.setter
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gtk/window.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -624,20 +624,20 @@
 
         self.statusbar = utils.StatusBar()
         main_grid.attach(self.statusbar, 1, 3, 1, 1)
 
         self.connect("destroy", self.application.on_exit_activate)
         self.connect("close-request", self.application.on_exit_activate)
 
-        loop = asyncio.get_event_loop()
+        self.loop = asyncio.get_event_loop()
 
-        plugin_status_task = loop.create_task(self.plugin_status())
+        plugin_status_task = self.loop.create_task(self.plugin_status())
         plugin_status_task.add_done_callback(utils.safe_task_callback)
 
-        user_info_task = loop.create_task(self.user_info())
+        user_info_task = self.loop.create_task(self.user_info())
         user_info_task.add_done_callback(utils.safe_task_callback)
 
     @property
     def theme(self) -> str:
         return config.parser.get('general', 'theme')
 
     async def user_info(self) -> None:
@@ -707,17 +707,19 @@
                         tree.disabled = True
                         main.set_sensitive(False)
                 else:
                     enabled = config.parser.getboolean(plugin_name, "enable")
                     status = getattr(self, f'{plugin_name}_status')
 
                     if not enabled:
-                        await asyncio.sleep(5)
-                        status.set_status(_("Disabled"))
-                        status.set_info("")
+                        def disabled_callback(status_) -> None:
+                            status_.set_status(_("Disabled"))
+                            status_.set_info("")
+
+                        self.loop.call_later(3, disabled_callback, status)
 
             await asyncio.sleep(3)
 
     @staticmethod
     def on_query_confirmations_tooltip(
             tree_view: Gtk.TreeView,
             x_coord: int,
@@ -742,14 +744,16 @@
         return False
 
     def on_fetch_coupons(self, button: Gtk.Button) -> None:
         self.fetch_coupon_event.set()
 
     def on_stop_fetching_coupons(self, button: Gtk.Button) -> None:
         self.fetch_coupon_event.clear()
+        self.coupon_progress.set_value(0)
+        self.coupon_progress.set_max_value(0)
 
     def on_coupon_action(self, button: Gtk.Button, model: Union[Gtk.TreeModel, Gtk.TreeSelection] = None) -> None:
         if model:
             coupon_dialog = coupon.CouponDialog(self, self.application, *model.get_selected())
         else:
             coupon_dialog = coupon.CouponDialog(self, self.application)
 
@@ -905,8 +909,8 @@
         config.new("login", "password", "")
 
         def reset_password_callback() -> None:
             login_dialog.destroy()
             self.destroy()
 
         login_dialog.status.info(_("Successful!\nExiting..."))
-        asyncio.get_event_loop().call_later(3, reset_password_callback)
+        self.loop.call_later(3, reset_password_callback)
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/gui.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/gui.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/i18n.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/i18n.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/icons/stng.ico` & `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/icons/stng.png` & `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_console.ico` & `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_console.png` & `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_nc.ico` & `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/icons/stng_nc.png` & `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/logger_handlers.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/logger_handlers.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng/steam_api_executor.py` & `steam-tools-ng-3.0.1/src/steam_tools_ng/steam_api_executor.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng.egg-info/PKG-INFO` & `steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.0
+Version: 3.0.1
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
@@ -56,15 +56,15 @@
 
 * More (**Coming Soon**)
 
 Graphical User Interface
 -------------
 
 ```
-Just run and follow on-screen instructions
+Just run steam-tools-ng-gui and follow on-screen instructions
 ```
 
 Command Line Interface
 -----------------
 ```
 usage: steam-tools-ng [-h] [--reset] [--reset-password] [--add-authenticator] [-v] [<module>]
```

### Comparing `steam-tools-ng-3.0/src/steam_tools_ng.egg-info/SOURCES.txt` & `steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

