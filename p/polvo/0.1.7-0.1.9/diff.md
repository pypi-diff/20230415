# Comparing `tmp/polvo-0.1.7.tar.gz` & `tmp/polvo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/polvo-0.1.7.tar", last modified: Thu Jan 19 20:52:07 2023, max compression
+gzip compressed data, was "dist/polvo-0.1.9.tar", last modified: Sat Apr 15 12:37:24 2023, max compression
```

## Comparing `polvo-0.1.7.tar` & `polvo-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/
--rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)    11337 2022-07-27 02:12:47.000000 polvo-0.1.7/LICENSE
--rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)      111 2022-07-27 02:12:47.000000 polvo-0.1.7/MANIFEST.in
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1450 2023-01-19 20:52:07.000000 polvo-0.1.7/PKG-INFO
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      664 2023-01-17 18:33:28.000000 polvo-0.1.7/README.md
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      151 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/__init__.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)    15159 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/_modidx.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo/classification/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       83 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/classification/__init__.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo/classification/baseline/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       23 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/classification/baseline/__init__.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1842 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/classification/baseline/baseline.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1925 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/classification/explorer.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     2772 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/common.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo/segmentation/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       29 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/segmentation/__init__.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     2221 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/segmentation/core.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      863 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/segmentation/vis.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      377 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/test.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo/utils/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       64 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/utils/__init__.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1698 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/utils/download.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     4841 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/utils/io.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      368 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/utils/logging.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      381 2023-01-19 20:52:03.000000 polvo-0.1.7/polvo/utils/misc.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1450 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/PKG-INFO
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      663 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/SOURCES.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/dependency_links.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       91 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/entry_points.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2022-07-30 08:39:10.000000 polvo-0.1.7/polvo.egg-info/not-zip-safe
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        7 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/requires.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        6 2023-01-19 20:52:07.000000 polvo-0.1.7/polvo.egg-info/top_level.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      829 2023-01-19 20:52:03.000000 polvo-0.1.7/settings.ini
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       38 2023-01-19 20:52:07.000000 polvo-0.1.7/setup.cfg
--rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)     2528 2022-07-27 02:12:47.000000 polvo-0.1.7/setup.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/
+-rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)    11337 2022-07-27 02:12:47.000000 polvo-0.1.9/LICENSE
+-rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)      111 2022-07-27 02:12:47.000000 polvo-0.1.9/MANIFEST.in
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1450 2023-04-15 12:37:23.000000 polvo-0.1.9/PKG-INFO
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      664 2023-01-17 18:33:28.000000 polvo-0.1.9/README.md
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      146 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)    10897 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/_modidx.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo/classification/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       44 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/classification/__init__.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo/classification/baseline/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       23 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/classification/baseline/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1842 2023-02-02 20:50:20.000000 polvo-0.1.9/polvo/classification/baseline/baseline.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1882 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/classification/explorer.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo/datasets/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       23 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/datasets/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      555 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/datasets/download.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo/segmentation/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       29 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/segmentation/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      863 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/segmentation/vis.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      377 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/test.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo/utils/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      136 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1698 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/download.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     5219 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/io.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      368 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/logging.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1109 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/misc.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1843 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/script.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     3160 2023-04-15 12:32:23.000000 polvo-0.1.9/polvo/utils/visualization.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1450 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/PKG-INFO
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      725 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/SOURCES.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/dependency_links.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      161 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/entry_points.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2022-07-30 08:39:10.000000 polvo-0.1.9/polvo.egg-info/not-zip-safe
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       67 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/requires.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        6 2023-04-15 12:37:23.000000 polvo-0.1.9/polvo.egg-info/top_level.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      990 2023-04-15 12:32:23.000000 polvo-0.1.9/settings.ini
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       38 2023-04-15 12:37:23.000000 polvo-0.1.9/setup.cfg
+-rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)     2528 2022-07-27 02:12:47.000000 polvo-0.1.9/setup.py
```

### Comparing `polvo-0.1.7/LICENSE` & `polvo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polvo-0.1.7/PKG-INFO` & `polvo-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polvo
-Version: 0.1.7
+Version: 0.1.9
 Summary: A collection of computer vision tools that fits anywhere
 Home-page: https://github.com/lgvaz/polvo/
 Author: lgvaz
 Author-email: lgvaz42@gmail.com
 License: Apache Software License 2.0
 Keywords: computer-vision deep-learning fastai
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `polvo-0.1.7/README.md` & `polvo-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `polvo-0.1.7/polvo/classification/baseline/baseline.py` & `polvo-0.1.9/polvo/classification/baseline/baseline.py`

 * *Files identical despite different names*

### Comparing `polvo-0.1.7/polvo/classification/explorer.py` & `polvo-0.1.9/polvo/classification/explorer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/02a_classification.explorer.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05a_classification.explorer.ipynb.
 
 # %% auto 0
 __all__ = ['DataExplorer']
 
