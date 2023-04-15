# Comparing `tmp/locate_pixelcolor_c-0.10.tar.gz` & `tmp/locate_pixelcolor_c-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_c-0.10.tar", last modified: Fri Apr 14 00:22:05 2023, max compression
+gzip compressed data, was "locate_pixelcolor_c-0.11.tar", last modified: Sat Apr 15 00:33:34 2023, max compression
```

## Comparing `locate_pixelcolor_c-0.10.tar` & `locate_pixelcolor_c-0.11.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:22:05.666936 locate_pixelcolor_c-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-14 00:22:03.000000 locate_pixelcolor_c-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      203 2023-04-14 00:22:03.000000 locate_pixelcolor_c-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3476 2023-04-14 00:22:05.666936 locate_pixelcolor_c-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2700 2023-04-14 00:14:38.000000 locate_pixelcolor_c-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 00:22:05.661950 locate_pixelcolor_c-0.10/locate_pixelcolor_c/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c/LICENSE
--rw-rw-rw-   0        0        0     2700 2023-04-14 00:14:38.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c/README.md
--rw-rw-rw-   0        0        0     4204 2023-04-14 00:18:18.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c/__init__.py
--rw-rw-rw-   0        0        0    45876 2023-04-13 23:47:48.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c/cloop.so
--rw-rw-rw-   0        0        0        5 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c/requirements.txt
--rw-rw-rw-   0        0        0    49102 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 00:22:05.665939 locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/
--rw-rw-rw-   0        0        0     3476 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 00:22:05.666936 locate_pixelcolor_c-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1238 2023-04-14 00:22:05.000000 locate_pixelcolor_c-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:33:34.616262 locate_pixelcolor_c-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:33:29.000000 locate_pixelcolor_c-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      166 2023-04-15 00:33:28.000000 locate_pixelcolor_c-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3361 2023-04-15 00:33:34.616262 locate_pixelcolor_c-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2700 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:33:34.610280 locate_pixelcolor_c-0.11/locate_pixelcolor_c/
+-rw-rw-rw-   0        0        0     2700 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/README.md
+-rw-rw-rw-   0        0        0     4204 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/__init__.py
+-rw-rw-rw-   0        0        0    45876 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/cloop.so
+-rw-rw-rw-   0        0        0        5 2023-04-15 00:33:32.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/requirements.txt
+-rw-rw-rw-   0        0        0     2342 2023-04-15 00:33:32.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:33:34.615265 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/
+-rw-rw-rw-   0        0        0     3361 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:33:34.617263 locate_pixelcolor_c-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1315 2023-04-15 00:33:32.000000 locate_pixelcolor_c-0.11/setup.py
```

### Comparing `locate_pixelcolor_c-0.10/LICENSE.rst` & `locate_pixelcolor_c-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_c-0.10/PKG-INFO` & `locate_pixelcolor_c-0.11/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,87 @@
 Metadata-Version: 2.1
 Name: locate_pixelcolor_c
-Version: 0.10
+Version: 0.11
 Summary: Detects colors in images 10 x faster than Numpy 
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_c
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: C,image,search,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Detects colors in images 10 x faster than Numpy 
 
-# Detects colors in images 10 x faster than Numpy 
-
-### pip install locate-pixelcolor-c
-
-#### Tested against Windows 10 / Python 3.10 / Anaconda
-
-
-
-### How to use it in Python 
-
-```python
-import numpy as np
-import cv2
-from locate_pixelcolor_c import search_colors
-# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
-pic = cv2.imread(picx)
-colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
-resus0 = search_colors(pic=pic, colors=colors0)
-colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
-resus1 =  search_colors(pic=pic, colors=colors1)
-####################################################################
-%timeit search_colors(pic=pic, colors=colors0)
-17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
-
-b,g,r = pic[...,0],pic[...,1],pic[...,2]
-%timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-####################################################################
-%timeit resus1 =  search_colors(pic=pic, colors=colors1)
-138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-####################################################################
-```
-
-
-### The C Code 
-
-```c
-
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
-{
-    int counter = 0;
-
-    for (int i = 0; i <= totallengthcolor; i += 3)
-    {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
-        for (int j = 0; j <= totallengthpic; j += 3)
-        {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
-            {
-
-                int dividend = j / 3;
-                int quotient = dividend / width;
-                int remainder = dividend % width;
-                int upcounter = counter;
-                outputx[upcounter] = quotient;
-                outputy[upcounter] = remainder;
-                lastresult[0] = upcounter;
-                counter++;
-            }
-        }
-    }
-}
-// gcc -O2 -fPIC -shared -o cloop.so cloop.c
+### pip install locate-pixelcolor-c
+
+#### Tested against Windows 10 / Python 3.10 / Anaconda
+
+
+
+### How to use it in Python 
+
+```python
+import numpy as np
+import cv2
+from locate_pixelcolor_c import search_colors
+# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
+pic = cv2.imread(picx)
+colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
+resus0 = search_colors(pic=pic, colors=colors0)
+colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
+resus1 =  search_colors(pic=pic, colors=colors1)
+####################################################################
+%timeit search_colors(pic=pic, colors=colors0)
+17.6 ms Â± 245 Âµs per loop (mean Â± std. dev. of 7 runs, 100 loops each)
+
+b,g,r = pic[...,0],pic[...,1],pic[...,2]
+%timeit np.where(((b==255)&(g==255)&(r==255)))
+150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+####################################################################
+%timeit resus1 =  search_colors(pic=pic, colors=colors1)
+138 ms Â± 10 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
+1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+####################################################################
+```
+
+
+### The C Code 
+
+```c
+
+void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    int counter = 0;
+
+    for (int i = 0; i <= totallengthcolor; i += 3)
+    {
+        int r = i;
+        int g = i + 1;
+        int b = i + 2;
+        for (int j = 0; j <= totallengthpic; j += 3)
+        {
+            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            {
+
+                int dividend = j / 3;
+                int quotient = dividend / width;
+                int remainder = dividend % width;
+                int upcounter = counter;
+                outputx[upcounter] = quotient;
+                outputy[upcounter] = remainder;
+                lastresult[0] = upcounter;
+                counter++;
+            }
+        }
+    }
+}
+// gcc -O2 -fPIC -shared -o cloop.so cloop.c
 ```
```

