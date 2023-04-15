# Comparing `tmp/al_otto-0.2.1.tar.gz` & `tmp/al_otto-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "al_otto-0.2.1.tar", last modified: Tue Apr  4 01:36:53 2023, max compression
+gzip compressed data, was "al_otto-0.2.2.tar", last modified: Sat Apr 15 18:02:58 2023, max compression
```

## Comparing `al_otto-0.2.1.tar` & `al_otto-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      354 2023-04-04 01:36:45.685910 al_otto-0.2.1/README.md
--rw-r--r--   0        0        0       34 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/__init__.py
--rw-r--r--   0        0        0       22 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/_version.py
--rw-r--r--   0        0        0     1268 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/chartransitions.py
--rw-r--r--   0        0        0      899 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/cliparse.py
--rw-r--r--   0        0        0    10667 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/colortransitions.py
--rw-r--r--   0        0        0      232 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/config.py
--rw-r--r--   0        0        0     1016 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/config_otto.json
--rw-r--r--   0        0        0      877 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/config_otto.json
--rw-r--r--   0        0        0     1887 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/data.csv
--rw-r--r--   0        0        0     1730 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/data.json
--rw-r--r--   0        0        0      581 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/example.json
--rw-r--r--   0        0        0      969 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/export.json
--rw-r--r--   0        0        0     1109 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/otto.json
--rw-r--r--   0        0        0     5048 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/examples/talavideo.json
--rw-r--r--   0        0        0      259 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/exceptions.py
--rwxr-xr-x   0        0        0       55 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/export.sh
--rw-r--r--   0        0        0     2268 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/getdata.py
--rw-r--r--   0        0        0      693 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/log.py
--rw-r--r--   0        0        0      947 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/main.py
--rw-r--r--   0        0        0     2381 2023-04-04 01:36:45.685910 al_otto-0.2.1/otto/models.py
--rw-r--r--   0        0        0      956 2023-04-04 01:36:45.689910 al_otto-0.2.1/otto/preview.py
--rw-r--r--   0        0        0     3390 2023-04-04 01:36:45.689910 al_otto-0.2.1/otto/render.py
--rw-r--r--   0        0        0    11732 2023-04-04 01:36:45.689910 al_otto-0.2.1/otto/templates.py
--rw-r--r--   0        0        0     1854 2023-04-04 01:36:45.689910 al_otto-0.2.1/otto/templates/VideoForm.html
--rw-r--r--   0        0        0      617 2023-04-04 01:36:45.689910 al_otto-0.2.1/otto/utils.py
--rw-r--r--   0        0        0     1331 2023-04-04 01:36:53.265843 al_otto-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2468 2023-04-04 01:36:45.689910 al_otto-0.2.1/tests/black.mp4
--rw-r--r--   0        0        0      316 2023-04-04 01:36:45.689910 al_otto-0.2.1/tests/black.png
--rw-r--r--   0        0        0      933 2023-04-04 01:36:45.689910 al_otto-0.2.1/tests/test_otto.py
--rw-r--r--   0        0        0     3045 2023-04-04 01:36:45.689910 al_otto-0.2.1/tests/test_preview.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 al_otto-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2047 2023-04-15 18:02:49.866119 al_otto-0.2.2/README.md
+-rw-r--r--   0        0        0       61 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/_version.py
+-rw-r--r--   0        0        0     1268 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/chartransitions.py
+-rw-r--r--   0        0        0      899 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/cliparse.py
+-rw-r--r--   0        0        0    10667 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/colortransitions.py
+-rw-r--r--   0        0        0      232 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/config.py
+-rw-r--r--   0        0        0     1016 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/config_otto.json
+-rw-r--r--   0        0        0      877 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/config_otto.json
+-rw-r--r--   0        0        0     1887 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/data.csv
+-rw-r--r--   0        0        0     1730 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/data.json
+-rw-r--r--   0        0        0      581 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/example.json
+-rw-r--r--   0        0        0      969 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/export.json
+-rw-r--r--   0        0        0     1109 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/otto.json
+-rw-r--r--   0        0        0     5048 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/examples/talavideo.json
+-rw-r--r--   0        0        0      259 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/exceptions.py
+-rwxr-xr-x   0        0        0       55 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/export.sh
+-rw-r--r--   0        0        0     2268 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/getdata.py
+-rw-r--r--   0        0        0      693 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/log.py
+-rw-r--r--   0        0        0      947 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/main.py
+-rw-r--r--   0        0        0     2381 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/models.py
+-rw-r--r--   0        0        0      947 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/preview.py
+-rw-r--r--   0        0        0     3390 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/render.py
+-rw-r--r--   0        0        0    11732 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/templates.py
+-rw-r--r--   0        0        0     1854 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/templates/VideoForm.html
+-rw-r--r--   0        0        0      617 2023-04-15 18:02:49.866119 al_otto-0.2.2/otto/utils.py
+-rw-r--r--   0        0        0     1243 2023-04-15 18:02:58.662099 al_otto-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2468 2023-04-15 18:02:49.866119 al_otto-0.2.2/tests/black.mp4
+-rw-r--r--   0        0        0      316 2023-04-15 18:02:49.866119 al_otto-0.2.2/tests/black.png
+-rw-r--r--   0        0        0      933 2023-04-15 18:02:49.866119 al_otto-0.2.2/tests/test_otto.py
+-rw-r--r--   0        0        0     3045 2023-04-15 18:02:49.866119 al_otto-0.2.2/tests/test_preview.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 al_otto-0.2.2/PKG-INFO
```

### Comparing `al_otto-0.2.1/otto/chartransitions.py` & `al_otto-0.2.2/otto/chartransitions.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/cliparse.py` & `al_otto-0.2.2/otto/cliparse.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/colortransitions.py` & `al_otto-0.2.2/otto/colortransitions.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/config_otto.json` & `al_otto-0.2.2/otto/config_otto.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/config_otto.json` & `al_otto-0.2.2/otto/examples/config_otto.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/data.csv` & `al_otto-0.2.2/otto/examples/data.csv`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/data.json` & `al_otto-0.2.2/otto/examples/data.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/example.json` & `al_otto-0.2.2/otto/examples/example.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/export.json` & `al_otto-0.2.2/otto/examples/export.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/otto.json` & `al_otto-0.2.2/otto/examples/otto.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/examples/talavideo.json` & `al_otto-0.2.2/otto/examples/talavideo.json`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/getdata.py` & `al_otto-0.2.2/otto/getdata.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/log.py` & `al_otto-0.2.2/otto/log.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/main.py` & `al_otto-0.2.2/otto/main.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/models.py` & `al_otto-0.2.2/otto/models.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/preview.py` & `al_otto-0.2.2/otto/preview.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @previewAPI.post('/')
 async def previewFrame(t: float, render: Render):
     """# Preview frame
     Generates a frame of a given `edl` at time `t`, with `width` and `height`.
 
-     Returns the name of a file on this server when available, or a relevant error message
+    Returns the name of a file on this server when available, or a relevant error
     """
     print('previewing', render.edl, 'at frame', t)
     active_clips = [
         c for c in render.edl.clips if t >= (c.start or 0) + (c.offset or 0)
     ]
     print('generating active clips', active_clips, t)
     video = generateEdl(
```

### Comparing `al_otto-0.2.1/otto/render.py` & `al_otto-0.2.2/otto/render.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/templates.py` & `al_otto-0.2.2/otto/templates.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/templates/VideoForm.html` & `al_otto-0.2.2/otto/templates/VideoForm.html`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/otto/utils.py` & `al_otto-0.2.2/otto/utils.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/pyproject.toml` & `al_otto-0.2.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -8,59 +8,59 @@
 name = "al-otto"
 dynamic = []
 description = "The ottomatic video engine"
 authors = [
     { name = "Quaternion Media", email = "qm@quaternion.media" },
 ]
 dependencies = [
-    "fastapi<1.0.0,>=0.94.0",
-    "moviepy<2.0.0,>=1.0.3",
-    "pydantic<2.0.0,>=1.10.5",
+    "fastapi~=0.95",
+    "moviepy~=1.0",
+    "pydantic~=1.10",
 ]
 requires-python = ">=3.8.1,<4.0"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/quaternionmedia/otto"
 documentation = "https://quaternionmedia.github.io/otto/"
 repository = "https://github.com/quaternionmedia/otto"
 
 [project.optional-dependencies]
 render = [
-    "gizeh >= 0.1.11",
-    "bezier >= 2021.2.12",
-    "tqdm >= 4.64.1",
+    "gizeh~=0.1",
+    "bezier~=2021.2",
+    "tqdm~=4.65",
 ]
 test = [
-    "pytest >= 7.2.1",
-    "httpx >= 0.23.3",
-    "pytest-cov >= 4.0.0",
-    "pytest-xdist>=3.2.1",
+    "pytest~=7.3",
+    "httpx~=0.24",
+    "pytest-cov~=4.0",
+    "pytest-xdist~=3.2",
 ]
 docs = [
-    "mkdocs >= 1.4.2",
-    "mkdocs-material >= 9.1.2",
-    "mkdocs-git-revision-date-localized-plugin >= 1.2.0",
-    "mike >= 1.1.2",
-    "mkdocstrings[python] >= 0.20.0",
-    "setuptools",
+    "mkdocs~=1.4",
+    "mkdocs-material~=9.1",
+    "mkdocs-git-revision-date-localized-plugin~=1.2",
+    "mike~=1.1",
+    "mkdocstrings[python]~=0.21",
+    "setuptools~=67.6",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "uvicorn >= 0.21.1",
-    "black >= 23.1.0",
-    "flake8 >= 6.0.0",
+    "uvicorn~=0.21",
+    "black~=23.3",
+    "ruff~=0.0",
 ]
 nox = [
-    "nox >= 2022.11.21",
+    "nox~=2022.11",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "otto/_version.py"
 
 [tool.pytest.ini_options]
```

### Comparing `al_otto-0.2.1/tests/black.mp4` & `al_otto-0.2.2/tests/black.mp4`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/tests/test_otto.py` & `al_otto-0.2.2/tests/test_otto.py`

 * *Files identical despite different names*

### Comparing `al_otto-0.2.1/tests/test_preview.py` & `al_otto-0.2.2/tests/test_preview.py`

 * *Files identical despite different names*

