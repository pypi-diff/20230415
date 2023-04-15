# Comparing `tmp/locate_pixelcolor_cpp_parallelfor-0.10.tar.gz` & `tmp/locate_pixelcolor_cpp_parallelfor-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_cpp_parallelfor-0.10.tar", last modified: Thu Apr 13 23:09:11 2023, max compression
+gzip compressed data, was "locate_pixelcolor_cpp_parallelfor-0.11.tar", last modified: Sat Apr 15 00:36:11 2023, max compression
```

## Comparing `locate_pixelcolor_cpp_parallelfor-0.10.tar` & `locate_pixelcolor_cpp_parallelfor-0.11.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 23:09:11.965439 locate_pixelcolor_cpp_parallelfor-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-13 23:09:09.000000 locate_pixelcolor_cpp_parallelfor-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      274 2023-04-13 23:09:09.000000 locate_pixelcolor_cpp_parallelfor-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4272 2023-04-13 23:09:11.965439 locate_pixelcolor_cpp_parallelfor-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3437 2023-04-13 23:08:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 23:09:11.960452 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/LICENSE
--rw-rw-rw-   0        0        0     3437 2023-04-13 23:08:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/README.md
--rw-rw-rw-   0        0        0     4618 2023-04-13 22:58:58.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/__init__.py
--rw-rw-rw-   0        0        0    24064 2023-04-13 22:48:31.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/cloop.dll
--rw-rw-rw-   0        0        0        5 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/requirements.txt
--rw-rw-rw-   0        0        0    49102 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-13 23:09:11.964481 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/
--rw-rw-rw-   0        0        0     4272 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      613 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 23:09:11.966436 locate_pixelcolor_cpp_parallelfor-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-13 23:09:11.000000 locate_pixelcolor_cpp_parallelfor-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:36:11.626522 locate_pixelcolor_cpp_parallelfor-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:36:06.000000 locate_pixelcolor_cpp_parallelfor-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      223 2023-04-15 00:36:05.000000 locate_pixelcolor_cpp_parallelfor-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4146 2023-04-15 00:36:11.626522 locate_pixelcolor_cpp_parallelfor-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3437 2023-04-15 00:17:54.000000 locate_pixelcolor_cpp_parallelfor-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:36:11.622510 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/
+-rw-rw-rw-   0        0        0     3437 2023-04-15 00:17:54.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/README.md
+-rw-rw-rw-   0        0        0     4618 2023-04-15 00:17:54.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/__init__.py
+-rw-rw-rw-   0        0        0    24064 2023-04-15 00:17:54.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/cloop.dll
+-rw-rw-rw-   0        0        0        5 2023-04-15 00:36:09.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/requirements.txt
+-rw-rw-rw-   0        0        0     2342 2023-04-15 00:36:09.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:36:11.626522 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/
+-rw-rw-rw-   0        0        0     4146 2023-04-15 00:36:11.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2023-04-15 00:36:11.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:36:11.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 00:36:11.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 00:36:11.000000 locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:36:11.627490 locate_pixelcolor_cpp_parallelfor-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1369 2023-04-15 00:36:09.000000 locate_pixelcolor_cpp_parallelfor-0.11/setup.py
```

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/LICENSE.rst` & `locate_pixelcolor_cpp_parallelfor-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/PKG-INFO` & `locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,98 @@
 Metadata-Version: 2.1
-Name: locate_pixelcolor_cpp_parallelfor
-Version: 0.10
+Name: locate-pixelcolor-cpp-parallelfor
+Version: 0.11
 Summary: Detects colors in images up to 10 x faster than Numpy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_cpp_parallelfor
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: cpp,c++,image,search,parallel,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Detects colors in images up to 10 x faster than Numpy 
 
-# Detects colors in images up to 10 x faster than Numpy 
-
-### pip install locate-pixelcolor-cpp-parallelfor
-
-#### Tested against Windows 10 / Python 3.10 / Anaconda
-
-### Important!
-The module imports a function from a compiled .dll (C++). 
-If you get any import errors, install:  https://download.visualstudio.microsoft.com/download/pr/8b92f460-7e03-4c75-a139-e264a770758d/26C2C72FBA6438F5E29AF8EBC4826A1E424581B3C446F8C735361F1DB7BEFF72/VC_redist.x64.exe
-
-
-### How to use it in Python 
-
-```python
-import cv2
-import numpy as np
-from locate_pixelcolor_cpp_parallelfor import search_colors
-# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
-pic = cv2.imread(picx)
-colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
-resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
-colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
-resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
-print(resus1)
-####################################################################
-# Pretty good, but this one is better: https://github.com/hansalemaos/locate_pixelcolor_cpppragma
-%timeit resus0 =  search_colors(pic=pic, colors=colors0, cpus=5)
-69.4 ms ± 302 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-b,g,r = pic[...,0],pic[...,1],pic[...,2]
-%timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-####################################################################
-%timeit resus1 =  search_colors(pic=pic, colors=colors1, cpus=5)
-151 ms ± 10.2 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-####################################################################
-```
-
-
-### The C++ Code 
-
-```cpp
-#include <atomic>
-#include <ppl.h>
-
-std::atomic<int> value(0);
-
-int create_id()
-{
-    return std::atomic_fetch_add(&value, 1);
-}
-
-extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
-{
-    value = 0;
-
-    concurrency::parallel_for(0, totallengthcolor / 3 + 1, [&](int i)
-                              {
-        int r = i * 3;
-        int g = i * 3 + 1;
-        int b = i * 3 + 2;
-        for (int j = 0; j <= totallengthpic; j += 3)
-        {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
-            {
-                int dividend = j / 3;
-                int quotient = dividend / width;
-                int remainder = dividend % width;
-                int upcounter = create_id();
-                outputx[upcounter] = quotient;
-                outputy[upcounter] = remainder;
-                lastresult[0] = upcounter;
-            }
-        } });
-}
-// cl.exe /std:c++20 /fp:fast /EHsc /Oi /Ot /Oy /Ob3 /GF /Gy /MD /openmp /LD cloop.cpp /Fe:cloop.dll
+### pip install locate-pixelcolor-cpp-parallelfor
+
+#### Tested against Windows 10 / Python 3.10 / Anaconda
+
+### Important!
+The module imports a function from a compiled .dll (C++). 
+If you get any import errors, install:  https://download.visualstudio.microsoft.com/download/pr/8b92f460-7e03-4c75-a139-e264a770758d/26C2C72FBA6438F5E29AF8EBC4826A1E424581B3C446F8C735361F1DB7BEFF72/VC_redist.x64.exe
+
+
+### How to use it in Python 
+
+```python
+import cv2
+import numpy as np
+from locate_pixelcolor_cpp_parallelfor import search_colors
+# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
+pic = cv2.imread(picx)
+colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
+resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
+colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
+resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
+print(resus1)
+####################################################################
+# Pretty good, but this one is better: https://github.com/hansalemaos/locate_pixelcolor_cpppragma
+%timeit resus0 =  search_colors(pic=pic, colors=colors0, cpus=5)
+69.4 ms Â± 302 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+b,g,r = pic[...,0],pic[...,1],pic[...,2]
+%timeit np.where(((b==255)&(g==255)&(r==255)))
+150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+####################################################################
+%timeit resus1 =  search_colors(pic=pic, colors=colors1, cpus=5)
+151 ms Â± 10.2 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
+1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+####################################################################
+```
+
+
+### The C++ Code 
+
+```cpp
+#include <atomic>
+#include <ppl.h>
+
+std::atomic<int> value(0);
+
+int create_id()
+{
+    return std::atomic_fetch_add(&value, 1);
+}
+
+extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    value = 0;
+
+    concurrency::parallel_for(0, totallengthcolor / 3 + 1, [&](int i)
+                              {
+        int r = i * 3;
+        int g = i * 3 + 1;
+        int b = i * 3 + 2;
+        for (int j = 0; j <= totallengthpic; j += 3)
+        {
+            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            {
+                int dividend = j / 3;
+                int quotient = dividend / width;
+                int remainder = dividend % width;
+                int upcounter = create_id();
+                outputx[upcounter] = quotient;
+                outputy[upcounter] = remainder;
+                lastresult[0] = upcounter;
+            }
+        } });
+}
+// cl.exe /std:c++20 /fp:fast /EHsc /Oi /Ot /Oy /Ob3 /GF /Gy /MD /openmp /LD cloop.cpp /Fe:cloop.dll
 ```
