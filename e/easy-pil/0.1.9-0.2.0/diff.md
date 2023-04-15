# Comparing `tmp/easy-pil-0.1.9.tar.gz` & `tmp/easy-pil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-pil-0.1.9.tar", last modified: Thu Jul 28 08:33:34 2022, max compression
+gzip compressed data, was "easy-pil-0.2.0.tar", last modified: Sat Apr 15 12:11:22 2023, max compression
```

## Comparing `easy-pil-0.1.9.tar` & `easy-pil-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.853093 easy-pil-0.1.9/
--rw-rw-rw-   0        0        0     1055 2022-01-29 12:43:13.000000 easy-pil-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       62 2022-01-29 12:43:13.000000 easy-pil-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1863 2022-07-28 08:33:34.853093 easy-pil-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      812 2022-01-29 12:53:52.000000 easy-pil-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.834090 easy-pil-0.1.9/easy_pil/
--rw-rw-rw-   0        0        0      219 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/__init__.py
--rw-rw-rw-   0        0        0      208 2022-07-28 08:32:53.000000 easy-pil-0.1.9/easy_pil/_version.py
--rw-rw-rw-   0        0        0     1073 2022-02-05 13:46:25.000000 easy-pil-0.1.9/easy_pil/canvas.py
--rw-rw-rw-   0        0        0      127 2022-07-28 08:30:51.000000 easy-pil-0.1.9/easy_pil/color.py
--rw-rw-rw-   0        0        0    17630 2022-07-25 20:58:54.000000 easy-pil-0.1.9/easy_pil/editor.py
--rw-rw-rw-   0        0        0     3065 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/font.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.824091 easy-pil-0.1.9/easy_pil/fonts/
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.838089 easy-pil-0.1.9/easy_pil/fonts/caveat/
--rw-rw-rw-   0        0        0   256900 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/caveat/caveat.ttf
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.845098 easy-pil-0.1.9/easy_pil/fonts/montserrat/
--rw-rw-rw-   0        0        0   244468 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_bold.ttf
--rw-rw-rw-   0        0        0   249088 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_italic.ttf
--rw-rw-rw-   0        0        0   242068 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_light.ttf
--rw-rw-rw-   0        0        0   245708 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_regular.ttf
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.851092 easy-pil-0.1.9/easy_pil/fonts/poppins/
--rw-rw-rw-   0        0        0   153900 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_bold.ttf
--rw-rw-rw-   0        0        0   181972 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_italic.ttf
--rw-rw-rw-   0        0        0   159848 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_light.ttf
--rw-rw-rw-   0        0        0   158192 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_regular.ttf
--rw-rw-rw-   0        0        0      689 2022-07-25 20:42:29.000000 easy-pil-0.1.9/easy_pil/text.py
--rw-rw-rw-   0        0        0     1297 2022-01-29 12:43:13.000000 easy-pil-0.1.9/easy_pil/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:33:34.838089 easy-pil-0.1.9/easy_pil.egg-info/
--rw-rw-rw-   0        0        0     1863 2022-07-28 08:33:34.000000 easy-pil-0.1.9/easy_pil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2022-07-28 08:33:34.000000 easy-pil-0.1.9/easy_pil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-28 08:33:34.000000 easy-pil-0.1.9/easy_pil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2022-07-28 08:33:34.000000 easy-pil-0.1.9/easy_pil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-28 08:33:34.000000 easy-pil-0.1.9/easy_pil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-28 08:33:34.853093 easy-pil-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1857 2022-01-29 12:43:13.000000 easy-pil-0.1.9/setup.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1055 2023-04-14 18:03:37.000000 easy-pil-0.2.0/LICENSE
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       62 2023-04-14 18:03:37.000000 easy-pil-0.2.0/MANIFEST.in
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1845 2023-04-15 12:11:22.039843 easy-pil-0.2.0/PKG-INFO
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      812 2023-04-14 18:03:37.000000 easy-pil-0.2.0/README.md
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      253 2023-04-14 18:28:11.000000 easy-pil-0.2.0/easy_pil/__init__.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      201 2023-04-14 18:15:55.000000 easy-pil-0.2.0/easy_pil/_version.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1082 2023-04-15 11:41:28.000000 easy-pil-0.2.0/easy_pil/canvas.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)    17851 2023-04-15 11:31:58.000000 easy-pil-0.2.0/easy_pil/editor.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     3339 2023-04-14 18:15:55.000000 easy-pil-0.2.0/easy_pil/font.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil/fonts/
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil/fonts/caveat/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   256900 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/caveat/caveat.ttf
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/easy_pil/fonts/montserrat/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   244468 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_bold.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   249088 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_italic.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   242068 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_light.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   245708 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_regular.ttf
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/easy_pil/fonts/poppins/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   153900 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_bold.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   181972 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_italic.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   159848 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_light.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   158192 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_regular.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      807 2023-04-15 11:41:19.000000 easy-pil-0.2.0/easy_pil/text.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/easy_pil/types/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 11:29:53.000000 easy-pil-0.2.0/easy_pil/types/__init__.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      106 2023-04-15 11:31:59.000000 easy-pil-0.2.0/easy_pil/types/common.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1012 2023-04-15 11:31:58.000000 easy-pil-0.2.0/easy_pil/types/workspace.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1373 2023-04-14 18:15:55.000000 easy-pil-0.2.0/easy_pil/utils.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     6490 2023-04-15 11:48:03.000000 easy-pil-0.2.0/easy_pil/workspace.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil.egg-info/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1845 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/PKG-INFO
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      897 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/SOURCES.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        1 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/dependency_links.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      121 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/requires.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        9 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/top_level.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      408 2023-04-15 12:08:59.000000 easy-pil-0.2.0/pyproject.toml
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       38 2023-04-15 12:11:22.039843 easy-pil-0.2.0/setup.cfg
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     2085 2023-04-14 18:15:55.000000 easy-pil-0.2.0/setup.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/tests/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      288 2023-04-04 09:25:35.000000 easy-pil-0.2.0/tests/test_canvas.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     5152 2023-04-14 18:15:55.000000 easy-pil-0.2.0/tests/test_editor.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      705 2023-04-14 18:15:55.000000 easy-pil-0.2.0/tests/test_utils.py
```

### Comparing `easy-pil-0.1.9/LICENSE` & `easy-pil-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/PKG-INFO` & `easy-pil-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1
-Name: easy-pil
-Version: 0.1.9
-Summary: A library to make common tasks of Pillow easy.
-Home-page: https://github.com/shahriyardx/easy-pil
-Author: Md Shahriyar Alam
-Author-email: contact@shahriyar.dev
-Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
-Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
-Project-URL: Source, https://github.com/shahriyardx/easy-pil/
-Keywords: Pillow,PIL,Pillow wrapper,PIL wrapper,Easy Pillow,Easy PIL,discord rank card,discord card
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Easy PIL
-A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
-
-## Getting Started
-Using this for the first time? Here are some links to help you get started.
-
-- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
-- First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
-- Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
-- Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
-- [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
-
-## Get help
-- Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
-- Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
+Metadata-Version: 2.1
+Name: easy-pil
+Version: 0.2.0
+Summary: A library to make common tasks of Pillow easy.
+Home-page: https://github.com/shahriyardx/easy-pil
+Author: Md Shahriyar Alam
+Author-email: contact@shahriyar.dev
+Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
+Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
+Project-URL: Source, https://github.com/shahriyardx/easy-pil/
+Keywords: Pillow,PIL,Pillow wrapper,PIL wrapper,Easy Pillow,Easy PIL,discord rank card,discord card
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Easy PIL
+A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+
+## Getting Started
+Using this for the first time? Here are some links to help you get started.
+
+- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
+- First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
+- Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
+- Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
+- [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
+
+## Get help
+- Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
+- Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
```

### Comparing `easy-pil-0.1.9/README.md` & `easy-pil-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/canvas.py` & `easy-pil-0.2.0/easy_pil/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Tuple, Union
 
 from PIL import Image
 
-from .color import Color
+from .types.common import Color
+
 
 class Canvas:
     """Canvas class
 
     Parameters
     ----------
     size : Tuple[float, float], optional
```

### Comparing `easy-pil-0.1.9/easy_pil/editor.py` & `easy-pil-0.2.0/easy_pil/editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,63 +5,65 @@
 
 from PIL import Image, ImageDraw, ImageFilter, ImageFont
 from typing_extensions import Literal
 
 from .canvas import Canvas
 from .font import Font
 from .text import Text
-from .color import Color
+from .types.common import Color
 
 
 class Editor:
     """Editor class. It does all the editing operations.
 
     Parameters
     ----------
     image : Union[Image.Image, str, Editor, Canvas]
         Image or Canvas to edit.
     """
 
-    def __init__(self, image: Union[Image.Image, str, BytesIO, Editor, Canvas]) -> None:
+    def __init__(
+        self, image: Union[Image.Image, str, BytesIO, Editor, Canvas]
+    ) -> None:
+        self.image = None
+
         if isinstance(image, str) or isinstance(image, BytesIO):
-            self.image = Image.open(image)
+            self.image = Image.open(image).convert("RGBA")
         elif isinstance(image, Canvas) or isinstance(image, Editor):
-            self.image = image.image
+            self.image = image.image.convert("RGBA")
         else:
-            self.image = image
-
-        self.image = self.image.convert("RGBA")
+            self.image = image.convert("RGBA")
 
     @property
     def image_bytes(self) -> BytesIO:
         """Return image bytes
 
         Returns
         -------
         BytesIO
             Bytes from the image of Editor
         """
         _bytes = BytesIO()
         self.image.save(_bytes, "png")
-        _bytes.seek(0)
 
+        _bytes.seek(0)
         return _bytes
 
     def resize(self, size: Tuple[float, float], crop=False) -> Editor:
         """Resize image
 
         Parameters
         ----------
         size : Tuple[float, float]
             New Size of image
         crop : bool, optional
             Crop the image to bypass distortion, by default False
         """
         if not crop:
-            self.image = self.image.resize(size, Image.ANTIALIAS)
+            self.image = self.image.resize(size, Image.LANCZOS)
 
         else:
             width, height = self.image.size
             ideal_width, ideal_height = size
 
             aspect = width / float(height)
             ideal_aspect = ideal_width / float(ideal_height)
@@ -72,50 +74,64 @@
                 resize = (offset, 0, width - offset, height)
             else:
                 new_height = int(width / ideal_aspect)
                 offset = (height - new_height) / 2
                 resize = (0, offset, width, height - offset)
 
             self.image = self.image.crop(resize).resize(
-                (ideal_width, ideal_height), Image.ANTIALIAS
+                (ideal_width, ideal_height), Image.LANCZOS
             )
 
         return self
 
     def rounded_corners(self, radius: int = 10, offset: int = 2) -> Editor:
         """Make image rounded corners
 
         Parameters
         ----------
         radius : int, optional
             Radius of roundness, by default 10
         offset : int, optional
             Offset pixel while making rounded, by default 2
         """
-        background = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
-        holder = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
-        mask = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
+        background = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
+        holder = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
+        mask = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
         mask_draw = ImageDraw.Draw(mask)
         mask_draw.rounded_rectangle(
-            (offset, offset) + (self.image.size[0] - offset, self.image.size[1] - offset),
+            (offset, offset)
+            + (self.image.size[0] - offset, self.image.size[1] - offset),
             radius=radius,
             fill="black",
         )
         holder.paste(self.image, (0, 0))
         self.image = Image.composite(holder, background, mask)
 
         return self
 
     def circle_image(self) -> Editor:
         """Make image circle"""
-        background = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
-        holder = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
-        mask = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
+        background = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
+        holder = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
+        mask = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
         mask_draw = ImageDraw.Draw(mask)
-        mask_draw.ellipse((0, 0) + self.image.size, fill="black")
+        ellipse_size = tuple(i - 1 for i in self.image.size)
+        mask_draw.ellipse((0, 0) + ellipse_size, fill="black")
         holder.paste(self.image, (0, 0))
         self.image = Image.composite(holder, background, mask)
 
         return self
 
     def rotate(self, deg: float = 0, expand: bool = False) -> Editor:
         """Rotate image
@@ -141,15 +157,17 @@
             Blur mode, by default "gussian"
         amount : float, optional
             Amount of blur, by default 1
         """
         if mode == "box":
             self.image = self.image.filter(ImageFilter.BoxBlur(radius=amount))
         if mode == "gussian":
-            self.image = self.image.filter(ImageFilter.GaussianBlur(radius=amount))
+            self.image = self.image.filter(
+                ImageFilter.GaussianBlur(radius=amount)
+            )
 
         return self
 
     def blend(
         self,
         image: Union[Image.Image, Editor, Canvas],
         alpha: float = 0.0,
@@ -176,26 +194,30 @@
             self.image = Image.blend(self.image, image, alpha=alpha)
         else:
             self.image = Image.blend(image, self.image, alpha=alpha)
 
         return self
 
     def paste(
-        self, image: Union[Image.Image, Editor, Canvas], position: Tuple[float, float]
+        self,
+        image: Union[Image.Image, Editor, Canvas],
+        position: Tuple[float, float],
     ) -> Editor:
         """Paste image into editor
 
         Parameters
         ----------
         image : Union[Image.Image, Editor, Canvas]
             Image to paste
         position : Tuple[float, float]
             Position to paste
         """
-        blank = Image.new("RGBA", size=self.image.size, color=(255, 255, 255, 0))
+        blank = Image.new(
+            "RGBA", size=self.image.size, color=(255, 255, 255, 0)
+        )
 
         if isinstance(image, Editor) or isinstance(image, Canvas):
             image = image.image
 
         blank.paste(image, position)
         self.image = Image.alpha_composite(self.image, blank)
 
@@ -259,38 +281,35 @@
         if align == "left":
             position = position
 
         if align == "right":
             total_width = 0
 
             for text in texts:
-                total_width += text.font.getsize(text.text)[0]
+                total_width += text.font.getlength(text.text)
 
             position = (position[0] - total_width, position[1])
 
         if align == "center":
             total_width = 0
 
             for text in texts:
-                total_width += text.font.getsize(text.text)[0]
+                total_width += text.font.getlength(text.text)
 
             position = (position[0] - (total_width / 2), position[1])
 
         for text in texts:
             sentence = text.text
             font = text.font
             color = text.color
 
             if space_separated:
-                width, _ = (
-                    font.getsize(sentence)[0] + font.getsize(" ")[0],
-                    font.getsize(sentence)[1],
-                )
+                width = font.getlength(sentence + " ")
             else:
-                width, _ = font.getsize(sentence)
+                width = font.getlength(sentence)
 
             draw.text(position, sentence, color, font=font, anchor="lm")
             position = (position[0] + width, position[1])
 
         return self
 
     def rectangle(
```

### Comparing `easy-pil-0.1.9/easy_pil/font.py` & `easy-pil-0.2.0/easy_pil/font.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from memoization import cached
 from PIL import ImageFont
 from typing_extensions import Literal
 
 fonts_directory = os.path.join(os.path.dirname(__file__), "fonts")
 fonts_path = {
     "caveat": {
         "regular": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
@@ -11,22 +12,32 @@
         "italic": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
         "light": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
     },
     "montserrat": {
         "regular": os.path.join(
             fonts_directory, "montserrat", "montserrat_regular.ttf"
         ),
-        "bold": os.path.join(fonts_directory, "montserrat", "montserrat_bold.ttf"),
-        "italic": os.path.join(fonts_directory, "montserrat", "montserrat_italic.ttf"),
-        "light": os.path.join(fonts_directory, "montserrat", "montserrat_light.ttf"),
+        "bold": os.path.join(
+            fonts_directory, "montserrat", "montserrat_bold.ttf"
+        ),
+        "italic": os.path.join(
+            fonts_directory, "montserrat", "montserrat_italic.ttf"
+        ),
+        "light": os.path.join(
+            fonts_directory, "montserrat", "montserrat_light.ttf"
+        ),
     },
     "poppins": {
-        "regular": os.path.join(fonts_directory, "poppins", "poppins_regular.ttf"),
+        "regular": os.path.join(
+            fonts_directory, "poppins", "poppins_regular.ttf"
+        ),
         "bold": os.path.join(fonts_directory, "poppins", "poppins_bold.ttf"),
-        "italic": os.path.join(fonts_directory, "poppins", "poppins_italic.ttf"),
+        "italic": os.path.join(
+            fonts_directory, "poppins", "poppins_italic.ttf"
+        ),
         "light": os.path.join(fonts_directory, "poppins", "poppins_light.ttf"),
     },
 }
 
 
 class Font:
     """Font class
@@ -38,15 +49,19 @@
     size : int, optional
         Size of font, by default 10
     """
 
     def __init__(self, path: str, size: int = 10, **kwargs) -> None:
         self.font = ImageFont.truetype(path, size=size, **kwargs)
 
+    def getsize(self, text: str):
+        return self.font.getsize(text)
+
     @staticmethod
+    @cached()
     def poppins(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Poppins font
 
         Parameters
@@ -55,14 +70,15 @@
             Font variant, by default "regular"
         size : int, optional
             Font size, by default 10
         """
         return ImageFont.truetype(fonts_path["poppins"][variant], size=size)
 
     @staticmethod
+    @cached()
     def caveat(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Caveat font
 
         Parameters
@@ -71,14 +87,15 @@
             Font variant, by default "regular"
         size : int, optional
             Font size, by default 10
         """
         return ImageFont.truetype(fonts_path["caveat"][variant], size=size)
 
     @staticmethod
+    @cached()
     def montserrat(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Montserrat font
 
         Parameters
```

### Comparing `easy-pil-0.1.9/easy_pil/fonts/caveat/caveat.ttf` & `easy-pil-0.2.0/easy_pil/fonts/caveat/caveat.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_bold.ttf` & `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_italic.ttf` & `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_light.ttf` & `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/montserrat/montserrat_regular.ttf` & `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_bold.ttf` & `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_italic.ttf` & `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_light.ttf` & `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/fonts/poppins/poppins_regular.ttf` & `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.1.9/easy_pil/text.py` & `easy-pil-0.2.0/easy_pil/text.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, Union
 
 from PIL import ImageFont
 
-from .color import Color
 from .font import Font
 
+
 class Text:
     """Text class
 
     Parameters
     ----------
     text : str
         Text
@@ -18,17 +18,21 @@
         Font color, by default "black"
     """
 
     def __init__(
         self,
         text: str,
         font: Union[ImageFont.FreeTypeFont, Font],
-        color: Color = "black",
+        color: Union[
+            int, str, Tuple[int, int, int], Tuple[int, int, int, int]
+        ] = "black",
     ) -> None:
         self.text = text
         self.color = color
 
         if isinstance(font, Font):
             self.font = font.font
         else:
             self.font = font
-            
+
+    def getsize(self):
+        return self.font.getsize(self.text)
```

### Comparing `easy-pil-0.1.9/easy_pil/utils.py` & `easy-pil-0.2.0/easy_pil/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import functools
 from io import BytesIO
 
 import aiohttp
 import requests
+from memoization import cached
 from PIL import Image
 
 
 async def run_in_executor(func, **kwargs):
     """Run function in executor
 
     Parameters
@@ -16,14 +17,15 @@
         Function to run
     """
     func = functools.partial(func, **kwargs)
     data = await asyncio.get_event_loop().run_in_executor(None, func)
     return data
 
 
+@cached(max_size=50)
 def load_image(link: str) -> Image.Image:
     """Load image from link
 
     Parameters
     ----------
     link : str
         Image link
@@ -35,14 +37,15 @@
     """
     _bytes = BytesIO(requests.get(link).content)
     image = Image.open(_bytes).convert("RGBA")
 
     return image
 
 
+@cached(max_size=50)
 async def load_image_async(link: str) -> Image.Image:
     """Load image from link (async)
 
     Parameters
     ----------
     link : str
         Image from the provided link (if any)
```

### Comparing `easy-pil-0.1.9/easy_pil.egg-info/PKG-INFO` & `easy-pil-0.2.0/easy_pil.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1
-Name: easy-pil
-Version: 0.1.9
-Summary: A library to make common tasks of Pillow easy.
-Home-page: https://github.com/shahriyardx/easy-pil
-Author: Md Shahriyar Alam
-Author-email: contact@shahriyar.dev
-Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
-Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
-Project-URL: Source, https://github.com/shahriyardx/easy-pil/
-Keywords: Pillow,PIL,Pillow wrapper,PIL wrapper,Easy Pillow,Easy PIL,discord rank card,discord card
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Easy PIL
-A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
-
-## Getting Started
-Using this for the first time? Here are some links to help you get started.
-
-- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
-- First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
-- Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
-- Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
-- [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
-
-## Get help
-- Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
-- Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
+Metadata-Version: 2.1
+Name: easy-pil
+Version: 0.2.0
+Summary: A library to make common tasks of Pillow easy.
+Home-page: https://github.com/shahriyardx/easy-pil
+Author: Md Shahriyar Alam
+Author-email: contact@shahriyar.dev
+Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
+Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
+Project-URL: Source, https://github.com/shahriyardx/easy-pil/
+Keywords: Pillow,PIL,Pillow wrapper,PIL wrapper,Easy Pillow,Easy PIL,discord rank card,discord card
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Easy PIL
+A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+
+## Getting Started
+Using this for the first time? Here are some links to help you get started.
+
+- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
+- First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
+- Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
+- Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
+- [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
+
+## Get help
+- Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
+- Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
```

### Comparing `easy-pil-0.1.9/setup.py` & `easy-pil-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-with open("requirements.txt") as f:
-    requirements = f.read().splitlines()
-
 current_directory = Path(__file__).parent.resolve()
 
-long_description = (current_directory / "README.md").read_text(encoding="utf-8")
 
-vpath = current_directory / "easy_pil" / "_version.py"
-spec = spec_from_file_location(vpath.name[:-3], vpath)
-mod = module_from_spec(spec)
-spec.loader.exec_module(mod)
+def _get_requirements() -> list:
+    with open("requirements.txt") as f:
+        return f.read().splitlines()
+
+
+def _get_long_desc() -> str:
+    return (current_directory / "README.md").read_text(encoding="utf-8")
+
+
+def _get_version() -> str:
+    vpath = current_directory / "easy_pil" / "_version.py"
+    spec = spec_from_file_location(vpath.name[:-3], vpath)
+    mod = module_from_spec(spec)
+    spec.loader.exec_module(mod)
+
+    return mod.__version__
+
 
 setup(
     name="easy-pil",
-    version=mod.__version__,
+    version=_get_version(),
     description="A library to make common tasks of Pillow easy.",  # Optional
-    long_description=long_description,
+    long_description=_get_long_desc(),
     long_description_content_type="text/markdown",
     url="https://github.com/shahriyardx/easy-pil",
     author="Md Shahriyar Alam",
     author_email="contact@shahriyar.dev",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
@@ -36,14 +45,17 @@
     ],
     keywords="Pillow, PIL, Pillow wrapper, PIL wrapper, Easy Pillow, Easy PIL, discord rank card, discord card",
     packages=find_packages(),
     package_data={
         "easy_pil": ["fonts/*/*.ttf"],
     },
     python_requires=">=3.7, <4",
-    install_requires=requirements,
+    install_requires=_get_requirements(),
+    extras_require={
+        "dev": ["black", "isort", "click", "twine"],
+    },
     project_urls={
         "Documentation": "https://easy-pil.readthedocs.io/en/latest/",
         "Bug Reports": "https://github.com/shahriyardx/easy-pil/issues",
         "Source": "https://github.com/shahriyardx/easy-pil/",
     },
 )
```

