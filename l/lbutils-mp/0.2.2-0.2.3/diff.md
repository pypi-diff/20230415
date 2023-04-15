# Comparing `tmp/lbutils-mp-0.2.2.tar.gz` & `tmp/lbutils-mp-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbutils-mp-0.2.2.tar", last modified: Fri Apr 14 20:26:36 2023, max compression
+gzip compressed data, was "lbutils-mp-0.2.3.tar", last modified: Sat Apr 15 10:21:12 2023, max compression
```

## Comparing `lbutils-mp-0.2.2.tar` & `lbutils-mp-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/
--rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.2/LICENCE
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.2/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/
--rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.2/lbutils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.2/lbutils/abc.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/drivers/
--rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.2/lbutils/drivers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.2/lbutils/drivers/seven_segment.py
--rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.2/lbutils/drivers/seven_segment_hex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/examples/
--rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.2/lbutils/examples/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/graphics/
--rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.2/lbutils/graphics/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    22594 2023-04-14 20:24:00.000000 lbutils-mp-0.2.2/lbutils/graphics/canvas.py
--rw-rw-r--   0 david     (1000) david     (1000)     9715 2023-04-14 20:24:00.000000 lbutils-mp-0.2.2/lbutils/graphics/colours.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/graphics/fonts/
--rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/base_font.py
--rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/font06.py
--rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/font08.py
--rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/org_01.py
--rw-rw-r--   0 david     (1000) david     (1000)    12178 2023-04-14 20:24:00.000000 lbutils-mp-0.2.2/lbutils/graphics/helpers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/helpers/
--rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.2/lbutils/helpers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.2/lbutils/helpers/i2c.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils/pmods/
--rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.2/lbutils/pmods/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils/pmods/i2c/
--rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 19:33:01.000000 lbutils-mp-0.2.2/lbutils/pmods/i2c/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils/pmods/spi/
--rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 17:16:30.000000 lbutils-mp-0.2.2/lbutils/pmods/spi/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    23548 2023-04-14 20:24:55.000000 lbutils-mp-0.2.2/lbutils/pmods/spi/oledrgb.py
--rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.2/lbutils/typing.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils_mp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      796 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-04-14 20:23:41.000000 lbutils-mp-0.2.2/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/
+-rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.3/LICENCE
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.3/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/
+-rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.3/lbutils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.3/lbutils/abc.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/drivers/
+-rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.3/lbutils/drivers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.3/lbutils/drivers/seven_segment.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.3/lbutils/drivers/seven_segment_hex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/examples/
+-rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.3/lbutils/examples/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/graphics/
+-rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.3/lbutils/graphics/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    25143 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/graphics/canvas.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11384 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/graphics/colours.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/graphics/fonts/
+-rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/base_font.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/font06.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/font08.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/org_01.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14044 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/graphics/helpers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/helpers/
+-rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.3/lbutils/helpers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.3/lbutils/helpers/i2c.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/pmods/
+-rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.3/lbutils/pmods/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/pmods/i2c/
+-rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 20:27:40.000000 lbutils-mp-0.2.3/lbutils/pmods/i2c/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/pmods/spi/
+-rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 20:27:40.000000 lbutils-mp-0.2.3/lbutils/pmods/spi/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20877 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/pmods/spi/oledrgb.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.3/lbutils/typing.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils_mp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      796 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-04-15 10:13:32.000000 lbutils-mp-0.2.3/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/setup.cfg
```

### Comparing `lbutils-mp-0.2.2/LICENCE` & `lbutils-mp-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/PKG-INFO` & `lbutils-mp-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.2/README.md` & `lbutils-mp-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/__init__.py` & `lbutils-mp-0.2.3/lbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/abc.py` & `lbutils-mp-0.2.3/lbutils/abc.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/drivers/__init__.py` & `lbutils-mp-0.2.3/lbutils/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/drivers/seven_segment.py` & `lbutils-mp-0.2.3/lbutils/drivers/seven_segment.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/drivers/seven_segment_hex.py` & `lbutils-mp-0.2.3/lbutils/drivers/seven_segment_hex.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/examples/__init__.py` & `lbutils-mp-0.2.3/lbutils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/__init__.py` & `lbutils-mp-0.2.3/lbutils/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/canvas.py` & `lbutils-mp-0.2.3/lbutils/graphics/canvas.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,39 +134,50 @@
     Attributes
     ----------
 
     bg_colour:
          The background [`Colour`][lbutils.graphics.colours.Colour] to use when
          drawing.
     cursor:
