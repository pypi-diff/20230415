# Comparing `tmp/locate_pixelcolor_numba-0.10.tar.gz` & `tmp/locate_pixelcolor_numba-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_numba-0.10.tar", last modified: Thu Apr 13 03:06:20 2023, max compression
+gzip compressed data, was "locate_pixelcolor_numba-0.11.tar", last modified: Sat Apr 15 00:40:16 2023, max compression
```

## Comparing `locate_pixelcolor_numba-0.10.tar` & `locate_pixelcolor_numba-0.11.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:06:20.977406 locate_pixelcolor_numba-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-13 03:06:18.000000 locate_pixelcolor_numba-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      236 2023-04-13 03:06:17.000000 locate_pixelcolor_numba-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2934 2023-04-13 03:06:20.978412 locate_pixelcolor_numba-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2142 2023-04-13 03:01:07.000000 locate_pixelcolor_numba-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 03:06:20.971402 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/LICENSE
--rw-rw-rw-   0        0        0     2142 2023-04-13 03:01:07.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/README.md
--rw-rw-rw-   0        0        0      458 2023-04-13 02:11:06.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/__init__.py
--rw-rw-rw-   0        0        0        5 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/requirements.txt
--rw-rw-rw-   0        0        0    46592 2023-04-13 02:01:43.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/searchcolorsnumba.pyd
--rw-rw-rw-   0        0        0    49102 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-13 03:06:20.977406 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/
--rw-rw-rw-   0        0        0     2934 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 03:06:20.978412 locate_pixelcolor_numba-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-04-13 03:06:20.000000 locate_pixelcolor_numba-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:40:16.883801 locate_pixelcolor_numba-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:40:11.000000 locate_pixelcolor_numba-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      195 2023-04-15 00:40:10.000000 locate_pixelcolor_numba-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2803 2023-04-15 00:40:16.883801 locate_pixelcolor_numba-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2142 2023-04-15 00:17:54.000000 locate_pixelcolor_numba-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:40:16.880296 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/
+-rw-rw-rw-   0        0        0     2142 2023-04-15 00:17:54.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/README.md
+-rw-rw-rw-   0        0        0      458 2023-04-15 00:17:54.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/__init__.py
+-rw-rw-rw-   0        0        0        5 2023-04-15 00:40:15.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/requirements.txt
+-rw-rw-rw-   0        0        0    46592 2023-04-15 00:17:54.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/searchcolorsnumba.pyd
+-rw-rw-rw-   0        0        0     2342 2023-04-15 00:40:15.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:40:16.883289 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/
+-rw-rw-rw-   0        0        0     2803 2023-04-15 00:40:16.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-04-15 00:40:16.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:40:16.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 00:40:16.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-15 00:40:16.000000 locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:40:16.883801 locate_pixelcolor_numba-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-04-15 00:40:15.000000 locate_pixelcolor_numba-0.11/setup.py
```

### Comparing `locate_pixelcolor_numba-0.10/LICENSE.rst` & `locate_pixelcolor_numba-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numba-0.10/PKG-INFO` & `locate_pixelcolor_numba-0.11/locate_pixelcolor_numba.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,86 @@
 Metadata-Version: 2.1
-Name: locate_pixelcolor_numba
-Version: 0.10
+Name: locate-pixelcolor-numba
+Version: 0.11
 Summary: RGB search with numba - 2-3 x faster than numpy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_numba
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numba,aot,compiled,rgb,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# RGB search with numba - 2-3 x faster than numpy 
 
