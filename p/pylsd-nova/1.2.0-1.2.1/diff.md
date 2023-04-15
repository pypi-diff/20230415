# Comparing `tmp/pylsd-nova-1.2.0.tar.gz` & `tmp/pylsd-nova-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylsd-nova-1.2.0.tar", last modified: Mon Aug 17 21:31:41 2020, max compression
+gzip compressed data, was "pylsd-nova-1.2.1.tar", last modified: Sat Apr 15 16:02:03 2023, max compression
```

## Comparing `pylsd-nova-1.2.0.tar` & `pylsd-nova-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/
--rw-r--r--   0 andranik  (1000) andranik  (1000)       79 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/setup.cfg
--rw-r--r--   0 andranik  (1000) andranik  (1000)      952 2020-08-17 21:31:24.000000 pylsd-nova-1.2.0/setup.py
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd_nova.egg-info/
--rw-r--r--   0 andranik  (1000) andranik  (1000)        6 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd_nova.egg-info/top_level.txt
--rw-r--r--   0 andranik  (1000) andranik  (1000)        1 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd_nova.egg-info/dependency_links.txt
--rw-r--r--   0 andranik  (1000) andranik  (1000)      369 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd_nova.egg-info/SOURCES.txt
--rw-r--r--   0 andranik  (1000) andranik  (1000)     5022 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd_nova.egg-info/PKG-INFO
--rw-r--r--   0 andranik  (1000) andranik  (1000)     5022 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/PKG-INFO
--rw-r--r--   0 andranik  (1000) andranik  (1000)     3740 2020-08-17 21:26:30.000000 pylsd-nova-1.2.0/README.md
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/
--rw-r--r--   0 andranik  (1000) andranik  (1000)       67 2020-04-04 12:10:59.000000 pylsd-nova-1.2.0/pylsd/__init__.py
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/lib/
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/lib/linux/
--rwxr-xr-x   0 andranik  (1000) andranik  (1000)    40160 2020-03-24 10:53:07.000000 pylsd-nova-1.2.0/pylsd/lib/linux/liblsd.so
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/lib/win32/
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/lib/win32/x86/
--rw-r--r--   0 andranik  (1000) andranik  (1000)   358377 2020-08-17 21:26:30.000000 pylsd-nova-1.2.0/pylsd/lib/win32/x86/liblsd.dll
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/lib/win32/x64/
--rw-r--r--   0 andranik  (1000) andranik  (1000)    76913 2020-08-17 21:26:30.000000 pylsd-nova-1.2.0/pylsd/lib/win32/x64/liblsd.dll
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/lib/darwin/
--rwxr-xr-x   0 andranik  (1000) andranik  (1000)    50784 2020-04-04 11:02:46.000000 pylsd-nova-1.2.0/pylsd/lib/darwin/liblsd.dylib
-drwxr-xr-x   0 andranik  (1000) andranik  (1000)        0 2020-08-17 21:31:41.000000 pylsd-nova-1.2.0/pylsd/bindings/
--rw-r--r--   0 andranik  (1000) andranik  (1000)       73 2020-04-04 12:10:19.000000 pylsd-nova-1.2.0/pylsd/bindings/__init__.py
--rw-r--r--   0 andranik  (1000) andranik  (1000)     1302 2020-04-04 12:18:21.000000 pylsd-nova-1.2.0/pylsd/bindings/lsd_ctypes.py
--rw-r--r--   0 andranik  (1000) andranik  (1000)     2350 2020-04-04 12:25:42.000000 pylsd-nova-1.2.0/pylsd/lsd.py
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)     1275 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/LICENSE
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)     4097 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/PKG-INFO
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)     3740 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/README.md
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)       67 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/__init__.py
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/bindings/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)       73 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/bindings/__init__.py
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)     1434 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/bindings/lsd_ctypes.py
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.314080 pylsd-nova-1.2.1/pylsd/lib/
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.314080 pylsd-nova-1.2.1/pylsd/lib/darwin/
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/lib/darwin/arm64/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)    70074 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/lib/darwin/arm64/liblsd.dylib
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/lib/darwin/x64/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)    50784 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/lib/darwin/x64/liblsd.dylib
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/lib/linux/
+-rwxrwxr-x   0 andranik  (1000) andranik  (1000)    40160 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/lib/linux/liblsd.so
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.314080 pylsd-nova-1.2.1/pylsd/lib/win32/
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/lib/win32/x64/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)    76913 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/lib/win32/x64/liblsd.dll
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd/lib/win32/x86/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)   358377 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/lib/win32/x86/liblsd.dll
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)     2350 2023-04-15 15:55:44.000000 pylsd-nova-1.2.1/pylsd/lsd.py
+drwxrwxr-x   0 andranik  (1000) andranik  (1000)        0 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/pylsd_nova.egg-info/
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)     4097 2023-04-15 16:02:03.000000 pylsd-nova-1.2.1/pylsd_nova.egg-info/PKG-INFO
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)      417 2023-04-15 16:02:03.000000 pylsd-nova-1.2.1/pylsd_nova.egg-info/SOURCES.txt
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)        1 2023-04-15 16:02:03.000000 pylsd-nova-1.2.1/pylsd_nova.egg-info/dependency_links.txt
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)        6 2023-04-15 16:02:03.000000 pylsd-nova-1.2.1/pylsd_nova.egg-info/top_level.txt
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)       79 2023-04-15 16:02:03.318080 pylsd-nova-1.2.1/setup.cfg
+-rw-rw-r--   0 andranik  (1000) andranik  (1000)      988 2023-04-15 15:58:57.000000 pylsd-nova-1.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylsd-nova-1.2.0/setup.py` & `pylsd-nova-1.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='pylsd-nova',
-    version='1.2.0',
+    version='1.2.1',
     author='Andranik Sargsyan',
     author_email='and.sargsyan@yahoo.com',
     description='pylsd-nova is a python binding for LSD - Line Segment Detector',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='BSD',
     keywords='LSD',
     url='https://github.com/AndranikSargsyan/pylsd-nova',
     packages=['pylsd', 'pylsd.bindings', 'pylsd.lib'],
     package_dir={'pylsd.lib': 'pylsd/lib'},
     package_data={'pylsd.lib': [
-        'darwin/*.dylib',
+        'darwin/arm64/*.dylib',
+        'darwin/x64/*.dylib',
         'win32/x86/*.dll',
         'win32/x64/*.dll',
         'linux/*.so'
     ]},
 )