-         The location of the current write (or read) operation.
+         The [`x`][lbutils.graphics.helpers.BoundPixel] and [`y`]
+         [lbutils.graphics.helpers.BoundPixel] locations  of the current write
+         (or read) operation.
     font:
          The sub-class of [`BaseFont`][lbutils.graphics.fonts.base_font.BaseFont]
          to use when drawing characters.
     fg_colour:
          The foreground [`Colour`][lbutils.graphics.colours.Colour] to use when
          drawing.
     pen:
          The [`Pen`][lbutils.graphics.Pen] to use when drawing on the canvas.
     height:
          A read-only value for the height of the canvas in pixels.
     width:
          A read-only value for the width of the canvas in pixels.
+    x: int
+            The X co-ordinate value of the `cursor`
+    y: int
+            The Y co-ordinate value of the `cursor`
+    x_y: int
+            A tuple representing the co-ordinate (x ,y) of the `cursor`
 
     Methods
     ----------
 
     * `draw_line()`. Draw a line from two co-ordinates.
 
     * `draw_rectangle()`. Draw a rectangle at the co-ordinate (x, y) of height
     and width, using the linecolour for the frame of the rectangle and fillcolour
     as the interior colour.
 
     * `fill_screen()`. Fill the entire `Canvas` with the background colour.
 
+    * `move_to()`. Move the internal [`cursor`]
+    [lbutils.graphics.helpers.BoundPixel]  to the co-ordinate values (x, y).
+
     * `read_pixel()`. Return the [`Colour`][lbutils.graphics.colours.Colour] of
     the specified pixel.
 
     * `write_char()`. Write a character (using the current font) starting at the
     stated pixel position.
 
     * `write_pixel()`. Set the pixel at the specified position to the foreground
@@ -214,21 +225,68 @@
         else:
             self.fg_color = graphics.color.Colour(255, 255, 255, isARM=False)
             self.bg_color = graphics.color.Colour(0, 0, 0, isARM=False)
 
         self.pen = None
 
         self.cursor = graphics.helpers.BoundPixel(
-            0, 0, min_x=0, max_x=width, min_y=0, max_y=height
+            0, 0, min_x=0, max_x=width, min_y=0, max_y=height, clip=True
         )
 
     ##
     ## Properties
     ##
 
+    @property
+    def x(self) -> int:
+        """The `x` co-ordinate of the `cursor`; checking that it lies within the
+        specified `width` of the `Canvas` when setting."""
+        return self.cursor.x
+
+    @x.setter
+    def x(self, value: int) -> None:
+        self.cursor.x = value
+
+    @property
+    def y(self) -> int:
+        """The `y` co-ordinate of the `cursor`; checking that it lies within the
+        specified `height` of the `Canvas` when setting."""
+        return self.cursor.y
+
+    @y.setter
+    def y(self, value: int) -> None:
+        self.cursor.y = value
+
+    @property
+    def x_y(self) -> tuple:
+        """Sets, or returns, the internal `x` and `y` co-ordinates of the
+        `cursor` as tuple.
+
+        When _reading_ from this property, a tuple is returned with the first
+        value of the tuple representing the `x` co-ordinate and the second
+        value of the tuple representing the `y` co-ordinate.
+
+        When _writing_ to this property the first value of the tuple represents
+        the `x` co-ordinate, and the second value of the tuple represents the `y`
+        co-ordinate. All other values in the tuple are ignored.
+
+        Raises
+        ------
+
+        ValueError:
+            If the `x` or `y` co-ordinate in the `xy` tuple cannot be converted
+            to an integer.
+        """
+        return self.cursor.x_y
+
+    @x_y.setter
+    def x_y(self, xy: tuple) -> None:
+        self.cursor.x = int(xy[0])
+        self.cursor.y = int(xy[1])
+
     ##
     ## Abstract Methods. These must be defined in sub-classes.
     ##
 
     @abstractmethod
     def read_pixel(self, x: int, y: int) -> Type[graphics.Colour]:
         """Read the colour value of the pixel at position (`x`, `y`) and return
@@ -344,60 +402,14 @@
              background colour for the fill. If not specified, use the preference
              order for the foreground and background colours of the `Canvas` to
              find suitable colours.
         filled: bool, optional
              If `True` (the default) the rectangle is filled with the background
              colour: otherwise the rectangle is not filled.
         """