-# RGB search with numba - 2-3 x faster than numpy 
-
-### pip install locate-pixelcolor-numba
-
-
-### Important!
-This is a compiled .pyd file (Numba AOT), if you can't import it, run the following code to generate a new pyd file, and replace it with the old .pyd file.
-
-
-```python
-from numba_aot_compiler import compnumba #pip install numba-aot-compiler
-import numpy as np
-from numba import uint8, uint16
-
-
-def search_colors(r, g, b, rgbs, divider):
-    res = np.zeros(b.shape, dtype=np.uint16)
-    res2 = np.zeros(b.shape, dtype=np.uint16)
-    zaehler = 0
-    for rgb in rgbs:
-        rr, gg, bb = rgb
-        for i in range(r.shape[0]):
-            if r[i] == rr:
-                if g[i] == gg:
-                    if b[i] == bb:
-                        dvquot, dvrem = divmod(i, divider)
-                        res[zaehler] = dvquot
-                        res2[zaehler] = dvrem
-                        zaehler = zaehler + 1
-    results = np.dstack((res[:zaehler], res2[:zaehler]))
-    return results
-
-
-compi2 = compnumba(
-    fu=search_colors,
-    funcname="search_colors",
-    file="searchcolorsnumba",
-    folder="locate_pixelcolor_numba",
-    signature=(uint8[:], uint8[:], uint8[:], uint8[:, :], uint16),
-    parallel=True,
-    fastmath=True,
-    nogil=True,
-)
-```
-
-### How to use it
-
-```python
-from locate_pixelcolor_numba import search_colors
-import cv2
-import time
-import numpy as np
-pic = cv2.imread(r"pexels-alex-andrews-2295744.jpg") # https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-colors = np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
-search_colors(pic,colors)
-Out[2]: 
-array([[[   0, 4522],
-        [   3, 4522],
-        [   3, 4523],
-        ...,
-        [6622, 4522],
-        [6622, 4523],
-        [6622, 4524]]], dtype=uint16)
-%timeit search_colors(pic,colors)
-413 ms ± 1.22 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-
-# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
-
-```
+### pip install locate-pixelcolor-numba
+
+
+### Important!
+This is a compiled .pyd file (Numba AOT), if you can't import it, run the following code to generate a new pyd file, and replace it with the old .pyd file.
+
+
+```python
+from numba_aot_compiler import compnumba #pip install numba-aot-compiler
+import numpy as np
+from numba import uint8, uint16
+
+
+def search_colors(r, g, b, rgbs, divider):
+    res = np.zeros(b.shape, dtype=np.uint16)
+    res2 = np.zeros(b.shape, dtype=np.uint16)
+    zaehler = 0
+    for rgb in rgbs:
+        rr, gg, bb = rgb
+        for i in range(r.shape[0]):
+            if r[i] == rr:
+                if g[i] == gg:
+                    if b[i] == bb:
+                        dvquot, dvrem = divmod(i, divider)
+                        res[zaehler] = dvquot
+                        res2[zaehler] = dvrem
+                        zaehler = zaehler + 1
+    results = np.dstack((res[:zaehler], res2[:zaehler]))
+    return results
+
+
+compi2 = compnumba(
+    fu=search_colors,
+    funcname="search_colors",
+    file="searchcolorsnumba",
+    folder="locate_pixelcolor_numba",
+    signature=(uint8[:], uint8[:], uint8[:], uint8[:, :], uint16),
+    parallel=True,
+    fastmath=True,
+    nogil=True,
+)
+```
+
+### How to use it
+
+```python
+from locate_pixelcolor_numba import search_colors
+import cv2
+import time
+import numpy as np
+pic = cv2.imread(r"pexels-alex-andrews-2295744.jpg") # https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+colors = np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
+search_colors(pic,colors)
+Out[2]: 
+array([[[   0, 4522],
+        [   3, 4522],
+        [   3, 4523],
+        ...,
+        [6622, 4522],
+        [6622, 4523],
+        [6622, 4524]]], dtype=uint16)
+%timeit search_colors(pic,colors)
+413 ms Â± 1.22 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+
+# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
+
+```
```

### Comparing `locate_pixelcolor_numba-0.10/README.md` & `locate_pixelcolor_numba-0.11/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numba-0.10/locate_pixelcolor_numba/README.md` & `locate_pixelcolor_numba-0.11/locate_pixelcolor_numba/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numba-0.10/locate_pixelcolor_numba.egg-info/PKG-INFO` & `locate_pixelcolor_numba-0.11/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,86 @@
 Metadata-Version: 2.1
-Name: locate-pixelcolor-numba
-Version: 0.10
+Name: locate_pixelcolor_numba
+Version: 0.11
 Summary: RGB search with numba - 2-3 x faster than numpy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_numba
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numba,aot,compiled,rgb,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# RGB search with numba - 2-3 x faster than numpy 
 
