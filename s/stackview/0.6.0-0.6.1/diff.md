# Comparing `tmp/stackview-0.6.0.tar.gz` & `tmp/stackview-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackview-0.6.0.tar", last modified: Sun Mar 26 11:54:29 2023, max compression
+gzip compressed data, was "stackview-0.6.1.tar", last modified: Sat Apr 15 09:29:08 2023, max compression
```

## Comparing `stackview-0.6.0.tar` & `stackview-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 11:54:29.361131 stackview-0.6.0/
--rw-rw-rw-   0        0        0     1549 2022-06-18 13:26:20.000000 stackview-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     9608 2023-03-26 11:54:29.361131 stackview-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     9024 2023-03-26 11:39:00.000000 stackview-0.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-26 11:54:29.362131 stackview-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      948 2023-03-26 11:52:41.000000 stackview-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 11:54:29.348131 stackview-0.6.0/stackview/
--rw-rw-rw-   0        0        0      549 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/__init__.py
--rw-rw-rw-   0        0        0     7234 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_annotate.py
--rw-rw-rw-   0        0        0     5101 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_assist.py
--rw-rw-rw-   0        0        0     2060 2023-03-26 11:39:00.000000 stackview-0.6.0/stackview/_context.py
--rw-rw-rw-   0        0        0     4693 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_crop.py
--rw-rw-rw-   0        0        0     3572 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_curtain.py
--rw-rw-rw-   0        0        0     3852 2023-03-26 11:39:00.000000 stackview-0.6.0/stackview/_image_widget.py
--rw-rw-rw-   0        0        0     7090 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_interact.py
--rw-rw-rw-   0        0        0     1547 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_orthogonal.py
--rw-rw-rw-   0        0        0     2864 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_picker.py
--rw-rw-rw-   0        0        0     4500 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_side_by_side.py
--rw-rw-rw-   0        0        0     1683 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_slice.py
--rw-rw-rw-   0        0        0     2024 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_slice_viewer.py
--rw-rw-rw-   0        0        0     8266 2023-03-26 11:39:00.000000 stackview-0.6.0/stackview/_static_view.py
--rw-rw-rw-   0        0        0     2736 2023-03-26 11:52:41.000000 stackview-0.6.0/stackview/_switch.py
--rw-rw-rw-   0        0        0     1066 2023-03-26 11:39:00.000000 stackview-0.6.0/stackview/_uint_field.py
--rw-rw-rw-   0        0        0     2567 2023-03-26 11:39:00.000000 stackview-0.6.0/stackview/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-26 11:54:29.360131 stackview-0.6.0/stackview.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-03-26 11:54:29.000000 stackview-0.6.0/stackview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      585 2023-03-26 11:54:29.000000 stackview-0.6.0/stackview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 11:54:29.000000 stackview-0.6.0/stackview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-03-26 11:54:29.000000 stackview-0.6.0/stackview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-26 11:54:29.000000 stackview-0.6.0/stackview.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 09:29:08.228073 stackview-0.6.1/
+-rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0    10414 2023-04-15 09:29:08.228073 stackview-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9830 2023-04-15 09:27:34.000000 stackview-0.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 09:29:08.228073 stackview-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-04-15 09:27:34.000000 stackview-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:29:08.201527 stackview-0.6.1/stackview/
+-rw-rw-rw-   0        0        0      586 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/__init__.py
+-rw-rw-rw-   0        0        0     7781 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_annotate.py
+-rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.6.1/stackview/_assist.py
+-rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_colormaps.py
+-rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.6.1/stackview/_context.py
+-rw-rw-rw-   0        0        0     5487 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_crop.py
+-rw-rw-rw-   0        0        0     4684 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_curtain.py
+-rw-rw-rw-   0        0        0     4070 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_image_widget.py
+-rw-rw-rw-   0        0        0     7597 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_interact.py
+-rw-rw-rw-   0        0        0     2124 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_orthogonal.py
+-rw-rw-rw-   0        0        0     3384 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_picker.py
+-rw-rw-rw-   0        0        0     5023 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_side_by_side.py
+-rw-rw-rw-   0        0        0     2149 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_slice.py
+-rw-rw-rw-   0        0        0     2350 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_slice_viewer.py
+-rw-rw-rw-   0        0        0     8266 2023-01-15 16:10:46.000000 stackview-0.6.1/stackview/_static_view.py
+-rw-rw-rw-   0        0        0     6146 2023-04-15 09:27:34.000000 stackview-0.6.1/stackview/_switch.py
+-rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.6.1/stackview/_uint_field.py
+-rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.6.1/stackview/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:29:08.225590 stackview-0.6.1/stackview.egg-info/
+-rw-rw-rw-   0        0        0    10414 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-15 09:29:08.000000 stackview-0.6.1/stackview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 09:29:07.000000 stackview-0.6.1/stackview.egg-info/top_level.txt
```

### Comparing `stackview-0.6.0/LICENSE` & `stackview-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stackview-0.6.0/PKG-INFO` & `stackview-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -162,14 +162,35 @@
     binary,
     labels
 ])
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch.gif)
 
