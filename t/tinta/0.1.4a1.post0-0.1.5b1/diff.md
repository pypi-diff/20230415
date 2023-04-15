# Comparing `tmp/tinta-0.1.4a1.post0.tar.gz` & `tmp/tinta-0.1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinta-0.1.4a1.post0.tar", last modified: Wed Jun 29 08:09:48 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `tinta-0.1.4a1.post0.tar` & `tinta-0.1.5b1.tar`

### file list

```diff
@@ -1,19 +1,35 @@
-drwxr-xr-x   0 brandon    (501) staff       (20)        0 2022-06-29 08:09:48.864662 tinta-0.1.4a1.post0/
--rw-r--r--   0 brandon    (501) staff       (20)     1081 2022-06-29 06:33:27.000000 tinta-0.1.4a1.post0/LICENSE
--rw-r--r--   0 brandon    (501) staff       (20)       24 2022-06-29 06:33:27.000000 tinta-0.1.4a1.post0/MANIFEST.in
--rw-r--r--   0 brandon    (501) staff       (20)    12082 2022-06-29 08:09:48.864356 tinta-0.1.4a1.post0/PKG-INFO
--rw-r--r--   0 brandon    (501) staff       (20)     9192 2022-06-29 06:42:16.000000 tinta-0.1.4a1.post0/README.md
--rw-r--r--   0 brandon    (501) staff       (20)       38 2022-06-29 08:09:48.864724 tinta-0.1.4a1.post0/setup.cfg
--rw-r--r--   0 brandon    (501) staff       (20)     2057 2022-06-29 06:50:46.000000 tinta-0.1.4a1.post0/setup.py
-drwxr-xr-x   0 brandon    (501) staff       (20)        0 2022-06-29 08:09:48.862842 tinta-0.1.4a1.post0/tinta/
--rw-r--r--   0 brandon    (501) staff       (20)     1043 2022-06-29 06:42:26.000000 tinta-0.1.4a1.post0/tinta/__init__.py
--rw-r--r--   0 brandon    (501) staff       (20)      891 2022-06-29 06:33:27.000000 tinta-0.1.4a1.post0/tinta/__main__.py
--rw-r--r--   0 brandon    (501) staff       (20)      329 2022-06-29 06:33:27.000000 tinta-0.1.4a1.post0/tinta/colors.ini
--rw-r--r--   0 brandon    (501) staff       (20)    13962 2022-06-29 06:40:30.000000 tinta-0.1.4a1.post0/tinta/tinta.py
-drwxr-xr-x   0 brandon    (501) staff       (20)        0 2022-06-29 08:09:48.863549 tinta-0.1.4a1.post0/tinta.egg-info/
--rw-r--r--   0 brandon    (501) staff       (20)    12082 2022-06-29 08:09:48.000000 tinta-0.1.4a1.post0/tinta.egg-info/PKG-INFO
--rw-r--r--   0 brandon    (501) staff       (20)      278 2022-06-29 08:09:48.000000 tinta-0.1.4a1.post0/tinta.egg-info/SOURCES.txt
--rw-r--r--   0 brandon    (501) staff       (20)        1 2022-06-29 08:09:48.000000 tinta-0.1.4a1.post0/tinta.egg-info/dependency_links.txt
--rw-r--r--   0 brandon    (501) staff       (20)        1 2022-06-29 06:52:58.000000 tinta-0.1.4a1.post0/tinta.egg-info/not-zip-safe
--rw-r--r--   0 brandon    (501) staff       (20)       11 2022-06-29 08:09:48.000000 tinta-0.1.4a1.post0/tinta.egg-info/requires.txt
--rw-r--r--   0 brandon    (501) staff       (20)        6 2022-06-29 08:09:48.000000 tinta-0.1.4a1.post0/tinta.egg-info/top_level.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.5b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.5b1/DESCRIPTION.rst
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.5b1/MANIFEST.in
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 tinta-0.1.5b1/Pipfile
+-rw-r--r--   0        0        0    24383 2020-02-02 00:00:00.000000 tinta-0.1.5b1/Pipfile.lock
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 tinta-0.1.5b1/license.md
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 tinta-0.1.5b1/publish.sh
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinta-0.1.5b1/pytest.ini
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tinta-0.1.5b1/requirements.txt
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 tinta-0.1.5b1/setup.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.vscode/launch.json
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.vscode/settings.json
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.vscode/tasks.json
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 tinta-0.1.5b1/examples/basic_usage.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.5b1/examples/colors.ini
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.5b1/examples/tinta-discover.png
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tests/conftest.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tests/launch.json
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tests/test_discover.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tests/test_tinta.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tinta/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tinta/__main__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tinta/colors.ini
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tinta/discover.py
+-rw-r--r--   0        0        0    14170 2020-02-02 00:00:00.000000 tinta-0.1.5b1/tinta/tinta.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 tinta-0.1.5b1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.5b1/LICENSE
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 tinta-0.1.5b1/README.md
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 tinta-0.1.5b1/pyproject.toml
+-rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 tinta-0.1.5b1/PKG-INFO
```

