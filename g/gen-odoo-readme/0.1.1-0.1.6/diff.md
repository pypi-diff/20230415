# Comparing `tmp/gen-odoo-readme-0.1.1.tar.gz` & `tmp/gen-odoo-readme-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-odoo-readme-0.1.1.tar", last modified: Sat Apr 15 16:30:17 2023, max compression
+gzip compressed data, was "gen-odoo-readme-0.1.6.tar", last modified: Sat Apr 15 18:01:29 2023, max compression
```

## Comparing `gen-odoo-readme-0.1.1.tar` & `gen-odoo-readme-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/
--rw-rw-r--   0 root         (0) root         (0)    34523 2023-01-28 13:41:54.000000 gen-odoo-readme-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2912 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2273 2023-04-15 14:41:28.000000 gen-odoo-readme-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2912 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      360 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       59 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       42 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        6 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-15 16:30:17.859699 gen-odoo-readme-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1182 2023-04-15 15:24:49.000000 gen-odoo-readme-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/tools/
--rw-rw-r--   0 root         (0) root         (0)       22 2023-04-15 16:22:39.000000 gen-odoo-readme-0.1.1/tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3030 2023-01-28 15:40:07.000000 gen-odoo-readme-0.1.1/tools/gen_addon_readme.template
--rw-rw-r--   0 root         (0) root         (0)     9361 2023-04-15 15:34:36.000000 gen-odoo-readme-0.1.1/tools/gen_readme.py
--rw-rw-r--   0 root         (0) root         (0)     1199 2023-01-28 15:13:03.000000 gen-odoo-readme-0.1.1/tools/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/gen_addon_readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/gen_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/manifest.py
```

### Comparing `gen-odoo-readme-0.1.1/LICENSE` & `gen-odoo-readme-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.1/PKG-INFO` & `gen-odoo-readme-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.1
+Version: 0.1.6
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-0.1.1/README.md` & `gen-odoo-readme-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/PKG-INFO` & `gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.1
+Version: 0.1.6
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-0.1.1/setup.py` & `gen-odoo-readme-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.1/tools/gen_addon_readme.template` & `gen-odoo-readme-0.1.6/tools/gen_addon_readme.template`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.1/tools/gen_readme.py` & `gen-odoo-readme-0.1.6/tools/gen_readme.py`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.1/tools/manifest.py` & `gen-odoo-readme-0.1.6/tools/manifest.py`

 * *Files identical despite different names*