+### Switch toggleable
+
+You can also view multiple channels with different colormaps at the same time using the `toggleable` parameter of `switch`. 
+It is recommended to also pass a list of colormaps. Colormap names can be taken from [Matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html) and stackview aims at compatibility with [microfilm](https://github.com/guiwitz/microfilm).
+
+```
+hela_cells = imread("data/hela-cells.tif")
+
+stackview.switch(
+    {"lysosomes":   hela_cells[:,:,0],
+     "mitochondria":hela_cells[:,:,1],
+     "nuclei":      hela_cells[:,:,2]
+    },
+    colormap=["pure_magenta", "pure_green", "pure_blue"],
+    toggleable=True
+)
+```
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch_toggleable.gif)
+
+
 ### Crop
 
 You can crop images interactively:
 ```python
 crop_widget = stackview.crop(image_stack, continuous_update=True)
 crop_widget
 ```
```

### Comparing `stackview-0.6.0/README.md` & `stackview-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,35 @@
     binary,
     labels
 ])
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch.gif)
 
+### Switch toggleable
+
+You can also view multiple channels with different colormaps at the same time using the `toggleable` parameter of `switch`. 
+It is recommended to also pass a list of colormaps. Colormap names can be taken from [Matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html) and stackview aims at compatibility with [microfilm](https://github.com/guiwitz/microfilm).
+
+```
+hela_cells = imread("data/hela-cells.tif")
+
+stackview.switch(
+    {"lysosomes":   hela_cells[:,:,0],
+     "mitochondria":hela_cells[:,:,1],
+     "nuclei":      hela_cells[:,:,2]
+    },
+    colormap=["pure_magenta", "pure_green", "pure_blue"],
+    toggleable=True
+)
+```
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch_toggleable.gif)
+
+
 ### Crop
 
 You can crop images interactively:
 ```python
 crop_widget = stackview.crop(image_stack, continuous_update=True)
 crop_widget
 ```
```

### Comparing `stackview-0.6.0/setup.py` & `stackview-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackview",
-    version="0.6.0",
+    version="0.6.1",
     author="Robert Haase",
     author_email="robert.haase@tu-dresden.de",
     description="Interactive image stack viewing in jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/haesleinhuepf/stackview/",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=["numpy!=1.19.4", "ipycanvas", "ipywidgets", "scikit-image", "ipyevents", "toolz", "matplotlib"],
+    install_requires=["numpy!=1.19.4", "ipycanvas", "ipywidgets", "scikit-image", "ipyevents", "toolz", "matplotlib", "ipykernel"],
     python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Development Status :: 3 - Alpha",