```

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/README.md` & `locate_pixelcolor_cpp_parallelfor-0.11/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/README.md` & `locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/__init__.py` & `locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/__init__.py`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor/cloop.dll` & `locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor/cloop.dll`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/PKG-INFO` & `locate_pixelcolor_cpp_parallelfor-0.11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,98 @@
 Metadata-Version: 2.1
-Name: locate-pixelcolor-cpp-parallelfor
-Version: 0.10
+Name: locate_pixelcolor_cpp_parallelfor
+Version: 0.11
 Summary: Detects colors in images up to 10 x faster than Numpy
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_cpp_parallelfor
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: cpp,c++,image,search,parallel,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Detects colors in images up to 10 x faster than Numpy 
 
-# Detects colors in images up to 10 x faster than Numpy 
-
-### pip install locate-pixelcolor-cpp-parallelfor
-
-#### Tested against Windows 10 / Python 3.10 / Anaconda
-
-### Important!
-The module imports a function from a compiled .dll (C++). 
-If you get any import errors, install:  https://download.visualstudio.microsoft.com/download/pr/8b92f460-7e03-4c75-a139-e264a770758d/26C2C72FBA6438F5E29AF8EBC4826A1E424581B3C446F8C735361F1DB7BEFF72/VC_redist.x64.exe
-
-
-### How to use it in Python 
-
-```python
-import cv2
-import numpy as np
-from locate_pixelcolor_cpp_parallelfor import search_colors
-# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
-picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
-pic = cv2.imread(picx)
-colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
-resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
-colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
-resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
-print(resus1)
-####################################################################
-# Pretty good, but this one is better: https://github.com/hansalemaos/locate_pixelcolor_cpppragma
-%timeit resus0 =  search_colors(pic=pic, colors=colors0, cpus=5)
-69.4 ms ± 302 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-b,g,r = pic[...,0],pic[...,1],pic[...,2]
-%timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-####################################################################
-%timeit resus1 =  search_colors(pic=pic, colors=colors1, cpus=5)
-151 ms ± 10.2 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-
-%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-####################################################################
-```
-
-
-### The C++ Code 
-
-```cpp
-#include <atomic>
-#include <ppl.h>
-
-std::atomic<int> value(0);
-
-int create_id()
-{
-    return std::atomic_fetch_add(&value, 1);
-}
-
-extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
-{
-    value = 0;
-
-    concurrency::parallel_for(0, totallengthcolor / 3 + 1, [&](int i)
-                              {
-        int r = i * 3;
-        int g = i * 3 + 1;
-        int b = i * 3 + 2;
-        for (int j = 0; j <= totallengthpic; j += 3)
-        {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
-            {
-                int dividend = j / 3;
-                int quotient = dividend / width;
-                int remainder = dividend % width;
-                int upcounter = create_id();
-                outputx[upcounter] = quotient;
-                outputy[upcounter] = remainder;
-                lastresult[0] = upcounter;
-            }
-        } });
-}
-// cl.exe /std:c++20 /fp:fast /EHsc /Oi /Ot /Oy /Ob3 /GF /Gy /MD /openmp /LD cloop.cpp /Fe:cloop.dll
+### pip install locate-pixelcolor-cpp-parallelfor
+
+#### Tested against Windows 10 / Python 3.10 / Anaconda
+
+### Important!
+The module imports a function from a compiled .dll (C++). 
+If you get any import errors, install:  https://download.visualstudio.microsoft.com/download/pr/8b92f460-7e03-4c75-a139-e264a770758d/26C2C72FBA6438F5E29AF8EBC4826A1E424581B3C446F8C735361F1DB7BEFF72/VC_redist.x64.exe
+
+
+### How to use it in Python 
+
+```python
+import cv2
+import numpy as np
+from locate_pixelcolor_cpp_parallelfor import search_colors
+# 4525 x 6623 x 3 picture https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/
+picx = r"C:\Users\hansc\Downloads\pexels-alex-andrews-2295744.jpg"
+pic = cv2.imread(picx)
+colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
+resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
+colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
+resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
+print(resus1)
+####################################################################
+# Pretty good, but this one is better: https://github.com/hansalemaos/locate_pixelcolor_cpppragma
+%timeit resus0 =  search_colors(pic=pic, colors=colors0, cpus=5)
+69.4 ms Â± 302 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+b,g,r = pic[...,0],pic[...,1],pic[...,2]
+%timeit np.where(((b==255)&(g==255)&(r==255)))
+150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+####################################################################
+%timeit resus1 =  search_colors(pic=pic, colors=colors1, cpus=5)
+151 ms Â± 10.2 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+
+%timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
+1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+####################################################################
+```
+
+
+### The C++ Code 
+
+```cpp
+#include <atomic>
+#include <ppl.h>
+
+std::atomic<int> value(0);
+
+int create_id()
+{
+    return std::atomic_fetch_add(&value, 1);
+}
+
+extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    value = 0;
+
+    concurrency::parallel_for(0, totallengthcolor / 3 + 1, [&](int i)
+                              {
+        int r = i * 3;
+        int g = i * 3 + 1;
+        int b = i * 3 + 2;
+        for (int j = 0; j <= totallengthpic; j += 3)
+        {
+            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            {
+                int dividend = j / 3;
+                int quotient = dividend / width;
+                int remainder = dividend % width;
+                int upcounter = create_id();
+                outputx[upcounter] = quotient;
+                outputy[upcounter] = remainder;
+                lastresult[0] = upcounter;
+            }
+        } });
+}
+// cl.exe /std:c++20 /fp:fast /EHsc /Oi /Ot /Oy /Ob3 /GF /Gy /MD /openmp /LD cloop.cpp /Fe:cloop.dll
 ```
