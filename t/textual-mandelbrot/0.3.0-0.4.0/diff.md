# Comparing `tmp/textual_mandelbrot-0.3.0-py3-none-any.whl.zip` & `tmp/textual_mandelbrot-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 8822 bytes, number of entries: 9
--rw-r--r--  2.0 unx      806 b- defN 23-Apr-03 20:58 textual_mandelbrot/__init__.py
--rw-r--r--  2.0 unx     4669 b- defN 23-Apr-03 20:58 textual_mandelbrot/__main__.py
--rw-r--r--  2.0 unx     2162 b- defN 23-Apr-03 20:58 textual_mandelbrot/colouring.py
--rw-r--r--  2.0 unx    12498 b- defN 23-Apr-03 20:58 textual_mandelbrot/mandelbrot.py
--rw-r--r--  2.0 unx     4203 b- defN 23-Apr-03 20:58 textual_mandelbrot-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 20:58 textual_mandelbrot-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-03 20:58 textual_mandelbrot-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-03 20:58 textual_mandelbrot-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      799 b- defN 23-Apr-03 20:58 textual_mandelbrot-0.3.0.dist-info/RECORD
-9 files, 25311 bytes uncompressed, 7424 bytes compressed:  70.7%
+-rw-r--r--  2.0 unx      806 b- defN 23-Apr-15 07:41 textual_mandelbrot/__init__.py
+-rw-r--r--  2.0 unx     4790 b- defN 23-Apr-15 07:41 textual_mandelbrot/__main__.py
+-rw-r--r--  2.0 unx     2162 b- defN 23-Apr-03 21:37 textual_mandelbrot/colouring.py
+-rw-r--r--  2.0 unx    12575 b- defN 23-Apr-15 07:41 textual_mandelbrot/mandelbrot.py
+-rw-r--r--  2.0 unx     4203 b- defN 23-Apr-15 07:41 textual_mandelbrot-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 07:41 textual_mandelbrot-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Apr-15 07:41 textual_mandelbrot-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-15 07:41 textual_mandelbrot-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      799 b- defN 23-Apr-15 07:41 textual_mandelbrot-0.4.0.dist-info/RECORD
+9 files, 25509 bytes uncompressed, 7424 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: textual_mandelbrot/colouring.py
 Comment: 
 
 Filename: textual_mandelbrot/mandelbrot.py
 Comment: 
 
-Filename: textual_mandelbrot-0.3.0.dist-info/METADATA
+Filename: textual_mandelbrot-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: textual_mandelbrot-0.3.0.dist-info/WHEEL
+Filename: textual_mandelbrot-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: textual_mandelbrot-0.3.0.dist-info/entry_points.txt
+Filename: textual_mandelbrot-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: textual_mandelbrot-0.3.0.dist-info/top_level.txt
+Filename: textual_mandelbrot-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_mandelbrot-0.3.0.dist-info/RECORD
+Filename: textual_mandelbrot-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_mandelbrot/__init__.py

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.3.0"
+__version__    = "0.4.0"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
 from .mandelbrot import Mandelbrot
 from .colouring  import default_map, blue_brown_map, shades_of_green
```

## textual_mandelbrot/__main__.py

```diff
@@ -97,18 +97,22 @@
     def on_mandelbrot_changed( self, event: Mandelbrot.Changed ) -> None:
         """Handle the parameters of the Mandelbrot being changed.
 
         Args:
             event: The event with the change details.
         """
         plot                 = self.query_one( Mandelbrot )
-        plot.border_title    = f"{event.from_x:.10f}, {event.from_y:.10f} -> {event.to_x:.10f}, {event.to_y:.10f}"
+        plot.border_title    = (
+            f"{event.mandelbrot.from_x:.10f}, {event.mandelbrot.from_y:.10f}"
+            " -> "
+            f"{event.mandelbrot.to_x:.10f}, {event.mandelbrot.to_y:.10f}"
+        )
         plot.border_subtitle = (
-            f"{event.multibrot:0.2f} multibrot | "
-            f"{event.max_iteration:0.2f} iterations | "
+            f"{event.mandelbrot.multibrot:0.2f} multibrot | "
+            f"{event.mandelbrot.max_iteration:0.2f} iterations | "
             f"{event.elapsed:0.4f} seconds"
         )
 
     def action_colour( self, colour: int ) -> None:
         """Set a colour scheme for the plot.
 
         Args:
```

## textual_mandelbrot/mandelbrot.py

```diff
@@ -1,35 +1,33 @@
 """Provides a Textual widget for plotting a Mandelbrot set."""
 
 ##############################################################################
 # Python imports.
 from __future__        import annotations
 from decimal           import Decimal
 from operator          import mul, truediv
-from functools         import lru_cache
 from time              import monotonic
 from typing            import Iterator, Callable
 from typing_extensions import Self
 
 ##############################################################################
 # Textual imports.
-from textual.binding  import Binding
-from textual.color    import Color
-from textual.message  import Message
+from textual.binding import Binding
+from textual.color   import Color
+from textual.message import Message
 
 ##############################################################################
 # Textual-canvas imports.
 from textual_canvas import Canvas
 
 ##############################################################################
 # Local imports.
 from .colouring import default_map
 
 ##############################################################################
-@lru_cache()
 def _mandelbrot( x: Decimal, y: Decimal, multibrot: float, max_iteration: int ) -> int:
     """Return the Mandelbrot calculation for the point.
 
     Args:
         x: The x location of the point to calculate.
         y: The y location of the point to calculate.
         multibrot: The 'multibrot' value to use in the calculation.