```

### Comparing `stackview-0.6.0/stackview/__init__.py` & `stackview-0.6.1/stackview/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 from ._static_view import jupyter_displayable_output, insight
 from ._utilities import merge_rgb
 from ._context import nop
 from ._crop import crop
 from ._slice_viewer import _SliceViewer
 from ._annotate import annotate
@@ -11,11 +11,10 @@
 from ._slice import slice
 from ._curtain import curtain
 from ._orthogonal import orthogonal
 from ._side_by_side import side_by_side
 from ._picker import picker
 from ._assist import assist
 from ._switch import switch
-
-
+from ._colormaps import create_colormap
```

### Comparing `stackview-0.6.0/stackview/_annotate.py` & `stackview-0.6.1/stackview/_annotate.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         labels,
         slice_number: int = None,
         alpha: float = 0.5,
         axis: int = 0,
         continuous_update: bool = True,
         slider_text: str = "Slice",
         zoom_factor: float = 1.0,
-        zoom_spline_order: int = 0
+        zoom_spline_order: int = 0,
+        colormap:str = None,
+        display_min:float = None,
+        display_max:float = None
 ):
     """Shows an image with a slider to go through a stack plus a label with the current mouse position and intensity at that position.
 
     Parameters
     ----------
     image : image
         Image shown
@@ -45,14 +48,20 @@
         Alpha blending value for the labels on top of the image
     continuous_update : bool, optional
         Update the image while dragging the mouse on the slider, default: False
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
 
     Returns
     -------
     An ipywidget with an image display, a slider and a label showing mouse position and intensity.
     """
     from ._utilities import _no_resize
     from ._image_widget import _is_label_image, _img_to_rgb
@@ -97,16 +106,16 @@
             slice_image1 = image
             slice_image2 = labels
 
         if not _is_label_image(slice_image2):
             # necessary to display the labels in colour correctly
             slice_image2 = slice_image2.astype(np.uint64)
 
-        rgb_image1 = _img_to_rgb(slice_image1)
-        rgb_image2 = _img_to_rgb(slice_image2)
+        rgb_image1 = _img_to_rgb(slice_image1, colormap=colormap, display_min=display_min, display_max=display_max)
+        rgb_image2 = _img_to_rgb(slice_image2, colormap=colormap, display_min=display_min, display_max=display_max)
 
         factor1 = 1.0 - alpha
         factor2 = alpha
 
         rgb_mix = factor1 * rgb_image1 + factor2 * rgb_image2
 
         view.data = rgb_mix
@@ -182,15 +191,16 @@
                             axis,
                             radius,
                             label_id_to_draw,
                             labels)
 
         # store position
         for i in range(4):
-            former_drawn_position[i] = position[i]
+            if i < len(position):
+                former_drawn_position[i] = position[i]
         update_display()
 
     # draw everything once
     update_display()
 
     # connect events
     event_handler.on_dom_event(update_display_while_drawing)
