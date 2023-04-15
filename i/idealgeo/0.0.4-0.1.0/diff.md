# Comparing `tmp/idealgeo-0.0.4.tar.gz` & `tmp/idealgeo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idealgeo-0.0.4.tar", last modified: Sat Apr 15 05:33:19 2023, max compression
+gzip compressed data, was "idealgeo-0.1.0.tar", last modified: Sat Apr 15 05:41:38 2023, max compression
```

## Comparing `idealgeo-0.0.4.tar` & `idealgeo-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.316453 idealgeo-0.0.4/
--rw-rw-r--   0 josh      (1000) josh      (1000)       61 2023-04-14 23:21:21.000000 idealgeo-0.0.4/AUTHORS.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       86 2023-04-14 23:21:21.000000 idealgeo-0.0.4/CHANGELOG.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)     2414 2023-04-14 23:21:21.000000 idealgeo-0.0.4/CONTRIBUTING.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      584 2023-04-14 23:21:21.000000 idealgeo-0.0.4/LICENSE
--rw-rw-r--   0 josh      (1000) josh      (1000)      427 2023-04-14 23:21:21.000000 idealgeo-0.0.4/MANIFEST.in
--rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 05:33:19.316453 idealgeo-0.0.4/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      756 2023-04-14 23:21:21.000000 idealgeo-0.0.4/README.rst
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.312453 idealgeo-0.0.4/ci/
--rwxrwxr-x   0 josh      (1000) josh      (1000)     2930 2023-04-14 23:21:21.000000 idealgeo-0.0.4/ci/bootstrap.py
--rw-rw-r--   0 josh      (1000) josh      (1000)       72 2023-04-14 23:21:21.000000 idealgeo-0.0.4/ci/requirements.txt
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.308453 idealgeo-0.0.4/ci/templates/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.308453 idealgeo-0.0.4/ci/templates/.github/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.312453 idealgeo-0.0.4/ci/templates/.github/workflows/
--rw-rw-r--   0 josh      (1000) josh      (1000)     2001 2023-04-14 23:21:21.000000 idealgeo-0.0.4/ci/templates/.github/workflows/github-actions.yml
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.312453 idealgeo-0.0.4/docs/
--rw-rw-r--   0 josh      (1000) josh      (1000)       28 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/authors.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       30 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/changelog.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)     1195 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/conf.py
--rw-rw-r--   0 josh      (1000) josh      (1000)       33 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/contributing.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      244 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/index.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       88 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/installation.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       27 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/readme.rst
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.312453 idealgeo-0.0.4/docs/reference/
--rw-rw-r--   0 josh      (1000) josh      (1000)      102 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/reference/idealgeo.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       60 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/reference/index.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)       29 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/requirements.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)      109 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/spelling_wordlist.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       68 2023-04-14 23:21:21.000000 idealgeo-0.0.4/docs/usage.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      160 2023-04-14 23:21:21.000000 idealgeo-0.0.4/pyproject.toml
--rw-rw-r--   0 josh      (1000) josh      (1000)      773 2023-04-14 23:21:21.000000 idealgeo-0.0.4/pytest.ini
--rw-rw-r--   0 josh      (1000) josh      (1000)      304 2023-04-15 05:33:19.316453 idealgeo-0.0.4/setup.cfg
--rwxrwxr-x   0 josh      (1000) josh      (1000)     4939 2023-04-15 05:32:24.000000 idealgeo-0.0.4/setup.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.308453 idealgeo-0.0.4/src/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.312453 idealgeo-0.0.4/src/idealgeo/
--rw-rw-r--   0 josh      (1000) josh      (1000)       59 2023-04-15 05:32:39.000000 idealgeo-0.0.4/src/idealgeo/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      363 2023-04-14 23:21:21.000000 idealgeo-0.0.4/src/idealgeo/__main__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      735 2023-04-14 23:21:21.000000 idealgeo-0.0.4/src/idealgeo/cli.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     3398 2023-04-15 05:31:32.000000 idealgeo-0.0.4/src/idealgeo/client.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.316453 idealgeo-0.0.4/src/idealgeo/geometries/
--rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-04-14 23:25:34.000000 idealgeo-0.0.4/src/idealgeo/geometries/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1939 2023-04-15 02:21:55.000000 idealgeo-0.0.4/src/idealgeo/geometries/buffer.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      553 2023-04-15 05:08:11.000000 idealgeo-0.0.4/src/idealgeo/geometries/custom.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      249 2023-04-15 02:16:33.000000 idealgeo-0.0.4/src/idealgeo/geometries/location.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2084 2023-04-15 02:19:03.000000 idealgeo-0.0.4/src/idealgeo/geometries/region.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.316453 idealgeo-0.0.4/src/idealgeo/insights/
--rw-rw-r--   0 josh      (1000) josh      (1000)      271 2023-04-15 02:57:52.000000 idealgeo-0.0.4/src/idealgeo/insights/__init__.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.316453 idealgeo-0.0.4/src/idealgeo/vehicletraffic/
--rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-04-15 04:51:56.000000 idealgeo-0.0.4/src/idealgeo/vehicletraffic/__init__.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.316453 idealgeo-0.0.4/src/idealgeo.egg-info/
--rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 05:33:19.000000 idealgeo-0.0.4/src/idealgeo.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)     1138 2023-04-15 05:33:19.000000 idealgeo-0.0.4/src/idealgeo.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 05:33:19.000000 idealgeo-0.0.4/src/idealgeo.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       47 2023-04-15 05:33:19.000000 idealgeo-0.0.4/src/idealgeo.egg-info/entry_points.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 03:35:38.000000 idealgeo-0.0.4/src/idealgeo.egg-info/not-zip-safe
--rw-rw-r--   0 josh      (1000) josh      (1000)       41 2023-04-15 05:33:19.000000 idealgeo-0.0.4/src/idealgeo.egg-info/requires.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        9 2023-04-15 05:33:19.000000 idealgeo-0.0.4/src/idealgeo.egg-info/top_level.txt
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:33:19.316453 idealgeo-0.0.4/tests/
--rw-rw-r--   0 josh      (1000) josh      (1000)     2569 2023-04-15 05:31:22.000000 idealgeo-0.0.4/tests/test_client.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      218 2023-04-14 23:21:21.000000 idealgeo-0.0.4/tests/test_idealgeo.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      321 2023-04-15 02:58:39.000000 idealgeo-0.0.4/tests/test_insights.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2819 2023-04-15 05:08:37.000000 idealgeo-0.0.4/tests/test_locations.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1732 2023-04-14 23:21:21.000000 idealgeo-0.0.4/tox.ini
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/
+-rw-rw-r--   0 josh      (1000) josh      (1000)       61 2023-04-14 23:21:21.000000 idealgeo-0.1.0/AUTHORS.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       86 2023-04-14 23:21:21.000000 idealgeo-0.1.0/CHANGELOG.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2414 2023-04-14 23:21:21.000000 idealgeo-0.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      584 2023-04-14 23:21:21.000000 idealgeo-0.1.0/LICENSE
+-rw-rw-r--   0 josh      (1000) josh      (1000)      427 2023-04-14 23:21:21.000000 idealgeo-0.1.0/MANIFEST.in
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 05:41:38.553001 idealgeo-0.1.0/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)      756 2023-04-14 23:21:21.000000 idealgeo-0.1.0/README.rst
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.549001 idealgeo-0.1.0/ci/
+-rwxrwxr-x   0 josh      (1000) josh      (1000)     2930 2023-04-14 23:21:21.000000 idealgeo-0.1.0/ci/bootstrap.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)       72 2023-04-14 23:21:21.000000 idealgeo-0.1.0/ci/requirements.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.545001 idealgeo-0.1.0/ci/templates/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.545001 idealgeo-0.1.0/ci/templates/.github/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.549001 idealgeo-0.1.0/ci/templates/.github/workflows/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2001 2023-04-14 23:21:21.000000 idealgeo-0.1.0/ci/templates/.github/workflows/github-actions.yml
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.549001 idealgeo-0.1.0/docs/
+-rw-rw-r--   0 josh      (1000) josh      (1000)       28 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/authors.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       30 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/changelog.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1195 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/conf.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)       33 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/contributing.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      244 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/index.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       88 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/installation.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       27 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/readme.rst
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.549001 idealgeo-0.1.0/docs/reference/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      102 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/reference/idealgeo.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       60 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/reference/index.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)       29 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/requirements.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)      109 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       68 2023-04-14 23:21:21.000000 idealgeo-0.1.0/docs/usage.rst
+-rw-rw-r--   0 josh      (1000) josh      (1000)      160 2023-04-14 23:21:21.000000 idealgeo-0.1.0/pyproject.toml
+-rw-rw-r--   0 josh      (1000) josh      (1000)      773 2023-04-14 23:21:21.000000 idealgeo-0.1.0/pytest.ini
+-rw-rw-r--   0 josh      (1000) josh      (1000)      304 2023-04-15 05:41:38.553001 idealgeo-0.1.0/setup.cfg
+-rwxrwxr-x   0 josh      (1000) josh      (1000)     4939 2023-04-15 05:41:03.000000 idealgeo-0.1.0/setup.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.549001 idealgeo-0.1.0/src/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/src/idealgeo/
+-rw-rw-r--   0 josh      (1000) josh      (1000)       59 2023-04-15 05:41:12.000000 idealgeo-0.1.0/src/idealgeo/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      363 2023-04-14 23:21:21.000000 idealgeo-0.1.0/src/idealgeo/__main__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      735 2023-04-14 23:21:21.000000 idealgeo-0.1.0/src/idealgeo/cli.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     4045 2023-04-15 05:39:04.000000 idealgeo-0.1.0/src/idealgeo/client.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/src/idealgeo/geometries/
+-rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-04-14 23:25:34.000000 idealgeo-0.1.0/src/idealgeo/geometries/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1939 2023-04-15 02:21:55.000000 idealgeo-0.1.0/src/idealgeo/geometries/buffer.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      553 2023-04-15 05:08:11.000000 idealgeo-0.1.0/src/idealgeo/geometries/custom.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      249 2023-04-15 02:16:33.000000 idealgeo-0.1.0/src/idealgeo/geometries/location.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2084 2023-04-15 02:19:03.000000 idealgeo-0.1.0/src/idealgeo/geometries/region.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/src/idealgeo/insights/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      271 2023-04-15 02:57:52.000000 idealgeo-0.1.0/src/idealgeo/insights/__init__.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/src/idealgeo/vehicletraffic/
+-rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-04-15 04:51:56.000000 idealgeo-0.1.0/src/idealgeo/vehicletraffic/__init__.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/src/idealgeo.egg-info/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3808 2023-04-15 05:41:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1138 2023-04-15 05:41:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/SOURCES.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 05:41:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/dependency_links.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       47 2023-04-15 05:41:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/entry_points.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-04-15 03:35:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/not-zip-safe
+-rw-rw-r--   0 josh      (1000) josh      (1000)       41 2023-04-15 05:41:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/requires.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        9 2023-04-15 05:41:38.000000 idealgeo-0.1.0/src/idealgeo.egg-info/top_level.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-04-15 05:41:38.553001 idealgeo-0.1.0/tests/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2843 2023-04-15 05:39:54.000000 idealgeo-0.1.0/tests/test_client.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      218 2023-04-14 23:21:21.000000 idealgeo-0.1.0/tests/test_idealgeo.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      321 2023-04-15 02:58:39.000000 idealgeo-0.1.0/tests/test_insights.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2819 2023-04-15 05:08:37.000000 idealgeo-0.1.0/tests/test_locations.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1732 2023-04-14 23:21:21.000000 idealgeo-0.1.0/tox.ini
```

### Comparing `idealgeo-0.0.4/CONTRIBUTING.rst` & `idealgeo-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/LICENSE` & `idealgeo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/PKG-INFO` & `idealgeo-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idealgeo
-Version: 0.0.4
+Version: 0.1.0
 Summary: Client library for IdealSpot's Geodata API.
 Home-page: https://gitlab.com/idealspot/geodata/python-idealgeo
 Author: Josh Winters
 Author-email: josh@idealspot.com
 License: Apache-2.0
 Project-URL: Documentation, https://python-idealgeo.readthedocs.io/
 Project-URL: Changelog, https://python-idealgeo.readthedocs.io/en/latest/changelog.html
