# Comparing `tmp/wagtail-sb-socialnetworks-0.4.0.tar.gz` & `tmp/wagtail_sb_socialnetworks-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-sb-socialnetworks-0.4.0.tar", max compression
+gzip compressed data, was "wagtail_sb_socialnetworks-0.5.0.tar", max compression
```

## Comparing `wagtail-sb-socialnetworks-0.4.0.tar` & `wagtail_sb_socialnetworks-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      567 2022-10-02 14:44:44.129040 wagtail-sb-socialnetworks-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2022-03-27 20:03:51.145403 wagtail-sb-socialnetworks-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2555 2022-07-03 17:11:12.984241 wagtail-sb-socialnetworks-0.4.0/README.md
--rw-r--r--   0        0        0     1896 2022-10-02 14:44:44.125039 wagtail-sb-socialnetworks-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       88 2022-06-20 04:31:36.400690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/__init__.py
--rw-r--r--   0        0        0        0 2022-06-20 04:31:36.396690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/admin.py
--rw-r--r--   0        0        0      180 2022-06-20 04:31:36.400690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/apps.py
--rw-r--r--   0        0        0     1204 2022-06-20 04:31:36.400690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4536 2022-06-20 04:31:36.400690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py
--rw-r--r--   0        0        0      684 2022-10-02 14:44:28.576980 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py
--rw-r--r--   0        0        0      574 2022-10-02 14:44:28.576980 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py
--rw-r--r--   0        0        0        0 2022-06-20 04:31:36.396690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/__init__.py
--rw-r--r--   0        0        0     3736 2022-10-02 14:44:28.576980 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/models.py
--rw-r--r--   0        0        0        0 2022-06-20 04:31:36.396690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/tests.py
--rw-r--r--   0        0        0       20 2022-10-02 14:44:44.133040 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/version.py
--rw-r--r--   0        0        0        0 2022-06-20 04:31:36.396690 wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/views.py
--rw-r--r--   0        0        0     3512 2022-10-02 14:44:49.085582 wagtail-sb-socialnetworks-0.4.0/setup.py
--rw-r--r--   0        0        0     3872 2022-10-02 14:44:49.085818 wagtail-sb-socialnetworks-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      743 2023-04-15 13:44:49.126311 wagtail_sb_socialnetworks-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2022-12-12 01:51:13.643284 wagtail_sb_socialnetworks-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1661 2023-04-15 13:42:21.077778 wagtail_sb_socialnetworks-0.5.0/README.md
+-rw-r--r--   0        0        0     1996 2023-04-15 13:44:49.126311 wagtail_sb_socialnetworks-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/admin.py
+-rw-r--r--   0        0        0      180 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/apps.py
+-rw-r--r--   0        0        0     1204 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4536 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py
+-rw-r--r--   0        0        0      684 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py
+-rw-r--r--   0        0        0      574 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py
+-rw-r--r--   0        0        0        0 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/__init__.py
+-rw-r--r--   0        0        0     3736 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/models.py
+-rw-r--r--   0        0        0        0 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/tests.py
+-rw-r--r--   0        0        0       20 2023-04-15 13:44:49.130311 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/version.py
+-rw-r--r--   0        0        0        0 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/views.py
+-rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 wagtail_sb_socialnetworks-0.5.0/PKG-INFO
```

### Comparing `wagtail-sb-socialnetworks-0.4.0/LICENSE.txt` & `wagtail_sb_socialnetworks-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-sb-socialnetworks-0.4.0/README.md` & `wagtail_sb_socialnetworks-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-socialnetworks)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-socialnetworks)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-socialnetworks)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-socialnetworks)
 