```

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/locate_pixelcolor_cpp_parallelfor.egg-info/SOURCES.txt` & `locate_pixelcolor_cpp_parallelfor-0.11/locate_pixelcolor_cpp_parallelfor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.rst
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-locate_pixelcolor_cpp_parallelfor/LICENSE
 locate_pixelcolor_cpp_parallelfor/README.md
 locate_pixelcolor_cpp_parallelfor/__init__.py
 locate_pixelcolor_cpp_parallelfor/cloop.dll
 locate_pixelcolor_cpp_parallelfor/requirements.txt
 locate_pixelcolor_cpp_parallelfor/thirdparty.json
 locate_pixelcolor_cpp_parallelfor.egg-info/PKG-INFO
 locate_pixelcolor_cpp_parallelfor.egg-info/SOURCES.txt
```

### Comparing `locate_pixelcolor_cpp_parallelfor-0.10/setup.py` & `locate_pixelcolor_cpp_parallelfor-0.11/setup.py`

 * *Files 16% similar despite different names*

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
-DESCRIPTION = "Detects colors in images up to 10 x faster than Numpy"
+VERSION = '''0.11'''
+DESCRIPTION = '''Detects colors in images up to 10 x faster than Numpy'''
 
 # Setting up
 setup(
     name="locate_pixelcolor_cpp_parallelfor",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/locate_pixelcolor_cpp_parallelfor',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['numpy'],
     keywords=['cpp', 'c++', 'image', 'search', 'parallel', 'rgb'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['numpy'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

