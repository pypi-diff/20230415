# Comparing `tmp/ra_utils-1.9.2.tar.gz` & `tmp/ra_utils-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra_utils-1.9.2.tar", max compression
+gzip compressed data, was "ra_utils-1.9.3.tar", max compression
```

## Comparing `ra_utils-1.9.2.tar` & `ra_utils-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0        0        0        0 2023-02-09 10:18:13.206511 ra_utils-1.9.2/LICENSES/
--rw-r--r--   0        0        0      351 2023-02-09 10:18:13.206511 ra_utils-1.9.2/README.md
--rw-r--r--   0        0        0     1580 2023-02-09 12:31:43.182510 ra_utils-1.9.2/pyproject.toml
--rw-r--r--   0        0        0       99 2023-02-09 10:18:13.206511 ra_utils-1.9.2/ra_utils/__init__.py
--rw-r--r--   0        0        0     2263 2023-02-09 10:18:13.206511 ra_utils-1.9.2/ra_utils/apply.py
--rw-r--r--   0        0        0     1035 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/async_to_sync.py
--rw-r--r--   0        0        0     2883 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/asyncio_utils.py
--rw-r--r--   0        0        0      805 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/attrdict.py
--rw-r--r--   0        0        0     1539 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/catchtime.py
--rw-r--r--   0        0        0      979 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/deprecation.py
--rw-r--r--   0        0        0     3961 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/dict_map.py
--rw-r--r--   0        0        0     2404 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/ensure_hashable.py
--rw-r--r--   0        0        0     3624 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/ensure_single_run.py
--rw-r--r--   0        0        0     1723 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/generate_uuid.py
--rw-r--r--   0        0        0     5698 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/headers.py
--rw-r--r--   0        0        0     3488 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/jinja_filter.py
--rw-r--r--   0        0        0     6637 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/job_settings.py
--rw-r--r--   0        0        0     6027 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/lazy_dict.py
--rw-r--r--   0        0        0     2918 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/load_settings.py
--rw-r--r--   0        0        0     2935 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/multiple_replace.py
--rw-r--r--   0        0        0     3026 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/semantic_version_type.py
--rw-r--r--   0        0        0     1514 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/sentry_init.py
--rw-r--r--   0        0        0     1124 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/strategies.py
--rw-r--r--   0        0        0     3131 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/structured_url.py
--rw-r--r--   0        0        0     4717 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/syncable.py
--rw-r--r--   0        0        0      548 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/tqdm_wrapper.py
--rw-r--r--   0        0        0     1842 2023-02-09 10:18:13.210511 ra_utils-1.9.2/ra_utils/transpose_dict.py
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 ra_utils-1.9.2/setup.py
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ra_utils-1.9.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-02-09 10:43:46.892882 ra_utils-1.9.3/LICENSES/
+-rw-r--r--   0        0        0      351 2023-02-09 10:43:46.892882 ra_utils-1.9.3/README.md
+-rw-r--r--   0        0        0     1580 2023-02-09 14:28:15.729827 ra_utils-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/__init__.py
+-rw-r--r--   0        0        0     2263 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/apply.py
+-rw-r--r--   0        0        0     1035 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/async_to_sync.py
+-rw-r--r--   0        0        0     2883 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/asyncio_utils.py
+-rw-r--r--   0        0        0      805 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/attrdict.py
+-rw-r--r--   0        0        0     1539 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/catchtime.py
+-rw-r--r--   0        0        0      979 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/deprecation.py
+-rw-r--r--   0        0        0     3961 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/dict_map.py
+-rw-r--r--   0        0        0     2404 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/ensure_hashable.py
+-rw-r--r--   0        0        0     3699 2023-02-09 14:28:15.733827 ra_utils-1.9.3/ra_utils/ensure_single_run.py
+-rw-r--r--   0        0        0     1723 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/generate_uuid.py
+-rw-r--r--   0        0        0     5698 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/headers.py
+-rw-r--r--   0        0        0     3488 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/jinja_filter.py
+-rw-r--r--   0        0        0     6637 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/job_settings.py
+-rw-r--r--   0        0        0     6027 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/lazy_dict.py
+-rw-r--r--   0        0        0     2918 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/load_settings.py
+-rw-r--r--   0        0        0     2935 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/multiple_replace.py
+-rw-r--r--   0        0        0     3026 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/semantic_version_type.py
+-rw-r--r--   0        0        0     1514 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/sentry_init.py
+-rw-r--r--   0        0        0     1124 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/strategies.py
+-rw-r--r--   0        0        0     3131 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/structured_url.py
+-rw-r--r--   0        0        0     4717 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/syncable.py
+-rw-r--r--   0        0        0      548 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/tqdm_wrapper.py
+-rw-r--r--   0        0        0     1842 2023-02-09 10:43:46.896882 ra_utils-1.9.3/ra_utils/transpose_dict.py
+-rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 ra_utils-1.9.3/setup.py
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ra_utils-1.9.3/PKG-INFO
```

### Comparing `ra_utils-1.9.2/pyproject.toml` & `ra_utils-1.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ra-utils"
-version = "1.9.2"
+version = "1.9.3"
 description = "Utilities for OS2mo/LoRa"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ra-utils"
 keywords = ["os2mo", "lora"]