```

### Comparing `pylsd-nova-1.2.0/pylsd_nova.egg-info/PKG-INFO` & `pylsd-nova-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,132 @@
 Metadata-Version: 2.1
 Name: pylsd-nova
-Version: 1.2.0
+Version: 1.2.1
 Summary: pylsd-nova is a python binding for LSD - Line Segment Detector
 Home-page: https://github.com/AndranikSargsyan/pylsd-nova
 Author: Andranik Sargsyan
 Author-email: and.sargsyan@yahoo.com
 License: BSD
-Description: pylsd-nova
-        =============
-        
-        ### 1. Introduction
-        
-        pylsd-nova is a python binding for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
-        
-        This is a fork from original [pylsd binding](https://github.com/primetang/pylsd/). This fork works for Python 3 and adds the ability to change lsd parameters from python call. 
-        
-        ### 2. Install
-        
-        This package uses distutils, which is the default way of installing python modules. For installing by cloning the repository you can run the following commands:
-        ```
-        git clone https://github.com/AndranikSargsyan/pylsd-nova.git
-        cd pylsd-nova
-        pip install .
-        ```
-        
-        Or install directly through `pip`:
-        ```
-        pip install pylsd-nova
-        ```
-        
-        ### 3. Usage
-        
-        You can use the package by importing like  `from pylsd import lsd`, and calling `segments = lsd(img)` by optionally passing other lsd parameters mentioned below. `img` is a Grayscale Image (`H x W` numpy.ndarray), and the return value `segments` contains detected line segments.
-        
-        `segments` is an `N x 5` numpy.ndarray. Each row represents a straight line. The 5-dimensional row format is:
-        
-        ```
-        [point1.x, point1.y, point2.x, point2.y, width]
-        ```
-        
-        These are the parameters of lsd, which can be changed through keyword arguments of lsd call:
-        
-        
-        * `scale (float)`: Scale the image by Gaussian filter to 'scale'.
-        
-        * `sigma_scale (float)`: Sigma for Gaussian filter is computed as `sigma = sigma_scale / scale`.
-        
-        * `quant (float)`: Bound to the quantization error on the gradient norm.
-        
-        * `ang_th (float)`: Gradient angle tolerance in degrees.
-        
-        * `eps (float)`: Detection threshold, `-log10(NFA)`.
-        
-        * `density_th (float)`: Minimal density of region points in rectangle.
-        
-        * `n_bins (int)`: Number of bins in pseudo-ordering of gradient modulus.
-        
-        * `max_grad (float)`: Gradient modulus in the highest bin. The default value corresponds to the highest gradient modulus on images with gray levels in [0,255].
-        
-        
-        You can use it just like the following code ([here is the link to examples](https://github.com/AndranikSargsyan/pylsd-nova/tree/master/example)):
-        
-        * by using cv2 module
-        
-        ```python
-        import cv2
-        import numpy as np
-        import os
-        from pylsd import lsd
-        
-        full_name = 'car.jpg'
-        folder, img_name = os.path.split(full_name)
-        img = cv2.imread(full_name, cv2.IMREAD_COLOR)
-        img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-        
-        segments = lsd(img_gray, scale=0.5)
-        
-        for i in range(segments.shape[0]):
-            pt1 = (int(segments[i, 0]), int(segments[i, 1]))
-            pt2 = (int(segments[i, 2]), int(segments[i, 3]))
-            width = segments[i, 4]
-            cv2.line(img, pt1, pt2, (0, 0, 255), int(np.ceil(width / 2)))
-        
-        cv2.imwrite(os.path.join(folder, 'cv2_' + img_name.split('.')[0] + '.jpg'), img)
-        ```
-        
-        * by using PIL(Image) module
-        
-        ```python
-        import numpy as np
-        import os
-        from PIL import Image, ImageDraw
-        from pylsd import lsd
-        
-        full_name = 'house.png'
-        folder, img_name = os.path.split(full_name)
-        img = Image.open(full_name)
-        img_gray = np.asarray(img.convert('L'))
-        
-        segments = lsd(img_gray, scale=0.5)
-        
-        draw = ImageDraw.Draw(img)
-        for i in range(segments.shape[0]):
-            pt1 = (int(segments[i, 0]), int(segments[i, 1]))
-            pt2 = (int(segments[i, 2]), int(segments[i, 3]))
-            width = segments[i, 4]
-            draw.line((pt1, pt2), fill=(0, 0, 255), width=int(np.ceil(width / 2)))
-        
-        img.save(os.path.join(folder, 'PIL_' + img_name.split('.')[0] + '.jpg'))
-        ```
-        
-        The following is the result:
-        
-        * car.jpg by using cv2 module
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/car.jpg)
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/cv2_car.jpg)
-        
-        * house.png by using PIL(Image) module
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/house.png)
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/PIL_house.jpg)
-        
 Keywords: LSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+pylsd-nova