-[![Build Status](https://www.travis-ci.org/softbutterfly/wagtail-sb-socialnetworks.svg?branch=develop)](https://www.travis-ci.org/softbutterfly/wagtail-sb-socialnetworks)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/3d703e48c1e44e9b830da5026f07c52d)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-socialnetworks/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=softbutterfly/wagtail-sb-socialnetworks&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/3d703e48c1e44e9b830da5026f07c52d)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-socialnetworks/dashboard?utm_source=github.com&utm_medium=referral&utm_content=softbutterfly/wagtail-sb-socialnetworks&utm_campaign=Badge_Coverage)
-[![codecov](https://codecov.io/gh/softbutterfly/wagtail-sb-socialnetworks/branch/master/graph/badge.svg?token=pbqXUUOu1F)](https://codecov.io/gh/softbutterfly/wagtail-sb-socialnetworks)
-[![Requirements Status](https://requires.io/github/softbutterfly/wagtail-sb-socialnetworks/requirements.svg?branch=master)](https://requires.io/github/softbutterfly/wagtail-sb-socialnetworks/requirements/?branch=master)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/329484ea99434c708f5c8dbd611f3d35)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-socialnetworks/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 # Wagtail Social Networks
 
 Wagtail package to manage sites social network profiles.
 
 ## Requirements
 
@@ -36,21 +32,21 @@
   "wagtail_sb_socialnetworks",
   # ...
 ]
 ```
 
 ## Docs
 
-- [Ejemplos](https://github.com/softbutterfly/wagtail-sb-socialnetworks/wiki)
-- [Wiki](https://github.com/softbutterfly/wagtail-sb-socialnetworks/wiki)
+- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/wikis)
+- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/wikis)
 
 ## Changelog
 
 All changes to versions of this library are listed in the [change history](CHANGELOG.md).
 
 ## Development
 
 Check out our [contribution guide](CONTRIBUTING.md).
 
 ## Contributors
 
-See the list of contributors [here](https://github.com/softbutterfly/wagtail-sb-socialnetworks/graphs/contributors).
+See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/graphs/develop).
```

### Comparing `wagtail-sb-socialnetworks-0.4.0/pyproject.toml` & `wagtail_sb_socialnetworks-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "wagtail-sb-socialnetworks"
-version = "0.4.0"
+version = "0.5.0"
 description = "Social Networks settings for wagtail sites."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
-homepage = "https://github.com/softbutterfly/wagtail-sb-socialnetworks"
-repository = "https://github.com/softbutterfly/wagtail-sb-socialnetworks"
-documentation = "https://github.com/softbutterfly/wagtail-sb-socialnetworks/wiki"
+homepage = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks"
+repository = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks"
+documentation = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/wikis"
 keywords = ["Softbutterfly", "Django", "Migrations"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
@@ -28,40 +28,40 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://github.com/softbutterfly/wagtail-sb-socialnetworks/archive/v0.4.0.tar.gz"
-"Bug Tracker" = "https://github.com/softbutterfly/wagtail-sb-socialnetworks/issues"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.5.0/wagtail-sb-socialnetworks-v0.5.0.tar.gz"
+"Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/issues"
 
 
 [tool.poetry.dependencies]
-python = ">= 3.8, < 4.0.0"
+python = ">= 3.8.1, < 4.0.0"
 Django = "< 5.0"
 wagtail = "< 5.0"
 
-[tool.poetry.dev-dependencies]
-autopep8 = "^1.7.0"
-black = "^22.8.0"
-codecov = "^2.1.12"
-coverage = "^6.5.0"
-flake8 = "^5.0.4"
-flake8-black = "^0.3.3"
-jupyterlab = "^3.4.7"
-mypy = "^0.981"
-pre-commit = "^2.20.0"
-pydocstyle = "^6.1.1"
-pylint = "^2.15.3"
+[tool.poetry.group.dev.dependencies]
+autopep8 = "^2.0.1"
+bandit = "^1.7.4"
+black = "^23.1.0"
+coverage = "^7.1.0"
+flake8 = "^6.0.0"
+flake8-black = "^0.3.6"
+isort = "^5.12.0"
+mypy = "^1.0.1"
+pre-commit = "^3.0.4"
+pydocstyle = "^6.3.0"
+pylint = "^2.16.2"
 pylint-django = "^2.5.3"
-pytest = "^7.1.3"
+pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-vcr = "^1.0.2"
-python-dotenv = "^0.21.0"
-tox = "^3.26.0"
-twine = "^4.0.1"
+python-dotenv = "^0.21.1"
 tbump = "^6.9.0"
+tox = "^4.4.6"
+twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po` & `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py` & `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py` & `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py`

 * *Files identical despite different names*

### Comparing `wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py` & `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-sb-socialnetworks-0.4.0/src/wagtail_sb_socialnetworks/models.py` & `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/models.py`

 * *Files identical despite different names*