@@ -146,26 +144,14 @@
             Args:
                 mandelbrot: The Mandelbrot causing the message.
                 elapsed: The time elapsed while calculating the plot.
             """
             super().__init__()
             self.mandelbrot: Mandelbrot = mandelbrot
             """The Mandelbrot widget that caused the event."""
-            self.multibrot: Decimal = mandelbrot._multibrot
-            """The 'multibrot' value."""
-            self.from_x: Decimal = mandelbrot._from_x
-            """Start X position for the plot."""
-            self.to_x: Decimal = mandelbrot._to_x
-            """End X position for the plot."""
-            self.from_y: Decimal = mandelbrot._from_y
-            """Start Y position for the plot."""
-            self.to_y: Decimal = mandelbrot._to_y
-            """End Y position for the plot."""
-            self.max_iteration = mandelbrot._max_iteration
-            "Maximum number of iterations to perform."
             self.elapsed = elapsed
             """The time that elapsed during the drawing of the current view."""
 
     def __init__(
         self,
         width: int,
         height: int,
@@ -184,28 +170,58 @@
             name: The name of the Mandelbrot widget.
             id: The ID of the Mandelbrot widget in the DOM.
             classes: The CSS classes of the Mandelbrot widget.
             disabled: Whether the Mandelbrot widget is disabled or not.
         """
         super().__init__( width, height, name=name, id=id, classes=classes, disabled=disabled )
         self._max_iteration: int = 80
-        "Maximum number of iterations to perform."
+        """Maximum number of iterations to perform."""
         self._multibrot: Decimal = Decimal( 2.0 )
         """The 'multibrot' value."""
         self._from_x: Decimal = Decimal( -2.5 )
         """Start X position for the plot."""
         self._to_x: Decimal = Decimal( 1.5 )
         """End X position for the plot."""
         self._from_y: Decimal = Decimal( -1.5 )
         """Start Y position for the plot."""
         self._to_y: Decimal = Decimal( 1.5 )
         """End Y position for the plot."""
         self._colour_source = colour_source
         """Source of colour for the plot."""
 
+    @property
+    def max_iteration( self ) -> int:
+        """Maximum number of iterations to perform."""
+        return self._max_iteration
+
+    @property
+    def multibrot( self ) -> Decimal:
+        """The 'multibrot' value."""
+        return self._multibrot
+
+    @property
+    def from_x( self ) -> Decimal:
+        """Start X position for the plot."""
+        return self._from_x
+
+    @property
+    def to_x( self ) -> Decimal:
+        """End X position for the plot."""
+        return self._to_x
+
+    @property
+    def from_y( self ) -> Decimal:
+        """Start Y position for the plot."""
+        return self._from_y
+
+    @property
+    def to_y( self ) -> Decimal:
+        """End Y position for the plot."""
+        return self._to_y
+
     def reset( self ) -> Self:
         """Reset the plot.
 
         Returns:
             Self.
         """
         self._max_iteration = 80
```

## Comparing `textual_mandelbrot-0.3.0.dist-info/METADATA` & `textual_mandelbrot-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-mandelbrot
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple Mandelbrot explorer for the terminal.
 Home-page: https://github.com/davep/textual-mandelbrot
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: textual (>=0.17.0)
+Requires-Dist: textual (>=0.19.1)
 Requires-Dist: textual-canvas
 
 # textual-mandelbrot
 
 ![mandelexp in action](https://raw.githubusercontent.com/davep/textual-mandelbrot/main/img/mandelexp01.png)
 ![mandelexp in action](https://raw.githubusercontent.com/davep/textual-mandelbrot/main/img/mandelexp02.png)
```