-# RGB search with numba - 2-3 x faster than numpy 
-
-### pip install locate-pixelcolor-numba
-
-
-### Important!
-This is a compiled .pyd file (Numba AOT), if you can't import it, run the following code to generate a new pyd file, and replace it with the old .pyd file.
-
-
-```python
-from numba_aot_compiler import compnumba #pip install numba-aot-compiler
-import numpy as np
-from numba import uint8, uint16
-
-
-def search_colors(r, g, b, rgbs, divider):
-    res = np.zeros(b.shape, dtype=np.uint16)
-    res2 = np.zeros(b.shape, dtype=np.uint16)
-    zaehler = 0
-    for rgb in rgbs:
-        rr, gg, bb = rgb
-        for i in range(r.shape[0]):
-            if r[i] == rr:
-                if g[i] == gg:
-                    if b[i] == bb:
-                        dvquot, dvrem = divmod(i, divider)
-                        res[zaehler] = dvquot
-                        res2[zaehler] = dvrem
-                        zaehler = zaehler + 1
-    results = np.dstack((res[:zaehler], res2[:zaehler]))
-    return results
-
-
-compi2 = compnumba(
-    fu=search_colors,
-    funcname="search_colors",
-    file="searchcolorsnumba",
-    folder="locate_pixelcolor_numba",
-    signature=(uint8[:], uint8[:], uint8[:], uint8[:, :], uint16),
-    parallel=True,
-    fastmath=True,
-    nogil=True,
-)
-```
-
-### How to use it
-
-```python
-from locate_pixelcolor_numba import search_colors
-import cv2
-import time
-import numpy as np
-pic = cv2.imread(r"pexels-alex-andrews-2295744.jpg") # https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-colors = np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
-search_colors(pic,colors)
-Out[2]: 
-array([[[   0, 4522],
-        [   3, 4522],
-        [   3, 4523],
-        ...,
-        [6622, 4522],
-        [6622, 4523],
-        [6622, 4524]]], dtype=uint16)
-%timeit search_colors(pic,colors)
-413 ms ± 1.22 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-
-# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
-
-```
+### pip install locate-pixelcolor-numba
+
+
+### Important!
+This is a compiled .pyd file (Numba AOT), if you can't import it, run the following code to generate a new pyd file, and replace it with the old .pyd file.
+
+
+```python
+from numba_aot_compiler import compnumba #pip install numba-aot-compiler
+import numpy as np
+from numba import uint8, uint16
+
+
+def search_colors(r, g, b, rgbs, divider):
+    res = np.zeros(b.shape, dtype=np.uint16)
+    res2 = np.zeros(b.shape, dtype=np.uint16)
+    zaehler = 0
+    for rgb in rgbs:
+        rr, gg, bb = rgb
+        for i in range(r.shape[0]):
+            if r[i] == rr:
+                if g[i] == gg:
+                    if b[i] == bb:
+                        dvquot, dvrem = divmod(i, divider)
+                        res[zaehler] = dvquot
+                        res2[zaehler] = dvrem
+                        zaehler = zaehler + 1
+    results = np.dstack((res[:zaehler], res2[:zaehler]))
+    return results
+
+
+compi2 = compnumba(
+    fu=search_colors,
+    funcname="search_colors",
+    file="searchcolorsnumba",
+    folder="locate_pixelcolor_numba",
+    signature=(uint8[:], uint8[:], uint8[:], uint8[:, :], uint16),
+    parallel=True,
+    fastmath=True,
+    nogil=True,
+)
+```
+
+### How to use it
+
+```python
+from locate_pixelcolor_numba import search_colors
+import cv2
+import time
+import numpy as np
+pic = cv2.imread(r"pexels-alex-andrews-2295744.jpg") # https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+colors = np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
+search_colors(pic,colors)
+Out[2]: 
+array([[[   0, 4522],
+        [   3, 4522],
+        [   3, 4523],
+        ...,
+        [6622, 4522],
+        [6622, 4523],
+        [6622, 4524]]], dtype=uint16)
+%timeit search_colors(pic,colors)
+413 ms Â± 1.22 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+
+# More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
+
+```
```

### Comparing `locate_pixelcolor_numba-0.10/setup.py` & `locate_pixelcolor_numba-0.11/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
-import codecs
-import os
+# import codecs
+# import os
+# 
+# here = os.path.abspath(os.path.dirname(__file__))
+# 
+# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+#     long_description = "\n" + fh.read()\
 
-#change to dict
-here = os.path.abspath(os.path.dirname(__file__))
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.10'
-DESCRIPTION = "RGB search with numba - 2-3 x faster than numpy"
+VERSION = '''0.11'''
+DESCRIPTION = '''RGB search with numba - 2-3 x faster than numpy'''
 
 # Setting up
 setup(
     name="locate_pixelcolor_numba",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/locate_pixelcolor_numba',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['numpy'],
     keywords=['numba', 'aot', 'compiled', 'rgb', 'search'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['numpy'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