+=============
+
+### 1. Introduction
+
+pylsd-nova is a python binding for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
+
+This is a fork from original [pylsd binding](https://github.com/primetang/pylsd/). This fork works for Python 3 and adds the ability to change lsd parameters from python call. 
+
+### 2. Install
+
+This package uses distutils, which is the default way of installing python modules. For installing by cloning the repository you can run the following commands:
+```
+git clone https://github.com/AndranikSargsyan/pylsd-nova.git
+cd pylsd-nova
+pip install .
+```
+
+Or install directly through `pip`:
+```
+pip install pylsd-nova
+```
+
+### 3. Usage
+
+You can use the package by importing like  `from pylsd import lsd`, and calling `segments = lsd(img)` by optionally passing other lsd parameters mentioned below. `img` is a Grayscale Image (`H x W` numpy.ndarray), and the return value `segments` contains detected line segments.
+
+`segments` is an `N x 5` numpy.ndarray. Each row represents a straight line. The 5-dimensional row format is:
+
+```
+[point1.x, point1.y, point2.x, point2.y, width]
+```
+
+These are the parameters of lsd, which can be changed through keyword arguments of lsd call:
+
+
+* `scale (float)`: Scale the image by Gaussian filter to 'scale'.
+
+* `sigma_scale (float)`: Sigma for Gaussian filter is computed as `sigma = sigma_scale / scale`.
+
+* `quant (float)`: Bound to the quantization error on the gradient norm.
+
+* `ang_th (float)`: Gradient angle tolerance in degrees.
+
+* `eps (float)`: Detection threshold, `-log10(NFA)`.
+
+* `density_th (float)`: Minimal density of region points in rectangle.
+
+* `n_bins (int)`: Number of bins in pseudo-ordering of gradient modulus.
+
+* `max_grad (float)`: Gradient modulus in the highest bin. The default value corresponds to the highest gradient modulus on images with gray levels in [0,255].
+
+
+You can use it just like the following code ([here is the link to examples](https://github.com/AndranikSargsyan/pylsd-nova/tree/master/example)):
+
+* by using cv2 module
+
+```python
+import cv2
+import numpy as np
+import os
+from pylsd import lsd
+
+full_name = 'car.jpg'
+folder, img_name = os.path.split(full_name)
+img = cv2.imread(full_name, cv2.IMREAD_COLOR)
+img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+
+segments = lsd(img_gray, scale=0.5)
+
+for i in range(segments.shape[0]):
+    pt1 = (int(segments[i, 0]), int(segments[i, 1]))
+    pt2 = (int(segments[i, 2]), int(segments[i, 3]))
+    width = segments[i, 4]
+    cv2.line(img, pt1, pt2, (0, 0, 255), int(np.ceil(width / 2)))
+
+cv2.imwrite(os.path.join(folder, 'cv2_' + img_name.split('.')[0] + '.jpg'), img)
+```
+
+* by using PIL(Image) module
+
+```python
+import numpy as np
+import os
+from PIL import Image, ImageDraw
+from pylsd import lsd
+
+full_name = 'house.png'
+folder, img_name = os.path.split(full_name)
+img = Image.open(full_name)
+img_gray = np.asarray(img.convert('L'))
+
+segments = lsd(img_gray, scale=0.5)
+
+draw = ImageDraw.Draw(img)
+for i in range(segments.shape[0]):
+    pt1 = (int(segments[i, 0]), int(segments[i, 1]))
+    pt2 = (int(segments[i, 2]), int(segments[i, 3]))
+    width = segments[i, 4]
+    draw.line((pt1, pt2), fill=(0, 0, 255), width=int(np.ceil(width / 2)))
+
+img.save(os.path.join(folder, 'PIL_' + img_name.split('.')[0] + '.jpg'))
+```
+
+The following is the result:
+
+* car.jpg by using cv2 module
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/car.jpg)
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/cv2_car.jpg)
+
+* house.png by using PIL(Image) module
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/house.png)
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/PIL_house.jpg)
+
+
```

### Comparing `pylsd-nova-1.2.0/PKG-INFO` & `pylsd-nova-1.2.1/pylsd_nova.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,132 @@
 Metadata-Version: 2.1
 Name: pylsd-nova