```

### Comparing `stackview-0.6.0/stackview/_assist.py` & `stackview-0.6.1/stackview/_assist.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.0/stackview/_context.py` & `stackview-0.6.1/stackview/_context.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.0/stackview/_crop.py` & `stackview-0.6.1/stackview/_crop.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 def crop(image,
          slice_number: int = None,
          axis: int = 0,
          continuous_update: bool = True,
          slider_text: str = "Slice",
          axis_names=None,
          zoom_factor: float = 1.0,
-         zoom_spline_order: int = 0):
+         zoom_spline_order: int = 0,
+         colormap:str = None,
+         display_min:float = None,
+         display_max:float = None):
     """
     Allows cropping an image along all axes.
 
     Parameters
     ----------
     image : image
         2D or 3D image to be cropped
@@ -25,24 +28,33 @@
         Text to be shown next to the slider
     axis_names: list of str, optional
         Names of the axes. If not given, the default names Z,Y,X are used.
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
 
     """
     return _Cropper(image,
                     slice_number=slice_number,
                     axis=axis,
                     continuous_update=continuous_update,
                     slider_text=slider_text,
                     axis_names=axis_names,
                     zoom_factor=zoom_factor,
-                    zoom_spline_order=zoom_spline_order)
+                    zoom_spline_order=zoom_spline_order,
+                    colormap=colormap,
+                    display_min=display_min,
+                    display_max=display_max)
 
 
 class _Cropper(VBox):
     """
     See also
     --------
     crop()
@@ -51,30 +63,36 @@
                  image,
                  slice_number: int = None,
                  axis: int = 0,
                  continuous_update: bool = False,
                  slider_text: str = "Slice",
                  axis_names=None,
                  zoom_factor: float = 1.0,
-                 zoom_spline_order: int = 0):
+                 zoom_spline_order: int = 0,
+                 colormap:str = None,
+                 display_min:float = None,
+                 display_max:float = None):
         from ipywidgets import IntRangeSlider
         from ._slice_viewer import _SliceViewer
         from ._utilities import _no_resize
 
         self._image = image
 
         viewer = _SliceViewer(image,
                               slice_number,
                               axis,
                               0,
                               0,
                               continuous_update,
                               slider_text,
                               zoom_factor=zoom_factor,
-                              zoom_spline_order=zoom_spline_order
+                              zoom_spline_order=zoom_spline_order,
+                              colormap=colormap,
+                              display_min=display_min,
+                              display_max=display_max
                               )
 
         if len(image.shape) < 2 or len(image.shape) > 3:
             raise RuntimeError("Number of image dimensions must be 2 or 3, but is", len(image.shape))
 
         if axis_names is None:
             if len(image.shape) == 2:
```

### Comparing `stackview-0.6.0/stackview/_image_widget.py` & `stackview-0.6.1/stackview/_image_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from ipycanvas import Canvas
 import numpy as np
-from functools import lru_cache
+from ._colormaps import _labels_lut # for internal backwards compatibility
 
 class ImageWidget(Canvas):
-    def __init__(self, image, zoom_factor:float=1.0, zoom_spline_order:int=0):
+    def __init__(self, image, zoom_factor:float=1.0, zoom_spline_order:int=0, colormap:str=None, display_min:float=None, display_max:float=None):
         if not ((len(image.shape) == 2) or (len(image.shape) == 3 and image.shape[-1] == 3)):
             raise NotImplementedError("Only 2D images are supported" + str(image.shape))
         height = image.shape[0] * zoom_factor
         width = image.shape[1] * zoom_factor
         self.zoom_factor = zoom_factor
         self.zoom_spline_order = zoom_spline_order
         super().__init__(width=width * zoom_factor, height=height * zoom_factor)
+        self.colormap = colormap
+        self.display_min = display_min
+        self.display_max = display_max
         self.data = np.asarray(image)
         self.layout.stretch = False
 
     @property
     def data(self):
         """Image data as numpy array
         """
@@ -30,18 +33,18 @@
         self._data = np.asarray(new_data)
         self._update_image()
         self.height = self._data.shape[0] * self.zoom_factor
         self.width = self._data.shape[1] * self.zoom_factor
 
     def _update_image(self):
         if self.zoom_factor == 1.0:
-            self.put_image_data(_img_to_rgb(self._data), 0, 0)
+            self.put_image_data(_img_to_rgb(self._data, colormap=self.colormap, display_min=self.display_min, display_max=self.display_max), 0, 0)
         else:
             zoomed = self._zoom(self._data)
-            self.put_image_data(_img_to_rgb(zoomed), 0, 0)
+            self.put_image_data(_img_to_rgb(zoomed, colormap=self.colormap, display_min=self.display_min, display_max=self.display_max), 0, 0)
 
     def _zoom(self, data):
         if len(data.shape) == 3:
             # handle RGB images
             return np.asarray([self._zoom(data[:,:,i]) for i in range(data.shape[2])]).swapaxes(0, 2).swapaxes(1, 0)
 
         from scipy.ndimage import affine_transform
@@ -60,16 +63,18 @@
 
 def _is_label_image(image):
     return image.dtype == np.uint32 or image.dtype == np.uint64 or \
            image.dtype == np.int32 or image.dtype == np.int64
 
 
 def _img_to_rgb(image,
+                colormap=None,
                 display_min=None,
                 display_max=None):
+    from ._colormaps import _labels_lut, create_colormap
 
     if len(image.shape) == 3 and image.shape[2] == 3:
         return image
 
     if image.dtype == bool:
         image = image * 1
 
@@ -78,27 +83,20 @@
         return np.asarray([lut[:, c].take(image) for c in range(0, 3)]).swapaxes(0, 2).swapaxes(1, 0) * 255
 
     if display_min is None:
         display_min = image.min()
     if display_max is None:
         display_max = image.max()
 
-    img_range = (display_max - display_min)
-    if img_range == 0:
-        img_range = 1
-
-    image = (image - display_min) / img_range * 255
-    return np.asarray([image, image, image]).swapaxes(0, 2).swapaxes(1, 0)
-
-@lru_cache(maxsize=1)
-def _labels_lut():
-    from numpy.random import MT19937
-    from numpy.random import RandomState, SeedSequence
-    rs = RandomState(MT19937(SeedSequence(3)))
-    lut = rs.rand(65537, 3)
-    lut[0, :] = 0
-    # these are the first four colours from matplotlib's default
-    lut[1] = [0.12156862745098039, 0.4666666666666667, 0.7058823529411765]
-    lut[2] = [1.0, 0.4980392156862745, 0.054901960784313725]
-    lut[3] = [0.17254901960784313, 0.6274509803921569, 0.17254901960784313]
-    lut[4] = [0.8392156862745098, 0.15294117647058825, 0.1568627450980392]
-    return lut
+    diplay_range_width = (display_max - display_min)
+    if diplay_range_width == 0:
+        diplay_range_width = 1
+
+    image = (image.astype(float) - display_min) / diplay_range_width * 255
+    image = np.minimum(image, 255)
+    image = np.maximum(image, 0)
+
+    if colormap is None:
+        return np.asarray([image, image, image]).swapaxes(0, 2).swapaxes(1, 0)
+    else:
+        lut = np.asarray(create_colormap(colormap).colors)
+        return np.asarray([lut[:, c].take(image.astype(int)) for c in range(0, 3)]).swapaxes(0, 2).swapaxes(1, 0) * 255
```

### Comparing `stackview-0.6.0/stackview/_interact.py` & `stackview-0.6.1/stackview/_interact.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 def interact(func,
              image = None,
              *args,
              continuous_update: bool = True,
              context:dict = None,
              zoom_factor:float = 1.0,
              zoom_spline_order:int = 0,
+             colormap:str = None,
+             display_min:float = None,
+             display_max:float = None,
              viewer: _SliceViewer = None,
              **kwargs):
     """Takes a function which has an image as first parameter and additional parameters.
     It will build a user interface consisting of sliders for numeric parameters and parameters
     that are called "footprint" or "selem".
 
     Parameters