-
-    @abstractmethod
-    def write_char(
-        self,
-        x: int,
-        y: int,
-        utf8Char: str,
-        fg_colour: Type[graphics.Colour] = None,
-        pen: Type[graphics.Pen] = None,
-    ) -> int:
-        """Write a `utf8Char` character (using the current `font`) starting at
-        the pixel position (`x`, `y`) in the specified `colour`.
-
-        !!! note
-             Whilst the `utf8Char` character _must_ be a valid UTF-8
-             character, most fonts only support the equivalent of the (7-bit) ASCII character
-             set. This method _will not_ display character values that cannot be supported by
-             the underlying font. See the font description for the exact values that are
-             valid for the specific font being used.
-
-        Parameters
-        ----------
-
-        x: int
-             The X co-ordinate of the pixel for the character start position.
-        y: int
-             The Y co-ordinate of the pixel for the character start position.
-        utf8Char:
-             The character to write to the display.
-        fg_colour: Type[graphics.Colour], optional
-             The [`Colour`][lbutils.graphics.Colour] to be used when drawing the
-             line. If not specified, use the preference order for the foreground
-             colour of the `Canvas` to find a suitable colour.
-        pen: Type[graphics.Pen], optional
-             The [`Pen`][lbutils.graphics.Pen] to be used when drawing the line.
-             If not specified, use the preference order for the foreground colour
-             of the `Canvas` to find a suitable colour.
-
-        Returns
-        -------
-
-        int:
-             The X pixel co-ordinate immediately following the character written
-             in the specified font. This can be used to easily locate multiple
-             characters at a given Y position: see also `write_text()`.
-        """
         pass
 
     ##
     ## Methods
     ##
 
     def select_fg_color(
@@ -528,54 +540,120 @@
             width=self.width,
             height=self.height,
             fg_colour=fill_colour,
             bg_colour=fill_colour,
             filled=True,
         )
 
+    def move_to(self, xy: tuple) -> None:
+        """Sets the internal `x` and `y` co-ordinates of the `cursor` as a
+        tuple. An alias for the `x_y` property of `Canvas`.
+
+        Parameters
+        ----------
+
+        xy: tuple
+            The first value of the `xy` tuple represents the `x` co-ordinate, and
+            the second value of the `xy` tuple represents the `y` co-ordinate.
+            All other values in the `xy` tuple are ignored.
+
+        Raises
+        ------
+
+        ValueError:
+            If the `x` or `y` co-ordinate in the `xy` tuple cannot be converted
+            to an integer.
+        """
+        self.cursor.x_y = xy
+
     def write_text(
         self,
-        x: int,
-        y: int,
         txt_str: str,
         fg_colour: Type[graphics.Colour] = None,
         pen: Type[graphics.Pen] = None,
     ) -> None:
         """Write the string `txt_str` (using the current `font`) starting at the
-        pixel position (`x`, `y`) in the specified `colour` to the display.
+        the pixel position (`x`, `y`) of the `cursor` in the specified `colour`
+        to the display.
 
         !!! note
              Whilst the `txt_str` character _must_ be a valid UTF-8 string, most
              fonts only support the equivalent of the (7-bit) ASCII character
              set. This method _will not_ display character values that cannot be
              supported by the underlying font. See the font description for the
              exact values that are valid for the specific font being used.
 
         Parameters
         ----------
 
-        x: int
-             The X co-ordinate of the pixel for the text start position.
-        y: int
-             The Y co-ordinate of the pixel for the text start position.
         txt_str:
              The string of characters to write to the display.
         fg_colour: Type[graphics.Colour], optional
              The [`Colour`][lbutils.graphics.Colour] to be used when drawing the
              line. If not specified, use the preference order for the foreground
              colour of the `Canvas` to find a suitable colour.
         pen: Type[graphics.Pen], optional
              The [`Pen`][lbutils.graphics.Pen] to be used when drawing the line.
              If not specified, use the preference order for the foreground colour
              of the `Canvas` to find a suitable colour.
         """
 
         if self.font is not None:
