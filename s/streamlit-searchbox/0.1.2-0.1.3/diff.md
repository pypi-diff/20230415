# Comparing `tmp/streamlit-searchbox-0.1.2.tar.gz` & `tmp/streamlit-searchbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-searchbox-0.1.2.tar", last modified: Sun Mar 26 10:15:26 2023, max compression
+gzip compressed data, was "streamlit-searchbox-0.1.3.tar", last modified: Sat Apr 15 06:31:26 2023, max compression
```

## Comparing `streamlit-searchbox-0.1.2.tar` & `streamlit-searchbox-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.845222 streamlit-searchbox-0.1.2/
--rw-rw-r--   0 wrzr       (501) staff       (20)     1063 2022-04-12 22:00:53.000000 streamlit-searchbox-0.1.2/LICENSE
--rw-rw-r--   0 wrzr       (501) staff       (20)       55 2022-05-29 16:47:35.000000 streamlit-searchbox-0.1.2/MANIFEST.in
--rw-r--r--   0 wrzr       (501) staff       (20)      410 2023-03-26 10:15:26.845086 streamlit-searchbox-0.1.2/PKG-INFO
--rw-r--r--   0 wrzr       (501) staff       (20)     2020 2023-03-26 10:06:13.000000 streamlit-searchbox-0.1.2/README.md
--rw-r--r--   0 wrzr       (501) staff       (20)       38 2023-03-26 10:15:26.845255 streamlit-searchbox-0.1.2/setup.cfg
--rw-r--r--   0 wrzr       (501) staff       (20)      694 2023-03-26 10:14:14.000000 streamlit-searchbox-0.1.2/setup.py
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.840509 streamlit-searchbox-0.1.2/streamlit_searchbox/
--rw-r--r--   0 wrzr       (501) staff       (20)     4714 2023-03-26 10:13:31.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/__init__.py
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.839183 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.842172 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/
--rw-r--r--   0 wrzr       (501) staff       (20)     1023 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/asset-manifest.json
--rw-rw-r--   0 wrzr       (501) staff       (20)   197452 2023-03-26 10:15:02.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/bootstrap.min.css
--rw-r--r--   0 wrzr       (501) staff       (20)     2083 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/index.html
--rw-r--r--   0 wrzr       (501) staff       (20)      786 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/precache-manifest.2a78805e0087eaea58068ac04df3641d.js
--rw-r--r--   0 wrzr       (501) staff       (20)     1183 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/service-worker.js
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.839364 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.844640 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/
--rw-r--r--   0 wrzr       (501) staff       (20)   685180 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js
--rw-r--r--   0 wrzr       (501) staff       (20)     1803 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.LICENSE.txt
--rw-r--r--   0 wrzr       (501) staff       (20)  2024895 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.map
--rw-r--r--   0 wrzr       (501) staff       (20)     6296 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js
--rw-r--r--   0 wrzr       (501) staff       (20)    18039 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js.map
--rw-r--r--   0 wrzr       (501) staff       (20)     1580 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js
--rw-r--r--   0 wrzr       (501) staff       (20)     8299 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js.map
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.844905 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/media/
--rw-r--r--   0 wrzr       (501) staff       (20)      276 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/media/st-arrow.6dbfe07f.svg
--rw-r--r--   0 wrzr       (501) staff       (20)      750 2023-03-26 10:15:05.000000 streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/media/st-clear.53d62d3c.svg
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-03-26 10:15:26.841331 streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/
--rw-r--r--   0 wrzr       (501) staff       (20)      410 2023-03-26 10:15:26.000000 streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/PKG-INFO
--rw-r--r--   0 wrzr       (501) staff       (20)     1215 2023-03-26 10:15:26.000000 streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/SOURCES.txt
--rw-r--r--   0 wrzr       (501) staff       (20)        1 2023-03-26 10:15:26.000000 streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/dependency_links.txt
--rw-r--r--   0 wrzr       (501) staff       (20)       59 2023-03-26 10:15:26.000000 streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/requires.txt
--rw-r--r--   0 wrzr       (501) staff       (20)       20 2023-03-26 10:15:26.000000 streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/top_level.txt
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.746785 streamlit-searchbox-0.1.3/
+-rw-rw-r--   0 wrzr       (501) staff       (20)     1063 2022-04-12 22:00:53.000000 streamlit-searchbox-0.1.3/LICENSE
+-rw-rw-r--   0 wrzr       (501) staff       (20)       55 2022-05-29 16:47:35.000000 streamlit-searchbox-0.1.3/MANIFEST.in
+-rw-r--r--   0 wrzr       (501) staff       (20)      410 2023-04-15 06:31:26.746642 streamlit-searchbox-0.1.3/PKG-INFO
+-rw-r--r--   0 wrzr       (501) staff       (20)     2020 2023-03-26 10:06:13.000000 streamlit-searchbox-0.1.3/README.md
+-rw-r--r--   0 wrzr       (501) staff       (20)       38 2023-04-15 06:31:26.746817 streamlit-searchbox-0.1.3/setup.cfg
+-rw-r--r--   0 wrzr       (501) staff       (20)      694 2023-04-15 06:27:17.000000 streamlit-searchbox-0.1.3/setup.py
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.738988 streamlit-searchbox-0.1.3/streamlit_searchbox/
+-rw-r--r--   0 wrzr       (501) staff       (20)     4699 2023-04-15 06:28:20.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/__init__.py
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.737611 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.741160 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/
+-rw-r--r--   0 wrzr       (501) staff       (20)     1023 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/asset-manifest.json
+-rw-rw-r--   0 wrzr       (501) staff       (20)   197452 2023-04-15 06:28:48.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/bootstrap.min.css
+-rw-r--r--   0 wrzr       (501) staff       (20)     2083 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/index.html
+-rw-r--r--   0 wrzr       (501) staff       (20)      786 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/precache-manifest.2a78805e0087eaea58068ac04df3641d.js
+-rw-r--r--   0 wrzr       (501) staff       (20)     1183 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/service-worker.js
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.737793 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.746102 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/
+-rw-r--r--   0 wrzr       (501) staff       (20)   685180 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js
+-rw-r--r--   0 wrzr       (501) staff       (20)     1803 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.LICENSE.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)  2024895 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.map
+-rw-r--r--   0 wrzr       (501) staff       (20)     6296 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js
+-rw-r--r--   0 wrzr       (501) staff       (20)    18039 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js.map
+-rw-r--r--   0 wrzr       (501) staff       (20)     1580 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js
+-rw-r--r--   0 wrzr       (501) staff       (20)     8299 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js.map
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.746426 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/media/
+-rw-r--r--   0 wrzr       (501) staff       (20)      276 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/media/st-arrow.6dbfe07f.svg
+-rw-r--r--   0 wrzr       (501) staff       (20)      750 2023-04-15 06:28:52.000000 streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/media/st-clear.53d62d3c.svg
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2023-04-15 06:31:26.739808 streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/
+-rw-r--r--   0 wrzr       (501) staff       (20)      410 2023-04-15 06:31:26.000000 streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/PKG-INFO
+-rw-r--r--   0 wrzr       (501) staff       (20)     1215 2023-04-15 06:31:26.000000 streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)        1 2023-04-15 06:31:26.000000 streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)       59 2023-04-15 06:31:26.000000 streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/requires.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)       20 2023-04-15 06:31:26.000000 streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/top_level.txt
```

### Comparing `streamlit-searchbox-0.1.2/LICENSE` & `streamlit-searchbox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/README.md` & `streamlit-searchbox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/setup.py` & `streamlit-searchbox-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-searchbox",
-    version="0.1.2",
+    version="0.1.3",
     author="m-wrzr",
     description="Autocomplete Searchbox",
     long_description="Streamlit searchbox that dynamically updates "
     + "and provides a list of suggestions based on a provided function",
     long_description_content_type="text/plain",
     url="https://github.com/m-wrzr/streamlit-searchbox",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/__init__.py` & `streamlit-searchbox-0.1.3/streamlit_searchbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
     # nothing changed, avoid new search
     if searchterm == st.session_state[key]["search"]:
         return st.session_state[key]["result"]
 
     st.session_state[key]["search"] = searchterm
     search_results = search_function(searchterm)
 
-    if not search_results:
-        return st.session_state[key]["result"]
+    if search_results is None:
+        search_results = []
 
     def _get_label(label: any) -> str:
         return str(label[0]) if isinstance(label, tuple) else str(label)
 
     def _get_value(value: any) -> any:
         return value[1] if isinstance(value, tuple) else value
```

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/asset-manifest.json` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/bootstrap.min.css` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/index.html` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/precache-manifest.2a78805e0087eaea58068ac04df3641d.js` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/precache-manifest.2a78805e0087eaea58068ac04df3641d.js`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/service-worker.js` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.LICENSE.txt` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.map` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/2.1e75748d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js.map` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/main.3d532e07.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js.map` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/js/runtime-main.1401e97d.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox/frontend/build/static/media/st-clear.53d62d3c.svg` & `streamlit-searchbox-0.1.3/streamlit_searchbox/frontend/build/static/media/st-clear.53d62d3c.svg`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.2/streamlit_searchbox.egg-info/SOURCES.txt` & `streamlit-searchbox-0.1.3/streamlit_searchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