@@ -23,14 +26,20 @@
         Update the image while dragging the mouse, default: False
     context:dict, optional
         A dictionary of (name:image), allows showing a pulldown of available images, e.g.: globals()
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
     viewer: _SliceViewer, optional
         The viewer where the result image should be shown.
     kwargs
 
     """
     import inspect
     import ipywidgets
@@ -101,15 +110,15 @@
         if exposable:
             if key in kwargs.keys():
                 default_value = kwargs[key]
             exposable_parameters.append(inspect.Parameter(key, inspect.Parameter.KEYWORD_ONLY, default=default_value))
 
     viewer_was_none = viewer is None
     if viewer_was_none:
-        viewer = _SliceViewer(image, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order)
+        viewer = _SliceViewer(image, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order, colormap=colormap, display_min=display_min, display_max=display_max)
     viewer.slice_slider.continuous_update=continuous_update
     command_label = ipywidgets.Label(value=func_name + "()")
     command_label.style.font_family = "Courier"
 
     from skimage import morphology
     execution_blocked = True
 
@@ -134,17 +143,18 @@
             else:
                 command = command + ", " + key + "=" + str(kwargs[key])
         command = command + ")"
         command_label.value = command.replace("(,", "(")
 
         if not execution_blocked:
             if image_passed:
-                viewer.image = func(image, *args, **kwargs)
+                viewer.view.data = func(image, *args, **kwargs)
             else:
-                viewer.image = func(*args, **kwargs)
+                viewer.view.data = func(*args, **kwargs)
+            viewer.image = viewer.view.data
 
         viewer.slice_slider.max = viewer.image.shape[0] - 1
         viewer.configuration_updated(None)
 
 
     worker_function.__signature__ = inspect.Signature(exposable_parameters)
     inter = ipywidgets.interactive(worker_function, dict(manual=False, auto_display=False))
```

### Comparing `stackview-0.6.0/stackview/_orthogonal.py` & `stackview-0.6.1/stackview/_orthogonal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 
 def orthogonal(
         image,
         display_width : int = None,
         display_height : int = None,
         continuous_update:bool=True,
         zoom_factor:float = 1.0,
-        zoom_spline_order:int = 0
+        zoom_spline_order:int = 0,
+        colormap:str = None,
+        display_min:float = None,
+        display_max:float = None
 ):
     """Show three viewers slicing the image stack in Z,Y and X.
 
     Parameters
     ----------
     image : image
         Image to be displayed