```

### Comparing `idealgeo-0.0.4/README.rst` & `idealgeo-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/ci/bootstrap.py` & `idealgeo-0.1.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/ci/templates/.github/workflows/github-actions.yml` & `idealgeo-0.1.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/docs/conf.py` & `idealgeo-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/pytest.ini` & `idealgeo-0.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/setup.py` & `idealgeo-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='idealgeo',
-    version='0.0.4',
+    version='0.1.0',
     license='Apache-2.0',
     description="Client library for IdealSpot's Geodata API.",
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Josh Winters',
```

### Comparing `idealgeo-0.0.4/src/idealgeo/cli.py` & `idealgeo-0.1.0/src/idealgeo/cli.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/src/idealgeo/client.py` & `idealgeo-0.1.0/src/idealgeo/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -100,7 +100,21 @@
                 'properties': custom_polygon.geometry.properties
         }
         body = dict(geometry=body)
         r = requests.post(url, headers=headers, data=json.dumps(body))
         r.raise_for_status()
         return r.json().get('data')
 
+    def query_nearest_road_segments(self, latitude, longitude, n=3):
+        url = os.path.join(self.url, 'traffic', 'roads', 'nearest', str(latitude), str(longitude))
+        headers = dict(api_key=self.token)
+        params = dict(n=n)
+        r = requests.get(url, headers=headers, params=params)
+        r.raise_for_status()
+        return r.json().get('data', [])
+
+    def query_traffic_counts(self, segment_id):
+        url = os.path.join(self.url, 'traffic', 'counts', segment_id)
+        headers = dict(api_key=self.token)
+        r = requests.get(url, headers=headers)
+        r.raise_for_status()
+        return r.json().get('data', [])
```

### Comparing `idealgeo-0.0.4/src/idealgeo/geometries/buffer.py` & `idealgeo-0.1.0/src/idealgeo/geometries/buffer.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/src/idealgeo/geometries/custom.py` & `idealgeo-0.1.0/src/idealgeo/geometries/custom.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/src/idealgeo/geometries/region.py` & `idealgeo-0.1.0/src/idealgeo/geometries/region.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/src/idealgeo.egg-info/PKG-INFO` & `idealgeo-0.1.0/src/idealgeo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idealgeo
-Version: 0.0.4
+Version: 0.1.0
 Summary: Client library for IdealSpot's Geodata API.
 Home-page: https://gitlab.com/idealspot/geodata/python-idealgeo
 Author: Josh Winters
 Author-email: josh@idealspot.com
 License: Apache-2.0
 Project-URL: Documentation, https://python-idealgeo.readthedocs.io/
 Project-URL: Changelog, https://python-idealgeo.readthedocs.io/en/latest/changelog.html
```

### Comparing `idealgeo-0.0.4/src/idealgeo.egg-info/SOURCES.txt` & `idealgeo-0.1.0/src/idealgeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/tests/test_client.py` & `idealgeo-0.1.0/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -95,7 +95,15 @@
 
     poly = custom.CustomPolygon(
         id='123',
         geometry=feature)
     res = client.post_custom_polygon(poly)
     assert res.get('id')
 
+def test_query_nearest_road_segments(client):
+    data = client.query_nearest_road_segments(30.264757, -97.7356077)
+    assert len(data) > 0
+
+def test_query_traffic_counts(client):
+    data = client.query_traffic_counts('429440611')
+    print(data)
+    assert len(data) > 0
```

### Comparing `idealgeo-0.0.4/tests/test_locations.py` & `idealgeo-0.1.0/tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `idealgeo-0.0.4/tox.ini` & `idealgeo-0.1.0/tox.ini`

 * *Files identical despite different names*

