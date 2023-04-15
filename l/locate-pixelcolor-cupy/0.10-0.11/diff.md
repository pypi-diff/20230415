# Comparing `tmp/locate_pixelcolor_cupy-0.10.tar.gz` & `tmp/locate_pixelcolor_cupy-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_cupy-0.10.tar", last modified: Fri Apr 14 01:00:14 2023, max compression
+gzip compressed data, was "locate_pixelcolor_cupy-0.11.tar", last modified: Sat Apr 15 00:32:12 2023, max compression
```

## Comparing `locate_pixelcolor_cupy-0.10.tar` & `locate_pixelcolor_cupy-0.11.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 01:00:14.411685 locate_pixelcolor_cupy-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-14 01:00:10.000000 locate_pixelcolor_cupy-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      177 2023-04-14 01:00:10.000000 locate_pixelcolor_cupy-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2746 2023-04-14 01:00:14.411685 locate_pixelcolor_cupy-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2023-04-14 00:57:00.000000 locate_pixelcolor_cupy-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 01:00:14.400206 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/LICENSE
--rw-rw-rw-   0        0        0     1973 2023-04-14 00:57:00.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/README.md
--rw-rw-rw-   0        0        0      475 2023-04-14 00:48:38.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/__init__.py
--rw-rw-rw-   0        0        0       11 2023-04-14 01:00:13.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/requirements.txt
--rw-rw-rw-   0        0        0     4021 2023-04-14 01:00:13.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 01:00:14.409690 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/
--rw-rw-rw-   0        0        0     2746 2023-04-14 01:00:14.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-14 01:00:14.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 01:00:14.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 01:00:14.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-14 01:00:14.000000 locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 01:00:14.420661 locate_pixelcolor_cupy-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1270 2023-04-14 01:00:13.000000 locate_pixelcolor_cupy-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:32:12.264515 locate_pixelcolor_cupy-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:32:07.000000 locate_pixelcolor_cupy-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      137 2023-04-15 00:32:07.000000 locate_pixelcolor_cupy-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2646 2023-04-15 00:32:12.264515 locate_pixelcolor_cupy-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2023-04-15 00:18:06.000000 locate_pixelcolor_cupy-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:32:12.260525 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/
+-rw-rw-rw-   0        0        0     1973 2023-04-15 00:18:06.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/README.md
+-rw-rw-rw-   0        0        0      475 2023-04-15 00:18:06.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-04-15 00:32:11.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/requirements.txt
+-rw-rw-rw-   0        0        0     4021 2023-04-15 00:32:11.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:32:12.263517 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/
+-rw-rw-rw-   0        0        0     2646 2023-04-15 00:32:12.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-15 00:32:12.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:32:12.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-15 00:32:12.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-15 00:32:12.000000 locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:32:12.265512 locate_pixelcolor_cupy-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-04-15 00:32:11.000000 locate_pixelcolor_cupy-0.11/setup.py
```

### Comparing `locate_pixelcolor_cupy-0.10/LICENSE.rst` & `locate_pixelcolor_cupy-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cupy-0.10/PKG-INFO` & `locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 Metadata-Version: 2.1
-Name: locate_pixelcolor_cupy
-Version: 0.10
+Name: locate-pixelcolor-cupy
+Version: 0.11
 Summary: Detects colors in images up to 8 times as fast as NumPy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_cupy
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Cupy,image,search,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Detects colors in images up to 8 times as fast as NumPy  
 