@@ -19,24 +22,30 @@
         This parameter is obsolete. Use zoom_factor instead
     continuous_update : bool, optional
         Update the image while dragging the mouse, default: False
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
 
     Returns
     -------
     An ipywidget with an image display and a slider.
 
     See Also
     --------
     slice()
     """
     import ipywidgets
     from ._slice import slice
 
     return ipywidgets.HBox([
-        slice(image, axis=0, slider_text="Z", continuous_update=continuous_update, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order),
-        slice(image, axis=1, slider_text="Y", continuous_update=continuous_update, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order),
-        slice(image, axis=2, slider_text="X", continuous_update=continuous_update, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order),
+        slice(image, axis=0, slider_text="Z", continuous_update=continuous_update, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order, colormap=colormap, display_min=display_min, display_max=display_max),
+        slice(image, axis=1, slider_text="Y", continuous_update=continuous_update, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order, colormap=colormap, display_min=display_min, display_max=display_max),
+        slice(image, axis=2, slider_text="X", continuous_update=continuous_update, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order, colormap=colormap, display_min=display_min, display_max=display_max),
     ])
```

### Comparing `stackview-0.6.0/stackview/_picker.py` & `stackview-0.6.1/stackview/_picker.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,18 @@
         image,
         slice_number: int = None,
         display_width: int = None,
         display_height: int = None,
         continuous_update: bool = True,
         slider_text: str = "Slice",
         zoom_factor:float = 1.0,
-        zoom_spline_order:int = 0
+        zoom_spline_order:int = 0,
+        colormap:str = None,
+        display_min:float = None,
+        display_max:float = None
 ):
     """Shows an image with a slider to go through a stack plus a label with the current mouse position and intensity at that position.
 
     Parameters
     ----------
     image : image
         Image shown
