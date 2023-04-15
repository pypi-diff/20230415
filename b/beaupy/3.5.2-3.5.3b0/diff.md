# Comparing `tmp/beaupy-3.5.2.tar.gz` & `tmp/beaupy-3.5.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaupy-3.5.2.tar", max compression
+gzip compressed data, was "beaupy-3.5.3b0.tar", max compression
```

## Comparing `beaupy-3.5.2.tar` & `beaupy-3.5.3b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1111 2023-03-29 11:23:12.949505 beaupy-3.5.2/LICENSE
--rw-r--r--   0        0        0     8118 2023-03-29 11:23:12.949505 beaupy-3.5.2/README.md
--rw-r--r--   0        0        0      260 2023-03-29 11:23:12.949505 beaupy-3.5.2/beaupy/__init__.py
--rwxr-xr-x   0        0        0    23689 2023-03-29 11:23:12.949505 beaupy-3.5.2/beaupy/_beaupy.py
--rw-r--r--   0        0        0     3500 2023-03-29 11:23:12.949505 beaupy-3.5.2/beaupy/_internals.py
--rw-r--r--   0        0        0      170 2023-03-29 11:23:12.949505 beaupy-3.5.2/beaupy/spinners/__init__.py
--rw-r--r--   0        0        0     2335 2023-03-29 11:23:12.949505 beaupy-3.5.2/beaupy/spinners/_spinners.py
--rw-r--r--   0        0        0     3662 2023-03-29 11:23:12.953505 beaupy-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     9166 1970-01-01 00:00:00.000000 beaupy-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/LICENSE
+-rw-r--r--   0        0        0     8118 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/README.md
+-rw-r--r--   0        0        0      260 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/__init__.py
+-rwxr-xr-x   0        0        0    23689 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/_beaupy.py
+-rw-r--r--   0        0        0     4059 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/_internals.py
+-rw-r--r--   0        0        0      170 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/spinners/__init__.py
+-rw-r--r--   0        0        0     2335 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/spinners/_spinners.py
+-rw-r--r--   0        0        0     3664 2023-04-15 15:17:25.867836 beaupy-3.5.3b0/pyproject.toml
+-rw-r--r--   0        0        0     9168 1970-01-01 00:00:00.000000 beaupy-3.5.3b0/PKG-INFO
```

### Comparing `beaupy-3.5.2/LICENSE` & `beaupy-3.5.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.2/README.md` & `beaupy-3.5.3b0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 - For user input from console, `beaupy` relies on [petereon/yakh](https://github.com/petereon/yakh), which is tested against all the major platforms and Python versions.
 - For printing to console `beaupy` relies on [Textualize/rich](https://github.com/Textualize/rich), which [claims to support](https://github.com/Textualize/rich#compatibility) all the major platforms.
 
 ## Known Issues
 
 - Version `2.x.x`: arrow keys reportedly don't always work on Windows. Resolved in `3.x.x`
-- Version `3.5.0`: only first 5 options are displayed for `select` and `select_multiple`. Resolved in `3.5.1`
+- Version `3.5.0`: only first 5 options are displayed for `select` and `select_multiple`. Resolved in `3.5.2`
 
 ## Awesome projects using `beaupy`
 
 - [therealOri/Genter](https://github.com/therealOri/Genter): A strong password generator and built in password manager made with python3!
 - [therealOri/byte](https://github.com/therealOri/byte): Steganography Image/Data Injector. For artists or people to inject their own Datamark "Watermark" into their images/art or files!
 
 ## License
```

### Comparing `beaupy-3.5.2/beaupy/_beaupy.py` & `beaupy-3.5.3b0/beaupy/_beaupy.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.2/beaupy/_internals.py` & `beaupy-3.5.3b0/beaupy/_internals.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import re
 from ast import literal_eval
 from contextlib import contextmanager
 from typing import Any, Callable, Iterator, List, Type, Union
 
 import emoji
 from rich.console import Console, ConsoleRenderable
 from rich.live import Live
+from rich.style import Style
 from yakh.key import Key
 
 TargetType = Any
 
 
 class ValidationError(Exception):
     pass
@@ -32,22 +34,34 @@
 
 def _format_option_select(i: int, cursor_index: int, option: str, cursor_style: str, cursor: str) -> str:
     return '{}{}'.format(
         f'[{cursor_style}]{cursor}[/{cursor_style}] ' if i == cursor_index else ' ' * (len(_replace_emojis(cursor)) + 1), option
     )
 
 
+def _wrap_style(string_w_styles: str, global_style_str: str) -> str:
+    RE_STYLE_PATTERN = r'\[(.*?)\]'
+
+    global_style = Style.parse(global_style_str)
+    style_strings = list(set([i.replace('/', '') for i in re.findall(RE_STYLE_PATTERN, string_w_styles)]))
+    for style_string in style_strings:
+        style = Style.combine([Style.parse(style_string), global_style])
+        string_w_styles = string_w_styles.replace(f'{style_string}', f'{style}')
+
+    return f'[{global_style_str}]{string_w_styles}[/{global_style_str}]'
+
+
 def _render_option_select_multiple(
     option: str, ticked: bool, tick_character: str, tick_style: str, selected: bool, cursor_style: str
 ) -> str:
     prefix = '\[{}]'.format(' ' * len(_replace_emojis(tick_character)))  # noqa: W605
     if ticked:
         prefix = f'\[[{tick_style}]{tick_character}[/{tick_style}]]'  # noqa: W605
     if selected:
-        option = f'[{cursor_style}]{option}[/{cursor_style}]'
+        option = _wrap_style(option, cursor_style)
     return f'{prefix} {option}'
 
 
 def _update_rendered(live: Live, renderable: Union[ConsoleRenderable, str]) -> None:
     live.update(renderable=renderable)
     live.refresh()
```

### Comparing `beaupy-3.5.2/beaupy/spinners/_spinners.py` & `beaupy-3.5.3b0/beaupy/spinners/_spinners.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.2/pyproject.toml` & `beaupy-3.5.3b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'beaupy'
-version = '3.5.2'
+version = '3.5.3b0'
 description = 'A library of elements for interactive TUIs in Python'
 authors = ['Peter Vyboch <pvyboch1@gmail.com>']
 license = 'MIT'
 repository = 'https://github.com/petereon/beaupy'
 readme = 'README.md'
 keywords = ["cli", "interactive", "console", "terminal", "interface"]
 classifiers = [
```

### Comparing `beaupy-3.5.2/PKG-INFO` & `beaupy-3.5.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaupy
-Version: 3.5.2
+Version: 3.5.3b0
 Summary: A library of elements for interactive TUIs in Python
 Home-page: https://github.com/petereon/beaupy
 License: MIT
 Keywords: cli,interactive,console,terminal,interface
 Author: Peter Vyboch
 Author-email: pvyboch1@gmail.com
 Requires-Python: >=3.7.8,<4.0.0
@@ -214,15 +214,15 @@
 
 - For user input from console, `beaupy` relies on [petereon/yakh](https://github.com/petereon/yakh), which is tested against all the major platforms and Python versions.
 - For printing to console `beaupy` relies on [Textualize/rich](https://github.com/Textualize/rich), which [claims to support](https://github.com/Textualize/rich#compatibility) all the major platforms.
 
 ## Known Issues
 
 - Version `2.x.x`: arrow keys reportedly don't always work on Windows. Resolved in `3.x.x`
-- Version `3.5.0`: only first 5 options are displayed for `select` and `select_multiple`. Resolved in `3.5.1`
+- Version `3.5.0`: only first 5 options are displayed for `select` and `select_multiple`. Resolved in `3.5.2`
 
 ## Awesome projects using `beaupy`
 
 - [therealOri/Genter](https://github.com/therealOri/Genter): A strong password generator and built in password manager made with python3!
 - [therealOri/byte](https://github.com/therealOri/byte): Steganography Image/Data Injector. For artists or people to inject their own Datamark "Watermark" into their images/art or files!
 
 ## License
```

