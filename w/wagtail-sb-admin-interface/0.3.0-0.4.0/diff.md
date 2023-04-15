# Comparing `tmp/wagtail_sb_admin_interface-0.3.0.tar.gz` & `tmp/wagtail_sb_admin_interface-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_admin_interface-0.3.0.tar", max compression
+gzip compressed data, was "wagtail_sb_admin_interface-0.4.0.tar", max compression
```

## Comparing `wagtail_sb_admin_interface-0.3.0.tar` & `wagtail_sb_admin_interface-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0      403 2023-02-23 01:01:28.388440 wagtail_sb_admin_interface-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-02-22 19:43:45.772297 wagtail_sb_admin_interface-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2605 2023-02-23 00:58:02.675253 wagtail_sb_admin_interface-0.3.0/README.md
--rw-r--r--   0        0        0     1942 2023-02-23 01:01:28.384440 wagtail_sb_admin_interface-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      216 2023-02-22 22:54:53.731936 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/__init__.py
--rw-r--r--   0        0        0     4840 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/admin.py
--rw-r--r--   0        0        0      716 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/apps.py
--rw-r--r--   0        0        0      533 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/cache.py
--rw-r--r--   0        0        0      336 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/compat.py
--rw-r--r--   0        0        0     6472 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py
--rw-r--r--   0        0        0     3602 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py
--rw-r--r--   0        0        0      389 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0003_remove_theme_sidebar_logo_background_color.py
--rw-r--r--   0        0        0     2040 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py
--rw-r--r--   0        0        0      484 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0005_rename_sidebar_logo_mobile_theme_sidebar_logo_collapsed.py
--rw-r--r--   0        0        0      606 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/__init__.py
--rw-r--r--   0        0        0     8365 2023-02-23 00:52:09.944694 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/models.py
--rw-r--r--   0        0        0     1192 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/settings.py
--rw-r--r--   0        0        0     2798 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/templatetags/__init__.py
--rw-r--r--   0        0        0     2783 2023-02-22 22:55:26.220082 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/tests.py
--rw-r--r--   0        0        0       20 2023-02-23 01:01:28.392440 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/version.py
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/views.py
--rw-r--r--   0        0        0      817 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/wagtail_hooks.py
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 wagtail_sb_admin_interface-0.3.0/setup.py
--rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 wagtail_sb_admin_interface-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      562 2023-04-15 07:12:58.612149 wagtail_sb_admin_interface-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-02-22 19:43:45.772297 wagtail_sb_admin_interface-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1915 2023-04-15 07:11:11.123751 wagtail_sb_admin_interface-0.4.0/README.md
+-rw-r--r--   0        0        0     2056 2023-04-15 07:12:58.612149 wagtail_sb_admin_interface-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      216 2023-02-22 22:54:53.731936 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/__init__.py
+-rw-r--r--   0        0        0     4840 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/admin.py
+-rw-r--r--   0        0        0      716 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/apps.py
+-rw-r--r--   0        0        0      533 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/cache.py
+-rw-r--r--   0        0        0      336 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/compat.py
+-rw-r--r--   0        0        0     6472 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3602 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py
+-rw-r--r--   0        0        0      389 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0003_remove_theme_sidebar_logo_background_color.py
+-rw-r--r--   0        0        0     2040 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py
+-rw-r--r--   0        0        0      484 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0005_rename_sidebar_logo_mobile_theme_sidebar_logo_collapsed.py
+-rw-r--r--   0        0        0      606 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/__init__.py
+-rw-r--r--   0        0        0     8365 2023-02-23 01:02:30.680771 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/models.py
+-rw-r--r--   0        0        0     1192 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/settings.py
+-rw-r--r--   0        0        0     2798 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templatetags/__init__.py
+-rw-r--r--   0        0        0     2783 2023-02-22 22:55:26.220082 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/tests.py
+-rw-r--r--   0        0        0       20 2023-04-15 07:12:58.616149 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/version.py
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/views.py
+-rw-r--r--   0        0        0      817 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/wagtail_hooks.py
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 wagtail_sb_admin_interface-0.4.0/PKG-INFO
```

### Comparing `wagtail_sb_admin_interface-0.3.0/LICENSE.txt` & `wagtail_sb_admin_interface-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/README.md` & `wagtail_sb_admin_interface-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-admin-interface)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-admin-interface)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-admin-interface)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-admin-interface)
 