@@ -23,14 +26,20 @@
         This parameter is obsolete. Use zoom_factor instead
     continuous_update : bool, optional
         Update the image while dragging the mouse, default: False
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
 
     Returns
     -------
     An ipywidget with an image display, a slider and a label showing mouse position and intensity.
     """
 
     import ipywidgets
@@ -38,15 +47,18 @@
     from ._utilities import _no_resize
 
     viewer = _SliceViewer(image,
                           slice_number=slice_number,
                           continuous_update=continuous_update,
                           slider_text=slider_text,
                           zoom_factor=zoom_factor,
-                          zoom_spline_order=zoom_spline_order
+                          zoom_spline_order=zoom_spline_order,
+                          colormap=colormap,
+                          display_min=display_min,
+                          display_max=display_max
                           )
     view = viewer.view
     slice_slider = viewer.slice_slider
     label = ipywidgets.Label("[]:")
 
     from ipyevents import Event
     event_handler = Event(source=view, watched_events=['mousemove'])
```

### Comparing `stackview-0.6.0/stackview/_side_by_side.py` & `stackview-0.6.1/stackview/_side_by_side.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-
+import warnings
 
 def side_by_side(
         image1,
         image2,
         slice_number: int = None,
         axis: int = 0,
         display_width: int = None,
         display_height: int = None,
         continuous_update: bool = True,
         slider_text: str = "Slice",
         zoom_factor:float = 1.0,
-        zoom_spline_order:int = 0
+        zoom_spline_order:int = 0,
+        colormap:str = None,
+        display_min:float = None,
+        display_max:float = None
 ):
     """Shows two images in magenta and green plus a third with their colocalization / overlap view and
     a slider to go through a stack.
 
     Parameters
     ----------
     image1 : image
@@ -31,14 +34,20 @@
         This parameter is obsolete. Use zoom_factor instead
     continuous_update : bool, optional
         Update the image while dragging the mouse, default: False
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
 
     Returns
     -------
     An ipywidget with three image displays and a slider.
     """
 
     import ipywidgets
@@ -79,16 +88,16 @@
             slice_image1 = np.take(image1, z, axis=axis)
             slice_image2 = np.take(image2, z, axis=axis)
         else:
             slice_image1 = image1
             slice_image2 = image2
 
         if _is_label_image(slice_image1) or _is_label_image(slice_image2):
-            rgb_image1 = _img_to_rgb(slice_image1)
-            rgb_image2 = _img_to_rgb(slice_image2)
+            rgb_image1 = _img_to_rgb(slice_image1, colormap=colormap, display_min=display_min, display_max=display_max)
+            rgb_image2 = _img_to_rgb(slice_image2, colormap=colormap, display_min=display_min, display_max=display_max)
 
             if _is_label_image(slice_image1) and _is_label_image(slice_image2):
                 warnings.warn("Side-by-side mixing two label images may look weird." +
                               "Consider showing original image and a label image side-by-side.")
                 factor1 = 0.5
                 factor2 = 0.5
             elif _is_label_image(slice_image1):
```

### Comparing `stackview-0.6.0/stackview/_slice.py` & `stackview-0.6.1/stackview/_slice.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,18 @@
         slice_number : int = None,
         axis : int = 0,
         display_width : int = None,
         display_height : int = None,
         continuous_update:bool = True,
         slider_text:str="Slice",
         zoom_factor:float = 1.0,
-        zoom_spline_order:int = 0
+        zoom_spline_order:int = 0,
+        colormap:str = None,
+        display_min:float = None,
+        display_max:float = None
 ):
     """Shows an image with a slider to go through a stack.
 
     Parameters
     ----------
     image : image
         Image shown
@@ -25,14 +28,20 @@
         This parameter is obsolete. Use zoom_factor instead
     continuous_update : bool, optional
         Update the image while dragging the mouse, default: False
     zoom_factor: float, optional
         Allows showing the image larger (> 1) or smaller (<1)
     zoom_spline_order: int, optional
         Spline order used for interpolation (default=0, nearest-neighbor)