-# %% ../../nbs/02a_classification.explorer.ipynb 2
+# %% ../../nbs/05a_classification.explorer.ipynb 2
 #TODO: optimize imports
 from fastcore.all import *
+
 import numpy as np
 import pandas as pd
 import polvo as pv
 
-# %% ../../nbs/02a_classification.explorer.ipynb 7
+from PIL import Image
+
+# %% ../../nbs/05a_classification.explorer.ipynb 7
 class DataExplorer:
     def __init__(self, label_ids, idx2image, id2label, label2id):
         store_attr()
         self.grouped_y = self._group_y()
         
     def _group_y(self):
         label_df = pd.DataFrame(self.label_ids, columns=["label_id"])
@@ -39,11 +42,10 @@
         return self.show_label_id(self.label2id(label), slice_=slice_) #
 
     def show_most_common(self, idx: int, slice_=slice(None)):
         item_idxs = self.grouped_y.iloc[idx].item_idx
         item_idxs = item_idxs[slice_]
         
         images = [self.idx2image(i) for i in item_idxs]
-        shows = [partial(pv.show_image, image) for image in images]
         xmax, ymax = np.max([image.size for image in images], axis=0)
         
-        return pv.image_grid(shows, xmax=xmax, ymax=ymax)
+        return pv.image_grid(images, xmax=xmax, ymax=ymax)
```

### Comparing `polvo-0.1.7/polvo/common.py` & `polvo-0.1.9/polvo/utils/visualization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_common.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/01p_utils.visualization.ipynb.
 
 # %% auto 0
-__all__ = ['show_image', 'get_image_grid', 'show_grid', 'normalize_axes', 'image_grid', 'grid_from_sequence', 'image_size',
-           'image_sizes_hist']
+__all__ = ['show_image', 'get_image_grid', 'show_grid', 'normalize_axes', 'plot_grid', 'image_grid', 'grid_from_sequence',
+           'image_size', 'image_sizes_hist']
 
-# %% ../nbs/00_common.ipynb 3
+# %% ../../nbs/01p_utils.visualization.ipynb 3
 from fastcore.all import *
 import random
 import polvo as pv
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import ImageGrid
 
-# %% ../nbs/00_common.ipynb 9
+# %% ../../nbs/01p_utils.visualization.ipynb 4
 @delegates(plt.subplots)
 def show_image(image, ax=None, cmap=None, show:bool=False, **kwargs):
     if ax is None: fig, ax = plt.subplots(**kwargs)
     ax.imshow(image, cmap=cmap)
     ax.set_axis_off()
     if show: plt.show()
     return ax
 
