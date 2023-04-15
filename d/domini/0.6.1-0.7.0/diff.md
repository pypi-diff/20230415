# Comparing `tmp/domini-0.6.1.tar.gz` & `tmp/domini-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domini-0.6.1.tar", max compression
+gzip compressed data, was "domini-0.7.0.tar", max compression
```

## Comparing `domini-0.6.1.tar` & `domini-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.6.1/LICENSE
--rw-r--r--   0        0        0     1409 2023-03-28 00:04:40.084130 domini-0.6.1/README.md
--rw-r--r--   0        0        0       21 2022-09-29 19:43:33.949294 domini-0.6.1/domini/__init__.py
--rw-r--r--   0        0        0    16344 2023-03-28 22:13:06.189173 domini-0.6.1/domini/html.py
--rw-r--r--   0        0        0      418 2023-03-28 22:11:42.640823 domini-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2038 1970-01-01 00:00:00.000000 domini-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1411 2023-04-15 00:45:13.796552 domini-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.7.0/domini/__init__.py
+-rw-r--r--   0        0        0    16388 2023-04-15 00:38:47.966969 domini-0.7.0/domini/html.py
+-rw-r--r--   0        0        0      418 2023-04-15 00:42:22.126370 domini-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 domini-0.7.0/PKG-INFO
```

### Comparing `domini-0.6.1/LICENSE` & `domini-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domini-0.6.1/README.md` & `domini-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 **NOTE**: `add` does add them to the current object. `>` returns a new, identical element with those children added.
 
 ```py
 ul(class_='todo')> (
     li()> 'Buy a fruit basket.',
     li()> (
-        'Read', a(href='https://wikipedia.org/')> 'Wikipedia',
-        'to learn more about things you may have not otherwise cared about.',
+        'Read ', a(href='https://wikipedia.org/')> 'Wikipedia',
+        ' to learn more about things you may have not otherwise cared about.',
     ),
 )
 ```
 
 ## Closing tags
 
 A tag is only closed if content is provided. E.g. `<p></p>` as opposed to `<p>`. This can be an empty tuple.
```

### Comparing `domini-0.6.1/domini/html.py` & `domini-0.7.0/domini/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 from contextlib import suppress
-from typing import Any, Sequence, Iterator, Generator
+from typing import Any, Sequence, Iterator, Generator, Union
 
 
 def conform_attribute_name(key: str) -> str:
     """
     Format an attribute name to fit the standard.
     """
     key = key.strip('_')
@@ -69,14 +69,17 @@
     # Close tag off if content is provided
     if content is not None:
         return f'{elm}>{content}</{tag}>'
     else:
         return f'{elm}>'
 
 
+Content = Union[str, 'HTMLTag', Sequence, Iterator, Generator]
+
+
 class HTMLTag:
     """
     Base class for all HTML tags
 
     Inherit from it to define a new tag type.
     Ex. `class landscape(HTMLTag): ...`
     """
@@ -97,40 +100,40 @@
         cls.tag = cls.__name__
 
         # Strip appended underscore from tag
         if cls.tag.endswith('_'):
             cls.tag = cls.tag[:-1]
 
     def __str__(self) -> str:
-        return self.render(pretty=True)
+        return self.render(pretty=False)
 
-    def __gt__(self, elements: str | HTMLTag | Sequence | Iterator | Generator, /) -> HTMLTag:
+    def __gt__(self, content: Content, /) -> HTMLTag:
         """
         Return a copy with the children added.
         """
 
         # Create a copy of the element
         copy = type(self)(*self.attrs, **self.kwattrs)
         
         if self.children is not None:
             copy.add(self.children)
 
         # Add children
 
         # o) Strings and HTML tags are obviously singular
-        if isinstance(elements, (str, HTMLTag)):
-            return copy.add(elements)
+        if isinstance(content, (str, HTMLTag)):
+            return copy.add(content)
         
         # o) Any other sequence, iterator, or generator
         # should be unravelled and have its elements added
-        if isinstance(elements, (Sequence, Iterator, Generator)):
-            return copy.add(*elements)
+        if isinstance(content, (Sequence, Iterator, Generator)):
+            return copy.add(*content)
         
         # o) Anything else, add it singularly
-        return copy.add(elements)
+        return copy.add(content)
 
     def __contains__(self, attribute: str, /) -> bool:
         """
         Get whether tag has attribute.
         """
         return attribute in self.attrs \
             or attribute in self.kwattrs
@@ -209,19 +212,21 @@
         children = []
         for child in self.children:
             if isinstance(child, HTMLTag):
                 children.append(child.render(pretty=False))
             else:
                 children.append(child)
 
-        content = " ".join(map(str, children))
+        content = "".join(map(str, children))
         return render_html_element(self.tag, content, *self.attrs, **self.kwattrs)
 
     def add(self, *elements: HTMLTag | str) -> HTMLTag:
-        """Add children."""
+        """
+        Add children.
+        """
         if self.children is None:
             self.children = []
         self.children.extend(elements)
         return self
```

### Comparing `domini-0.6.1/PKG-INFO` & `domini-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domini
-Version: 0.6.1
+Version: 0.7.0
 Summary: Create HTML documents using Pythonic syntax that mimics the real deal.
 Home-page: https://gitlab.com/deepadmax/domini
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -47,16 +47,16 @@
 
 **NOTE**: `add` does add them to the current object. `>` returns a new, identical element with those children added.
 
 ```py
 ul(class_='todo')> (
     li()> 'Buy a fruit basket.',
     li()> (
-        'Read', a(href='https://wikipedia.org/')> 'Wikipedia',
-        'to learn more about things you may have not otherwise cared about.',
+        'Read ', a(href='https://wikipedia.org/')> 'Wikipedia',
+        ' to learn more about things you may have not otherwise cared about.',
     ),
 )
 ```
 
 ## Closing tags
 
 A tag is only closed if content is provided. E.g. `<p></p>` as opposed to `<p>`. This can be an empty tuple.
```