-            for c in txt_str:
-                x = self.write_char(x, y, c, fg_colour=fg_colour, pen=pen)
+            for character in txt_str:
+                self.write_char(
+                    character,
+                    fg_colour=fg_colour,
+                    pen=pen,
+                )
+
+    def write_char(
+        self,
+        utf8Char: str,
+        fg_colour: Type[graphics.Colour] = None,
+        pen: Type[graphics.Pen] = None,
+    ) -> None:
+        """Write a `utf8Char` character (using the current `font`) starting at
+        the pixel position (`x`, `y`) of the `cursor` in the specified `colour`.
+
+        !!! note
+            Whilst the `utf8Char` character _must_ be a valid UTF-8 character,
+            most fonts only support the equivalent of the (7-bit) ASCII character
+            set. This method _will not_ display character values that cannot be
+            supported by the underlying font. See the font description for the
+            exact values that are valid for the specific font being used.
+
+        Parameters
+        ----------
+
+        utf8Char:
+            The character to write to the display.
+        fg_colour: Type[graphics.Colour], optional
+            The [`Colour`][lbutils.graphics.Colour] to be used when drawing the
+            character. If not specified, use the preference order for the
+            foreground colour of the `Canvas` to find a suitable colour.
+        pen: Type[graphics.Pen], optional
+            The [`Pen`][lbutils.graphics.Pen] to be used when drawing the line.
+            If not specified, use the preference order for the foreground colour
+            of the `Canvas` to find a suitable colour.
+        """
+
+        fg_colour = self.select_fg_color(fg_colour=fg_colour, pen=pen)
+
+        self.font.set_position(utf8Char)
+        _offset, _width, _height, _cursor, x_off, y_off = self.font.current_glyph
+
+        for y1 in range(_height):
+            for x1 in range(_width):
+                if self.font.get_next():
+                    self.write_pixel(
+                        self.cursor.x + x1 + x_off,
+                        self.cursor.y + y1 + y_off,
+                        fg_colour,
+                    )
+        self.cursor.x += _cursor
 
 
 class FrameBufferCanvas(Canvas):
     """A [Canvas][lbutils.graphics.Canvas] backed by a [`framebuffer`](https://d
     ocs.micropython.org/en/latest/library/framebuf.html)."""
 
     pass
```

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/colours.py` & `lbutils-mp-0.2.3/lbutils/graphics/colours.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,16 +90,20 @@
     bR: int, read-only
         The byte (`0..255`) of the red component of the colour
     bG: int, read-only
         The byte (`0..255`) of the green component of the colour
     bB: int, read-only
         The byte (`0..255`) of the blue component of the colour
     as_565: int, read-only
-        Provides the colour value in the RGB565 format, using the
-        standard representation.
+        Provides the colour value in the RGB565 format, using a single
+        byte in the the standard platform representation.
+    as_888: int, read-only
+        Provides the colour value in the RGB888 format, using a
+        double word for the colour value in the standard platform
+        representation.
     isARM: bool, read-write
         Flag indicating if the colour value should use the ARM byte
         packing order in colour conversions. Defaults to `True` as
         set by the default constructor.
 
     Implementation
     --------------
@@ -144,14 +148,16 @@
         self._g = int(g)
         self._b = int(b)
 
         self.isARM = isARM
 
         # Cached values
         self._565 = None
+        self._888 = None
+
         self._bR = None
         self._bG = None
         self._bB = None
 
     ##
     ## Properties
     ##
@@ -221,14 +227,59 @@
                 )
             else:
                 self._565(self._r & 0xF8) << 8 | (self._g & 0xFC) << 3 | self._b >> 3
 
         # Return the calculated value to the client
         return self._565
 
+    @property
+    def as_888(self) -> int:
+        """
+        Construct a packed double word from the internal colour representation,
+        with 8 bits of red data, 8 bits of green, and 8 of blue. For non-ARM
+        platforms this results in a byte order for the two colour words as
+        follows
+
+        ````
+        F  E  D  C  B  A  9  8  7  6  5  4  3  2  1  0
+        R4 R3 R2 R1 R0 G5 G4 G3 G2 G1 G0 B4 B3 B2 B1 B0
+        ````
+
+        On ARM platforms the packed word representation has the high and low
+        bytes swapped in each word, and so looks like
+
+        ````
+        F  E  D  C  B  A  9  8  7  6  5  4  3  2  1  0
+        G2 G1 G0 B4 B3 B2 B1 B0 R4 R3 R2 R1 R0 G5 G4 G3
+        ````
+
+        Returns
+        -------
+
+        int:
+            A packed double word value of the colour representation.
+
+        """
+        # Check for a cached value ...
+        if self._888 is None:
+            # ... if there isn't one, calculate what the byte representation
+            #     should look like
+            if self.isARM:
+                self._888 = (
+                    (self._g & 0x1C) << 1
+                    | (self._b >> 3)
+                    | (self._r & 0xF8)
+                    | self._g >> 5
+                )
+            else:
+                self._888(self._r & 0xF8) << 8 | (self._g & 0xFC) << 3 | self._b >> 3
+
+        # Return the calculated value to the client
+        return self._888
+
 
 ###
 ### Named Colours
 ###
 
 COLOUR_BLACK = Colour(0, 0, 0)
 COLOUR_BLUE = Colour(0, 0, 255)
```

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/fonts/__init__.py` & `lbutils-mp-0.2.3/lbutils/graphics/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/fonts/base_font.py` & `lbutils-mp-0.2.3/lbutils/graphics/fonts/base_font.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/fonts/font06.py` & `lbutils-mp-0.2.3/lbutils/graphics/fonts/font06.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/fonts/font08.py` & `lbutils-mp-0.2.3/lbutils/graphics/fonts/font08.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/fonts/org_01.py` & `lbutils-mp-0.2.3/lbutils/graphics/fonts/org_01.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/graphics/helpers.py` & `lbutils-mp-0.2.3/lbutils/graphics/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,31 +124,97 @@
 
     Attributes
     ----------
 
     x: int
             The X co-ordinate value.
     y: int
