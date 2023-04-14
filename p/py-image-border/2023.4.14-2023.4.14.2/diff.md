# Comparing `tmp/py-image-border-2023.4.14.tar.gz` & `tmp/py-image-border-2023.4.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-image-border-2023.4.14.tar", last modified: Fri Apr 14 21:06:41 2023, max compression
+gzip compressed data, was "py-image-border-2023.4.14.2.tar", last modified: Fri Apr 14 23:20:05 2023, max compression
```

## Comparing `py-image-border-2023.4.14.tar` & `py-image-border-2023.4.14.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1929 2023-04-14 18:55:23.420992 py-image-border-2023.4.14/README.md
--rw-r--r--   0        0        0        0 2023-04-14 18:09:58.625472 py-image-border-2023.4.14/py_image_border/__init__.py
--rw-r--r--   0        0        0      693 2023-04-14 18:41:53.719451 py-image-border-2023.4.14/py_image_border/add_border.py
--rw-r--r--   0        0        0     1658 2023-04-14 18:03:50.361451 py-image-border-2023.4.14/py_image_border/cli.py
--rw-r--r--   0        0        0      981 2023-04-14 18:42:03.108403 py-image-border-2023.4.14/py_image_border/image_processing.py
--rw-r--r--   0        0        0      662 2023-04-14 20:05:25.463654 py-image-border-2023.4.14/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 py-image-border-2023.4.14/PKG-INFO
+-rw-r--r--   0        0        0     1983 2023-04-14 23:14:56.400871 py-image-border-2023.4.14.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 18:09:58.625472 py-image-border-2023.4.14.2/py_image_border/__init__.py
+-rw-r--r--   0        0        0      693 2023-04-14 18:41:53.719451 py-image-border-2023.4.14.2/py_image_border/add_border.py
+-rw-r--r--   0        0        0     1658 2023-04-14 18:03:50.361451 py-image-border-2023.4.14.2/py_image_border/cli.py
+-rw-r--r--   0        0        0      981 2023-04-14 18:42:03.108403 py-image-border-2023.4.14.2/py_image_border/image_processing.py
+-rw-r--r--   0        0        0      664 2023-04-14 23:15:32.314092 py-image-border-2023.4.14.2/pyproject.toml
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 py-image-border-2023.4.14.2/PKG-INFO
```

### Comparing `py-image-border-2023.4.14/README.md` & `py-image-border-2023.4.14.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,10 +60,10 @@
 Notes
 ---
 
 This project was motivated by the lack of an easy, consistent way to add borders to screenshots on macOS.
 
 The test image is a bear I caught with a game camera, scratching its back against a tree:
 
-![Bear scratching its back against a tree](tests/reference_images/bear_scratching_default.jpg)
+![Bear scratching its back against a tree](https://github.com/ehmatthes/py-image-border/raw/main/tests/reference_images/bear_scratching_default.jpg)
 
 I had left the game camera out much longer than expected, and had about 100k images to go through. I wrote a Python script to flag any image with an area of dark pixels. This was one of about 12 images flagged. :)
```

### Comparing `py-image-border-2023.4.14/py_image_border/add_border.py` & `py-image-border-2023.4.14.2/py_image_border/add_border.py`

 * *Files identical despite different names*

### Comparing `py-image-border-2023.4.14/py_image_border/cli.py` & `py-image-border-2023.4.14.2/py_image_border/cli.py`

 * *Files identical despite different names*

### Comparing `py-image-border-2023.4.14/py_image_border/image_processing.py` & `py-image-border-2023.4.14.2/py_image_border/image_processing.py`

 * *Files identical despite different names*

### Comparing `py-image-border-2023.4.14/pyproject.toml` & `py-image-border-2023.4.14.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "py-image-border"
-version = "2023.04.14"
+version = "2023.04.14.2"
 authors = [
     { name="Eric Matthes" },
 ]
 description = "Add a border to any image."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `py-image-border-2023.4.14/PKG-INFO` & `py-image-border-2023.4.14.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-image-border
-Version: 2023.4.14
+Version: 2023.4.14.2
 Summary: Add a border to any image.
 Author: Eric Matthes
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,10 +74,10 @@
 Notes
 ---
 
 This project was motivated by the lack of an easy, consistent way to add borders to screenshots on macOS.
 
 The test image is a bear I caught with a game camera, scratching its back against a tree:
 
-![Bear scratching its back against a tree](tests/reference_images/bear_scratching_default.jpg)
+![Bear scratching its back against a tree](https://github.com/ehmatthes/py-image-border/raw/main/tests/reference_images/bear_scratching_default.jpg)
 
 I had left the game camera out much longer than expected, and had about 100k images to go through. I wrote a Python script to flag any image with an area of dark pixels. This was one of about 12 images flagged. :)
```