+    colormap: str, optional
+        Matplotlib colormap name or "pure_green", "pure_magenta", ...
+    display_min: float, optional
+        Lower bound of properly shown intensities
+    display_max: float, optional
+        Upper bound of properly shown intensities
 
     Returns
     -------
     An ipywidget with an image display and a slider.
     """
     from ._utilities import _no_resize
     from ._slice_viewer import _SliceViewer
@@ -42,13 +51,16 @@
         slice_number,
         axis,
         display_width,
         display_height,
         continuous_update,
         slider_text,
         zoom_factor=zoom_factor,
-        zoom_spline_order=zoom_spline_order
+        zoom_spline_order=zoom_spline_order,
+        colormap=colormap,
+        display_min=display_min,
+        display_max=display_max
     )
     view = viewer.view
     slice_slider = viewer.slice_slider
 
     return ipywidgets.VBox([_no_resize(view), slice_slider])
```

### Comparing `stackview-0.6.0/stackview/_slice_viewer.py` & `stackview-0.6.1/stackview/_slice_viewer.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,38 @@
                  slice_number: int = None,
                  axis: int = 0,
                  display_width: int = None,
                  display_height: int = None,
                  continuous_update: bool = True,
                  slider_text: str = "Slice",
                  zoom_factor:float = 1.0,
-                 zoom_spline_order:int = 0
+                 zoom_spline_order:int = 0,
+                 colormap:str = None,
+                 display_min:float = None,
+                 display_max:float = None
                  ):
         import ipywidgets
         from ._image_widget import ImageWidget
         import numpy as np
 
         self.image = image
 
         if slice_number is None:
             slice_number = int(image.shape[axis] / 2)
 
         if len(self.image.shape) == 3 and self.image.shape[-1] != 3:
-            self.view = ImageWidget(np.take(image, slice_number, axis=axis), zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order)
+            sliced_image = np.take(image, slice_number, axis=axis)
         else:
-            self.view = ImageWidget(image, zoom_factor=zoom_factor, zoom_spline_order=zoom_spline_order)
+            sliced_image = image
+        self.view = ImageWidget(sliced_image,
+                                zoom_factor=zoom_factor,
+                                zoom_spline_order=zoom_spline_order,
+                                colormap=colormap,
+                                display_min=display_min,
+                                display_max=display_max)
 
         # setup user interface for changing the slice
         self.slice_slider = ipywidgets.IntSlider(
             value=slice_number,
             min=0,
             max=image.shape[axis] - 1,
             continuous_update=continuous_update,
```

### Comparing `stackview-0.6.0/stackview/_static_view.py` & `stackview-0.6.1/stackview/_static_view.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.0/stackview/_uint_field.py` & `stackview-0.6.1/stackview/_uint_field.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.0/stackview/_utilities.py` & `stackview-0.6.1/stackview/_utilities.py`

 * *Files identical despite different names*

### Comparing `stackview-0.6.0/stackview.egg-info/PKG-INFO` & `stackview-0.6.1/stackview.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -162,14 +162,35 @@
     binary,
     labels
 ])
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch.gif)
 
+### Switch toggleable
+
+You can also view multiple channels with different colormaps at the same time using the `toggleable` parameter of `switch`. 
+It is recommended to also pass a list of colormaps. Colormap names can be taken from [Matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html) and stackview aims at compatibility with [microfilm](https://github.com/guiwitz/microfilm).
+
+```
+hela_cells = imread("data/hela-cells.tif")
+
+stackview.switch(
+    {"lysosomes":   hela_cells[:,:,0],
+     "mitochondria":hela_cells[:,:,1],
+     "nuclei":      hela_cells[:,:,2]
+    },
+    colormap=["pure_magenta", "pure_green", "pure_blue"],
+    toggleable=True
+)
+```
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch_toggleable.gif)
+
+
 ### Crop
 
 You can crop images interactively:
 ```python
 crop_widget = stackview.crop(image_stack, continuous_update=True)
 crop_widget
 ```
```

### Comparing `stackview-0.6.0/stackview.egg-info/SOURCES.txt` & `stackview-0.6.1/stackview.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 stackview/__init__.py
 stackview/_annotate.py
 stackview/_assist.py
+stackview/_colormaps.py
 stackview/_context.py
 stackview/_crop.py
 stackview/_curtain.py
 stackview/_image_widget.py
 stackview/_interact.py
 stackview/_orthogonal.py
 stackview/_picker.py
```