### Comparing `tinta-0.1.4a1.post0/LICENSE` & `tinta-0.1.5b1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 github.com/brandonscript
+Copyright (c) 2023 github.com/brandonscript
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tinta-0.1.4a1.post0/README.md` & `tinta-0.1.5b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png">
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.4--alpha-green.svg) [![Build Status](https://travis-ci.com/brandonscript/tinta.svg?branch=main)](https://travis-ci.com/brandonscript/tinta) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=brandonscript/tinta&amp;utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) [![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs) [![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.5--beta-green.svg) [![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)](https://github.com/brandonscript/tinta/actions) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=brandonscript/tinta&amp;utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 Tinta takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -59,42 +59,51 @@
 
 Install Tinta:
 
 ```bash
 pip install tinta
 ```
 
+(Or visit https://pypi.org/project/tinta/)
+
 Add Tinta to your project, and optionally configure a path to your `colors.ini` file. This path can be relative, or absolute; the best way to make a path is using `pathlib.Path()`.
 
 ```python
 from tinta import Tinta
 
 # or to specify your custom colors,
 # relative to your project's cwd:
 
 from pathlib import Path
 from tinta import Tinta
 Tinta.load_colors(Path().cwd() / 'config/colors.ini')
 ```
 
-To discover what colors are available on your console:
+You can use `Tinta.discover()` to discover what colors are available on your console.
 
 ```python
 Tinta.discover()
+# or 
+Tinta.discover(background=True)
 ```
 
+<img src="https://github.com/brandonscript/tinta/blob/main/examples/tinta-discover.png?raw=true" style="max-width: 540px; !important" width="540" alt="Tinta.discover() output, a set of ansi color-coded numbers in the terminal" />
+
 An example `colors.ini` file might look like:
 
 ```ini
 # A list of ansi colors for your console.
 green: 35
 red: 1
 blue: 32
 yellow: 214
 ```
+
+(Or modify the Tinta colors.ini from [here](https://github.com/brandonscript/tinta/blob/main/tinta/colors.ini))
+
 ## API Reference
 
 ### Tinta (+ color methods)
 
 #### Dynamic methods
 
 These methods are loaded dynamically from your `colors.ini` file:
@@ -141,14 +150,15 @@
  - `line() -> self` – Appends the contents preceded by a newline char (`\n`).
  - `bold() -> self` – Sets segments to bold.
  - `underline() -> self` – Sets segments to underline.
  - `dim() -> self` – Sets segments to a darker, dimmed color.
  - `code() -> self` – Adds segments using the specified ansi code.
  - `normal() -> self` – Resets the style to default.
  - `reset() -> self` – Resets both style and color to default.
+ - `discover()` – Prints a list of available colors to the console.
 
 All style methods support the same arguments as `Tinta` and dynamic color methods:
 
 ```python
 Tinta().underline('Underlined', 'text').print()
 Tinta().bold('Bold', 'text', sep='+').print()
 Tinta().dim('Dimmed', 'text', sep='_').print()
@@ -229,20 +239,15 @@
 
 
 ## Running Tests
 
 To run tests, run the following command:
 
 ```bash
-pip install -r requirements-text.txt
-```
-
-then simply:
-
-```bash
+pip install pytest
 python -m pytest -xv
 ```
 
 ## Contributing
 
 Contributions are welcome! Please send in a PR with a clear explanation of what you're adding and why, and where applicable, add tests to validate. Please read our [code of conduct](CODE_OF_CONDUCT.md) before contributing.
```

### Comparing `tinta-0.1.4a1.post0/setup.py` & `tinta-0.1.5b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 
+"""
 # Tinta
-# Copyright 2021 github.com/brandoncript
+# Copyright 2023 github.com/brandoncript
 
 # This program is bound to the Hippocratic License 2.1
 # Full text is available here:
 # https://firstdonoharm.dev/version/2/1/license
 
 # Further to adherence to the Hippocratic Licenese, permission is hereby
 # granted, free of charge, to any person obtaining a copy of this software
@@ -14,41 +15,44 @@
 # limitation the rights to use, copy, modify, merge, publish, distribute,
 # sublicense, and / or sell copies of the Software, and to permit persons
 # to whom the Software is furnished to do so, subject to the conditions layed
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
+"""
 
-from setuptools import setup
 from pathlib import Path
 
-with Path('README.md').open() as f:
+from setuptools import setup
+
+with Path('README.md').open(encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='tinta',
-      version='0.1.4a1-0',
-      description='Tinta, the a magical console output tool.',
+      version='0.1.5b1',
+      description='Tinta, a magical console output tool.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/brandonscript/tinta',
       author='Brandon Shelley',
       author_email='brandon@pacificaviator.co',
       install_requires=['ansicolors'],
       include_package_data=True,
       license='MIT',
       packages=['tinta'],
       keywords='console colors ansi print terminal development',
       python_requires='>=3.6',
       classifiers=[
-          'Development Status :: 3 - Alpha',
+          'Development Status :: 4 - Beta',
           'Intended Audience :: Developers',
           'Environment :: Console',
           'Topic :: Utilities',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11'
       ],
       zip_safe=False)
```

### Comparing `tinta-0.1.4a1.post0/tinta/__init__.py` & `tinta-0.1.5b1/tinta/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 # Tinta
-# Copyright 2021 github.com/brandoncript
+# Copyright 2023 github.com/brandoncript
 
 # This program is bound to the Hippocratic License 2.1
 # Full text is available here:
 # https://firstdonoharm.dev/version/2/1/license
 
 # Further to adherence to the Hippocratic Licenese, permission is hereby
 # granted, free of charge, to any person obtaining a copy of this software
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = '0.1.4'
+__version__ = "0.1.5b1"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 except ImportError as e:
     logger.warning(e)
```

### Comparing `tinta-0.1.4a1.post0/tinta/__main__.py` & `tinta-0.1.5b1/tinta/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 # Tinta
-# Copyright 2021 github.com/brandoncript
+# Copyright 2023 github.com/brandoncript
 
 # This program is bound to the Hippocratic License 2.1
 # Full text is available here:
 # https://firstdonoharm.dev/version/2/1/license
 
 # Further to adherence to the Hippocratic Licenese, permission is hereby
 # granted, free of charge, to any person obtaining a copy of this software
@@ -15,8 +15,8 @@
 # sublicense, and / or sell copies of the Software, and to permit persons
 # to whom the Software is furnished to do so, subject to the conditions layed
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
-import __init__ as tinta
+import __init__ as tinta  # pylint: disable=W0611,E0401
```

### Comparing `tinta-0.1.4a1.post0/tinta/tinta.py` & `tinta-0.1.5b1/tinta/tinta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 # Tinta
-# Copyright 2021 github.com/brandoncript
+# Copyright 2023 github.com/brandoncript
 
 # This program is bound to the Hippocratic License 2.1
 # Full text is available here:
 # https://firstdonoharm.dev/version/2/1/license
 
 # Further to adherence to the Hippocratic Licenese, permission is hereby
 # granted, free of charge, to any person obtaining a copy of this software
@@ -20,24 +20,30 @@
 # shall take precedence.
 
 """Tinta is a magical console output tool with support for printing in beautiful
 colors and with rich formatting, like bold and underline. It's so pretty,
 it's almost like a unicorn.
 """
 
-import os, sys, re
-from pathlib import Path
 import configparser
-config = configparser.ConfigParser()
+import os
+import re
+import sys
+from pathlib import Path
+from typing import Optional, Union
 
 from colors import color
 
+config = configparser.ConfigParser()
+
+
 CURSOR_UP_ONE = '\x1b[1A'
 ERASE_LINE = '\x1b[2K'
 
+
 class Tinta(object):
     """Tinta is a magical console output tool with support for printing in
     beautiful colors and with rich formatting, like bold and underline. It's
     so pretty, it's almost like a unicorn.
 
     All public methods chain together to form a builder pattern, e.g.:
 
@@ -295,19 +301,19 @@
         Args:
             *s: Segments of text to add.
             sep (str, optional): Used to join strings. Defaults to ' '.
 
         Returns:
             self
         """
-        self._prefixes = os.linesep
+        self._prefixes = [os.linesep]
         self.add(*s, sep=self._sep(sep))
         return self
 
-    def _sep(self, sep=None) -> str:
+    def _sep(self, sep=None) -> Union[str, None]:
         """Returns an appropriate separator for the given sep arg.
 
         Args:
             sep (str, optional): Separator. Defaults to None.
 
         Returns:
             str: Separator to use.
@@ -341,26 +347,28 @@
             force (bool, option): Forces printing, overriding TINTA_STEALTH.
         """
         # We don't print if the TINTA_STEALTH env is set
         if os.environ.get('TINTA_STEALTH') is not None:
             return
 
         if plaintext or os.environ.get('TINTA_PLAINTEXT') is not None:
-            print(self.plaintext(self._sep(sep)), end=end, file=file, flush=flush)
+            print(self.plaintext(self._sep(sep)),
+                  end=end, file=file, flush=flush)
 
         else:
             print(self.text(self._sep(sep)), end=end, file=file, flush=flush)
 
         self.reset()
         self.parts = []
         print('\033[0m', end='')
 
     @staticmethod
-    def discover():
-        """Prints all 256 colors in a matrix on your system."""
+    def discover(text_only=False):
+        """Prints all 256 colors in a matrix on your system. If text_only is True,
+        it will print numbers in their colors instead of background colors."""
         print('\n')
         for i in range(0, 16):
             for j in range(0, 16):
                 code = str(i * 16 + j)
                 sys.stdout.write(
                     u"\u001b[38;5;" + code + "m " + code.ljust(4))
             print(u"\u001b[0m")
@@ -384,26 +392,25 @@
             sys.stdout.write(CURSOR_UP_ONE)
             sys.stdout.flush()
 
     @classmethod
     def load_colors(cls, path):
         cls.colors = cls._AnsiColors(path)
 
-
     class Part:
         """A segment part of text, intended to be joined together
         for a print statement.
 
         Args:
             fmt (str):      A formatted string of text.
             p (str):        A plaintext representation of fmt.
             sep (str):      Used to join segment strings. Defaults to ' '.
         """
 
-        def __init__(self, fmt: str, pln: str, sep: str=None):
+        def __init__(self, fmt: str, pln: str, sep: Optional[str] = None):
             self.fmt = fmt
             self.pln = pln
             self.sep = sep
 
     class _AnsiColors:
 
         """Color builder for Tinta's console output.
@@ -425,10 +432,11 @@
             config.read(path)
             for k, v in config['colors'].items():
                 self.__setattr__(k, int(v))
 
 
 Tinta.colors = Tinta._AnsiColors()
 
+
 def to_plaintext(*s):
     ansi_escape = re.compile(r'\x1b\[(K|.*?m)', re.I)
     return [re.sub(ansi_escape, '', x) for x in s]
```

