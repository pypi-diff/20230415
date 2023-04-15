# Comparing `tmp/defisheye-1.0.3.tar.gz` & `tmp/defisheye-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defisheye-1.0.3.tar", last modified: Fri Apr 14 11:20:35 2023, max compression
+gzip compressed data, was "defisheye-1.1.0.tar", last modified: Sat Apr 15 14:07:59 2023, max compression
```

## Comparing `defisheye-1.0.3.tar` & `defisheye-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-14 11:20:35.620569 defisheye-1.0.3/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4774 2023-04-13 12:43:38.000000 defisheye-1.0.3/README.md
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-14 11:20:35.620569 defisheye-1.0.3/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      707 2023-04-14 11:20:14.000000 defisheye-1.0.3/setup.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/src/
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/src/defisheye/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      750 2023-04-13 12:40:23.000000 defisheye-1.0.3/src/defisheye/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5197 2023-04-14 11:19:59.000000 defisheye-1.0.3/src/defisheye/defisheye.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/src/defisheye.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      255 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       20 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.093201 defisheye-1.1.0/
+-rw-rw-rw-   0        0        0     5776 2023-04-15 14:07:59.084847 defisheye-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5470 2023-04-15 13:58:18.000000 defisheye-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 14:07:59.093201 defisheye-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      892 2023-04-15 13:47:38.000000 defisheye-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.035705 defisheye-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.046727 defisheye-1.1.0/src/defisheye/
+-rw-rw-rw-   0        0        0      774 2023-04-15 12:41:29.000000 defisheye-1.1.0/src/defisheye/__init__.py
+-rw-rw-rw-   0        0        0     4613 2023-04-15 13:49:19.000000 defisheye-1.1.0/src/defisheye/__main__.py
+-rw-rw-rw-   0        0        0     5356 2023-04-15 12:41:29.000000 defisheye-1.1.0/src/defisheye/defisheye.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.084847 defisheye-1.1.0/src/defisheye.egg-info/
+-rw-rw-rw-   0        0        0     5776 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/top_level.txt
```

### Comparing `defisheye-1.0.3/PKG-INFO` & `defisheye-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,186 @@
-Metadata-Version: 2.1
-Name: defisheye
-Version: 1.0.3
-Summary: Fast defisheye algorithm
-Home-page: https://github.com/duducosmos/defisheye
-Author: Eduardo S. Pereira
-Author-email: pereira.somoza@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Defisheye
-
-Fast Corrects for fisheye distortion in an image.
-
-Defisheye is designed to transform a fisheye image into a normal perspective
-view looking towards the center of the fisheye image.
-
-## Install
-
-```bash
-python setup.py install
-```
-
-or:
-
-```bash
-pip install defisheye
-```
-
-## Usage
-
-```python
-from defisheye import Defisheye
-
-dtype = 'linear'
-format = 'fullframe'
-fov = 180
-pfov = 120
-
-img = "./images/example3.jpg"
-img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
-
-obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
-
-# To save image locally 
-obj.convert(outfile=img_out)
-
-# To use the converted image in memory
-
-new_image = obj.convert()
-```
-
-
-
-## Constructor atributes:
-### fov
-fisheye field of view (aperture) in degrees.
-
-
-IFOV is the input fisheye image field of view in degrees. A value of 180
-will correspond to a hemispherical fisheye image within the circular area.
-Values are floats in the range 0<ifov<=180. The default is 180 degrees for a
-full hemisphere.
-
-
-### pfov
-perspective field of view (aperture) in degrees.
-
-
-OFOV is the output perspective image field of view in degrees. Values are
-floats in the range 0<ofov<180. The default is to use 120 degrees both
-vertically and horizontally for a circular fisheye and diagonally for a full
-frame fisheye. The value for ofov relative to the ifov determines the
-proportional amount of the fisheye area that will be transformed.
-Note that in comparison, a value of 48.8 degrees corresponds to a diagonal
-field of view from a 35 mm camera (film size 36mm x 24mm) with a 50mm focal
-length lens, i.e. a "normal" view. Similarly, when the image diagonal is
-equal to the focal length of the camera, the field of view is about 53.1
-degrees. Although the default value is perhaps not appropriate to a
-normal perspective image, this will produce an image that maximizes the
-area covered, but without too much distortion. If the original fisheye
-image was viewed obliquely, i.e. the camera was tilted between horizontal
-and vertical, then the resulting perspective view will have perspective
-distortion. That is  vertical edges will be tilted outward or inward.
-Post processing with my 3Drotate or rotate3D script will then correct
-for this perspective distortion. Perspective distortion will be more
-pronounced with larger values for ofov.
-
-### dtype
-linear, equalarea, orthographic, stereographic
-
-TYPE is the type of fisheye lens. The choices are: linear (equidistant),
-equalarea (equisolid), orthographic and stereographic. The default is linear.
-
-### format
-circular, fullframe
-
-FORMAT is the format of the fisheye lens image. The choices are:
-circular (image fills a circle that spans the minimum of the width or height)
-or fullframe (image spans a circle that spans the diagonal dimension).
-The default is circular.
-
-### xcenter
-x center of fisheye area
-
-
-### ycenter
-y center of fisheye area
-
-### radius
-radius of fisheye area
-
-RADIUS is the radius of the fisheye circular area in the input image.
-Values are floats greater than zero. The default is half the minimum value
-between the input image width and height.
-
-### angle
-image rotation in degrees clockwise
-
-ANGLE is the clockwise positive rotation angle for the output perspective
-image relative to the orientation of the input fisheye image. Values are
-non-negative floats in range 0<=angle<360. The default is 0.
-
-## Example
-
-Original
-![Original](./example/images/example3.jpg)
-
-pfov = 120
-
-Equal area  Circular
-![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
-
-Equal area Fullframe
-![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
-
-Linear  Circular
-![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
-
-Linear Fullframe
-![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
-
-
-orthographic  Circular
-![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
-
-Stereographic Circular
-![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
-
-
-## Extra
-Developed by: E. S. Pereira.
-e-mail: pereira.somoza@gmail.com
-
-Based in the work of F. Weinhaus.
-http://www.fmwconcepts.com/imagemagick/defisheye/index.php
-
-Copyright [2019] [E. S. Pereira]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
+# Defisheye
+
+Fast Corrects for fisheye distortion in an image.
+
+Defisheye is designed to transform a fisheye image into a normal perspective
+view looking towards the center of the fisheye image.
+
+## Install
+
+```bash
+python setup.py install
+```
+
+or:
+
+```bash
+pip install defisheye
+```
+
+## Usage
+
+### CLI 
+
+For individual Image
+```bash
+defisheye --image example/images/example3.jpg
+```
+
+Process all image in a folder
+
+
+```bash
+defisheye --images_folder example/images --save_dir example/Defisheye
+```
+
+
+### Python Code
+
+```python
+from defisheye import Defisheye
+
+dtype = 'linear'
+format = 'fullframe'
+fov = 180
+pfov = 120
+
+img = "./images/example3.jpg"
+img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
+
+obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
+
+# To save image locally 
+obj.convert(outfile=img_out)
+
+# To use the converted image in memory
+
+new_image = obj.convert()
+```
+
+
+
+## Parameter/ Atributes:
+
+For CLI command, use "--" and the parameter to pass for the command line: Exemple
+
+```bash
+defisheye --images_folder example/images --save_dir example/Defisheye --fov 140
+```
+
+The default fov is 180, but now was changed by 140 from command line. Same rule for the following parameters.
+
+### fov
+fisheye field of view (aperture) in degrees.
+
+
+IFOV is the input fisheye image field of view in degrees. A value of 180
+will correspond to a hemispherical fisheye image within the circular area.
+Values are floats in the range 0<ifov<=180. The default is 180 degrees for a
+full hemisphere.
+
+
+### pfov
+perspective field of view (aperture) in degrees.
+
+
+OFOV is the output perspective image field of view in degrees. Values are
+floats in the range 0<ofov<180. The default is to use 120 degrees both
+vertically and horizontally for a circular fisheye and diagonally for a full
+frame fisheye. The value for ofov relative to the ifov determines the
+proportional amount of the fisheye area that will be transformed.
+Note that in comparison, a value of 48.8 degrees corresponds to a diagonal
+field of view from a 35 mm camera (film size 36mm x 24mm) with a 50mm focal
+length lens, i.e. a "normal" view. Similarly, when the image diagonal is
+equal to the focal length of the camera, the field of view is about 53.1
+degrees. Although the default value is perhaps not appropriate to a
+normal perspective image, this will produce an image that maximizes the
+area covered, but without too much distortion. If the original fisheye
+image was viewed obliquely, i.e. the camera was tilted between horizontal
+and vertical, then the resulting perspective view will have perspective
+distortion. That is  vertical edges will be tilted outward or inward.
+Post processing with my 3Drotate or rotate3D script will then correct
+for this perspective distortion. Perspective distortion will be more
+pronounced with larger values for ofov.
+
+### dtype
+linear, equalarea, orthographic, stereographic
+
+TYPE is the type of fisheye lens. The choices are: linear (equidistant),
+equalarea (equisolid), orthographic and stereographic. The default is linear.
+
+### format
+circular, fullframe
+
+FORMAT is the format of the fisheye lens image. The choices are:
+circular (image fills a circle that spans the minimum of the width or height)
+or fullframe (image spans a circle that spans the diagonal dimension).
+The default is circular.
+
+### xcenter
+x center of fisheye area
+
+
+### ycenter
+y center of fisheye area
+
+### radius
+radius of fisheye area
+
+RADIUS is the radius of the fisheye circular area in the input image.
+Values are floats greater than zero. The default is half the minimum value
+between the input image width and height.
+
+### angle
+image rotation in degrees clockwise
+
+ANGLE is the clockwise positive rotation angle for the output perspective
+image relative to the orientation of the input fisheye image. Values are
+non-negative floats in range 0<=angle<360. The default is 0.
+
+## Example
+
+Original
+![Original](./example/images/example3.jpg)
+
+pfov = 120
+
+Equal area  Circular
+![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
+
+Equal area Fullframe
+![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
+
+Linear  Circular
+![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
+
+Linear Fullframe
+![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
+
+
+orthographic  Circular
+![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
+
+Stereographic Circular
+![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
+
+
+## Extra
+Developed by: E. S. Pereira.
+e-mail: pereira.somoza@gmail.com
+
+Based in the work of F. Weinhaus.
+http://www.fmwconcepts.com/imagemagick/defisheye/index.php
+
+Copyright [2019] [E. S. Pereira]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `defisheye-1.0.3/README.md` & `defisheye-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,199 @@
-# Defisheye
-
-Fast Corrects for fisheye distortion in an image.
-
-Defisheye is designed to transform a fisheye image into a normal perspective
-view looking towards the center of the fisheye image.
-
-## Install
-
-```bash
-python setup.py install
-```
-
-or:
-
-```bash
-pip install defisheye
-```
-
-## Usage
-
-```python
-from defisheye import Defisheye
-
-dtype = 'linear'
-format = 'fullframe'
-fov = 180
-pfov = 120
-
-img = "./images/example3.jpg"
-img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
-
-obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
-
-# To save image locally 
-obj.convert(outfile=img_out)
-
-# To use the converted image in memory
-
-new_image = obj.convert()
-```
-
-
-
-## Constructor atributes:
-### fov
-fisheye field of view (aperture) in degrees.
-
-
-IFOV is the input fisheye image field of view in degrees. A value of 180
-will correspond to a hemispherical fisheye image within the circular area.
-Values are floats in the range 0<ifov<=180. The default is 180 degrees for a
-full hemisphere.
-
-
-### pfov
-perspective field of view (aperture) in degrees.
-
-
-OFOV is the output perspective image field of view in degrees. Values are
-floats in the range 0<ofov<180. The default is to use 120 degrees both
-vertically and horizontally for a circular fisheye and diagonally for a full
-frame fisheye. The value for ofov relative to the ifov determines the
-proportional amount of the fisheye area that will be transformed.
-Note that in comparison, a value of 48.8 degrees corresponds to a diagonal
-field of view from a 35 mm camera (film size 36mm x 24mm) with a 50mm focal
-length lens, i.e. a "normal" view. Similarly, when the image diagonal is
-equal to the focal length of the camera, the field of view is about 53.1
-degrees. Although the default value is perhaps not appropriate to a
-normal perspective image, this will produce an image that maximizes the
-area covered, but without too much distortion. If the original fisheye
-image was viewed obliquely, i.e. the camera was tilted between horizontal
-and vertical, then the resulting perspective view will have perspective
-distortion. That is  vertical edges will be tilted outward or inward.
-Post processing with my 3Drotate or rotate3D script will then correct
-for this perspective distortion. Perspective distortion will be more
-pronounced with larger values for ofov.
-
-### dtype
-linear, equalarea, orthographic, stereographic
-
-TYPE is the type of fisheye lens. The choices are: linear (equidistant),
-equalarea (equisolid), orthographic and stereographic. The default is linear.
-
-### format
-circular, fullframe
-
-FORMAT is the format of the fisheye lens image. The choices are:
-circular (image fills a circle that spans the minimum of the width or height)
-or fullframe (image spans a circle that spans the diagonal dimension).
-The default is circular.
-
-### xcenter
-x center of fisheye area
-
-
-### ycenter
-y center of fisheye area
-
-### radius
-radius of fisheye area
-
-RADIUS is the radius of the fisheye circular area in the input image.
-Values are floats greater than zero. The default is half the minimum value
-between the input image width and height.
-
-### angle
-image rotation in degrees clockwise
-
-ANGLE is the clockwise positive rotation angle for the output perspective
-image relative to the orientation of the input fisheye image. Values are
-non-negative floats in range 0<=angle<360. The default is 0.
-
-## Example
-
-Original
-![Original](./example/images/example3.jpg)
-
-pfov = 120
-
-Equal area  Circular
-![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
-
-Equal area Fullframe
-![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
-
-Linear  Circular
-![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
-
-Linear Fullframe
-![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
-
-
-orthographic  Circular
-![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
-
-Stereographic Circular
-![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
-
-
-## Extra
-Developed by: E. S. Pereira.
-e-mail: pereira.somoza@gmail.com
-
-Based in the work of F. Weinhaus.
-http://www.fmwconcepts.com/imagemagick/defisheye/index.php
-
-Copyright [2019] [E. S. Pereira]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Metadata-Version: 2.1
+Name: defisheye
+Version: 1.1.0
+Summary: Fast defisheye algorithm
+Home-page: https://github.com/duducosmos/defisheye
+Author: Eduardo S. Pereira
+Author-email: pereira.somoza@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+# Defisheye
+
+Fast Corrects for fisheye distortion in an image.
+
+Defisheye is designed to transform a fisheye image into a normal perspective
+view looking towards the center of the fisheye image.
+
+## Install
+
+```bash
+python setup.py install
+```
+
+or:
+
+```bash
+pip install defisheye
+```
+
+## Usage
+
+### CLI 
+
+For individual Image
+```bash
+defisheye --image example/images/example3.jpg
+```
+
+Process all image in a folder
+
+
+```bash
+defisheye --images_folder example/images --save_dir example/Defisheye
+```
+
+
+### Python Code
+
+```python
+from defisheye import Defisheye
+
+dtype = 'linear'
+format = 'fullframe'
+fov = 180
+pfov = 120
+
+img = "./images/example3.jpg"
+img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
+
+obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
+
+# To save image locally 
+obj.convert(outfile=img_out)
+
+# To use the converted image in memory
+
+new_image = obj.convert()
+```
+
+
+
+## Parameter/ Atributes:
+
+For CLI command, use "--" and the parameter to pass for the command line: Exemple
+
+```bash
+defisheye --images_folder example/images --save_dir example/Defisheye --fov 140
+```
+
+The default fov is 180, but now was changed by 140 from command line. Same rule for the following parameters.
+
+### fov
+fisheye field of view (aperture) in degrees.
+
+
+IFOV is the input fisheye image field of view in degrees. A value of 180
+will correspond to a hemispherical fisheye image within the circular area.
+Values are floats in the range 0<ifov<=180. The default is 180 degrees for a
+full hemisphere.
+
+
+### pfov
+perspective field of view (aperture) in degrees.
+
+
+OFOV is the output perspective image field of view in degrees. Values are
+floats in the range 0<ofov<180. The default is to use 120 degrees both
+vertically and horizontally for a circular fisheye and diagonally for a full
+frame fisheye. The value for ofov relative to the ifov determines the
+proportional amount of the fisheye area that will be transformed.
+Note that in comparison, a value of 48.8 degrees corresponds to a diagonal
+field of view from a 35 mm camera (film size 36mm x 24mm) with a 50mm focal
+length lens, i.e. a "normal" view. Similarly, when the image diagonal is
+equal to the focal length of the camera, the field of view is about 53.1
+degrees. Although the default value is perhaps not appropriate to a
+normal perspective image, this will produce an image that maximizes the
+area covered, but without too much distortion. If the original fisheye
+image was viewed obliquely, i.e. the camera was tilted between horizontal
+and vertical, then the resulting perspective view will have perspective
+distortion. That is  vertical edges will be tilted outward or inward.
+Post processing with my 3Drotate or rotate3D script will then correct
+for this perspective distortion. Perspective distortion will be more
+pronounced with larger values for ofov.
+
+### dtype
+linear, equalarea, orthographic, stereographic
+
+TYPE is the type of fisheye lens. The choices are: linear (equidistant),
+equalarea (equisolid), orthographic and stereographic. The default is linear.
+
+### format
+circular, fullframe
+
+FORMAT is the format of the fisheye lens image. The choices are:
+circular (image fills a circle that spans the minimum of the width or height)
+or fullframe (image spans a circle that spans the diagonal dimension).
+The default is circular.
+
+### xcenter
+x center of fisheye area
+
+
+### ycenter
+y center of fisheye area
+
+### radius
+radius of fisheye area
+
+RADIUS is the radius of the fisheye circular area in the input image.
+Values are floats greater than zero. The default is half the minimum value
+between the input image width and height.
+
+### angle
+image rotation in degrees clockwise
+
+ANGLE is the clockwise positive rotation angle for the output perspective
+image relative to the orientation of the input fisheye image. Values are
+non-negative floats in range 0<=angle<360. The default is 0.
+
+## Example
+
+Original
+![Original](./example/images/example3.jpg)
+
+pfov = 120
+
+Equal area  Circular
+![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
+
+Equal area Fullframe
+![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
+
+Linear  Circular
+![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
+
+Linear Fullframe
+![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
+
+
+orthographic  Circular
+![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
+
+Stereographic Circular
+![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
+
+
+## Extra
+Developed by: E. S. Pereira.
+e-mail: pereira.somoza@gmail.com
+
+Based in the work of F. Weinhaus.
+http://www.fmwconcepts.com/imagemagick/defisheye/index.php
+
+Copyright [2019] [E. S. Pereira]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
```

### Comparing `defisheye-1.0.3/src/defisheye/__init__.py` & `defisheye-1.1.0/src/defisheye/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#!/usr/bin/env python3
-#-*- Coding: UTF-8 -*-
-"""
-Defisheye algorithm.
-
-Developed by: E. S. Pereira.
-e-mail: pereira.somoza@gmail.com
-
-Copyright [2019] [E. S. Pereira]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-"""
-
-from .defisheye import *
+#!/usr/bin/env python3
+#-*- Coding: UTF-8 -*-
+"""
+Defisheye algorithm.
+
+Developed by: E. S. Pereira.
+e-mail: pereira.somoza@gmail.com
+
+Copyright [2019] [E. S. Pereira]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+"""
+
+from .defisheye import *
```

### Comparing `defisheye-1.0.3/src/defisheye.egg-info/PKG-INFO` & `defisheye-1.1.0/src/defisheye.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,199 @@
-Metadata-Version: 2.1
-Name: defisheye
-Version: 1.0.3
-Summary: Fast defisheye algorithm
-Home-page: https://github.com/duducosmos/defisheye
-Author: Eduardo S. Pereira
-Author-email: pereira.somoza@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Defisheye
-
-Fast Corrects for fisheye distortion in an image.
-
-Defisheye is designed to transform a fisheye image into a normal perspective
-view looking towards the center of the fisheye image.
-
-## Install
-
-```bash
-python setup.py install
-```
-
-or:
-
-```bash
-pip install defisheye
-```
-
-## Usage
-
-```python
-from defisheye import Defisheye
-
-dtype = 'linear'
-format = 'fullframe'
-fov = 180
-pfov = 120
-
-img = "./images/example3.jpg"
-img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
-
-obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
-
-# To save image locally 
-obj.convert(outfile=img_out)
-
-# To use the converted image in memory
-
-new_image = obj.convert()
-```
-
-
-
-## Constructor atributes:
-### fov
-fisheye field of view (aperture) in degrees.
-
-
-IFOV is the input fisheye image field of view in degrees. A value of 180
-will correspond to a hemispherical fisheye image within the circular area.
-Values are floats in the range 0<ifov<=180. The default is 180 degrees for a
-full hemisphere.
-
-
-### pfov
-perspective field of view (aperture) in degrees.
-
-
-OFOV is the output perspective image field of view in degrees. Values are
-floats in the range 0<ofov<180. The default is to use 120 degrees both
-vertically and horizontally for a circular fisheye and diagonally for a full
-frame fisheye. The value for ofov relative to the ifov determines the
-proportional amount of the fisheye area that will be transformed.
-Note that in comparison, a value of 48.8 degrees corresponds to a diagonal
-field of view from a 35 mm camera (film size 36mm x 24mm) with a 50mm focal
-length lens, i.e. a "normal" view. Similarly, when the image diagonal is
-equal to the focal length of the camera, the field of view is about 53.1
-degrees. Although the default value is perhaps not appropriate to a
-normal perspective image, this will produce an image that maximizes the
-area covered, but without too much distortion. If the original fisheye
-image was viewed obliquely, i.e. the camera was tilted between horizontal
-and vertical, then the resulting perspective view will have perspective
-distortion. That is  vertical edges will be tilted outward or inward.
-Post processing with my 3Drotate or rotate3D script will then correct
-for this perspective distortion. Perspective distortion will be more
-pronounced with larger values for ofov.
-
-### dtype
-linear, equalarea, orthographic, stereographic
-
-TYPE is the type of fisheye lens. The choices are: linear (equidistant),
-equalarea (equisolid), orthographic and stereographic. The default is linear.
-
-### format
-circular, fullframe
-
-FORMAT is the format of the fisheye lens image. The choices are:
-circular (image fills a circle that spans the minimum of the width or height)
-or fullframe (image spans a circle that spans the diagonal dimension).
-The default is circular.
-
-### xcenter
-x center of fisheye area
-
-
-### ycenter
-y center of fisheye area
-
-### radius
-radius of fisheye area
-
-RADIUS is the radius of the fisheye circular area in the input image.
-Values are floats greater than zero. The default is half the minimum value
-between the input image width and height.
-
-### angle
-image rotation in degrees clockwise
-
-ANGLE is the clockwise positive rotation angle for the output perspective
-image relative to the orientation of the input fisheye image. Values are
-non-negative floats in range 0<=angle<360. The default is 0.
-
-## Example
-
-Original
-![Original](./example/images/example3.jpg)
-
-pfov = 120
-
-Equal area  Circular
-![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
-
-Equal area Fullframe
-![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
-
-Linear  Circular
-![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
-
-Linear Fullframe
-![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
-
-
-orthographic  Circular
-![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
-
-Stereographic Circular
-![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
-
-
-## Extra
-Developed by: E. S. Pereira.
-e-mail: pereira.somoza@gmail.com
-
-Based in the work of F. Weinhaus.
-http://www.fmwconcepts.com/imagemagick/defisheye/index.php
-
-Copyright [2019] [E. S. Pereira]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
+Metadata-Version: 2.1
+Name: defisheye
+Version: 1.1.0
+Summary: Fast defisheye algorithm
+Home-page: https://github.com/duducosmos/defisheye
+Author: Eduardo S. Pereira
+Author-email: pereira.somoza@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+# Defisheye
+
+Fast Corrects for fisheye distortion in an image.
+
+Defisheye is designed to transform a fisheye image into a normal perspective
+view looking towards the center of the fisheye image.
+
+## Install
+
+```bash
+python setup.py install
+```
+
+or:
+
+```bash
+pip install defisheye
+```
+
+## Usage
+
+### CLI 
+
+For individual Image
+```bash
+defisheye --image example/images/example3.jpg
+```
+
+Process all image in a folder
+
+
+```bash
+defisheye --images_folder example/images --save_dir example/Defisheye
+```
+
+
+### Python Code
+
+```python
+from defisheye import Defisheye
+
+dtype = 'linear'
+format = 'fullframe'
+fov = 180
+pfov = 120
+
+img = "./images/example3.jpg"
+img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
+
+obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
+
+# To save image locally 
+obj.convert(outfile=img_out)
+
+# To use the converted image in memory
+
+new_image = obj.convert()
+```
+
+
+
+## Parameter/ Atributes:
+
+For CLI command, use "--" and the parameter to pass for the command line: Exemple
+
+```bash
+defisheye --images_folder example/images --save_dir example/Defisheye --fov 140
+```
+
+The default fov is 180, but now was changed by 140 from command line. Same rule for the following parameters.
+
+### fov
+fisheye field of view (aperture) in degrees.
+
+
+IFOV is the input fisheye image field of view in degrees. A value of 180
+will correspond to a hemispherical fisheye image within the circular area.
+Values are floats in the range 0<ifov<=180. The default is 180 degrees for a
+full hemisphere.
+
+
+### pfov
+perspective field of view (aperture) in degrees.
+
+
+OFOV is the output perspective image field of view in degrees. Values are
+floats in the range 0<ofov<180. The default is to use 120 degrees both
+vertically and horizontally for a circular fisheye and diagonally for a full
+frame fisheye. The value for ofov relative to the ifov determines the
+proportional amount of the fisheye area that will be transformed.
+Note that in comparison, a value of 48.8 degrees corresponds to a diagonal
+field of view from a 35 mm camera (film size 36mm x 24mm) with a 50mm focal
+length lens, i.e. a "normal" view. Similarly, when the image diagonal is
+equal to the focal length of the camera, the field of view is about 53.1
+degrees. Although the default value is perhaps not appropriate to a
+normal perspective image, this will produce an image that maximizes the
+area covered, but without too much distortion. If the original fisheye
+image was viewed obliquely, i.e. the camera was tilted between horizontal
+and vertical, then the resulting perspective view will have perspective
+distortion. That is  vertical edges will be tilted outward or inward.
+Post processing with my 3Drotate or rotate3D script will then correct
+for this perspective distortion. Perspective distortion will be more
+pronounced with larger values for ofov.
+
+### dtype
+linear, equalarea, orthographic, stereographic
+
+TYPE is the type of fisheye lens. The choices are: linear (equidistant),
+equalarea (equisolid), orthographic and stereographic. The default is linear.
+
+### format
+circular, fullframe
+
+FORMAT is the format of the fisheye lens image. The choices are:
+circular (image fills a circle that spans the minimum of the width or height)
+or fullframe (image spans a circle that spans the diagonal dimension).
+The default is circular.
+
+### xcenter
+x center of fisheye area
+
+
+### ycenter
+y center of fisheye area
+
+### radius
+radius of fisheye area
+
+RADIUS is the radius of the fisheye circular area in the input image.
+Values are floats greater than zero. The default is half the minimum value
+between the input image width and height.
+
+### angle
+image rotation in degrees clockwise
+
+ANGLE is the clockwise positive rotation angle for the output perspective
+image relative to the orientation of the input fisheye image. Values are
+non-negative floats in range 0<=angle<360. The default is 0.
+
+## Example
+
+Original
+![Original](./example/images/example3.jpg)
+
+pfov = 120
+
+Equal area  Circular
+![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
+
+Equal area Fullframe
+![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
+
+Linear  Circular
+![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
+
+Linear Fullframe
+![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
+
+
+orthographic  Circular
+![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
+
+Stereographic Circular
+![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
+
+
+## Extra
+Developed by: E. S. Pereira.
+e-mail: pereira.somoza@gmail.com
+
+Based in the work of F. Weinhaus.
+http://www.fmwconcepts.com/imagemagick/defisheye/index.php
+
+Copyright [2019] [E. S. Pereira]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
```