-            The Y co-ordinate value
+            The Y co-ordinate value.
+    x_y: int
+            A tuple representing the co-ordinate (x ,y).
+
+    Methods
+    ----------
+
+    * `move_to()`. Move the internal co-ordinate to the value (x, y).
     """
 
-    def __init__(self, x: int, y: int):
+    ##
+    ## Constructors
+    ##
+
+    def __init__(self, x: int, y: int) -> None:
         """Creates a `Pixel` instance holding the specified `x` and `y` co-
         ordinates, together representing the Cartesian point '(`x`, `y`)'.
 
         Parameters
         ----------
 
         x: int
                 The initial X co-ordinate value.
         y: int
                 The initial Y co-ordinate value
         """
-        self.y = int(x)
-        self.x = int(y)
+        self.x = int(x)
+        self.y = int(y)
+
+    ##
+    ## Properties
+    ##
+
+    @property
+    def x_y(self) -> tuple:
+        """Sets, or returns, the internal `x` and `y` co-ordinates as a tuple.
+
+        When _reading_ from this property, a tuple is returned with the first
+        value of the tuple representing the `x` co-ordinate and the second
+        value of the tuple representing the `y` co-ordinate.
+
+        When _writing_ to this property the first value of the tuple represents
+        the `x` co-ordinate, and the second value of the tuple represents the `y`
+        co-ordinate. All other values in the tuple are ignored.
+
+        Raises
+        ------
+
+        ValueError:
+            If the `x` or `y` co-ordinate in the `xy` tuple cannot be converted
+            to an integer.
+        """
+        return [self._x, self._y]
+
+    @x_y.setter
+    def x_y(self, xy: tuple) -> None:
+        self.x = int(xy[0])
+        self.y = int(xy[1])
+
+    ##
+    ## Methods
+    ##
+
+    def move_to(self, xy: tuple) -> None:
+        """Sets the internal `x` and `y` co-ordinates as a tuple. An alias for
+        the `x_y` property.
+
+        Parameters
+        ----------
+
+        xy: tuple
+            The first value of the `xy` tuple represents the `x` co-ordinate, and
+            the second value of the `xy` tuple represents the `y` co-ordinate.
+            All other values in the `xy` tuple are ignored.
+
+        Raises
+        ------
+
+        ValueError:
+            If the `x` or `y` co-ordinate in the `xy` tuple cannot be converted
+            to an integer.
+        """
+        self.x_y = xy
 
 
 class BoundPixel(Pixel):
     """Represents a Cartesian co-ordinate between limits. Used as a convenience
     class for instances such as cursors where a relationship between a X and a Y
     co-ordinate must be maintained. This is also useful when two or more co-
     ordinates need to be tracked, or to be switched between. For instance an