-# Detects colors in images up to 8 times as fast as NumPy  
-
-### pip install locate-pixelcolor-cupy
-If you haven't installed cupy yet, I recommend you installing it using conda:
-conda install -c conda-forge cupy
-
-#### Tested against Windows 10 / Python 3.10 / Anaconda
-
-
-
-### Usage
-
-```python
-
-import numpy as np
-import cv2
-from locate_pixelcolor_cupy import search_colors
-# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
-pic = cv2.imread(picx)
-colors0 = np.array([[255, 255, 255]], dtype=np.uint8)
-resus0 = search_colors(pic=pic, colors=colors0)
-colors1 = np.array(
-    [
-        (66, 71, 69),
-        (62, 67, 65),
-        (144, 155, 153),
-        (52, 57, 55),
-        (127, 138, 136),
-        (53, 58, 56),
-        (51, 56, 54),
-        (32, 27, 18),
-        (24, 17, 8),
-    ],
-    dtype=np.uint8,
-)
-resus1 = search_colors(pic=pic, colors=colors1)
-####################################################################
-%timeit resus0 = search_colors(pic=pic, colors=colors0)
-78.2 ms ± 1.29 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-
-b,g,r = pic[...,0],pic[...,1],pic[...,2]
-%timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-####################################################################
-%timeit resus1 = search_colors(pic=pic, colors=colors1)
-139 ms ± 9.78 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-
-%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-####################################################################
-```
+### pip install locate-pixelcolor-cupy
+If you haven't installed cupy yet, I recommend you installing it using conda:
+conda install -c conda-forge cupy
+
+#### Tested against Windows 10 / Python 3.10 / Anaconda
+
+
+
+### Usage
+
+```python
+
+import numpy as np
+import cv2
+from locate_pixelcolor_cupy import search_colors
+# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
+pic = cv2.imread(picx)
+colors0 = np.array([[255, 255, 255]], dtype=np.uint8)
+resus0 = search_colors(pic=pic, colors=colors0)
+colors1 = np.array(
+    [
+        (66, 71, 69),
+        (62, 67, 65),
+        (144, 155, 153),
+        (52, 57, 55),
+        (127, 138, 136),
+        (53, 58, 56),
+        (51, 56, 54),
+        (32, 27, 18),
+        (24, 17, 8),
+    ],
+    dtype=np.uint8,
+)
+resus1 = search_colors(pic=pic, colors=colors1)
+####################################################################
+%timeit resus0 = search_colors(pic=pic, colors=colors0)
+78.2 ms Â± 1.29 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+
+b,g,r = pic[...,0],pic[...,1],pic[...,2]
+%timeit np.where(((b==255)&(g==255)&(r==255)))
+150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+####################################################################
+%timeit resus1 = search_colors(pic=pic, colors=colors1)
+139 ms Â± 9.78 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+
+%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
+1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+####################################################################
+```
```

### Comparing `locate_pixelcolor_cupy-0.10/README.md` & `locate_pixelcolor_cupy-0.11/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/README.md` & `locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy/thirdparty.json` & `locate_pixelcolor_cupy-0.11/locate_pixelcolor_cupy/thirdparty.json`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cupy-0.10/locate_pixelcolor_cupy.egg-info/PKG-INFO` & `locate_pixelcolor_cupy-0.11/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 Metadata-Version: 2.1
-Name: locate-pixelcolor-cupy
-Version: 0.10
+Name: locate_pixelcolor_cupy
+Version: 0.11
 Summary: Detects colors in images up to 8 times as fast as NumPy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_cupy
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Cupy,image,search,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Detects colors in images up to 8 times as fast as NumPy  
 
-# Detects colors in images up to 8 times as fast as NumPy  
-
-### pip install locate-pixelcolor-cupy
-If you haven't installed cupy yet, I recommend you installing it using conda:
-conda install -c conda-forge cupy
-
-#### Tested against Windows 10 / Python 3.10 / Anaconda
-
-
-
-### Usage
-
-```python
-
-import numpy as np
-import cv2
-from locate_pixelcolor_cupy import search_colors
-# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
-pic = cv2.imread(picx)
-colors0 = np.array([[255, 255, 255]], dtype=np.uint8)
-resus0 = search_colors(pic=pic, colors=colors0)
-colors1 = np.array(
-    [
-        (66, 71, 69),
-        (62, 67, 65),
-        (144, 155, 153),
-        (52, 57, 55),
-        (127, 138, 136),
-        (53, 58, 56),
-        (51, 56, 54),
-        (32, 27, 18),
-        (24, 17, 8),
-    ],
-    dtype=np.uint8,
-)
-resus1 = search_colors(pic=pic, colors=colors1)
-####################################################################
-%timeit resus0 = search_colors(pic=pic, colors=colors0)
-78.2 ms ± 1.29 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-
-b,g,r = pic[...,0],pic[...,1],pic[...,2]
-%timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-####################################################################
-%timeit resus1 = search_colors(pic=pic, colors=colors1)
-139 ms ± 9.78 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-
-%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-####################################################################
-```
+### pip install locate-pixelcolor-cupy
+If you haven't installed cupy yet, I recommend you installing it using conda:
+conda install -c conda-forge cupy
+
+#### Tested against Windows 10 / Python 3.10 / Anaconda
+
+
+
+### Usage
+
+```python
+
+import numpy as np
+import cv2
+from locate_pixelcolor_cupy import search_colors
+# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
+pic = cv2.imread(picx)
+colors0 = np.array([[255, 255, 255]], dtype=np.uint8)
+resus0 = search_colors(pic=pic, colors=colors0)
+colors1 = np.array(
+    [
+        (66, 71, 69),
+        (62, 67, 65),
+        (144, 155, 153),
+        (52, 57, 55),
+        (127, 138, 136),
+        (53, 58, 56),
+        (51, 56, 54),
+        (32, 27, 18),
+        (24, 17, 8),
+    ],
+    dtype=np.uint8,
+)
+resus1 = search_colors(pic=pic, colors=colors1)
+####################################################################
+%timeit resus0 = search_colors(pic=pic, colors=colors0)
+78.2 ms Â± 1.29 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+
+b,g,r = pic[...,0],pic[...,1],pic[...,2]
+%timeit np.where(((b==255)&(g==255)&(r==255)))
+150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+####################################################################
+%timeit resus1 = search_colors(pic=pic, colors=colors1)
+139 ms Â± 9.78 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+
+%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
+1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+####################################################################
+```
```

### Comparing `locate_pixelcolor_cupy-0.10/setup.py` & `locate_pixelcolor_cupy-0.11/setup.py`

 * *Files 15% similar despite different names*

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
-DESCRIPTION = "Detects colors in images up to 8 times as fast as NumPy"
+VERSION = '''0.11'''
+DESCRIPTION = '''Detects colors in images up to 8 times as fast as NumPy'''
 
 # Setting up
 setup(
     name="locate_pixelcolor_cupy",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/locate_pixelcolor_cupy',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['cupy', 'numpy'],
     keywords=['Cupy', 'image', 'search', 'rgb'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['cupy', 'numpy'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

