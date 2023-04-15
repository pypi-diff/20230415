# Comparing `tmp/jupyter_capture_output-0.0.8.tar.gz` & `tmp/jupyter_capture_output-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_capture_output-0.0.8.tar", max compression
+gzip compressed data, was "jupyter_capture_output-0.0.9.tar", max compression
```

## Comparing `jupyter_capture_output-0.0.8.tar` & `jupyter_capture_output-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2022-10-27 06:44:41.372924 jupyter_capture_output-0.0.8/LICENSE
--rw-r--r--   0        0        0     2535 2022-10-27 06:44:41.372924 jupyter_capture_output-0.0.8/README.md
--rw-r--r--   0        0        0      395 2022-10-27 06:44:41.372924 jupyter_capture_output-0.0.8/jupyter_capture_output/__init__.py
--rw-r--r--   0        0        0     6687 2022-10-27 06:44:41.372924 jupyter_capture_output-0.0.8/jupyter_capture_output/co_cellmagic.py
--rw-r--r--   0        0        0      635 2022-10-27 06:44:41.372924 jupyter_capture_output-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 jupyter_capture_output-0.0.8/setup.py
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 jupyter_capture_output-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-02-27 20:11:20.436050 jupyter_capture_output-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3197 2023-02-27 20:11:20.436050 jupyter_capture_output-0.0.9/README.md
+-rw-r--r--   0        0        0      395 2023-02-27 20:11:20.436050 jupyter_capture_output-0.0.9/jupyter_capture_output/__init__.py
+-rw-r--r--   0        0        0     6687 2023-02-27 20:11:20.440050 jupyter_capture_output-0.0.9/jupyter_capture_output/co_cellmagic.py
+-rw-r--r--   0        0        0      635 2023-02-27 20:11:20.440050 jupyter_capture_output-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 jupyter_capture_output-0.0.9/setup.py
+-rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 jupyter_capture_output-0.0.9/PKG-INFO
```

### Comparing `jupyter_capture_output-0.0.8/LICENSE` & `jupyter_capture_output-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_capture_output-0.0.8/jupyter_capture_output/co_cellmagic.py` & `jupyter_capture_output-0.0.9/jupyter_capture_output/co_cellmagic.py`

 * *Files identical despite different names*

### Comparing `jupyter_capture_output-0.0.8/pyproject.toml` & `jupyter_capture_output-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "jupyter-capture-output"
-version = "0.0.8"
+version = "0.0.9"
 description = "Capture output from JupyterLab"
 authors = ["kolibril13 <44469195+kolibril13@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.14"
 ipython = ">=6.0.0"
 ipykernel = ">=5.0.0"
 Pillow = ">=9.1.0"
 
 [tool.poetry.dev-dependencies]
 black = {extras = ["jupyter"], version = ">=22.3.0"}
 matplotlib = ">=3.5.1"
```

### Comparing `jupyter_capture_output-0.0.8/setup.py` & `jupyter_capture_output-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,108 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# jupyter-caputure-output
+A cell magic that captures jupyter cell output
 
-packages = \
-['jupyter_capture_output']
 
-package_data = \
-{'': ['*']}
+[![JupyterLight](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://octoframes.github.io/jupyter_capture_output/)  
 
-install_requires = \
-['Pillow>=9.1.0', 'ipykernel>=5.0.0', 'ipython>=6.0.0']
-
-setup_kwargs = {
-    'name': 'jupyter-capture-output',
-    'version': '0.0.8',
-    'description': 'Capture output from JupyterLab',
-    'long_description': '# jupyter-caputure-output\nA cell magic that captures jupyter cell output\n\n\n[![JupyterLight](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://octoframes.github.io/jupyter_capture_output/)  \n\n## Install\nRequires Python >=3.8\n```py\npip install jupyter_capture_output\n```\n\n\n## Example\n\nhttps://user-images.githubusercontent.com/44469195/184531492-6bc34ed9-3640-447b-b09e-767d01ecf3da.mov\n\n\n```py\nimport jupyter_capture_output\n```\n\n```py \n%%capture_text --path "foo.txt"\nprint("Hello World")\n```\n\n```py\nimport matplotlib.pyplot as plt\n```\n\n```py\n%%capture_img --path "foo.png bar.png"\nplt.plot([1,2],[10,20])\nplt.show()\nplt.plot([3,4],[-10,-20])\nplt.show()\n```\n\n```py\n%%capture_img  --path "foo.jpg bar.jpg" --compression 50\nplt.plot([1,2],[10,20], color = "r")\nplt.show()\nplt.plot([3,4],[-10,-20],color = "r")\nplt.show()\n```\n\n\n\nImplemented\n* `%%capture_text`  ->  to .txt file with text output\n* `%%capture_img` -> to .png or .jpg with image output\n* `%%capture_video` -> to .mp4 file with the video output\n\n## Wishlist\n\n* `%%capture_svg` ->  to .svg file with svg vectorgraphic outout\n* `%%capture_numpy_array` -> to .np file with array \n* `%%capture_csv` -> to .csv with datapoints \n* `%%capture_gif` -> to .gif with animation\n* `%%capture_auto`-> automatically detects what output there is to capture\n\n## Changelog\n\n### 0.0.8 \n*  Add `capture_code` magic. Because this is not cell output but cell content, it might be worth to think about renaming this project from `capture-output` to only `capture` or even `capture-content`.\n* `remove experimental_capture_video_first_last` and `experimental_video_thumbnail` again. This package is not the right place for that.\n\n### 0.0.7 \n\n* Add relative path support and automatically create paths if they don\'t exist yet.\n\nAdd some experimental magic, but this will likely be removed in future versions:\n* * `experimental_capture_video_first_last` captures video and extracts first and last frame from it. Useful for post-processing of videos in other video editors. Needs ffmpeg installed\n\n* `experimental_video_thumbnail` extracts video from the Jupyter cell output, and replaces it with an image thumbnail of the video -> useful for Version control. Needs matplotlib and ffmpeg installed\n### 0.0.6\n\nbetter regex in capture video\nchange example images to dogs\n\n### 0.0.5\n\nRemove debugging code\nAdd JupyterLiteDemo\n### 0.0.4\n\nAdd Text and Video capture cell magic\nupdate example\n\n### 0.0.3\n\nSetup automatic release action.\n\n### 0.0.2\n\nUpdate example\n\n### 0.0.1\n\nInitial release\n',
-    'author': 'kolibril13',
-    'author_email': '44469195+kolibril13@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+## Install
+Requires Python >=3.8
+```py
+pip install jupyter_capture_output
+```
 
 
-setup(**setup_kwargs)
+## Example
+
+https://user-images.githubusercontent.com/44469195/199723257-ee428f53-d576-47be-93b9-d6ab98c46d8e.mov
+
+```py
+import jupyter_capture_output
+```
+
+```py 
+%%capture_text --path "foo.txt"
+print("Hello World")
+```
+
+```py
+import matplotlib.pyplot as plt
+```
+
+```py
+%%capture_img --path "foo.png bar.png"
+plt.plot([1,2],[10,20])
+plt.show()
+plt.plot([3,4],[-10,-20])
+plt.show()
+```
+
+```py
+%%capture_img  --path "foo.jpg bar.jpg" --compression 50
+plt.plot([1,2],[10,20], color = "r")
+plt.show()
+plt.plot([3,4],[-10,-20],color = "r")
+plt.show()
+```
+
+
+
+Implemented
+* `%%capture_text`  ->  to .txt file with text output
+* `%%capture_code`  ->  to .py file with cell content
+* `%%capture_img` -> to .png or .jpg with image output
+* `%%capture_video` -> to .mp4 file with the video output
+
+## Use cases
+
+* matplotlib, scipy, PIL , cv2, manim etc. have their own APIs to save images. With this package, one just have to learn one line of code and can use it to save all kind of image outputs made by different packages.
+
+* When tweaking plots, one can use this cell magic to track the process, so to say a visual version control system.
+
+* In context of Science, one can generate log files of experiments with this package. As the cell magic is always on the top of the cell, it's easy to see in which cells log files are generated and in which not.
+
+* This can be used to create sheet cheats, e.g. this [math-functions-cheat-sheet](https://kolibril13.github.io/plywood-gallery-functions/) website was generated from a jupyter notebook using a derivative of this capture package.
+
+* This package will also auto-generate the folder-tree of subdirectories for you.
+## Changelog
+
+
+### 0.0.9
+
+* support python 3.11
+### 0.0.8 
+*  Add `capture_code` magic. Because this is not cell output but cell content, it might be worth to think about renaming this project from `capture-output` to only `capture` or even `capture-content`.
+* `remove experimental_capture_video_first_last` and `experimental_video_thumbnail` again. This package is not the right place for that.
+
+### 0.0.7 
+
+* Add relative path support and automatically create paths if they don't exist yet.
+
+Add some experimental magic, but this will likely be removed in future versions:
+* * `experimental_capture_video_first_last` captures video and extracts first and last frame from it. Useful for post-processing of videos in other video editors. Needs ffmpeg installed
+
+* `experimental_video_thumbnail` extracts video from the Jupyter cell output, and replaces it with an image thumbnail of the video -> useful for Version control. Needs matplotlib and ffmpeg installed
+### 0.0.6
+
+better regex in capture video
+change example images to dogs
+
+### 0.0.5
+
+Remove debugging code
+Add JupyterLiteDemo
+### 0.0.4
+
+Add Text and Video capture cell magic
+update example
+
+### 0.0.3
+
+Setup automatic release action.
+
+### 0.0.2
+
+Update example
+
+### 0.0.1
+
+Initial release
```

