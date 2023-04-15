# Comparing `tmp/idealgeo-0.0.2.tar.gz` & `tmp/idealgeo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idealgeo-0.0.2.tar", last modified: Sat Apr 15 04:27:15 2023, max compression
+gzip compressed data, was "idealgeo-0.0.3.tar", last modified: Sat Apr 15 04:41:33 2023, max compression
```

## Comparing `idealgeo-0.0.2.tar` & `idealgeo-0.0.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/
--rw-rw-r--   0 josh      (1000) josh      (1000)       61 2023-04-14 23:21:21.000000 idealgeo-0.0.2/AUTHORS.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       86 2023-04-14 23:21:21.000000 idealgeo-0.0.2/CHANGELOG.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)     2414 2023-04-14 23:21:21.000000 idealgeo-0.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      584 2023-04-14 23:21:21.000000 idealgeo-0.0.2/LICENSE
--rw-rw-r--   0 josh      (1000) josh      (1000)      427 2023-04-14 23:21:21.000000 idealgeo-0.0.2/MANIFEST.in
--rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 04:27:15.248241 idealgeo-0.0.2/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      756 2023-04-14 23:21:21.000000 idealgeo-0.0.2/README.rst
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.244241 idealgeo-0.0.2/ci/
--rwxrwxr-x   0 josh      (1000) josh      (1000)     2930 2023-04-14 23:21:21.000000 idealgeo-0.0.2/ci/bootstrap.py
--rw-rw-r--   0 josh      (1000) josh      (1000)       72 2023-04-14 23:21:21.000000 idealgeo-0.0.2/ci/requirements.txt
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.244241 idealgeo-0.0.2/ci/templates/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.244241 idealgeo-0.0.2/ci/templates/.github/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.244241 idealgeo-0.0.2/ci/templates/.github/workflows/
--rw-rw-r--   0 josh      (1000) josh      (1000)     2001 2023-04-14 23:21:21.000000 idealgeo-0.0.2/ci/templates/.github/workflows/github-actions.yml
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/docs/
--rw-rw-r--   0 josh      (1000) josh      (1000)       28 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/authors.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       30 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/changelog.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)     1195 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/conf.py
--rw-rw-r--   0 josh      (1000) josh      (1000)       33 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/contributing.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      244 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/index.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       88 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/installation.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       27 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/readme.rst
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/docs/reference/
--rw-rw-r--   0 josh      (1000) josh      (1000)      102 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/reference/idealgeo.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       60 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/reference/index.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       29 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/requirements.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)      109 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/spelling_wordlist.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       68 2023-04-14 23:21:21.000000 idealgeo-0.0.2/docs/usage.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      160 2023-04-14 23:21:21.000000 idealgeo-0.0.2/pyproject.toml
--rw-rw-r--   0 josh      (1000) josh      (1000)      773 2023-04-14 23:21:21.000000 idealgeo-0.0.2/pytest.ini
--rw-rw-r--   0 josh      (1000) josh      (1000)      304 2023-04-15 04:27:15.248241 idealgeo-0.0.2/setup.cfg
--rwxrwxr-x   0 josh      (1000) josh      (1000)     4939 2023-04-15 04:27:07.000000 idealgeo-0.0.2/setup.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.244241 idealgeo-0.0.2/src/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/src/idealgeo/
--rw-rw-r--   0 josh      (1000) josh      (1000)       59 2023-04-15 03:06:22.000000 idealgeo-0.0.2/src/idealgeo/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      363 2023-04-14 23:21:21.000000 idealgeo-0.0.2/src/idealgeo/__main__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      735 2023-04-14 23:21:21.000000 idealgeo-0.0.2/src/idealgeo/cli.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1998 2023-04-15 04:26:00.000000 idealgeo-0.0.2/src/idealgeo/client.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/src/idealgeo/geometries/
--rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-04-14 23:25:34.000000 idealgeo-0.0.2/src/idealgeo/geometries/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1939 2023-04-15 02:21:55.000000 idealgeo-0.0.2/src/idealgeo/geometries/buffer.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      450 2023-04-15 02:48:47.000000 idealgeo-0.0.2/src/idealgeo/geometries/custom.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      249 2023-04-15 02:16:33.000000 idealgeo-0.0.2/src/idealgeo/geometries/location.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2084 2023-04-15 02:19:03.000000 idealgeo-0.0.2/src/idealgeo/geometries/region.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/src/idealgeo/insights/
--rw-rw-r--   0 josh      (1000) josh      (1000)      271 2023-04-15 02:57:52.000000 idealgeo-0.0.2/src/idealgeo/insights/__init__.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/src/idealgeo.egg-info/
--rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 04:27:15.000000 idealgeo-0.0.2/src/idealgeo.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)     1098 2023-04-15 04:27:15.000000 idealgeo-0.0.2/src/idealgeo.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 04:27:15.000000 idealgeo-0.0.2/src/idealgeo.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       47 2023-04-15 04:27:15.000000 idealgeo-0.0.2/src/idealgeo.egg-info/entry_points.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 03:35:38.000000 idealgeo-0.0.2/src/idealgeo.egg-info/not-zip-safe
--rw-rw-r--   0 josh      (1000) josh      (1000)       41 2023-04-15 04:27:15.000000 idealgeo-0.0.2/src/idealgeo.egg-info/requires.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        9 2023-04-15 04:27:15.000000 idealgeo-0.0.2/src/idealgeo.egg-info/top_level.txt
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:27:15.248241 idealgeo-0.0.2/tests/
--rw-rw-r--   0 josh      (1000) josh      (1000)       77 2023-04-15 03:06:03.000000 idealgeo-0.0.2/tests/test_client.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      218 2023-04-14 23:21:21.000000 idealgeo-0.0.2/tests/test_idealgeo.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      321 2023-04-15 02:58:39.000000 idealgeo-0.0.2/tests/test_insights.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2819 2023-04-15 02:56:52.000000 idealgeo-0.0.2/tests/test_locations.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1732 2023-04-14 23:21:21.000000 idealgeo-0.0.2/tox.ini
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.049238 idealgeo-0.0.3/
+-rw-rw-r--   0 josh      (1000) josh      (1000)       61 2023-04-14 23:21:21.000000 idealgeo-0.0.3/AUTHORS.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       86 2023-04-14 23:21:21.000000 idealgeo-0.0.3/CHANGELOG.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2414 2023-04-14 23:21:21.000000 idealgeo-0.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      584 2023-04-14 23:21:21.000000 idealgeo-0.0.3/LICENSE
+-rw-rw-r--   0 josh      (1000) josh      (1000)      427 2023-04-14 23:21:21.000000 idealgeo-0.0.3/MANIFEST.in
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 04:41:33.049238 idealgeo-0.0.3/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)      756 2023-04-14 23:21:21.000000 idealgeo-0.0.3/README.rst
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.045238 idealgeo-0.0.3/ci/
+-rwxrwxr-x   0 josh      (1000) josh      (1000)     2930 2023-04-14 23:21:21.000000 idealgeo-0.0.3/ci/bootstrap.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)       72 2023-04-14 23:21:21.000000 idealgeo-0.0.3/ci/requirements.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.041238 idealgeo-0.0.3/ci/templates/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.041238 idealgeo-0.0.3/ci/templates/.github/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.045238 idealgeo-0.0.3/ci/templates/.github/workflows/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2001 2023-04-14 23:21:21.000000 idealgeo-0.0.3/ci/templates/.github/workflows/github-actions.yml
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.045238 idealgeo-0.0.3/docs/
+-rw-rw-r--   0 josh      (1000) josh      (1000)       28 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/authors.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       30 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/changelog.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1195 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/conf.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)       33 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/contributing.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      244 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/index.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       88 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/installation.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       27 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/readme.rst
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.045238 idealgeo-0.0.3/docs/reference/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      102 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/reference/idealgeo.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       60 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/reference/index.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       29 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/requirements.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)      109 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/spelling_wordlist.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       68 2023-04-14 23:21:21.000000 idealgeo-0.0.3/docs/usage.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      160 2023-04-14 23:21:21.000000 idealgeo-0.0.3/pyproject.toml
+-rw-rw-r--   0 josh      (1000) josh      (1000)      773 2023-04-14 23:21:21.000000 idealgeo-0.0.3/pytest.ini
+-rw-rw-r--   0 josh      (1000) josh      (1000)      304 2023-04-15 04:41:33.049238 idealgeo-0.0.3/setup.cfg
+-rwxrwxr-x   0 josh      (1000) josh      (1000)     4939 2023-04-15 04:41:05.000000 idealgeo-0.0.3/setup.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.041238 idealgeo-0.0.3/src/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.045238 idealgeo-0.0.3/src/idealgeo/
+-rw-rw-r--   0 josh      (1000) josh      (1000)       59 2023-04-15 04:41:15.000000 idealgeo-0.0.3/src/idealgeo/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      363 2023-04-14 23:21:21.000000 idealgeo-0.0.3/src/idealgeo/__main__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      735 2023-04-14 23:21:21.000000 idealgeo-0.0.3/src/idealgeo/cli.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2030 2023-04-15 04:34:07.000000 idealgeo-0.0.3/src/idealgeo/client.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.049238 idealgeo-0.0.3/src/idealgeo/geometries/
+-rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-04-14 23:25:34.000000 idealgeo-0.0.3/src/idealgeo/geometries/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1939 2023-04-15 02:21:55.000000 idealgeo-0.0.3/src/idealgeo/geometries/buffer.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      450 2023-04-15 02:48:47.000000 idealgeo-0.0.3/src/idealgeo/geometries/custom.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      249 2023-04-15 02:16:33.000000 idealgeo-0.0.3/src/idealgeo/geometries/location.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2084 2023-04-15 02:19:03.000000 idealgeo-0.0.3/src/idealgeo/geometries/region.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.049238 idealgeo-0.0.3/src/idealgeo/insights/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      271 2023-04-15 02:57:52.000000 idealgeo-0.0.3/src/idealgeo/insights/__init__.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.049238 idealgeo-0.0.3/src/idealgeo.egg-info/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 04:41:33.000000 idealgeo-0.0.3/src/idealgeo.egg-info/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1098 2023-04-15 04:41:33.000000 idealgeo-0.0.3/src/idealgeo.egg-info/SOURCES.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 04:41:33.000000 idealgeo-0.0.3/src/idealgeo.egg-info/dependency_links.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       47 2023-04-15 04:41:33.000000 idealgeo-0.0.3/src/idealgeo.egg-info/entry_points.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 03:35:38.000000 idealgeo-0.0.3/src/idealgeo.egg-info/not-zip-safe
+-rw-rw-r--   0 josh      (1000) josh      (1000)       41 2023-04-15 04:41:33.000000 idealgeo-0.0.3/src/idealgeo.egg-info/requires.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        9 2023-04-15 04:41:33.000000 idealgeo-0.0.3/src/idealgeo.egg-info/top_level.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 04:41:33.049238 idealgeo-0.0.3/tests/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1863 2023-04-15 04:39:20.000000 idealgeo-0.0.3/tests/test_client.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      218 2023-04-14 23:21:21.000000 idealgeo-0.0.3/tests/test_idealgeo.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      321 2023-04-15 02:58:39.000000 idealgeo-0.0.3/tests/test_insights.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2819 2023-04-15 02:56:52.000000 idealgeo-0.0.3/tests/test_locations.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1732 2023-04-14 23:21:21.000000 idealgeo-0.0.3/tox.ini
```

### Comparing `idealgeo-0.0.2/CONTRIBUTING.rst` & `idealgeo-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/LICENSE` & `idealgeo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/PKG-INFO` & `idealgeo-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idealgeo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client library for IdealSpot's Geodata API.
 Home-page: https://gitlab.com/idealspot/geodata/python-idealgeo
 Author: Josh Winters
 Author-email: josh@idealspot.com
 License: Apache-2.0
 Project-URL: Documentation, https://python-idealgeo.readthedocs.io/
 Project-URL: Changelog, https://python-idealgeo.readthedocs.io/en/latest/changelog.html