-[![Build Status](https://www.travis-ci.org/softbutterfly/wagtail-sb-admin-interface.svg?branch=develop)](https://www.travis-ci.org/softbutterfly/wagtail-sb-admin-interface)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e35e7095857b416696eb58a4ed5d9a15)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-admin-interface/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=softbutterfly/wagtail-sb-admin-interface&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge Coverage](https://app.codacy.com/project/badge/Coverage/e35e7095857b416696eb58a4ed5d9a15)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-admin-interface/dashboard?utm_source=github.com&utm_medium=referral&utm_content=softbutterfly/wagtail-sb-admin-interface&utm_campaign=Badge_Coverage)
-[![codecov](https://codecov.io/gh/softbutterfly/wagtail-sb-admin-interface/branch/master/graph/badge.svg?token=pbqXUUOu1F)](https://codecov.io/gh/softbutterfly/wagtail-sb-admin-interface)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/f28072e8e0ac4605bd3235b7643929ad)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-admin-interface/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 # Wagtail Admin Interface
 
 Customize the Wagtail admin interface from the admin itself.
 
 Inspired by [django-admin-interface](https://github.com/fabiocaccamo/django-admin-interface).
 
@@ -41,21 +38,21 @@
   "colorfield",
   # ...
 ]
 ```
 
 ## Docs
 
-- [Ejemplos](https://github.com/softbutterfly/wagtail-sb-admin-interface/wiki)
-- [Wiki](https://github.com/softbutterfly/wagtail-sb-admin-interface/wiki)
+- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis)
+- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis)
 
 ## Changelog
 
 All changes to versions of this library are listed in the [change history](CHANGELOG.md).
 
 ## Development
 
 Check out our [contribution guide](CONTRIBUTING.md).
 
 ## Contributors
 
-See the list of contributors [here](https://github.com/softbutterfly/wagtail-sb-admin-interface/graphs/contributors).
+See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/graphs/develop).
```

### Comparing `wagtail_sb_admin_interface-0.3.0/pyproject.toml` & `wagtail_sb_admin_interface-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "wagtail-sb-admin-interface"
-version = "0.3.0"
+version = "0.4.0"
 description = "Social Networks settings for wagtail sites."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
-homepage = "https://github.com/softbutterfly/wagtail-sb-admin-interface"
-repository = "https://github.com/softbutterfly/wagtail-sb-admin-interface"
-documentation = "https://github.com/softbutterfly/wagtail-sb-admin-interface/wiki"
+homepage = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
+repository = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
+documentation = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis"
 keywords = ["Softbutterfly", "Django", "Migrations"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
@@ -28,29 +28,28 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://github.com/softbutterfly/wagtail-sb-admin-interface/archive/v0.3.0.tar.gz"
-"Bug Tracker" = "https://github.com/softbutterfly/wagtail-sb-admin-interface/issues"
-
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/archive/v0.4.0/wagtail-sb-admin-interface-v0.4.0.tar.gz"
+"Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 django = "< 5.0"
 django-colorfield = "<1.0.0"
 wagtail = "< 5.0"
+wagtail-sb-fontawesome = "<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
 bandit = "^1.7.4"
 black = "^23.1.0"
-codecov = "^2.1.12"
 coverage = "^7.1.0"
 flake8 = "^6.0.0"
 flake8-black = "^0.3.6"
 isort = "^5.12.0"
 mypy = "^1.0.1"
 pre-commit = "^3.0.4"
 pydocstyle = "^6.3.0"
```

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/admin.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/apps.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/cache.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/cache.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/models.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/settings.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/src/wagtail_sb_admin_interface/wagtail_hooks.py` & `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.3.0/setup.py` & `wagtail_sb_admin_interface-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wagtail-sb-admin-interface
+Version: 0.4.0
+Summary: Social Networks settings for wagtail sites.
+Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
+License: MIT
+Keywords: Softbutterfly,Django,Migrations
+Author: SoftButterfly Development Team
+Author-email: dev@softbutterfly.io
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: django (<5.0)
+Requires-Dist: django-colorfield (<1.0.0)
+Requires-Dist: wagtail (<5.0)
+Requires-Dist: wagtail-sb-fontawesome (<1.0.0)
+Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/issues
+Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/archive/v0.4.0/wagtail-sb-admin-interface-v0.4.0.tar.gz
+Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
+Description-Content-Type: text/markdown
+
+![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
+
+![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-admin-interface)
+![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-admin-interface)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-admin-interface)
+![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-admin-interface)
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/f28072e8e0ac4605bd3235b7643929ad)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-admin-interface/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+
+# Wagtail Admin Interface
+
+Customize the Wagtail admin interface from the admin itself.
+
+Inspired by [django-admin-interface](https://github.com/fabiocaccamo/django-admin-interface).
+
+## Requirements
+
+- Python 3.8.1 or higher
+- Django 4.0.0 or higher
+- Wagtail 4.0.0 or higher
+
+## Install
+
+```bash
+pip install wagtail-sb-admin-interface
+```
+
+## Usage
+
+Add `wagtail.contrib.settings`, `wagtail.contrib.modeladmin`, `colorfield` and `wagtail_sb_admin_interface` to your `INSTALLED_APPS` settings
+
+```
+INSTALLED_APPS = [
+  "wagtail_sb_admin_interface",
+  # ...
+  "wagtail.contrib.settings",
+  "wagtail.contrib.modeladmin",
+  "colorfield",
+  # ...
+]
+```
+
+## Docs
+
+- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis)
+- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis)
+
+## Changelog
+
+All changes to versions of this library are listed in the [change history](CHANGELOG.md).
 
-package_dir = \
-{'': 'src'}
+## Development
 
-packages = \
-['wagtail_sb_admin_interface',
- 'wagtail_sb_admin_interface.migrations',
- 'wagtail_sb_admin_interface.templatetags']
-
-package_data = \
-{'': ['*'], 'wagtail_sb_admin_interface': ['templates/wagtailadmin/*']}
-
-install_requires = \
-['django-colorfield<1.0.0', 'django<5.0', 'wagtail<5.0']
-
-setup_kwargs = {
-    'name': 'wagtail-sb-admin-interface',
-    'version': '0.3.0',
-    'description': 'Social Networks settings for wagtail sites.',
-    'long_description': '![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)\n\n![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-admin-interface)\n![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-admin-interface)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-admin-interface)\n![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-admin-interface)\n\n[![Build Status](https://www.travis-ci.org/softbutterfly/wagtail-sb-admin-interface.svg?branch=develop)](https://www.travis-ci.org/softbutterfly/wagtail-sb-admin-interface)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e35e7095857b416696eb58a4ed5d9a15)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-admin-interface/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=softbutterfly/wagtail-sb-admin-interface&amp;utm_campaign=Badge_Grade)\n[![Codacy Badge Coverage](https://app.codacy.com/project/badge/Coverage/e35e7095857b416696eb58a4ed5d9a15)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-admin-interface/dashboard?utm_source=github.com&utm_medium=referral&utm_content=softbutterfly/wagtail-sb-admin-interface&utm_campaign=Badge_Coverage)\n[![codecov](https://codecov.io/gh/softbutterfly/wagtail-sb-admin-interface/branch/master/graph/badge.svg?token=pbqXUUOu1F)](https://codecov.io/gh/softbutterfly/wagtail-sb-admin-interface)\n\n# Wagtail Admin Interface\n\nCustomize the Wagtail admin interface from the admin itself.\n\nInspired by [django-admin-interface](https://github.com/fabiocaccamo/django-admin-interface).\n\n## Requirements\n\n- Python 3.8.1 or higher\n- Django 4.0.0 or higher\n- Wagtail 4.0.0 or higher\n\n## Install\n\n```bash\npip install wagtail-sb-admin-interface\n```\n\n## Usage\n\nAdd `wagtail.contrib.settings`, `wagtail.contrib.modeladmin`, `colorfield` and `wagtail_sb_admin_interface` to your `INSTALLED_APPS` settings\n\n```\nINSTALLED_APPS = [\n  "wagtail_sb_admin_interface",\n  # ...\n  "wagtail.contrib.settings",\n  "wagtail.contrib.modeladmin",\n  "colorfield",\n  # ...\n]\n```\n\n## Docs\n\n- [Ejemplos](https://github.com/softbutterfly/wagtail-sb-admin-interface/wiki)\n- [Wiki](https://github.com/softbutterfly/wagtail-sb-admin-interface/wiki)\n\n## Changelog\n\nAll changes to versions of this library are listed in the [change history](CHANGELOG.md).\n\n## Development\n\nCheck out our [contribution guide](CONTRIBUTING.md).\n\n## Contributors\n\nSee the list of contributors [here](https://github.com/softbutterfly/wagtail-sb-admin-interface/graphs/contributors).\n',
-    'author': 'SoftButterfly Development Team',
-    'author_email': 'dev@softbutterfly.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/softbutterfly/wagtail-sb-admin-interface',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+Check out our [contribution guide](CONTRIBUTING.md).
 
+## Contributors
+
+See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/graphs/develop).
 
-setup(**setup_kwargs)
```

