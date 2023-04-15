# Comparing `tmp/vernac-0.0.3.tar.gz` & `tmp/vernac-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernac-0.0.3.tar", last modified: Fri Apr 14 23:15:21 2023, max compression
+gzip compressed data, was "vernac-0.0.4.tar", last modified: Sat Apr 15 17:43:18 2023, max compression
```

## Comparing `vernac-0.0.3.tar` & `vernac-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1980 2023-04-14 22:56:26.000000 vernac-0.0.3/.gitignore
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.3/LICENSE
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2478 2023-04-14 23:15:21.041238 vernac-0.0.3/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2195 2023-04-14 04:14:58.000000 vernac-0.0.3/README.md
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2985 2023-04-14 03:58:04.000000 vernac-0.0.3/dev-requirements.txt
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/examples/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/examples/reliable/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      283 2023-04-14 17:41:58.000000 vernac-0.0.3/examples/reliable/benchmark.vn
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      138 2023-04-14 17:41:58.000000 vernac-0.0.3/examples/reliable/fizzbuzz.vn
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      142 2023-04-14 17:41:58.000000 vernac-0.0.3/examples/reliable/mergesort.vn
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/examples/unreliable/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      433 2023-04-14 22:59:31.000000 vernac-0.0.3/examples/unreliable/count_gpt_titles.vn
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      921 2023-04-14 18:05:37.000000 vernac-0.0.3/examples/unreliable/hntoday.vn
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      312 2023-04-14 18:34:26.000000 vernac-0.0.3/examples/unreliable/snake.vn
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.3/local-dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      587 2023-04-13 18:57:07.000000 vernac-0.0.3/pyproject.toml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-14 23:15:21.041238 vernac-0.0.3/setup.cfg
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/src/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/src/vernac/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     6625 2023-04-14 23:04:53.000000 vernac-0.0.3/src/vernac/compile.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/src/vernac.egg-info/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2478 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      511 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/SOURCES.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/dependency_links.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/entry_points.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       71 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/requires.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.333872 vernac-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 17:43:04.000000 vernac-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-15 17:43:04.000000 vernac-0.0.4/.github/workflows/test-some-examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-15 17:43:04.000000 vernac-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-15 17:43:04.000000 vernac-0.0.4/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 17:43:04.000000 vernac-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-15 17:43:18.337872 vernac-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-15 17:43:04.000000 vernac-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-15 17:43:04.000000 vernac-0.0.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.333872 vernac-0.0.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/examples/reliable/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/reliable/benchmark.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/reliable/fizzbuzz.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/reliable/mergesort.vn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/examples/unreliable/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/unreliable/count_gpt_titles.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/unreliable/hntoday.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/unreliable/snake.vn
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 17:43:04.000000 vernac-0.0.4/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 17:43:04.000000 vernac-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:43:18.337872 vernac-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.333872 vernac-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/src/vernac/
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-15 17:43:04.000000 vernac-0.0.4/src/vernac/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/src/vernac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/top_level.txt
```

### Comparing `vernac-0.0.3/.gitignore` & `vernac-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `vernac-0.0.3/LICENSE` & `vernac-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vernac-0.0.3/PKG-INFO` & `vernac-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vernac
-Version: 0.0.3
-Project-URL: homepage, https://github.com/bsilverthorn/vernac
-Project-URL: repository, https://github.com/bsilverthorn/vernac
+Version: 0.0.4
+Project-URL: Homepage, https://github.com/bsilverthorn/vernac
+Project-URL: Repository, https://github.com/bsilverthorn/vernac
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Vernac: programming (in) language 📖
 ====================================
```

### Comparing `vernac-0.0.3/README.md` & `vernac-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vernac-0.0.3/dev-requirements.txt` & `vernac-0.0.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `vernac-0.0.3/examples/unreliable/hntoday.vn` & `vernac-0.0.4/examples/unreliable/hntoday.vn`

 * *Files identical despite different names*

### Comparing `vernac-0.0.3/pyproject.toml` & `vernac-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,22 +12,20 @@
     "shiv",
     "tomli_w",
     "rich",
 ]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "https://github.com/bsilverthorn/vernac"
-repository = "https://github.com/bsilverthorn/vernac"
+"Homepage" = "https://github.com/bsilverthorn/vernac"
+"Repository" = "https://github.com/bsilverthorn/vernac"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
-    "build",
-    "twine",
 ]
 
 [project.scripts]
 vernac = "vernac.compile:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `vernac-0.0.3/src/vernac/compile.py` & `vernac-0.0.4/src/vernac/compile.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.3/src/vernac.egg-info/PKG-INFO` & `vernac-0.0.4/src/vernac.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vernac
-Version: 0.0.3
-Project-URL: homepage, https://github.com/bsilverthorn/vernac
-Project-URL: repository, https://github.com/bsilverthorn/vernac
+Version: 0.0.4
+Project-URL: Homepage, https://github.com/bsilverthorn/vernac
+Project-URL: Repository, https://github.com/bsilverthorn/vernac
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Vernac: programming (in) language 📖
 ====================================
```