```

### Comparing `idealgeo-0.0.2/README.rst` & `idealgeo-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/ci/bootstrap.py` & `idealgeo-0.0.3/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/ci/templates/.github/workflows/github-actions.yml` & `idealgeo-0.0.3/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/docs/conf.py` & `idealgeo-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/pytest.ini` & `idealgeo-0.0.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/setup.py` & `idealgeo-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='idealgeo',
-    version='0.0.2',
+    version='0.0.3',
     license='Apache-2.0',
     description="Client library for IdealSpot's Geodata API.",
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Josh Winters',
```

### Comparing `idealgeo-0.0.2/src/idealgeo/cli.py` & `idealgeo-0.0.3/src/idealgeo/cli.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/src/idealgeo/client.py` & `idealgeo-0.0.3/src/idealgeo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 
 import requests
 
+from .insights import Insight
+
+
 class IdealSpotClient:
     '''Client for the IdealSpot API
 
     Parameters
     ----------
     token : str
     url : str, optional
```

### Comparing `idealgeo-0.0.2/src/idealgeo/geometries/buffer.py` & `idealgeo-0.0.3/src/idealgeo/geometries/buffer.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/src/idealgeo/geometries/region.py` & `idealgeo-0.0.3/src/idealgeo/geometries/region.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/src/idealgeo.egg-info/PKG-INFO` & `idealgeo-0.0.3/src/idealgeo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idealgeo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client library for IdealSpot's Geodata API.
 Home-page: https://gitlab.com/idealspot/geodata/python-idealgeo
 Author: Josh Winters
 Author-email: josh@idealspot.com
 License: Apache-2.0
 Project-URL: Documentation, https://python-idealgeo.readthedocs.io/
 Project-URL: Changelog, https://python-idealgeo.readthedocs.io/en/latest/changelog.html
```

### Comparing `idealgeo-0.0.2/src/idealgeo.egg-info/SOURCES.txt` & `idealgeo-0.0.3/src/idealgeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/tests/test_locations.py` & `idealgeo-0.0.3/tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.2/tox.ini` & `idealgeo-0.0.3/tox.ini`

 * *Files identical despite different names*