-Version: 1.2.0
+Version: 1.2.1
 Summary: pylsd-nova is a python binding for LSD - Line Segment Detector
 Home-page: https://github.com/AndranikSargsyan/pylsd-nova
 Author: Andranik Sargsyan
 Author-email: and.sargsyan@yahoo.com
 License: BSD
-Description: pylsd-nova
-        =============
-        
-        ### 1. Introduction
-        
-        pylsd-nova is a python binding for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
-        
-        This is a fork from original [pylsd binding](https://github.com/primetang/pylsd/). This fork works for Python 3 and adds the ability to change lsd parameters from python call. 
-        
-        ### 2. Install
-        
-        This package uses distutils, which is the default way of installing python modules. For installing by cloning the repository you can run the following commands:
-        ```
-        git clone https://github.com/AndranikSargsyan/pylsd-nova.git
-        cd pylsd-nova
-        pip install .
-        ```
-        
-        Or install directly through `pip`:
-        ```
-        pip install pylsd-nova
-        ```
-        
-        ### 3. Usage
-        
-        You can use the package by importing like  `from pylsd import lsd`, and calling `segments = lsd(img)` by optionally passing other lsd parameters mentioned below. `img` is a Grayscale Image (`H x W` numpy.ndarray), and the return value `segments` contains detected line segments.
-        
-        `segments` is an `N x 5` numpy.ndarray. Each row represents a straight line. The 5-dimensional row format is:
-        
-        ```
-        [point1.x, point1.y, point2.x, point2.y, width]
-        ```
-        
-        These are the parameters of lsd, which can be changed through keyword arguments of lsd call:
-        
-        
-        * `scale (float)`: Scale the image by Gaussian filter to 'scale'.
-        
-        * `sigma_scale (float)`: Sigma for Gaussian filter is computed as `sigma = sigma_scale / scale`.
-        
-        * `quant (float)`: Bound to the quantization error on the gradient norm.
-        
-        * `ang_th (float)`: Gradient angle tolerance in degrees.
-        
-        * `eps (float)`: Detection threshold, `-log10(NFA)`.
-        
-        * `density_th (float)`: Minimal density of region points in rectangle.
-        
-        * `n_bins (int)`: Number of bins in pseudo-ordering of gradient modulus.
-        
-        * `max_grad (float)`: Gradient modulus in the highest bin. The default value corresponds to the highest gradient modulus on images with gray levels in [0,255].
-        
-        
-        You can use it just like the following code ([here is the link to examples](https://github.com/AndranikSargsyan/pylsd-nova/tree/master/example)):
-        
-        * by using cv2 module
-        
-        ```python
-        import cv2
-        import numpy as np
-        import os
-        from pylsd import lsd
-        
-        full_name = 'car.jpg'
-        folder, img_name = os.path.split(full_name)
-        img = cv2.imread(full_name, cv2.IMREAD_COLOR)
-        img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-        
-        segments = lsd(img_gray, scale=0.5)
-        
-        for i in range(segments.shape[0]):
-            pt1 = (int(segments[i, 0]), int(segments[i, 1]))
-            pt2 = (int(segments[i, 2]), int(segments[i, 3]))
-            width = segments[i, 4]
-            cv2.line(img, pt1, pt2, (0, 0, 255), int(np.ceil(width / 2)))
-        
-        cv2.imwrite(os.path.join(folder, 'cv2_' + img_name.split('.')[0] + '.jpg'), img)
-        ```
-        
-        * by using PIL(Image) module
-        
-        ```python
-        import numpy as np
-        import os
-        from PIL import Image, ImageDraw
-        from pylsd import lsd
-        
-        full_name = 'house.png'
-        folder, img_name = os.path.split(full_name)
-        img = Image.open(full_name)
-        img_gray = np.asarray(img.convert('L'))
-        
-        segments = lsd(img_gray, scale=0.5)
-        
-        draw = ImageDraw.Draw(img)
-        for i in range(segments.shape[0]):
-            pt1 = (int(segments[i, 0]), int(segments[i, 1]))
-            pt2 = (int(segments[i, 2]), int(segments[i, 3]))
-            width = segments[i, 4]
-            draw.line((pt1, pt2), fill=(0, 0, 255), width=int(np.ceil(width / 2)))
-        
-        img.save(os.path.join(folder, 'PIL_' + img_name.split('.')[0] + '.jpg'))
-        ```
-        
-        The following is the result:
-        
-        * car.jpg by using cv2 module
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/car.jpg)
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/cv2_car.jpg)
-        
-        * house.png by using PIL(Image) module
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/house.png)
-        
-        ![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/PIL_house.jpg)
-        
 Keywords: LSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+pylsd-nova