@@ -181,46 +247,50 @@
     min_x: int
             The minimum value allowed for the `x` co-ordinate. Defaults to
             `0`.
     min_y: int
             The minimum value allowed for the `y` co-ordinate. Defaults to
             `0`.`
     max_x: int
-            The maximum value allowed for the `x` co-ordinate
+            The maximum value allowed for the `x` co-ordinate.
     max_y: int
-            The maximum value allowed for the `y` co-ordinate
+            The maximum value allowed for the `y` co-ordinate.
     """
 
+    ##
+    ## Constructors
+    ##
+
     def __init__(
         self,
         x: int,
         y: int,
         max_x: int,
         max_y: int,
         min_x: int = 0,
         min_y: int = 0,
         clip: bool = True,
-    ):
+    ) -> None:
         """Creates a `Pixel` instance holding the specified `x` and `y` co-
         ordinates, together representing the Cartesian point '(`x`, `y`)'. This
         `x` and `y` value is guaranteed to be maintained between `min_x` and
         `max_x` for the `x` co- ordinate, and `min_y` and `max_y` for the `y`
         co-ordinate.
 
         Parameters
         ----------
 
         x: int
                 The initial X co-ordinate value.
         y: int
-                The initial Y co-ordinate value
+                The initial Y co-ordinate value.
         max_x: int
-                The maximum value allowed for the `x` co-ordinate
+                The maximum value allowed for the `x` co-ordinate.
         max_y: int
-                The maximum value allowed for the `y` co-ordinate
+                The maximum value allowed for the `y` co-ordinate.
         min_x: int, optional
                 The minimum value allowed for the `x` co-ordinate. Defaults to
                 `0`.
         min_y: int, optional
                 The minimum value allowed for the `y` co-ordinate. Defaults to
                 `0`.`
         clip: bool, optional
@@ -242,34 +312,34 @@
                 in the common case where the lower limits for `x` and `y` are
                 `0`, and the positional parameter order is being used. If all
                 four limits are being used, consider the use of named
                 parameters to avoid ambiguity.
         """
 
         # Set-up the maximum and minimum parameters first
-        self.min_y = int(min_y)
-        self.max_y = int(max_y)
-
         self.min_x = int(min_x)
         self.max_x = int(max_x)
 
+        self.min_y = int(min_y)
+        self.max_y = int(max_y)
+
         # Now attempt to set the actual `x` and `y` inside those
         # parameters
-        self.y = int(y)
         self.x = int(x)
+        self.y = int(y)
 
         # Set the clipping switch
         self.clip = clip
 
     ##
     ## Properties
     ##
 
     @property
-    def x(self):
+    def x(self) -> int:
         """The `x` co-ordinate of the `BoundPxiel`, checking that it lies within
         the specified `min_x` and `max_x` limits.
 
         Raises
         ------
 
         `ValueError`:
@@ -286,29 +356,29 @@
 
                 return self._x
 
             else:
                 raise (ValueError("Pixel limits exceeded"))
 
     @x.setter
-    def x(self, value):
+    def x(self, value: int) -> None:
         if self.min_x <= value <= self.max_x:
             self._x = value
         else:
             if self.clip:
                 if value > self.max_x:
                     self._x = self.max_x
                 if value < self.min_x:
                     self._x = self.min_x
 
             else:
                 raise (ValueError("Pixel limits exceeded"))
 
     @property