### Comparing `locate_pixelcolor_c-0.10/README.md` & `locate_pixelcolor_c-0.11/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_c-0.10/locate_pixelcolor_c/README.md` & `locate_pixelcolor_c-0.11/locate_pixelcolor_c/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_c-0.10/locate_pixelcolor_c/__init__.py` & `locate_pixelcolor_c-0.11/locate_pixelcolor_c/__init__.py`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_c-0.10/locate_pixelcolor_c/cloop.so` & `locate_pixelcolor_c-0.11/locate_pixelcolor_c/cloop.so`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_c-0.10/locate_pixelcolor_c.egg-info/PKG-INFO` & `locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,87 @@
 Metadata-Version: 2.1
 Name: locate-pixelcolor-c
-Version: 0.10
+Version: 0.11
 Summary: Detects colors in images 10 x faster than Numpy 
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_c
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: C,image,search,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Detects colors in images 10 x faster than Numpy 
 
-# Detects colors in images 10 x faster than Numpy 
-
-### pip install locate-pixelcolor-c
-
-#### Tested against Windows 10 / Python 3.10 / Anaconda
-
-
-
-### How to use it in Python 
-
-```python
-import numpy as np
-import cv2
-from locate_pixelcolor_c import search_colors
-# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
-pic = cv2.imread(picx)
-colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
-resus0 = search_colors(pic=pic, colors=colors0)
-colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
-resus1 =  search_colors(pic=pic, colors=colors1)
-####################################################################
-%timeit search_colors(pic=pic, colors=colors0)
-17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
-
-b,g,r = pic[...,0],pic[...,1],pic[...,2]
-%timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-####################################################################
-%timeit resus1 =  search_colors(pic=pic, colors=colors1)
-138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-####################################################################
-```
-
-
-### The C Code 
-
-```c
-
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
-{
-    int counter = 0;
-
-    for (int i = 0; i <= totallengthcolor; i += 3)
-    {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
-        for (int j = 0; j <= totallengthpic; j += 3)
-        {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
-            {
-
-                int dividend = j / 3;
-                int quotient = dividend / width;
-                int remainder = dividend % width;
-                int upcounter = counter;
-                outputx[upcounter] = quotient;
-                outputy[upcounter] = remainder;
-                lastresult[0] = upcounter;
-                counter++;
-            }
-        }
-    }
-}
-// gcc -O2 -fPIC -shared -o cloop.so cloop.c
+### pip install locate-pixelcolor-c
+
+#### Tested against Windows 10 / Python 3.10 / Anaconda
+
+
+
+### How to use it in Python 
+
+```python
+import numpy as np
+import cv2
+from locate_pixelcolor_c import search_colors
+# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
+pic = cv2.imread(picx)
+colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
+resus0 = search_colors(pic=pic, colors=colors0)
+colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
+resus1 =  search_colors(pic=pic, colors=colors1)
+####################################################################
+%timeit search_colors(pic=pic, colors=colors0)
+17.6 ms Â± 245 Âµs per loop (mean Â± std. dev. of 7 runs, 100 loops each)
+
+b,g,r = pic[...,0],pic[...,1],pic[...,2]
+%timeit np.where(((b==255)&(g==255)&(r==255)))
+150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+####################################################################
+%timeit resus1 =  search_colors(pic=pic, colors=colors1)
+138 ms Â± 10 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
+1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+####################################################################
+```
+
+
+### The C Code 
+
+```c
+
+void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    int counter = 0;
+
+    for (int i = 0; i <= totallengthcolor; i += 3)
+    {
+        int r = i;
+        int g = i + 1;
+        int b = i + 2;
+        for (int j = 0; j <= totallengthpic; j += 3)
+        {
+            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            {
+
+                int dividend = j / 3;
+                int quotient = dividend / width;
+                int remainder = dividend % width;
+                int upcounter = counter;
+                outputx[upcounter] = quotient;
+                outputy[upcounter] = remainder;
+                lastresult[0] = upcounter;
+                counter++;
+            }
+        }
+    }
+}
+// gcc -O2 -fPIC -shared -o cloop.so cloop.c
 ```
```

### Comparing `locate_pixelcolor_c-0.10/setup.py` & `locate_pixelcolor_c-0.11/setup.py`

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
-DESCRIPTION = "Detects colors in images 10 x faster than Numpy "
+VERSION = '''0.11'''
+DESCRIPTION = '''Detects colors in images 10 x faster than Numpy '''
 
 # Setting up
 setup(
     name="locate_pixelcolor_c",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/locate_pixelcolor_c',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['numpy'],
     keywords=['C', 'image', 'search', 'rgb'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['numpy'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

