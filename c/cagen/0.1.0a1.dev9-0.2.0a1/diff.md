# Comparing `tmp/cagen-0.1.0a1.dev9.tar.gz` & `tmp/cagen-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.1.0a1.dev9.tar", last modified: Sat Jan 14 23:02:36 2023, max compression
+gzip compressed data, was "cagen-0.2.0a1.tar", last modified: Sat Apr 15 18:22:11 2023, max compression
```

## Comparing `cagen-0.1.0a1.dev9.tar` & `cagen-0.2.0a1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/
--rw-r--r--   0 xan       (1000) xan       (1000)    18093 2023-01-04 12:26:34.000000 cagen-0.1.0a1.dev9/LICENSE
--rw-r--r--   0 xan       (1000) xan       (1000)       30 2023-01-14 23:02:30.000000 cagen-0.1.0a1.dev9/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     3067 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     2165 2023-01-14 22:37:52.000000 cagen-0.1.0a1.dev9/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1099 2023-01-14 22:53:28.000000 cagen-0.1.0a1.dev9/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.732638 cagen-0.1.0a1.dev9/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.732638 cagen-0.1.0a1.dev9/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)        0 2023-01-08 15:44:40.000000 cagen-0.1.0a1.dev9/src/cagen/__init__.py
--rwxr-xr-x   0 xan       (1000) xan       (1000)      875 2023-01-13 16:37:28.000000 cagen-0.1.0a1.dev9/src/cagen/cagen-make.py
--rwxr-xr-x   0 xan       (1000) xan       (1000)     1248 2023-01-12 21:15:09.000000 cagen-0.1.0a1.dev9/src/cagen/cagen.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4455 2023-01-13 14:39:41.000000 cagen-0.1.0a1.dev9/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)     1076 2023-01-13 14:43:30.000000 cagen-0.1.0a1.dev9/src/cagen/templates/schema.tmpl
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     3067 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      327 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a1/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     3943 2023-04-15 18:22:11.005245 cagen-0.2.0a1/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3208 2023-04-15 08:10:27.000000 cagen-0.2.0a1/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-15 08:11:23.000000 cagen-0.2.0a1/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-15 18:22:11.005245 cagen-0.2.0a1/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.001911 cagen-0.2.0a1/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a1/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4757 2023-03-28 18:54:37.000000 cagen-0.2.0a1/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8233 2023-03-28 18:54:45.000000 cagen-0.2.0a1/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a1/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a1/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a1/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a1/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     3943 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-15 18:22:11.000000 cagen-0.2.0a1/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.1.0a1.dev9/PKG-INFO` & `cagen-0.2.0a1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,96 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.1.0a1.dev9
+Version: 0.2.0a1
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
-Project-URL: Homepage, https://sr.ht/~somenxavierb/cagen/
-Project-URL: Bug Tracker, https://todo.sr.ht/~somenxavierb/cagen-tasks
-Project-URL: Repository, https://git.sr.ht/~somenxavierb/cagen
+Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
+
+<!--
+SPDX-FileCopyrightText: 2023 Xavier Bordoy <somenxavier@posteo.net>
+
+SPDX-License-Identifier: GPL-2.0-only
+-->
 
 # cagen
 
 ## About
 