+=============
+
+### 1. Introduction
+
+pylsd-nova is a python binding for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
+
+This is a fork from original [pylsd binding](https://github.com/primetang/pylsd/). This fork works for Python 3 and adds the ability to change lsd parameters from python call. 
+
+### 2. Install
+
+This package uses distutils, which is the default way of installing python modules. For installing by cloning the repository you can run the following commands:
+```
+git clone https://github.com/AndranikSargsyan/pylsd-nova.git
+cd pylsd-nova
+pip install .
+```
+
+Or install directly through `pip`:
+```
+pip install pylsd-nova
+```
+
+### 3. Usage
+
+You can use the package by importing like  `from pylsd import lsd`, and calling `segments = lsd(img)` by optionally passing other lsd parameters mentioned below. `img` is a Grayscale Image (`H x W` numpy.ndarray), and the return value `segments` contains detected line segments.
+
+`segments` is an `N x 5` numpy.ndarray. Each row represents a straight line. The 5-dimensional row format is:
+
+```
+[point1.x, point1.y, point2.x, point2.y, width]
+```
+
+These are the parameters of lsd, which can be changed through keyword arguments of lsd call:
+
+
+* `scale (float)`: Scale the image by Gaussian filter to 'scale'.
+
+* `sigma_scale (float)`: Sigma for Gaussian filter is computed as `sigma = sigma_scale / scale`.
+
+* `quant (float)`: Bound to the quantization error on the gradient norm.
+
+* `ang_th (float)`: Gradient angle tolerance in degrees.
+
+* `eps (float)`: Detection threshold, `-log10(NFA)`.
+
+* `density_th (float)`: Minimal density of region points in rectangle.
+
+* `n_bins (int)`: Number of bins in pseudo-ordering of gradient modulus.
+
+* `max_grad (float)`: Gradient modulus in the highest bin. The default value corresponds to the highest gradient modulus on images with gray levels in [0,255].
+
+
+You can use it just like the following code ([here is the link to examples](https://github.com/AndranikSargsyan/pylsd-nova/tree/master/example)):
+
+* by using cv2 module
+
+```python
+import cv2
+import numpy as np
+import os
+from pylsd import lsd
+
+full_name = 'car.jpg'
+folder, img_name = os.path.split(full_name)
+img = cv2.imread(full_name, cv2.IMREAD_COLOR)
+img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+
+segments = lsd(img_gray, scale=0.5)
+
+for i in range(segments.shape[0]):
+    pt1 = (int(segments[i, 0]), int(segments[i, 1]))
+    pt2 = (int(segments[i, 2]), int(segments[i, 3]))
+    width = segments[i, 4]
+    cv2.line(img, pt1, pt2, (0, 0, 255), int(np.ceil(width / 2)))
+
+cv2.imwrite(os.path.join(folder, 'cv2_' + img_name.split('.')[0] + '.jpg'), img)
+```
+
+* by using PIL(Image) module
+
+```python
+import numpy as np
+import os
+from PIL import Image, ImageDraw
+from pylsd import lsd
+
+full_name = 'house.png'
+folder, img_name = os.path.split(full_name)
+img = Image.open(full_name)
+img_gray = np.asarray(img.convert('L'))
+
+segments = lsd(img_gray, scale=0.5)
+
+draw = ImageDraw.Draw(img)
+for i in range(segments.shape[0]):
+    pt1 = (int(segments[i, 0]), int(segments[i, 1]))
+    pt2 = (int(segments[i, 2]), int(segments[i, 3]))
+    width = segments[i, 4]
+    draw.line((pt1, pt2), fill=(0, 0, 255), width=int(np.ceil(width / 2)))
+
+img.save(os.path.join(folder, 'PIL_' + img_name.split('.')[0] + '.jpg'))
+```
+
+The following is the result:
+
+* car.jpg by using cv2 module
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/car.jpg)
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/cv2_car.jpg)
+
+* house.png by using PIL(Image) module
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/house.png)
+
+![](https://github.com/AndranikSargsyan/pylsd-nova/blob/master/example/PIL_house.jpg)
+
+
```

### Comparing `pylsd-nova-1.2.0/README.md` & `pylsd-nova-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pylsd-nova-1.2.0/pylsd/lib/linux/liblsd.so` & `pylsd-nova-1.2.1/pylsd/lib/linux/liblsd.so`

 * *Files identical despite different names*

### Comparing `pylsd-nova-1.2.0/pylsd/lib/win32/x86/liblsd.dll` & `pylsd-nova-1.2.1/pylsd/lib/win32/x86/liblsd.dll`

 * *Files identical despite different names*

### Comparing `pylsd-nova-1.2.0/pylsd/lib/win32/x64/liblsd.dll` & `pylsd-nova-1.2.1/pylsd/lib/win32/x64/liblsd.dll`

 * *Files identical despite different names*

### Comparing `pylsd-nova-1.2.0/pylsd/lib/darwin/liblsd.dylib` & `pylsd-nova-1.2.1/pylsd/lib/darwin/x64/liblsd.dylib`

 * *Files identical despite different names*

### Comparing `pylsd-nova-1.2.0/pylsd/bindings/lsd_ctypes.py` & `pylsd-nova-1.2.1/pylsd/bindings/lsd_ctypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import ctypes
 import os
 import sys
-
+import platform
 
 def load_lsd_library():
     root_dir = os.path.abspath(os.path.dirname(__file__))
 
     libnames = ['linux/liblsd.so']
     libdir = 'lib'
 
     if sys.platform == 'win32':
         if sys.maxsize > 2 ** 32:
             libnames = ['win32/x64/lsd.dll', 'win32/x64/liblsd.dll']
         else:
             libnames = ['win32/x86/lsd.dll', 'win32/x86/liblsd.dll']
 
     elif sys.platform == 'darwin':
-        libnames = ['darwin/liblsd.dylib']
+        if platform.processor() == 'arm':
+            libnames = ['darwin/arm64/liblsd.dylib']
+        else:
+            libnames = ['darwin/x64/liblsd.dylib']
 
     while root_dir is not None:
         for libname in libnames:
             try:
                 lsdlib = ctypes.cdll[os.path.join(root_dir, libdir, libname)]
                 return lsdlib
             except Exception as e:
```

### Comparing `pylsd-nova-1.2.0/pylsd/lsd.py` & `pylsd-nova-1.2.1/pylsd/lsd.py`

 * *Files identical despite different names*