```

### Comparing `ra_utils-1.9.2/ra_utils/apply.py` & `ra_utils-1.9.3/ra_utils/apply.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/async_to_sync.py` & `ra_utils-1.9.3/ra_utils/async_to_sync.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/asyncio_utils.py` & `ra_utils-1.9.3/ra_utils/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/attrdict.py` & `ra_utils-1.9.3/ra_utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/catchtime.py` & `ra_utils-1.9.3/ra_utils/catchtime.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/deprecation.py` & `ra_utils-1.9.3/ra_utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/dict_map.py` & `ra_utils-1.9.3/ra_utils/dict_map.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/ensure_hashable.py` & `ra_utils-1.9.3/ra_utils/ensure_hashable.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/ensure_single_run.py` & `ra_utils-1.9.3/ra_utils/ensure_single_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         log.warning("Cannot connect to Prometheus")
         log.warning(ue)
 
 
 def ensure_single_run(
     func: typing.Callable,
     lock_name: str,
+    *args: typing.Any,
+    **kwargs: typing.Any,
 ) -> typing.Any:
     """Wrapper function that ensures that no more than a single instance of a function
     is running at any given time. Checks if a lock for the function already exists, and
     is taken, or not. If a lock exists it raises a StopIteration exception. If no lock
     is taken creates a lock file, executes the function, removes the lock file, and
     returns the result of the function.
 
@@ -98,18 +100,18 @@
 
     if not locked:
         with open(file=lock_name, mode="w") as lock:
             lock.write(f"pid={os.getpid()}")
             lock.flush()
 
         try:
-            return_value = func()
+            return_value = func(*args, **kwargs)
         except Exception as e:
             raise e
         finally:
             os.remove(lock_name)
             notify_prometheus(lock_file_name=lock_name, lock_conflict=locked)
     else:
         notify_prometheus(lock_file_name=lock_name, lock_conflict=locked)
-        raise LockTaken
+        raise LockTaken(lock_name)
 
     return return_value
```

### Comparing `ra_utils-1.9.2/ra_utils/generate_uuid.py` & `ra_utils-1.9.3/ra_utils/generate_uuid.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/headers.py` & `ra_utils-1.9.3/ra_utils/headers.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/jinja_filter.py` & `ra_utils-1.9.3/ra_utils/jinja_filter.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/job_settings.py` & `ra_utils-1.9.3/ra_utils/job_settings.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/lazy_dict.py` & `ra_utils-1.9.3/ra_utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/load_settings.py` & `ra_utils-1.9.3/ra_utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/multiple_replace.py` & `ra_utils-1.9.3/ra_utils/multiple_replace.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/semantic_version_type.py` & `ra_utils-1.9.3/ra_utils/semantic_version_type.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/sentry_init.py` & `ra_utils-1.9.3/ra_utils/sentry_init.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/strategies.py` & `ra_utils-1.9.3/ra_utils/strategies.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/structured_url.py` & `ra_utils-1.9.3/ra_utils/structured_url.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/syncable.py` & `ra_utils-1.9.3/ra_utils/syncable.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/tqdm_wrapper.py` & `ra_utils-1.9.3/ra_utils/tqdm_wrapper.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/ra_utils/transpose_dict.py` & `ra_utils-1.9.3/ra_utils/transpose_dict.py`

 * *Files identical despite different names*

### Comparing `ra_utils-1.9.2/setup.py` & `ra_utils-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'headers': ['pydantic>=1.10.2,<2.0.0', 'requests>=2.28.1,<3.0.0'],
  'jinja': ['Jinja2>=3.1.2,<4.0.0'],
  'pydantic': ['pydantic>=1.10.2,<2.0.0'],
  'sentry': ['pydantic>=1.10.2,<2.0.0', 'sentry-sdk>=1.12.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'ra-utils',
-    'version': '1.9.2',
+    'version': '1.9.3',
     'description': 'Utilities for OS2mo/LoRa',
     'long_description': '<!--\nSPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>\nSPDX-License-Identifier: MPL-2.0\n-->\n\n\n# RA Utils\n\nVarious code utilities for OS2mo/LoRa\n\n## License\n- This project: [MPL-2.0](MPL-2.0.txt)\n\nThis project uses [REUSE](https://reuse.software) for licensing. All licenses can be found in the [LICENSES folder](LICENSES/) of the project.\n',
     'author': 'Magenta',
     'author_email': 'info@magenta.dk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://magenta.dk/',
```

### Comparing `ra_utils-1.9.2/PKG-INFO` & `ra_utils-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra-utils
-Version: 1.9.2
+Version: 1.9.3
 Summary: Utilities for OS2mo/LoRa
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,lora
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.8,<4.0
```