-cagen is a static site generator intented for [cmpalgorithms project](https://sr.ht/~somenxavierb/cmpalgorithms/). So it's very rare you are interested in that.
+cagen is a static site generator. Originally, it was intented for [cmpalgorithms project](https://sr.ht/~somenxavierb/cmpalgorithms/) but now it's an independent project.
 
 ## License
 
-The software is distributed under [GPL2-only license](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt).
+The software is distributed under [GPL 2-only license](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt).
 
 ## How it runs
 
-It assumes your documents are in markdown syntax. It is capable of convert those documents in any other format, using [pandoc](https://pandoc.org/) (specifically [pypandoc](https://github.com/JessicaTegner/pypandoc) wrapper) and [Mako Templating System](https://www.makotemplates.org/).
+It assumes your documents are written with markdown syntax. It is capable of convert those documents to any other format, using [pandoc](https://pandoc.org/) (specifically [pypandoc](https://github.com/JessicaTegner/pypandoc) wrapper) and [Mako templating system](https://www.makotemplates.org/).
 
-The reason to use "external" templating sytem instead of built-in pandoc templat system is because pandoc templates [are not capable to make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
+The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
-The program just convert markdown files to HTML ones by default in the same directory. There is no predefined structure by default unlike many other static site generators do: no `assets` directory nope `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
+The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
-- a [library](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/libcagen.py)
-- a [command line program](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen.py) for convert documents
-- a script called [`cagen-make`](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen-make.py) to generate a Makefile to convert automatically all markdown files to HTML ones.
+- a [library](src/cagen/libcagen.py)
+- a command line program (called `cagen`) for convert documents
+- a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
-
 ```
 pip install cagen
 ```
 
-## Issue tracker
+If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](extras/PKGBUILD) to make a pacman package.
+
+## Usage
+
+Basic use is:
+```
+cagen sourcefile.md generatedfile.html template.tmpl
+```
+where 
+
+- `sourcefile.md` is Markdown file
+- `generatedfile.html` is the HTML5 file
+- `template.tmpl` is Mako template file
+
+See `cagen --help` for more options.
+
+This tool is some kind of low-level tool. If you want some more higher-level one to automatically converts all markdown files to corresponding HTML5 files, we provide the `cagen-make` script (see above). The steps are:
+```
+cagen-make --init
+```
+
+It creates `Makefile`
+
+```
+make
+```
+
+It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
+
+## Other resources
+
+- You can see the [list of tasks](tasks/index.md) (completed and pending).
+- The [API documentation](src/cagen/docs/index.html) is available.
+
+## Contribute
+
+If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
 
-You can see the [issue tracker](https://todo.sr.ht/~somenxavierb/cagen-tasks) and contribute if you want suggesting new features or reporting a bug.
```

### Comparing `cagen-0.1.0a1.dev9/README.md` & `cagen-0.2.0a1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,77 @@
+<!--
+SPDX-FileCopyrightText: 2023 Xavier Bordoy <somenxavier@posteo.net>
+
+SPDX-License-Identifier: GPL-2.0-only
+-->
+
 # cagen
 
 ## About
 
-cagen is a static site generator intented for [cmpalgorithms project](https://sr.ht/~somenxavierb/cmpalgorithms/). So it's very rare you are interested in that.
+cagen is a static site generator. Originally, it was intented for [cmpalgorithms project](https://sr.ht/~somenxavierb/cmpalgorithms/) but now it's an independent project.
 
 ## License
 
-The software is distributed under [GPL2-only license](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt).
+The software is distributed under [GPL 2-only license](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt).
 
 ## How it runs
 
-It assumes your documents are in markdown syntax. It is capable of convert those documents in any other format, using [pandoc](https://pandoc.org/) (specifically [pypandoc](https://github.com/JessicaTegner/pypandoc) wrapper) and [Mako Templating System](https://www.makotemplates.org/).
+It assumes your documents are written with markdown syntax. It is capable of convert those documents to any other format, using [pandoc](https://pandoc.org/) (specifically [pypandoc](https://github.com/JessicaTegner/pypandoc) wrapper) and [Mako templating system](https://www.makotemplates.org/).
 
-The reason to use "external" templating sytem instead of built-in pandoc templat system is because pandoc templates [are not capable to make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
+The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
-The program just convert markdown files to HTML ones by default in the same directory. There is no predefined structure by default unlike many other static site generators do: no `assets` directory nope `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
+The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
-- a [library](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/libcagen.py)
-- a [command line program](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen.py) for convert documents
-- a script called [`cagen-make`](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen-make.py) to generate a Makefile to convert automatically all markdown files to HTML ones.
+- a [library](src/cagen/libcagen.py)
+- a command line program (called `cagen`) for convert documents
+- a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
-
 ```
 pip install cagen
 ```
 
-## Issue tracker
+If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](extras/PKGBUILD) to make a pacman package.
+
+## Usage
+
+Basic use is:
+```
+cagen sourcefile.md generatedfile.html template.tmpl
+```
+where 
+
+- `sourcefile.md` is Markdown file
+- `generatedfile.html` is the HTML5 file
+- `template.tmpl` is Mako template file
+
+See `cagen --help` for more options.
+
+This tool is some kind of low-level tool. If you want some more higher-level one to automatically converts all markdown files to corresponding HTML5 files, we provide the `cagen-make` script (see above). The steps are:
+```
+cagen-make --init
+```
+
+It creates `Makefile`
+
+```
+make
+```
+
+It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
+
+## Other resources
+
+- You can see the [list of tasks](tasks/index.md) (completed and pending).
+- The [API documentation](src/cagen/docs/index.html) is available.
+
+## Contribute
+
+If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
 
-You can see the [issue tracker](https://todo.sr.ht/~somenxavierb/cagen-tasks) and contribute if you want suggesting new features or reporting a bug.
```

### Comparing `cagen-0.1.0a1.dev9/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0a1/src/cagen.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,96 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.1.0a1.dev9
+Version: 0.2.0a1
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
-Project-URL: Homepage, https://sr.ht/~somenxavierb/cagen/
-Project-URL: Bug Tracker, https://todo.sr.ht/~somenxavierb/cagen-tasks
-Project-URL: Repository, https://git.sr.ht/~somenxavierb/cagen
+Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
+
+<!--
+SPDX-FileCopyrightText: 2023 Xavier Bordoy <somenxavier@posteo.net>
+
+SPDX-License-Identifier: GPL-2.0-only
+-->
 
 # cagen
 
 ## About
 
-cagen is a static site generator intented for [cmpalgorithms project](https://sr.ht/~somenxavierb/cmpalgorithms/). So it's very rare you are interested in that.
+cagen is a static site generator. Originally, it was intented for [cmpalgorithms project](https://sr.ht/~somenxavierb/cmpalgorithms/) but now it's an independent project.
 
 ## License
 
-The software is distributed under [GPL2-only license](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt).
+The software is distributed under [GPL 2-only license](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt).
 
 ## How it runs
 
-It assumes your documents are in markdown syntax. It is capable of convert those documents in any other format, using [pandoc](https://pandoc.org/) (specifically [pypandoc](https://github.com/JessicaTegner/pypandoc) wrapper) and [Mako Templating System](https://www.makotemplates.org/).
+It assumes your documents are written with markdown syntax. It is capable of convert those documents to any other format, using [pandoc](https://pandoc.org/) (specifically [pypandoc](https://github.com/JessicaTegner/pypandoc) wrapper) and [Mako templating system](https://www.makotemplates.org/).
 
-The reason to use "external" templating sytem instead of built-in pandoc templat system is because pandoc templates [are not capable to make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
+The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
-The program just convert markdown files to HTML ones by default in the same directory. There is no predefined structure by default unlike many other static site generators do: no `assets` directory nope `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
+The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
-- a [library](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/libcagen.py)
-- a [command line program](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen.py) for convert documents
-- a script called [`cagen-make`](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen-make.py) to generate a Makefile to convert automatically all markdown files to HTML ones.
+- a [library](src/cagen/libcagen.py)
+- a command line program (called `cagen`) for convert documents
+- a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
-
 ```
 pip install cagen
 ```
 
-## Issue tracker
+If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](extras/PKGBUILD) to make a pacman package.
+
+## Usage
+
+Basic use is:
+```
+cagen sourcefile.md generatedfile.html template.tmpl
+```
+where 
+
+- `sourcefile.md` is Markdown file
+- `generatedfile.html` is the HTML5 file
+- `template.tmpl` is Mako template file
+
+See `cagen --help` for more options.
+
+This tool is some kind of low-level tool. If you want some more higher-level one to automatically converts all markdown files to corresponding HTML5 files, we provide the `cagen-make` script (see above). The steps are:
+```
+cagen-make --init
+```
+
+It creates `Makefile`
+
+```
+make
+```
+
+It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
+
+## Other resources
+
+- You can see the [list of tasks](tasks/index.md) (completed and pending).
+- The [API documentation](src/cagen/docs/index.html) is available.
+
+## Contribute
+
+If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
 
-You can see the [issue tracker](https://todo.sr.ht/~somenxavierb/cagen-tasks) and contribute if you want suggesting new features or reporting a bug.
```