-# %% ../nbs/00_common.ipynb 13
+# %% ../../nbs/01p_utils.visualization.ipynb 8
 @delegates(ImageGrid)
 def get_image_grid(
     nitems=None,
     ncols=3,
     nrows=None,
     pad=0.0,
     figsize=None,
@@ -37,53 +37,59 @@
     figsize = figsize or (14, 4 * nrows)
 
     fig = plt.figure(figsize=figsize)
     grid = ImageGrid(fig, 111, (nrows, ncols), axes_pad=pad, **kwargs)
     
     return fig, grid
 
-# %% ../nbs/00_common.ipynb 14
+# %% ../../nbs/01p_utils.visualization.ipynb 9
 def show_grid(grid, shows, show=True):
     for ax, show in zip(grid, shows): show(ax=ax)
     if show: plt.show()
 
-# %% ../nbs/00_common.ipynb 15
+# %% ../../nbs/01p_utils.visualization.ipynb 10
 def normalize_axes(grid, xmax, ymax):
     "Expand all axes to have the same dimensions."
     for ax in grid:
         ax.set_xlim(right=xmax)
         ax.set_ylim(bottom=ymax)
 
-# %% ../nbs/00_common.ipynb 16
+# %% ../../nbs/01p_utils.visualization.ipynb 11
 @delegates(get_image_grid, but=['nitems'])
-def image_grid(shows, show=True, xmax=None, ymax=None, **kwargs):
+def plot_grid(shows, show=True, xmax=None, ymax=None, **kwargs):
     "Quickly plot a grid of images."
     fig, grid = get_image_grid(nitems=len(shows), **kwargs)
+    if xmax or ymax: normalize_axes(grid, xmax, ymax)
     show_grid(grid, shows, show=show)
-    normalize_axes(grid, xmax, ymax)
     return fig, grid
 
-# %% ../nbs/00_common.ipynb 18
+# %% ../../nbs/01p_utils.visualization.ipynb 12
+@delegates(plot_grid, but=['shows'])
+def image_grid(images, *args, **kwargs):
+    shows = [partial(show_image, o) for o in images]
+    return plot_grid(shows, *args, **kwargs)
+
+# %% ../../nbs/01p_utils.visualization.ipynb 14
 @delegates(image_grid)
 def grid_from_sequence(sequence, get_image, nitems=9, idxs=None, **kwargs):
     "Generates a grid of images from a subset of items from the sequence."
     idxs = idxs or random.sample(range(0, len(sequence)), nitems)
     images = []
     for idx in idxs:
         item = sequence[idx]
         images.append(get_image(item))
     
-    return image_grid([partial(show_image, o) for o in images], **kwargs)
+    return image_grid(images, **kwargs)
 
-# %% ../nbs/00_common.ipynb 20
+# %% ../../nbs/01p_utils.visualization.ipynb 16
 def image_size(image_file):
     with pv.open_image(image_file) as image:
         return image.size
 
-# %% ../nbs/00_common.ipynb 21
+# %% ../../nbs/01p_utils.visualization.ipynb 17
 def image_sizes_hist(
     image_files # Sequence of image filepaths.
 ):
     "Plot a histogram of widths and heights."
     sizes = parallel(image_size, image_files, progress=pv.pbar)
     widths, heights = zip(*sizes)
     plt.hist(widths, label='width')
```

### Comparing `polvo-0.1.7/polvo/segmentation/vis.py` & `polvo-0.1.9/polvo/segmentation/vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/03a_segmentation.vis.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/08a_segmentation.vis.ipynb.
 
 # %% auto 0
 __all__ = ['overlay_mask']
 
-# %% ../../nbs/03a_segmentation.vis.ipynb 3
+# %% ../../nbs/08a_segmentation.vis.ipynb 3
 import polvo as pv
 import PIL
 import numpy as np
 import matplotlib as mpl
 
-# %% ../../nbs/03a_segmentation.vis.ipynb 4
+# %% ../../nbs/08a_segmentation.vis.ipynb 4
 def overlay_mask(
     image:PIL.Image,
     mask:PIL.Image,
     nclasses:int,
     cmap:mpl.colors.Colormap=mpl.colormaps['gist_ncar'],
     alpha:float=0.5,
 ):
```

### Comparing `polvo-0.1.7/polvo/utils/download.py` & `polvo-0.1.9/polvo/utils/download.py`

 * *Files identical despite different names*

### Comparing `polvo-0.1.7/polvo/utils/io.py` & `polvo-0.1.9/polvo/utils/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,67 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/01e_utils.io.ipynb.
 
 # %% auto 0
-__all__ = ['image_extensions', 'write_txt', 'load_txt', 'mkdir', 'extract_files', 'get_files', 'get_image_files', 'open_image',
-           'open_mask', 'RenderDict', 'read_json']
+__all__ = ['image_extensions', 'save_txt', 'open_txt', 'open_json', 'save_json', 'mkdir', 'extract_files', 'get_files',
+           'get_image_files', 'open_image', 'open_mask', 'save_image', 'RenderDict']
 
 # %% ../../nbs/01e_utils.io.ipynb 2
 import shutil, tempfile
+import numpy as np
 import polvo as pv
 import uuid, json, mimetypes
 from pathlib import Path
 from fastcore.all import *
 from PIL import Image, ImageOps
 
 # %% ../../nbs/01e_utils.io.ipynb 3
-def write_txt(s, path):
-    with open(str(path), 'w') as f: f.write(s)
+def save_txt(s, path, append=False):
+    mode = 'a' if append else 'w'
+    with open(str(path), mode) as f: f.write(s)
 
 # %% ../../nbs/01e_utils.io.ipynb 4
-def load_txt(path):
+def open_txt(path):
     with open(str(path), 'r') as f: return f.read()
 #     return np.loadtxt(path, dtype=str, delimiter="\n").tolist()
 
 # %% ../../nbs/01e_utils.io.ipynb 6
+def open_json(path):
+    with open(str(path)) as f: return json.load(f)
+
+# %% ../../nbs/01e_utils.io.ipynb 7
+def save_json(d, path):
+    with open(str(path), 'w') as f: json.dump(d, f)
+
+# %% ../../nbs/01e_utils.io.ipynb 9
 def mkdir(path, exist_ok=False, parents=False, overwrite=False, tmp=False, **kwargs):
     "Creates and returns a directory defined by `path`, optionally removing previous existing directory if `overwrite` is `True`"
     path = Path(path)
     if tmp:
         path = tempfile.gettempdir() / path
         parents = True
     if path.exists() and overwrite: shutil.rmtree(path)
     path.mkdir(exist_ok=exist_ok, parents=parents, **kwargs)
     return path
 
-# %% ../../nbs/01e_utils.io.ipynb 8
+# %% ../../nbs/01e_utils.io.ipynb 11
 def extract_files(files, extract_to_dir, show_pbar=True):
     for file in pbar(files, show=show_pbar):
         extract_path = extract_to_dir / Path(file).with_suffix("").name
         shutil.unpack_archive(file, extract_path)
     return extract_to_dir
 
-# %% ../../nbs/01e_utils.io.ipynb 9
+# %% ../../nbs/01e_utils.io.ipynb 12
 def _get_files(p, fs, extensions=None):
     "COPIED FROM https://github.com/fastai/fastai/blob/master/nbs/05_data.transforms.ipynb"
     p = Path(p)
     res = [p/f for f in fs if not f.startswith('.')
            and ((not extensions) or f'.{f.split(".")[-1].lower()}' in extensions)]
     return res
 
-# %% ../../nbs/01e_utils.io.ipynb 10
+# %% ../../nbs/01e_utils.io.ipynb 13
 def get_files(path, extensions=None, recurse=True, folders=None, followlinks=True):
     """Get all the files in `path` with optional `extensions`, optionally with `recurse`, only in `folders`, if specified.
     COPIED FROM https://github.com/fastai/fastai/blob/master/nbs/05_data.transforms.ipynb
     """
     path = Path(path)
     folders=L(folders)
     extensions = setify(extensions)
@@ -64,38 +74,43 @@
             if len(folders) !=0 and i==0 and '.' not in folders: continue
             res += _get_files(p, f, extensions)
     else:
         f = [o.name for o in os.scandir(path) if o.is_file()]
         res = _get_files(path, f, extensions)
     return L(res)
 
-# %% ../../nbs/01e_utils.io.ipynb 12
+# %% ../../nbs/01e_utils.io.ipynb 15
 image_extensions = set(k for k,v in mimetypes.types_map.items() if v.startswith('image/'))
 
-# %% ../../nbs/01e_utils.io.ipynb 13
+# %% ../../nbs/01e_utils.io.ipynb 16
 def get_image_files(path, recurse=True, folders=None):
     """Get image files in `path` recursively, only in `folders`, if specified.
     COPIED FROM https://github.com/fastai/fastai/blob/master/nbs/05_data.transforms.ipynb
     """
     return get_files(path, extensions=image_extensions, recurse=recurse, folders=folders)
 
-# %% ../../nbs/01e_utils.io.ipynb 15
-def open_image(fn, gray=False, ignore_exif=True) -> Image.Image:
-    "Open an image from disk `fn` as a PIL Image"
+# %% ../../nbs/01e_utils.io.ipynb 18
+def open_image(path, gray=False, ignore_exif=True) -> Image.Image:
+    "Open an image from disk `path` as a PIL Image"
     color = "L" if gray else "RGB"
-    image = Image.open(str(fn))
+    image = Image.open(str(path))
     if not ignore_exif: image = ImageOps.exif_transpose(image)
     return image.convert(color)
 
-# %% ../../nbs/01e_utils.io.ipynb 17
+# %% ../../nbs/01e_utils.io.ipynb 20
 @delegates(open_image)
-def open_mask(fn, gray=True, **kwargs) -> Image.Image:
-    return open_image(fn, gray=gray, **kwargs)
+def open_mask(path, gray=True, **kwargs) -> Image.Image:
+    return open_image(path, gray=gray, **kwargs)
+
+# %% ../../nbs/01e_utils.io.ipynb 22
+def save_image(image, path):
+    if isinstance(image, np.ndarray): image = Image.fromarray(image)
+    return image.save(str(path))
 
-# %% ../../nbs/01e_utils.io.ipynb 19
+# %% ../../nbs/01e_utils.io.ipynb 24
 class RenderDict:
     "From https://www.reddit.com/r/IPython/comments/34t4m7/lpt_print_json_in_collapsible_format_in_ipython/"
     def __init__(self, json_data):
         if isinstance(json_data, dict):
             self.json_str = json.dumps(json_data)
         else:
             self.json_str = json_data
@@ -105,12 +120,7 @@
         from IPython.display import display_javascript, display_html, display
         display_html('<div id="{}" style="height: 600px; width:100%;"></div>'.format(self.uuid), raw=True)
         display_javascript("""
         require(["https://rawgit.com/caldwell/renderjson/master/renderjson.js"], function() {
         document.getElementById('%s').appendChild(renderjson(%s))
         });
         """ % (self.uuid, self.json_str), raw=True)
-
-# %% ../../nbs/01e_utils.io.ipynb 21
-def read_json(path):
-    with open(str(path)) as f:
-        return json.load(f)
```

### Comparing `polvo-0.1.7/polvo.egg-info/PKG-INFO` & `polvo-0.1.9/polvo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polvo
-Version: 0.1.7
+Version: 0.1.9
 Summary: A collection of computer vision tools that fits anywhere
 Home-page: https://github.com/lgvaz/polvo/
 Author: lgvaz
 Author-email: lgvaz42@gmail.com
 License: Apache Software License 2.0
 Keywords: computer-vision deep-learning fastai
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `polvo-0.1.7/polvo.egg-info/SOURCES.txt` & `polvo-0.1.9/polvo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 polvo/__init__.py
 polvo/_modidx.py
-polvo/common.py
 polvo/test.py
 polvo.egg-info/PKG-INFO
 polvo.egg-info/SOURCES.txt
 polvo.egg-info/dependency_links.txt
 polvo.egg-info/entry_points.txt
 polvo.egg-info/not-zip-safe
 polvo.egg-info/requires.txt
 polvo.egg-info/top_level.txt
 polvo/classification/__init__.py
 polvo/classification/explorer.py
 polvo/classification/baseline/__init__.py
 polvo/classification/baseline/baseline.py
+polvo/datasets/__init__.py
+polvo/datasets/download.py
 polvo/segmentation/__init__.py
-polvo/segmentation/core.py
 polvo/segmentation/vis.py
 polvo/utils/__init__.py
 polvo/utils/download.py
 polvo/utils/io.py
 polvo/utils/logging.py
-polvo/utils/misc.py
+polvo/utils/misc.py
+polvo/utils/script.py
+polvo/utils/visualization.py
```

### Comparing `polvo-0.1.7/setup.py` & `polvo-0.1.9/setup.py`

 * *Files identical despite different names*

