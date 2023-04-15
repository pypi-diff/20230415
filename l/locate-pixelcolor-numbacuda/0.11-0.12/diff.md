# Comparing `tmp/locate_pixelcolor_numbacuda-0.11.tar.gz` & `tmp/locate_pixelcolor_numbacuda-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_numbacuda-0.11.tar", last modified: Wed Apr 12 00:46:45 2023, max compression
+gzip compressed data, was "locate_pixelcolor_numbacuda-0.12.tar", last modified: Sat Apr 15 00:45:08 2023, max compression
```

## Comparing `locate_pixelcolor_numbacuda-0.11.tar` & `locate_pixelcolor_numbacuda-0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 00:46:45.172691 locate_pixelcolor_numbacuda-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-12 00:46:43.000000 locate_pixelcolor_numbacuda-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      197 2023-04-12 00:46:42.000000 locate_pixelcolor_numbacuda-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     1770 2023-04-12 00:46:45.172691 locate_pixelcolor_numbacuda-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2023-04-12 00:45:56.000000 locate_pixelcolor_numbacuda-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 00:46:45.168702 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/LICENSE
--rw-rw-rw-   0        0        0     1066 2023-04-12 00:45:56.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/README.MD
--rw-rw-rw-   0        0        0     1880 2023-04-12 00:39:36.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/__init__.py
--rw-rw-rw-   0        0        0       12 2023-04-12 00:46:44.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-04-12 00:46:44.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-12 00:46:45.172691 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/
--rw-rw-rw-   0        0        0     1770 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-04-12 00:46:45.173689 locate_pixelcolor_numbacuda-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-12 00:46:44.000000 locate_pixelcolor_numbacuda-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:45:08.395684 locate_pixelcolor_numbacuda-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:45:03.000000 locate_pixelcolor_numbacuda-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      197 2023-04-15 00:45:02.000000 locate_pixelcolor_numbacuda-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     1737 2023-04-15 00:45:08.395684 locate_pixelcolor_numbacuda-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2023-04-15 00:18:27.000000 locate_pixelcolor_numbacuda-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:45:08.391718 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/LICENSE
+-rw-rw-rw-   0        0        0     1066 2023-04-15 00:18:27.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/README.MD
+-rw-rw-rw-   0        0        0     1880 2023-04-15 00:18:27.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-04-15 00:45:07.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/requirements.txt
+-rw-rw-rw-   0        0        0     3732 2023-04-15 00:45:07.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:45:08.395684 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/
+-rw-rw-rw-   0        0        0     1737 2023-04-15 00:45:08.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-04-15 00:45:08.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:45:08.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 00:45:08.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-15 00:45:08.000000 locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:45:08.396681 locate_pixelcolor_numbacuda-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1364 2023-04-15 00:45:07.000000 locate_pixelcolor_numbacuda-0.12/setup.py
```

### Comparing `locate_pixelcolor_numbacuda-0.11/LICENSE.rst` & `locate_pixelcolor_numbacuda-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.11/PKG-INFO` & `locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
-Name: locate_pixelcolor_numbacuda
-Version: 0.11
+Name: locate-pixelcolor-numbacuda
+Version: 0.12
+Summary: RGB search with numba.cuda - 10 x faster than numpy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_numbacuda
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numpy,numba,CUDA,rgb,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# RGB search with numba.cuda - 10 x faster than numpy 
 
-# RGB search with numba.cuda - 10 x faster than numpy 
-
-### pip install locate-pixelcolor-numbacuda
-
-
-```python
-from locate_pixelcolor_numbacuda import search_colors
-from a_cv_imwrite_imread_plus import open_image_in_cv
-import numpy as np
-colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
-```
-
-#### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
-
-```python
-picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
-coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
-print(coords)
-%timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
-
-
-# [[[  19   14]
-#   [  19   14]
-#   [  11   17]
-#   ...
-#   [6613 4524]
-#   [6614 4524]
-#   [6615 4524]]]
-# 135 ms ± 3.5 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
-
-```
+### pip install locate-pixelcolor-numbacuda
+
+
+```python
+from locate_pixelcolor_numbacuda import search_colors
+from a_cv_imwrite_imread_plus import open_image_in_cv
+import numpy as np
+colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
+```
+
+#### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
+
+```python
+picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
+coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
+print(coords)
+%timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
+
+
+# [[[  19   14]
+#   [  19   14]
+#   [  11   17]
+#   ...
+#   [6613 4524]
+#   [6614 4524]
+#   [6615 4524]]]
+# 135 ms Â± 3.5 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
+
+```
```

### Comparing `locate_pixelcolor_numbacuda-0.11/README.md` & `locate_pixelcolor_numbacuda-0.12/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/LICENSE` & `locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-MIT License
-
-Copyright (c) 2022 Hans Alemão
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+
+ The MIT License (MIT)
+ Copyright (c) 2023 Johannes Fischer
+ 
+ Permission is hereby granted, free of charge, to any person obtaining a copy
+ of this software and associated documentation files (the "Software"), to deal
+ in the Software without restriction, including without limitation the rights
+ to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+ copies of the Software, and to permit persons to whom the Software is
+ furnished to do so, subject to the following conditions:
+ 
+ The above copyright notice and this permission notice shall be included in all
+ copies or substantial portions of the Software.
+ 
+ THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+ EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+ MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+ IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+ DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+ OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
+ OR OTHER DEALINGS IN THE SOFTWARE.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/README.MD` & `locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/README.MD`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/__init__.py` & `locate_pixelcolor_numbacuda-0.12/locate_pixelcolor_numbacuda/__init__.py`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/PKG-INFO` & `locate_pixelcolor_numbacuda-0.12/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
-Name: locate-pixelcolor-numbacuda
-Version: 0.11
+Name: locate_pixelcolor_numbacuda
+Version: 0.12
+Summary: RGB search with numba.cuda - 10 x faster than numpy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_numbacuda
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numpy,numba,CUDA,rgb,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# RGB search with numba.cuda - 10 x faster than numpy 
 
-# RGB search with numba.cuda - 10 x faster than numpy 
-
-### pip install locate-pixelcolor-numbacuda
-
-
-```python
-from locate_pixelcolor_numbacuda import search_colors
-from a_cv_imwrite_imread_plus import open_image_in_cv
-import numpy as np
-colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
-```
-
-#### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
-
-```python
-picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
-coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
-print(coords)
-%timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
-
-
-# [[[  19   14]
-#   [  19   14]
-#   [  11   17]
-#   ...
-#   [6613 4524]
-#   [6614 4524]
-#   [6615 4524]]]
-# 135 ms ± 3.5 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
-
-```
+### pip install locate-pixelcolor-numbacuda
+
+
+```python
+from locate_pixelcolor_numbacuda import search_colors
+from a_cv_imwrite_imread_plus import open_image_in_cv
+import numpy as np
+colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
+```
+
+#### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
+
+```python
+picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
+coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
+print(coords)
+%timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
+
+
+# [[[  19   14]
+#   [  19   14]
+#   [  11   17]
+#   ...
+#   [6613 4524]
+#   [6614 4524]
+#   [6615 4524]]]
+# 135 ms Â± 3.5 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
+
+```
```