-    def y(self):
+    def y(self) -> int:
         """The `y` co-ordinate of the `BoundPxiel`, checking that it lies within
         the specified `min_x` and `max_y` limits.
 
         Raises
         ------
 
         `ValueError`:
@@ -325,15 +395,15 @@
 
                 return self._y
 
             else:
                 raise (ValueError("Pixel limits exceeded"))
 
     @y.setter
-    def y(self, value):
+    def y(self, value: int) -> None:
         if self.min_y <= value <= self.max_y:
             self._y = value
         else:
             if self.clip:
                 if value > self.max_y:
                     self._y = self.max_y
                 if value < self.min_y:
```

### Comparing `lbutils-mp-0.2.2/lbutils/helpers/__init__.py` & `lbutils-mp-0.2.3/lbutils/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/helpers/i2c.py` & `lbutils-mp-0.2.3/lbutils/helpers/i2c.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/pmods/__init__.py` & `lbutils-mp-0.2.3/lbutils/pmods/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/pmods/i2c/__init__.py` & `lbutils-mp-0.2.3/lbutils/pmods/i2c/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/pmods/spi/__init__.py` & `lbutils-mp-0.2.3/lbutils/pmods/spi/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils/pmods/spi/oledrgb.py` & `lbutils-mp-0.2.3/lbutils/pmods/spi/oledrgb.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,19 +72,19 @@
 # Import the typing hints if available. Use our backup version
 # if the offical library is missing
 try:
     from typing import Type
 except ImportError:
     from lbutils.typing import Type
 
-# Import the lbutils graphics library
-try:
+    # Import the lbutils graphics library
+    # try:
     import lbutils.graphics as graphics
-except ImportError:
-    raise RuntimeError("Error: Missing required LBUtils graphics library")
+# except ImportError:
+#    raise RuntimeError("Error: Missing required LBUtils graphics library")
 
 # Import the core libraries
 import ustruct
 import utime
 
 # Allow the use of MicroPython constants
 from micropython import const
@@ -577,72 +577,7 @@
 
     def reset(self) -> None:
         """Resets the display, clearing the current contents."""
         if self.reset_pin is not None:
             self.reset_pin.value(0)
             utime.sleep(0.1)
             self.reset_pin.value(1)
-
-    def write_char(
-        self,
-        x: int,
-        y: int,
-        utf8Char: str,
-        fg_colour: Type[graphics.Colour] = None,
-        pen: Type[graphics.Pen] = None,
-    ) -> int:
-        """Write a `utf8Char` character (using the current `font`) starting at
-        the pixel position (`x`, `y`) in the specified `colour`.
-
-        !!! note
-            Whilst the `utf8Char` character _must_ be a valid UTF-8 character,
-            most fonts only support the equivalent of the (7-bit) ASCII character
-            set. This method _will not_ display character values that cannot be
-            supported by the underlying font. See the font description for the
-            exact values that are valid for the specific font being used.
-
-        Parameters
-        ----------
-
-        x: int
-            The X co-ordinate of the pixel for the character start position.
-        y: int
-            The Y co-ordinate of the pixel for the character start position.
-        utf8Char:
-            The character to write to the display.
-        fg_colour: Type[graphics.Colour], optional
-            The [`Colour`][lbutils.graphics.Colour] to be used when drawing the
-            character. If not specified, use the preference order for the
-            foreground colour of the `Canvas` to find a suitable colour.
-        pen: Type[graphics.Pen], optional
-            The [`Pen`][lbutils.graphics.Pen] to be used when drawing the line.
-            If not specified, use the preference order for the foreground colour
-            of the `Canvas` to find a suitable colour.
-
-        Returns
-        -------
-
-        int:
-            The X pixel co-ordinate immediately following the character written
-            in the specified font. This can be used to easily locate multiple
-            characters at a given Y position: see also `write_text()`.
-        """
-
-        fg_colour = self.select_fg_color(fg_colour=fg_colour, pen=pen)
-
-        # print("write_char(x={},y={},c={},colour={})".format(x,y,utf8Char,colour))
-        if self.font is None:
-            return x
-        # {offset, width, height, advance cursor, x offset, y offset} */
-        self.font.set_position(utf8Char)
-        _offset, _width, _height, _cursor, x_off, y_off = self.font.current_glyph
-        # print("_offset",_offset)
-        # print("Width",_width)
-        # print("height",_height)
-        # print("cursor",_cursor)
-        # print("xoff",x_off)
-        # print("yoff",y_off)
-        for y1 in range(_height):
-            for x1 in range(_width):
-                if self.font.get_next():
-                    self.write_pixel(x + x1 + x_off, y + y1 + y_off, fg_colour)
-        return x + _cursor
```

### Comparing `lbutils-mp-0.2.2/lbutils/typing.py` & `lbutils-mp-0.2.3/lbutils/typing.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/lbutils_mp.egg-info/PKG-INFO` & `lbutils-mp-0.2.3/lbutils_mp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.2/lbutils_mp.egg-info/SOURCES.txt` & `lbutils-mp-0.2.3/lbutils_mp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.2/pyproject.toml` & `lbutils-mp-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lbutils-mp"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="David Love", email="david.love@leedsbeckett.ac.uk" },
 ]
 description = "Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers"
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
```

