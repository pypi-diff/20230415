# Comparing `tmp/lpminimk3-0.5.1.tar.gz` & `tmp/lpminimk3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpminimk3-0.5.1.tar", last modified: Tue Apr 11 00:43:11 2023, max compression
+gzip compressed data, was "lpminimk3-0.6.0.tar", last modified: Sat Apr 15 10:13:35 2023, max compression
```

## Comparing `lpminimk3-0.5.1.tar` & `lpminimk3-0.6.0.tar`

### file list

```diff
@@ -1,60 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36820 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_lpminimk3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/colors/_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/display_character.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/light_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/party.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/print_text_scroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/sync_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/text_scroll_region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29194 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_renderable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/art/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/art/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/art/_art.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/bitmaps/smiley.bitmap.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/glyphs/basic_latin.glyph.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/movies/
--rw-r--r--   0 runner    (1001) docker     (123)   130587 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/movies/ping_pong.movie.json
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/schema/bitmap.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/schema/glyph.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/schema/movie.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/midi_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.657907 lpminimk3-0.6.0/lpminimk3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/colors/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38543 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/display_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/light_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/party.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/print_text_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/text_scroll_region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29194 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_renderable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/art.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/bitmaps/smiley.bitmap.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/glyphs/basic_latin.glyph.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)   130587 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/movies/ping_pong.movie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/schema/bitmap.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/schema/glyph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/schema/movie.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/midi_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21494 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.657907 lpminimk3-0.6.0/lpminimk3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/setup.py
```

### Comparing `lpminimk3-0.5.1/LICENSE` & `lpminimk3-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/PKG-INFO` & `lpminimk3-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpminimk3
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python API for the Novation Launchpad Mini MK3
 Home-page: https://github.com/obeezzy/lpminimk3
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpminimk3
 Python API for the [Novation Launchpad Mini MK3](https://novationmusic.com/en/launch/launchpad-mini)
 
 [![CI](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml)
-[![CD](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.3.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Documentation Status](https://readthedocs.org/projects/lpminimk3/badge/?version=latest)](https://lpminimk3.readthedocs.io/en/latest/?badge=latest)
 
 The goals of this project are as follows:
 * Intuitive, object-oriented design
 * Convenient for use in script and shell
 * Access to all (or most) of the Launchpad Mini MK3 MIDI features
 
 
@@ -37,16 +38,15 @@
 
 ## Usage example
 Make sure your Launchpad is connected to your computer.
 
 ### In script
 Control LEDs individually:
 ```python
-"""
-Display a random array of colors for 5 seconds.
+"""Display a random array of colors for 5 seconds.
 """
 
 from lpminimk3 import Mode, find_launchpads
 import random
 import time
 
 lp = find_launchpads()[0]  # Get the first available launchpad
@@ -60,16 +60,15 @@
 time.sleep(5)  # Keep LEDs on for a while
 
 for led in lp.panel.led_range():
     del led.color  # Turn off LED
 ```
 Render text on Launchpad's surface:
 ```python
-"""
-Scroll text from right to left across the Launchpad's surface.
+"""Scroll text from right to left across the Launchpad's surface.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
@@ -92,15 +91,15 @@
 >>> lp.open()
 ```
 Query the device to ensure we can read and write to it:
 ```python
 >>> lp.device_inquiry()  # Query device
 MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=150.938086752)
 ```
-Switch to `programmer` mode to start manipulating button LEDs.
+Switch to `programmer` mode to start manipulating button LEDs:
 ```python
 >>> lp.mode = 'prog'  # Switch to programmer mode
 >>> lp.grid.led('0x0').color = 10  # Set color to yellow (Valid values: 0 - 127)
 >>> lp.grid.led(1,0).color = lpminimk3.colors.ColorPalette.Red.SHADE_1  # Set from palette
 >>> lp.panel.led('logo').color = 'violet'  # Set logo LED color to violet
 >>> lp.panel.led('drums').color = 'green2'  # Set 'Drums' LED color to second shade of green
 >>> lp.panel.led('stop').color = 'w1'  # Set 'Stop/Solo/Mute' LED color to first shade of white
@@ -109,15 +108,15 @@
 >>> lp.panel.led('scene_launch_1').color = '#ff0000'  # Set color to red using hex
 >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)  # Set color to blue using rgb
 >>> lp.panel.led('mute').color = 0  # Turn off LED
 >>> lp.panel.led('logo').reset()  # Another way to turn off LED
 >>> del lp.panel.led('stop').color  # Another way to turn off LED
 ```
 Note in the above snippet that `lp.grid` only contains the __*grid*__ buttons
-(i.e. the faceless white buttons) and `lp.panel` contains all buttons
+(i.e. the translucent, faceless buttons) and `lp.panel` contains all buttons
 (including the __*logo*__ LED at the top right corner).  
 
 Wait for and respond to button presses and releases:
 ```python
 >>> ev = lp.panel.buttons().poll_for_event()  # Block until any button is pressed/released
 >>> ev
 ButtonEvent(button='7x5', type='press', deltatime=0.0)
@@ -130,14 +129,15 @@
 ```
 Pass button names as arguments to wait for specific button events:
 ```python
 >>> lp.panel.buttons('up', '0x0', 'stop').poll_for_event()
 ```
 Render `A` on Launchpad's surface:
 ```python
+>>> from lpminimk3.graphics import Text
 >>> lp.grid.render(Text('A'))
 ```
 Print `A` in console:
 ```python
 >>> Text('A').print()
   XX    
  XXXX   
@@ -162,32 +162,30 @@
 $ python -m lpminimk3.graphics.sync
 ```
 Once the server is running, visit the [LP Sketch](https://www.github.com/obeezzy/lpsketch) website to start creating bitmaps and movies live.
 
 ### Rendering bitmaps and movies
 Render `smiley.bitmap.json` on Launchpad's surface:
 ```python
-"""
-Render "Smiley" bitmap.
+"""Render "Smiley" bitmap.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Bitmap
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
 lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))  # Display bitmap
 ```
 Render `ping_pong.movie.json` on Launchpad's surface:
 ```python
-"""
-Render "Ping/Pong" movie.
+"""Render "Ping/Pong" movie.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Movie
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
```

### Comparing `lpminimk3-0.5.1/README.md` & `lpminimk3-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # lpminimk3
 Python API for the [Novation Launchpad Mini MK3](https://novationmusic.com/en/launch/launchpad-mini)
 
 [![CI](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml)
-[![CD](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.3.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Documentation Status](https://readthedocs.org/projects/lpminimk3/badge/?version=latest)](https://lpminimk3.readthedocs.io/en/latest/?badge=latest)
 
 The goals of this project are as follows:
 * Intuitive, object-oriented design
 * Convenient for use in script and shell
 * Access to all (or most) of the Launchpad Mini MK3 MIDI features
 
 
@@ -23,16 +24,15 @@
 
 ## Usage example
 Make sure your Launchpad is connected to your computer.
 
 ### In script
 Control LEDs individually:
 ```python
-"""
-Display a random array of colors for 5 seconds.
+"""Display a random array of colors for 5 seconds.
 """
 
 from lpminimk3 import Mode, find_launchpads
 import random
 import time
 
 lp = find_launchpads()[0]  # Get the first available launchpad
@@ -46,16 +46,15 @@
 time.sleep(5)  # Keep LEDs on for a while
 
 for led in lp.panel.led_range():
     del led.color  # Turn off LED
 ```
 Render text on Launchpad's surface:
 ```python
-"""
-Scroll text from right to left across the Launchpad's surface.
+"""Scroll text from right to left across the Launchpad's surface.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
@@ -78,15 +77,15 @@
 >>> lp.open()
 ```
 Query the device to ensure we can read and write to it:
 ```python
 >>> lp.device_inquiry()  # Query device
 MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=150.938086752)
 ```
-Switch to `programmer` mode to start manipulating button LEDs.
+Switch to `programmer` mode to start manipulating button LEDs:
 ```python
 >>> lp.mode = 'prog'  # Switch to programmer mode
 >>> lp.grid.led('0x0').color = 10  # Set color to yellow (Valid values: 0 - 127)
 >>> lp.grid.led(1,0).color = lpminimk3.colors.ColorPalette.Red.SHADE_1  # Set from palette
 >>> lp.panel.led('logo').color = 'violet'  # Set logo LED color to violet
 >>> lp.panel.led('drums').color = 'green2'  # Set 'Drums' LED color to second shade of green
 >>> lp.panel.led('stop').color = 'w1'  # Set 'Stop/Solo/Mute' LED color to first shade of white
@@ -95,15 +94,15 @@
 >>> lp.panel.led('scene_launch_1').color = '#ff0000'  # Set color to red using hex
 >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)  # Set color to blue using rgb
 >>> lp.panel.led('mute').color = 0  # Turn off LED
 >>> lp.panel.led('logo').reset()  # Another way to turn off LED
 >>> del lp.panel.led('stop').color  # Another way to turn off LED
 ```
 Note in the above snippet that `lp.grid` only contains the __*grid*__ buttons
-(i.e. the faceless white buttons) and `lp.panel` contains all buttons
+(i.e. the translucent, faceless buttons) and `lp.panel` contains all buttons
 (including the __*logo*__ LED at the top right corner).  
 
 Wait for and respond to button presses and releases:
 ```python
 >>> ev = lp.panel.buttons().poll_for_event()  # Block until any button is pressed/released
 >>> ev
 ButtonEvent(button='7x5', type='press', deltatime=0.0)
@@ -116,14 +115,15 @@
 ```
 Pass button names as arguments to wait for specific button events:
 ```python
 >>> lp.panel.buttons('up', '0x0', 'stop').poll_for_event()
 ```
 Render `A` on Launchpad's surface:
 ```python
+>>> from lpminimk3.graphics import Text
 >>> lp.grid.render(Text('A'))
 ```
 Print `A` in console:
 ```python
 >>> Text('A').print()
   XX    
  XXXX   
@@ -148,32 +148,30 @@
 $ python -m lpminimk3.graphics.sync
 ```
 Once the server is running, visit the [LP Sketch](https://www.github.com/obeezzy/lpsketch) website to start creating bitmaps and movies live.
 
 ### Rendering bitmaps and movies
 Render `smiley.bitmap.json` on Launchpad's surface:
 ```python
-"""
-Render "Smiley" bitmap.
+"""Render "Smiley" bitmap.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Bitmap
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
 lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))  # Display bitmap
 ```
 Render `ping_pong.movie.json` on Launchpad's surface:
 ```python
-"""
-Render "Ping/Pong" movie.
+"""Render "Ping/Pong" movie.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Movie
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
```

### Comparing `lpminimk3-0.5.1/lpminimk3/_core/components.py` & `lpminimk3-0.6.0/lpminimk3/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,98 @@
-"""
-Software representation of physical components for Launchpad Mini MK3.
+"""Components that make up the Launchpad Mini MK3.
 """
 
 import math
 import re
 from abc import ABC
-from ..colors._colors import ColorShade, ColorShadeStore, RgbColor
-from ..midi_messages import Colorspec,\
-                            ColorspecFragment,\
-                            Constants,\
-                            Lighting
-from ..match import ButtonMatch
+from .colors._colors import ColorShade, ColorShadeStore, RgbColor
+from .midi_messages import Colorspec,\
+                           ColorspecFragment,\
+                           Constants,\
+                           Lighting
+from .match import ButtonMatch
 from .utils import ButtonEvent
-from ..region import Region
+from .region import Region
 
 
 class Matrix(ABC):
-    """
-    A matrix of pad buttons/LEDs on the surface of the Launchpad.
+    """A matrix of pad buttons/LEDs on the surface of the Launchpad.
     """
     @property
     def launchpad(self):
+        """Launchpad reference.
+        """
         pass
 
     @property
     def width(self):
+        """Width of matrix.
+        """
         return -1
 
     @property
     def height(self):
+        """Height of matrix.
+        """
         return -1
 
     @property
     def max_x(self):
+        """Max X.
+        """
         return -1
 
     @property
     def max_y(self):
+        """Max Y.
+        """
         return -1
 
     def led_range(self):
+        """LED range.
+        """
         pass
 
     def render(self, renderable):
+        """Render `renderable` on matrix.
+        """
         renderable.render(self)
 
 
 class FlipAxis:
+    """Flip axis.
+    """
     X = 'x'
     Y = 'y'
     XY = 'xy'
 
 
 class _MatrixTransform:
+    """Matrix transform.
+    """
     def __init__(self, matrix, layout, led_mode):
         self._matrix = matrix
         self._layout = layout
         self._led_mode = led_mode
 
     def rotated_led_range(self, angle, *, flip_axis=''):
+        """Returns an immutable sequence of rotated LEDs.
+
+        Parameters
+        ----------
+        angle : int
+            Angle of rotation.
+        flip_axis : str, optional
+            Flip axis.
+
+        Yields
+        ------
+        Led
+            Sequence of LEDs.
+        """
         assert angle, 'Angle cannot be zero.'
         angle = self._normalize_angle(angle)
         angle = self._flip_angle(angle)
         angle_rad = math.radians(angle)
         for led in self._matrix.led_range(layout=self._layout,
                                           mode=self._led_mode):
             rotated_x = round((led.y * math.sin(angle_rad)) + (led.x * math.cos(angle_rad)))  # noqa
@@ -88,14 +118,25 @@
             else:
                 yield self._matrix.led(x=rotated_x,
                                        y=rotated_y,
                                        layout=self._layout,
                                        mode=self._led_mode)
 
     def flipped_led_range(self, axis):
+        """Returns an immutable sequence of flipped LEDs.
+
+        Parameters
+        ----------
+        axis : str
+            Flip axis. (Possible values: 'x', 'y', 'xy')
+
+        Yields
+        ------
+            Sequence of LEDs.
+        """
         for led in self._matrix.led_range(layout=self._layout,
                                           mode=self._led_mode):
             flipped_x = (self._flip_axis(led.x)
                          if FlipAxis.X in axis
                          else led.x)
             flipped_y = (self._flip_axis(led.y)
                          if FlipAxis.Y in axis
@@ -160,44 +201,58 @@
                 f'name={self.name}, '
                 f'x={self.x}, '
                 f'y={self.y}, '
                 f'id={self.id})')
 
     @property
     def id(self):
+        """Matrix coordinate ID.
+        """
         within_range = (self._x >= 0
                         and self._y >= 0
                         and self._x < self._matrix_width
                         and self._y < self._matrix_height)
         if not within_range:
             return -1
         return (self._y * self._matrix_height) + self._x + 1
 
     @property
     def name(self):
+        """Matrix coordinate name.
+        """
         return self._name
 
     @property
     def x(self):
+        """X position.
+        """
         return self._x
 
     @property
     def y(self):
+        """Y position.
+        """
         return self._y
 
     @property
     def midi_value(self):
+        """MIDI value.
+        """
         return self._midi_value
 
     @property
     def matrix_width(self):
+        """Matrix width.
+        """
         return self._matrix_width
 
     @property
     def matrix_height(self):
+        """Matrix height.
+        """
         return self._matrix_height
 
     def _determine_coordinate_from_id(self, led_id, bounds):
         width, height = bounds
         x = int(led_id % width)
         y = int(led_id / height)
         return x, y
@@ -296,14 +351,16 @@
             lighting = self._create_lighting_message(value,
                                                      lighting_mode,
                                                      midi_value)
             self._message = lighting
 
     @property
     def message(self):
+        """Message.
+        """
         return self._message
 
     def _create_colorspec_message(self, value, lighting_type, midi_value):
         rgb_color = RgbColor(value)
         colorspec = Colorspec(ColorspecFragment(lighting_type,
                                                 midi_value,
                                                 rgb_color.r,
@@ -333,16 +390,15 @@
         lighting = Lighting(lighting_mode,
                             midi_value,
                             0x0)
         return lighting
 
 
 class ButtonFace:
-    """
-    A button face.
+    """A button face.
 
     A button face is the marking placed on the top of
     some Launchpad buttons.
     """
     UP = 'up'
     DOWN = 'down'
     LEFT = 'left'
@@ -359,16 +415,15 @@
     SCENE_LAUNCH_5 = 'scene_launch_5'
     SCENE_LAUNCH_6 = 'scene_launch_6'
     SCENE_LAUNCH_7 = 'scene_launch_7'
     STOP_SOLO_MUTE = 'stop_solo_mute'
 
 
 class ButtonGroup:
-    """
-    A group of buttons.
+    """A group of buttons.
     """
 
     def __init__(self, launchpad,
                  layout,
                  button_names,
                  args):
         self._launchpad = launchpad
@@ -384,43 +439,48 @@
 
     def __repr__(self):
         names = list(map(lambda name: f"'{name}'", self.names))
         return f'ButtonGroup({names})'
 
     @property
     def launchpad(self):
-        """
-        Launchpad reference.
+        """Launchpad reference.
         """
         return self._launchpad
 
     @property
     def names(self):
-        """
-        Names of buttons in group.
+        """Names of buttons in group.
         """
         return [button.name for button in self._buttons]
 
     def poll_for_event(self, *, interface='midi', timeout=None,
                        type=ButtonEvent.PRESS_RELEASE):
-        """
-        Polls for MIDI events of buttons specified
+        """Polls for MIDI events of buttons specified
         in this group. If `timeout` is `None`, this function will
         wait indefinitely until a :class:`ButtonEvent` is
         received. If no event is received, `None` is returned.
 
-        Keyword Args:
-            interface (str): Interface to which to send message.
-                (See :class:`Interface`.)
-            timeout (float): Duration in seconds to wait for event to occur
-            type (str): Event type.
-                (Possible values: 'press', 'release', 'press|release')
-
-        Returns:
-            ButtonEvent: Button event (See :class:`ButtonEvent`).
+        Parameters
+        ----------
+        interface : str
+            Interface to which to send message.
+        timeout : float or None
+            Duration in seconds to wait for event to occur.
+        type : str
+            Event type. (Possible values: 'press', 'release', 'press|release')
+
+        Returns
+        -------
+            ButtonEvent: Button event.
+
+        See Also
+        --------
+        Interface
+        ButtonEvent
         """
         if (not type
                 or (type.lower().replace('|', '_') != ButtonEvent.PRESS_RELEASE  # noqa
                     and type.lower() != ButtonEvent.RELEASE
                     and type.lower() != ButtonEvent.PRESS)):
             raise ValueError('Not a valid event type.')
 
@@ -429,24 +489,31 @@
                                                     match=ButtonMatch(self._buttons,  # noqa
                                                                       type))  # noqa
         return (ButtonEvent(midi_event, self._buttons)
                 if midi_event
                 else None)
 
     def clear_event_queue(self, *, interface='midi'):
-        """
-        Clears event queue.
+        """Clears event queue.
 
-        Keyword Args:
-            interface (str): Interface to clear.
-                (See :class:`Interface`.)
-
-        Raises:
-            ValueError: If `interface` is invalid.
-            RuntimeError: If device is closed.
+        Parameters
+        ----------
+        interface : str
+            Interface to clear.
+
+        Raises
+        ------
+        ValueError
+            If `interface` is invalid.
+        RuntimeError
+            If device is closed.
+
+        See Also
+        --------
+        Interface
         """
         self._launchpad.clear_event_queue()
 
     # FIXME: Too complex
     def _create_buttons(self, launchpad, layout, button_names, args):  # noqa
         buttons = []
         for arg in args:
@@ -481,16 +548,15 @@
                         found = True
                     else:
                         raise ValueError(f'Invalid button "{str(arg)}".')
         return set(buttons)
 
 
 class Led:
-    """
-    An LED on the Launchpad.
+    """An LED on the Launchpad.
     """
 
     OFF = 'off'
     STATIC = 'static'
     FLASH = 'flash'
     PULSE = 'pulse'
 
@@ -545,104 +611,102 @@
         return hash(repr(self))
 
     def __repr__(self):
         return f"Led(x={self.x}, y={self.x}, name='{self.name}')"
 
     @property
     def id(self):
-        """
-        Unique ID of LED.
+        """Unique, nonzero ID.
         """
         if not self._is_within_range():
             return -1
         return (self._y * self._matrix_height) + self._x + 1
 
     @property
     def x(self):
-        """
-        X position of LED.
+        """X position.
         """
         return self._x
 
     @property
     def y(self):
-        """
-        Y position of LED.
+        """Y position.
         """
         return self._y
 
     @property
     def name(self):
-        """
-        Name of LED.
+        """Name.
         """
         return (self._button_names[self.y][self.x]
                 if self._is_within_range()
                 else '')
 
     @property
     def midi_value(self):
-        """
-        Midi value of LED.
+        """MIDI value.
         """
         return self._midi_value
 
     @property
     def launchpad(self):
-        """
-        Launchpad reference.
+        """Launchpad reference.
         """
         return self._launchpad
 
     @property
     def color(self):
-        """
-        Color. Retrieving the set color is not supported.
+        """Color. Retrieving the set color is not supported.
         """
         return None
 
     @color.setter
     def color(self, value):
-        """
-        Sets the color of the LED to `value`.
-
-        Args:
-            value (ColorShade or str or int): Color value.
+        """Sets the color of the LED to `value`.
 
-        Raises:
-            ValueError: When invalid value is used.
-            TypeError: When invalid type is used.
+        Parameters
+        ----------
+        value : ColorShade or str or int
+            Color value.
+
+        Raises
+        ------
+        ValueError
+            If invalid value is set.
+        TypeError
+            If invalid type is set.
         """
         message = _LedColor(value,
                             lighting_mode=self._LIGHTING_MODE[self._mode],
                             lighting_type=self._LIGHTING_TYPE['rgb'],
                             midi_value=self._midi_value).message
         self.launchpad.send_message(message)
 
     @color.deleter
     def color(self):
-        """Turns LED off."""
+        """Turns LED off.
+        """
         self.reset()
 
     def reset(self):
-        """Turns LED off."""
+        """Turns LED off.
+        """
         message = _LedColor(lighting_mode=self._LIGHTING_MODE[self._mode],
                             midi_value=self._midi_value).message
         self.launchpad.send_message(message)
 
     def _is_within_range(self):
         return (self._x >= 0
                 and self._y >= 0
                 and self._x < self._matrix_width
                 and self._y < self._matrix_height)
 
 
 class Button:
-    """
-    A button on the Launchpad.
+    """A button on the Launchpad.
     """
 
     def __init__(self, launchpad,
                  layout,
                  button_names, *,
                  x=-1, y=-1,
                  name='',
@@ -676,86 +740,76 @@
                 f"name='{self.name}', "
                 f"x={self.x}, "
                 f"y={self.y}, "
                 f"id={self.id})")
 
     @property
     def launchpad(self):
-        """
-        Launchpad reference.
+        """Launchpad reference.
         """
         return self._launchpad
 
     @property
     def x(self):
-        """
-        X position of button.
+        """X position of button.
         """
         return self._x
 
     @property
     def y(self):
-        """
-        Y position of button.
+        """Y position of button.
         """
         return self._y
 
     @property
     def name(self):
-        """
-        Name of button.
+        """Name of button.
         """
         return self._name
 
     @property
     def midi_value(self):
-        """
-        MIDI value of button.
+        """MIDI value of button.
         """
         return self._midi_value
 
     @property
     def id(self):
-        """
-        Unique ID of button.
+        """Unique ID of button.
         """
         return self._button_id
 
     @property
     def parent(self):
-        """
-        Parent of button, either 'grid' or 'panel'.
+        """Parent of button, either 'grid' or 'panel'.
         """
         match = re.match('^\\d+x\\d+$', self._name)
         if match:
             return 'grid'
         return 'panel' if self._button_id else ''
 
     @property
     def led(self):
-        """
-        LED of button.
+        """LED of button.
         """
         return Led(launchpad=self._launchpad,
                    layout=self._layout,
                    button_names=self._button_names,
                    x=self._x,
                    y=self._y)
 
     @property
     def layout(self):
-        """
-        Button layout.
+        """Button layout.
         """
         return self._layout
 
 
 class Panel(Matrix):
-    """
-    Panel of Launchpad.
+    """Panel of Launchpad.
 
     The panel represents the 9x9 matrix of pad buttons
     on the surface of the Launchpad.
     """
     PROG = 'prog'
     CUSTOM = 'custom'
     _PROG_MODE_MIDI_LAYOUT = [
@@ -802,70 +856,72 @@
         return self.launchpad == other.launchpad
 
     def __repr__(self):
         return f'Panel({self.width}x{self.height})'
 
     @Matrix.launchpad.getter
     def launchpad(self):
-        """
-        Launchpad reference.
+        """Launchpad reference.
         """
         return self._launchpad
 
     @Matrix.width.getter
     def width(self):
-        """
-        Max X.
+        """Max X.
         """
         return len(Panel._BUTTON_NAMES[0])
 
     @Matrix.height.getter
     def height(self):
-        """
-        Max Y.
+        """Max Y.
         """
         return len(Panel._BUTTON_NAMES)
 
     @property
     def max_id(self):
-        """
-        Max ID.
+        """Max ID.
         """
         return self.width * self.height
 
     @Matrix.max_x.getter
     def max_x(self):
-        """
-        Max X.
+        """Max X.
         """
         return (self.width - 1
                 if self.width >= 0
                 else -1)
 
     @Matrix.max_y.getter
     def max_y(self):
-        """
-        Max Y.
+        """Max Y.
         """
         return (self.height - 1
                 if self.height >= 0
                 else -1)
 
     def led(self, x=-1, y=-1, *, name='', layout=PROG, mode=Led.STATIC):
-        """
-        Returns an LED.
+        """Returns an LED.
 
-        Args:
-            x (int): X position of LED.
-            y (int): Y position of LED.
-
-        Keyword Args:
-            name (str): Name of LED.
-            layout (Layout): Layout of buttons.
-            mode (str): Lighting mode.
+        Parameters
+        ----------
+        x : int
+            X position of LED, or index of LED
+            if ``y=-1``.
+        y : int, optional
+            Y position of LED.
+        name : str, optional
+            Name of LED.
+        layout : Layout, optional
+            Layout of buttons.
+        mode : str, optional
+            Lighting mode.
+
+        Returns
+        -------
+            Led: An LED.
         """
         return Led(launchpad=self._launchpad,
                    button_names=Panel._BUTTON_NAMES,
                    layout=(Panel._CUSTOM_MODE_MIDI_LAYOUT
                            if layout == Panel.CUSTOM
                            else Panel._PROG_MODE_MIDI_LAYOUT),
                    x=x, y=y,
@@ -874,25 +930,31 @@
     # FIXME: Too complex
     def led_range(self, *,  # noqa
                   layout=PROG,
                   mode=Led.STATIC,
                   rotation=0,
                   flip_axis='',
                   region=None):
-        """
-        Returns an immutable sequence of LEDs.
-
-        Keyword Args:
-            layout (Layout): Layout of buttons.
-            mode (str): Lighting mode.
-            rotation (int): Rotation angle in degrees.
-                (Possible values: 0, 90, 180, 270, -90)
+        """Returns an immutable sequence of LEDs.
 
-        Yields:
-            Led: Sequence of LEDs
+        Parameters
+        ----------
+        layout : Layout, optional
+            Layout of buttons.
+        mode : str, optional
+            Lighting mode.
+        rotation : int, optional
+            Rotation angle in degrees. (Possible values: 0, 90, 180, 270, -90)
+        region : Region or None, optional
+            Region of LEDs on the matrix.
+
+        Yields
+        ------
+        Led
+            Sequence of LEDs.
         """
         if region and not isinstance(region, Region):
             raise TypeError("'region' must be of type 'Region'.")
         elif rotation and not isinstance(rotation, int):
             raise TypeError("'rotation' must be of type 'int'.")
         elif flip_axis and not isinstance(flip_axis, str):
             raise TypeError("'flip_axis' must be of type 'str'.")
@@ -908,23 +970,26 @@
             for led in _MatrixTransform(self, layout, mode).flipped_led_range(flip_axis):  # noqa
                 yield led
         else:
             for led_id in range(self.max_id):
                 yield self.led(led_id, layout=layout, mode=mode)
 
     def buttons(self, *args, layout=PROG):
-        """
-        Returns a :class:`ButtonGroup`.
-
-        Args:
-            args (list): Button names, button IDs
-                or button XY-pairs
+        """Returns a ButtonGroup.
 
-        Keyword Args:
-            layout (Layout): Layout of buttons.
+        Parameters
+        ----------
+        args : list
+            Button names, button IDs or button XY-pairs.
+        layout : Layout, optional
+            Layout of buttons.
+
+        Returns
+        -------
+            ButtonGroup: Button group.
         """
         args = (args
                 if len(args) > 0
                 else [button_name
                       for button_row in Panel._BUTTON_NAMES
                       for button_name in button_row])
         return ButtonGroup(launchpad=self._launchpad,
@@ -932,18 +997,17 @@
                                    if layout == Panel.CUSTOM
                                    else Panel._PROG_MODE_MIDI_LAYOUT),
                            button_names=Panel._BUTTON_NAMES,
                            args=list(args))
 
 
 class Grid(Matrix):
-    """
-    Grid of Launchpad.
+    """Grid of Launchpad.
 
-    The grid represents the 8x8 grid of white, faceless
+    The grid represents the 8x8 grid of translucent, faceless
     buttons of the Launchpad.
     """
     PROG = 'prog'
     CUSTOM = 'custom'
     _PROG_MODE_MIDI_LAYOUT = [
             [0x51, 0x52, 0x53, 0x54, 0x55, 0x56, 0x57, 0x58],
             [0x47, 0x48, 0x49, 0x4a, 0x4b, 0x4c, 0x4d, 0x4e],
@@ -984,70 +1048,72 @@
         return self.launchpad == other.launchpad
 
     def __repr__(self):
         return f'Grid({self.width}x{self.height})'
 
     @Matrix.launchpad.getter
     def launchpad(self):
-        """
-        Launchpad reference.
+        """Launchpad reference.
         """
         return self._launchpad
 
     @Matrix.width.getter
     def width(self):
-        """
-        Max X.
+        """Max X.
         """
         return len(Grid._BUTTON_NAMES[0])
 
     @Matrix.height.getter
     def height(self):
-        """
-        Max Y.
+        """Max Y.
         """
         return len(Grid._BUTTON_NAMES)
 
     @property
     def max_id(self):
-        """
-        Max ID.
+        """Max ID.
         """
         return self.width * self.height
 
     @Matrix.max_x.getter
     def max_x(self):
-        """
-        Max X.
+        """Max X.
         """
         return (self.width - 1
                 if self.width >= 0
                 else -1)
 
     @Matrix.max_y.getter
     def max_y(self):
-        """
-        Max Y.
+        """Max Y.
         """
         return (self.height - 1
                 if self.height >= 0
                 else -1)
 
     def led(self, x=-1, y=-1, *, name='', layout=PROG, mode=Led.STATIC):
-        """
-        Returns an LED.
+        """Returns an LED.
 
-        Args:
-            x (int): X position of LED.
-            y (int): Y position of LED.
-
-        Keyword Args:
-            name (str): Name of LED.
-            layout (Layout): Layout of buttons.
-            mode (str): Lighting mode.
+        Parameters
+        ----------
+        x : int
+            X position of LED, or index of LED
+            if y=-1.
+        y : int, optional
+            Y position of LED.
+        name : str, optional
+            Name of LED.
+        layout : Layout, optional
+            Layout of buttons.
+        mode : str, optional
+            Lighting mode.
+
+        Returns
+        -------
+            Led: An LED.
         """
         return Led(launchpad=self._launchpad,
                    button_names=Grid._BUTTON_NAMES,
                    layout=(Grid._CUSTOM_MODE_MIDI_LAYOUT
                            if layout == Grid.CUSTOM
                            else Grid._PROG_MODE_MIDI_LAYOUT),
                    x=x, y=y,
@@ -1056,25 +1122,31 @@
     # FIXME: Too complex
     def led_range(self, *,  # noqa
                   layout=PROG,
                   mode=Led.STATIC,
                   rotation=0,
                   flip_axis='',
                   region=None):
-        """
-        Returns an immutable sequence of LEDs.
-
-        Keyword Args:
-            layout (Layout): Layout of buttons.
-            mode (str): Lighting mode.
-            rotation (int): Rotation angle in degrees.
-                (Possible values: 0, 90, 180, 270, -90)
+        """Returns an immutable sequence of LEDs.
 
-        Yields:
-            Led: Sequence of LEDs
+        Parameters
+        ----------
+        layout : Layout, optional
+            Layout of buttons.
+        mode : str, optional
+            Lighting mode.
+        rotation : int, optional
+            Rotation angle in degrees. (Possible values: 0, 90, 180, 270, -90)
+        region : Region or None, optional
+            Region of LEDs on the matrix.
+
+        Yields
+        ------
+        Led
+            Sequence of LEDs.
         """
         if region and not isinstance(region, Region):
             raise TypeError("'region' must be of type 'Region'.")
         elif rotation and not isinstance(rotation, int):
             raise TypeError("'rotation' must be of type 'int'.")
         elif flip_axis and not isinstance(flip_axis, str):
             raise TypeError("'flip_axis' must be of type 'str'.")
@@ -1090,23 +1162,26 @@
             for led in _MatrixTransform(self, layout, mode).flipped_led_range(flip_axis):  # noqa
                 yield led
         else:
             for led_id in range(self.max_id):
                 yield self.led(led_id, layout=layout, mode=mode)
 
     def buttons(self, *args, layout=PROG):
-        """
-        Returns a :class:`ButtonGroup`.
-
-        Args:
-            args (list): Button names, button IDs
-                or button XY-pairs
+        """Returns a ButtonGroup.
 
-        Keyword Args:
-            layout (Layout): Layout of buttons.
+        Parameters
+        ----------
+        args : list
+            Button names, button IDs or button XY-pairs.
+        layout : Layout, optional
+            Layout of buttons.
+
+        Returns
+        -------
+            ButtonGroup: Button group.
         """
         args = (args
                 if len(args) > 0
                 else [button_name
                       for button_row in Grid._BUTTON_NAMES
                       for button_name in button_row])
         return ButtonGroup(launchpad=self._launchpad,
```

### Comparing `lpminimk3-0.5.1/lpminimk3/_core/logging.py` & `lpminimk3-0.6.0/lpminimk3/_logging.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/_core/utils.py` & `lpminimk3-0.6.0/lpminimk3/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-"""
-Utility classes for Launchpad Mini MK3.
+"""Utility classes for Launchpad Mini MK3.
 """
 
 import enum
 import time
 import re
 import platform
 from collections import namedtuple
-from . import logging
-from ..match import Match
+from . import _logging
+from .match import Match
 
-logger = logging.getLogger(__name__)
+logger = _logging.getLogger(__name__)
 
 MIDI_MESSAGE_LENGTH = 9
 
 
 class MidiEvent:
-    """
-    A MIDI event.
+    """A MIDI event.
 
     A MIDI event is received every time the Launchpad's MIDI port
     is read.
     """
 
     def __init__(self, message, deltatime=0):
         self._message = message
@@ -32,29 +30,32 @@
             return False
         if isinstance(other, list):
             return self.message == other
         return self.message == other.message
 
     @property
     def message(self):
+        """Message.
+        """
         return self._message
 
     @property
     def deltatime(self):
+        """Deltatime.
+        """
         return self._deltatime
 
     def __repr__(self):
         return ('MidiEvent('
                 f'message={self.message}, '
                 f'deltatime={self.deltatime})')
 
 
 class ButtonEvent:
-    """
-    A button event.
+    """A button event.
 
     A button event is received every time a button on the Launchpad
     is pushed.
     """
 
     PRESS = 'press'
     RELEASE = 'release'
@@ -73,26 +74,34 @@
         return ("ButtonEvent("
                 f"button='{self.button.name}', "
                 f"type='{self.type}', "
                 f"deltatime={self.deltatime})")
 
     @property
     def message(self):
+        """Message.
+        """
         return self._midi_event.message
 
     @property
     def deltatime(self):
+        """Deltatime.
+        """
         return self._midi_event.deltatime
 
     @property
     def button(self):
+        """Button.
+        """
         return self._button
 
     @property
     def type(self):
+        """Type.
+        """
         if not self._midi_event:
             return ''
         return (ButtonEvent.RELEASE
                 if self._midi_event
                 and len(self._midi_event.message) == 3
                 and self._midi_event.message[2] == 0x0
                 else ButtonEvent.PRESS)
@@ -103,16 +112,15 @@
                          else None)
         return (found_buttons[0]
                 if found_buttons and len(found_buttons)
                 else None)
 
 
 class MidiPort:
-    """
-    A MIDI port.
+    """A MIDI port.
     """
 
     OUT = 'out'
     IN = 'in'
     DEFAULT_CLIENT_NAME = 'lpminimk3'
 
     def __init__(self, port_name, port_number, port_index,
@@ -142,72 +150,102 @@
                 f"index={self.port_index})")
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
     @property
     def port_name(self):
+        """Port name.
+        """
         return self._port_name
 
     @property
     def port_number(self):
+        """Port number.
+        """
         return self._port_number
 
     @property
     def port_index(self):
+        """Port index.
+        """
         return self._port_index
 
     @property
     def system_port_name(self):
+        """System port name.
+        """
         return self._system_port_name
 
     @property
     def midi_in_handle(self):
+        """MIDI IN handle.
+        """
         return self._midi_in
 
     @property
     def midi_out_handle(self):
+        """MIDI OUT handle.
+        """
         return self._midi_out
 
     def is_open(self):
+        """Checks to see if port is open.
+
+        Returns
+        -------
+        bool
+            `True` if port is open, otherwise `False`.
+        """
         if self._midi_in and self._direction == MidiPort.IN:
             return self._midi_in.is_port_open()
         elif self._midi_out and self._direction == MidiPort.OUT:
             return self._midi_out.is_port_open()
         return False
 
     def open(self):
+        """Opens MIDI port.
+        """
         if (self._direction == MidiPort.OUT
                 and not self._midi_out.is_port_open()):
             if self._virtual:
                 self._midi_out.open_virtual_port(self._system_port_name)
             else:
                 self._midi_out.open_port(self.port_index, MidiPort.OUT)
 
-            if platform.system() != 'Windows' and platform.system() != 'Darwin':
+            if platform.system() != 'Windows' and platform.system() != 'Darwin':  # noqa
                 self._midi_out.set_client_name(MidiPort.DEFAULT_CLIENT_NAME)
 
         elif (self._direction == MidiPort.IN
                 and not self._midi_in.is_port_open()):
             if self._virtual:
                 self._midi_in.open_virtual_port(self._system_port_name)
             else:
                 self._midi_in.open_port(self.port_index, MidiPort.IN)
 
-            if platform.system() != 'Windows' and platform.system() != 'Darwin':
+            if platform.system() != 'Windows' and platform.system() != 'Darwin':  # noqa
                 self._midi_in.set_client_name(MidiPort.DEFAULT_CLIENT_NAME)
 
     def close(self):
+        """Closes MIDI port.
+        """
         if self.is_open():
             if self._midi_out and self._direction == MidiPort.OUT:
                 self._midi_out.close_port()
             elif self._midi_in and self._direction == MidiPort.IN:
                 self._midi_in.close_port()
 
     def send_message(self, message):
+        """Sends raw MIDI message to Launchpad.
+
+        Parameters
+        ----------
+        message : list of str
+            Message of raw integers to send to Launchpad.
+        """
         if (not message
                 or (not isinstance(message, list)
                     and not hasattr(message, 'data'))):
             raise TypeError('Message must be of type list or MidiMessage.')
         message = (message.data
                    if hasattr(message, 'data')
                    else message)
@@ -218,14 +256,34 @@
         elif self._midi_out and self._direction == MidiPort.OUT:
             self._midi_out.send_message(message)
             logger.debug(f'MIDI message sent: {message}')
         else:
             raise RuntimeError('Failed to send message.')
 
     def poll_for_event(self, *, timeout=5, match=None, read_delay=.001):
+        """Polls for button event.
+
+        Parameters
+        ----------
+        timeout : int
+            Timeout in seconds.
+        match : Match or None
+            Button match.
+        read_delay : float
+            Delay duration between reads.
+
+        Returns
+        -------
+        ButtonEvent or None
+            Received event.
+
+        See Also
+        --------
+        Match
+        """
         assert self._midi_in
         event = None
         polling = True
         elapsed = 0 if timeout else -1
         timeout = 0 if not timeout else timeout
         timeout = 0 if timeout < 0 else timeout
         while polling and timeout > elapsed:
@@ -248,16 +306,15 @@
 
     def clear_event_queue(self, *, read_delay=.001):
         while self._midi_in and self._midi_in.get_message():
             time.sleep(read_delay)
 
 
 class Interface:
-    """
-    Interface of the launchpad.
+    """Interface of the launchpad.
     """
 
     DAW = 'daw'
     MIDI = 'midi'
     READBACK_POSITION = 7
 
     class MidiWord(enum.IntEnum):
@@ -285,20 +342,21 @@
     def __repr__(self):
         return ('Interface()'
                 if not self._interface
                 else f"Interface('Interface.{self._interface.upper()}')")
 
     @property
     def midi_event(self):
+        """MIDI event.
+        """
         return self._midi_event
 
 
 class Mode:
-    """
-    A Launchpad mode.
+    """A Launchpad mode.
     """
 
     LIVE = 'live'
     PROG = 'prog'
     READBACK_POSITION = 7
 
     class MidiWord(enum.IntEnum):
@@ -326,20 +384,21 @@
     def __repr__(self):
         return ('Mode()'
                 if not self._mode
                 else f"Mode('Mode.{self._mode.upper()}')")
 
     @property
     def midi_event(self):
+        """MIDI event.
+        """
         return self._midi_event
 
 
 class Layout:
-    """
-    A Launchpad layout.
+    """A Launchpad layout.
     """
 
     SESSION = 'session'
     CUSTOM_1 = 'custom_1'
     CUSTOM_2 = 'custom_2'
     CUSTOM_3 = 'custom_3'
     DAW_FADERS = 'daw_faders'
@@ -377,14 +436,16 @@
     def __repr__(self):
         return ('Layout()'
                 if not self._layout
                 else f"Layout('Layout.{self._layout.upper()}')")
 
     @property
     def midi_event(self):
+        """Midi event.
+        """
         return self._midi_event
 
     def _determine_layout(self, midi_value):
         if midi_value == Layout.MidiWord.SESSION:
             layout = Layout.SESSION
         elif midi_value == Layout.MidiWord.CUSTOM_1:
             layout = Layout.CUSTOM_1
@@ -396,16 +457,15 @@
             layout = Layout.DAW_FADERS
         else:
             layout = Layout.PROG
         return layout
 
 
 class MidiClient:
-    """
-    A MIDI client.
+    """A MIDI client.
     """
 
     def __init__(self, client_name, client_number):
         self._client_name = client_name
         self._client_number = client_number
         self._out_ports = []
         self._in_ports = []
@@ -419,95 +479,154 @@
     def __repr__(self):
         return ("MidiClient("
                 f"name='{self.client_name}', "
                 f"number={self.client_number})")
 
     @property
     def daw_out_port(self):
+        """DAW out port.
+        """
         daw_ports = list(filter(lambda port: re.search(r'1|DA',
                                 port.port_name),
                                 self._out_ports))
         return daw_ports[0] if len(daw_ports) > 0 else None
 
     @property
     def daw_in_port(self):
+        """DAW in port.
+        """
         daw_ports = list(filter(lambda port: re.search(r'1|DA',
                                 port.port_name),
                                 self._in_ports))
         return daw_ports[0] if len(daw_ports) > 0 else None
 
     @property
     def midi_out_port(self):
+        """MIDI out port.
+        """
         midi_ports = list(filter(lambda port: re.search(r'2|MI',
                                  port.port_name),
                                  self._out_ports))
         return midi_ports[0] if len(midi_ports) > 0 else None
 
     @property
     def midi_in_port(self):
+        """MIDI in port.
+        """
         midi_ports = list(filter(lambda port: re.search(r'2|MI',
                                  port.port_name),
                                  self._in_ports))
         return midi_ports[0] if len(midi_ports) > 0 else None
 
     @property
     def ports(self):
+        """Ports.
+        """
         return self._out_ports + self._in_ports
 
     @property
     def out_ports(self):
+        """Out ports.
+        """
         return self._out_ports
 
     @property
     def in_ports(self):
+        """In ports.
+        """
         return self._in_ports
 
     @property
     def client_name(self):
+        """Client name.
+        """
         return self._client_name
 
     @property
     def client_number(self):
+        """Client number.
+        """
         return self._client_number
 
     def is_open(self):
+        """Checks if ports all ports are open.
+
+        Returns
+        -------
+        bool
+            `True` if all ports are open, otherwise `False`.
+        """
         return all(port.is_open() for port in self.ports)
 
     def open(self, interface=Interface.MIDI):
+        """Opens a MIDI port for interface `interface`.
+
+        Parameters
+        ----------
+        interface : str, optional
+            Interface to open.
+
+        See Also
+        --------
+        Interface
+        """
         self.close()
         if interface == Interface.DAW:
             self.daw_in_port.open()
             self.daw_out_port.open()
         elif interface == Interface.MIDI:
             self.midi_in_port.open()
             self.midi_out_port.open()
         else:
             raise ValueError('Must be a valid Interface.')
 
     def close(self):
+        """Closes MIDI ports.
+        """
         for port in self.ports:
             if port.is_open():
                 port.close()
 
     def append_out_port(self, port):
+        """Appends out port `port`.
+
+        Parameters
+        ----------
+        port : MidiPort
+            Port to append.
+
+        See Also
+        --------
+        MidiPort
+        """
         if not isinstance(port, MidiPort):
             raise TypeError('Must be of type MidiPort.')
         if port not in self._out_ports:
             self._out_ports.append(port)
 
     def append_in_port(self, port):
+        """Appends in port `port`.
+
+        Parameters
+        ----------
+        port : MidiPort
+            Port to append.
+
+        See Also
+        --------
+        MidiPort
+        """
         if not isinstance(port, MidiPort):
             raise TypeError('Must be of type MidiPort.')
         if port not in self._in_ports:
             self._in_ports.append(port)
 
 
 class SystemMidiPortParser:
-    """
-    System-specific way of parsing MIDI port names.
+    """System-specific way of parsing MIDI port names.
     """
 
     def __init__(self, in_ports, out_ports):
         lp_in_ports = list(filter(lambda port: re.search(r'Mini\s*MK3',
                                                          port,
                                                          re.IGNORECASE),
                                   in_ports))
@@ -578,8 +697,10 @@
                 client_data.ports.append(port_data)
                 self._found_clients.append(client_data)
             else:
                 existing_client_data.ports.append(port_data)
 
     @property
     def found_clients(self):
+        """Found clients.
+        """
         return self._found_clients
```

### Comparing `lpminimk3-0.5.1/lpminimk3/_lpminimk3.py` & `lpminimk3-0.6.0/lpminimk3/device.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,215 @@
+"""Software model and discovery functions for Launchpad Mini MK3.
+"""
 from rtmidi import MidiOut, MidiIn
-from ._core.components import Grid, Panel
-from ._core.utils import SystemMidiPortParser, \
-                          MidiPort, MidiClient, \
-                          Interface, Mode, Layout # noqa
+from .components import Grid, Panel
+from .utils import SystemMidiPortParser, \
+                   MidiPort, MidiClient, \
+                   Interface, Mode, Layout # noqa
 from .midi_messages import SysExMessages
 
 
 class LaunchpadMiniMk3:
-    """
-    A Launchpad Mini MK3 device.
+    """A Launchpad Mini MK3 device.
     """
 
     def __init__(self, midi_client):
         self._midi_client = midi_client
 
     def __eq__(self, other):
         if not isinstance(other, LaunchpadMiniMk3):
             return False
         return self.id == other.id
 
     def __repr__(self):
         return f'LaunchpadMiniMk3(id={self.id})'
 
     def is_open(self):
-        """
-        Returns `True` if the device is open, otherwise
+        """Returns `True` if the device is open, otherwise
         returns `False`. An open device is a device that can
         be read from and/or written to.
+
+        Returns
+        -------
+        Boolean
+            `True` if device is open, otherwise `False`.
         """
         return self._midi_client.is_open()
 
     def open(self, interface=Interface.MIDI):
-        """
-        Opens interface `interface` on this device for reading
+        """Opens interface `interface` on this device for reading
         and writing.
 
-        Args:
-            interface (str): Interface to open.
-                (See :class:`Interface`.)
-
-        Raise:
-            ValueError: If `interface` is invalid.
+        Parameters
+        ----------
+        interface : str, optional
+            Interface to open.
+
+        Raises
+        ------
+        ValueError
+            If `interface` is invalid.
+
+        See Also
+        --------
+        Interface
         """
         self._midi_client.open(interface)
         self.interface = interface
 
     def close(self):
-        """
-        Closes this device.
+        """Closes this device.
         """
         self._midi_client.close()
 
     def send_message(self, msg, *, interface=Interface.MIDI):
-        """
-        Sends a MIDI message `msg` to the `interface` of
+        """Sends a MIDI message `msg` to the `interface` of
         this device.
 
-        Args:
-            message (list): MIDI message
-
-        Keyword Args:
-            interface (str): Interface to which to send message.
-                (See :class:`Interface`.)
-
-        Raises:
-            ValueError: If `interface` is invalid.
-            RuntimeError: If device is closed.
+        Parameters
+        ----------
+        message : list
+            MIDI message.
+        interface : str, optional
+            Interface to which to send message.
+
+        Raises
+        ------
+        ValueError
+            If `interface` is invalid.
+        RuntimeError
+            If device is closed.
         """
         if self.is_open():
             if interface == Interface.DAW:
                 self.daw_out_port.send_message(msg)
             elif interface == Interface.MIDI:
                 self.midi_out_port.send_message(msg)
             else:
                 raise ValueError('Must be a valid Interface')
         else:
             raise RuntimeError('Port closed.')
 
     def poll_for_event(self, *, interface=Interface.MIDI,
                        timeout=5, match=None):
-        """
-        Polls for a MIDI event from interface `interface` either until
+        """Polls for a MIDI event from interface `interface` either until
         `timeout` is reached or `match` is found.
 
-        Keyword Args:
-            interface (str): Interface to poll.
-                (See :class:`Interface`.)
-            timeout (float): Duration in seconds to wait for event
-                before returning `None`.
-            match (Match): Match criterion. (See :class:`Match`).
-
-        Returns:
-            MidiEvent: MIDI event received. (See :class:`MidiEvent`).
-
-        Raises:
-            ValueError: If `interface` is invalid.
-            RuntimeError: If this device is closed.
+        Parameters
+        ----------
+        interface : str, optional
+            Interface to poll.
+        timeout : float, optional
+            Duration in seconds to wait for event before returning `None`.
+        match : Match or None, optional
+            Match criterion.
+
+        Returns
+        -------
+        MidiEvent
+            MIDI event received.
+
+        Raises
+        ------
+        ValueError
+            If `interface` is invalid.
+        RuntimeError
+            If this device is closed.
+
+        See Also
+        --------
+        Interface
+        MidiEvent
         """
         if self.is_open():
             if interface == Interface.DAW:
                 return self.daw_in_port.poll_for_event(timeout=timeout,
                                                        match=match)
             elif interface == Interface.MIDI:
                 return self.midi_in_port.poll_for_event(timeout=timeout,
                                                         match=match)
             else:
                 raise ValueError('Must be a valid Interface.')
         else:
             raise RuntimeError('Port closed.')
 
     def clear_event_queue(self, *, interface=Interface.MIDI):
-        """
-        Clears MIDI event queue for interface `interface`.
+        """Clears MIDI event queue for interface `interface`.
 
-        Keyword Args:
-            interface (str): Interface to clear.
-                (See :class:`Interface`.)
-
-        Raises:
-            ValueError: If `interface` is invalid.
-            RuntimeError: If device is closed.
+        Parameters
+        ----------
+        interface : str
+            Interface to clear.
+
+        Raises
+        ------
+        ValueError
+            If `interface` is invalid.
+        RuntimeError
+            If device is closed.
+
+        See Also
+        --------
+        Interface
         """
         if self.is_open():
             if interface == Interface.DAW:
                 return self.daw_in_port.clear_event_queue()
             elif interface == Interface.MIDI:
                 return self.midi_in_port.clear_event_queue()
             else:
                 raise ValueError('Must be a valid Interface.')
         else:
             raise RuntimeError('Port closed.')
 
     @property
     def id(self):
-        """
-        Unique ID of this device.
+        """Unique ID of this device.
         """
         return self._midi_client.client_number
 
     @property
     def daw_in_port(self):
-        """
-        DAW interface MIDI-in port.
+        """DAW interface MIDI-in port.
+
         Used for internal purposes.
         """
         return self._midi_client.daw_in_port
 
     @property
     def daw_out_port(self):
-        """
-        DAW interface MIDI-out port.
+        """DAW interface MIDI-out port.
+
         Used for internal purposes.
         """
         return self._midi_client.daw_out_port
 
     @property
     def midi_in_port(self):
-        """
-        MIDI interface MIDI-in port.
+        """MIDI interface MIDI-in port.
+
         Used for internal purposes.
         """
         return self._midi_client.midi_in_port
 
     @property
     def midi_out_port(self):
-        """
-        MIDI interface MIDI-out port.
+        """MIDI interface MIDI-out port.
+
         Used for internal purposes.
         """
         return self._midi_client.midi_out_port
 
     @property
     def interface(self):
-        """
-        Interface of Launchpad. (See :class:`Interface`.)
+        """Interface of Launchpad.
+
+        See Also
+        --------
+        Interface
         """
         self.send_message(SysExMessages.Interfaces.READBACK)
         return Interface(self.poll_for_event())
 
     @interface.setter
     def interface(self, value):
         if value.lower() == Interface.MIDI:
@@ -185,32 +217,42 @@
         elif value.lower() == Interface.DAW:
             self.send_message(SysExMessages.Interfaces.DAW)
         else:
             raise ValueError('Invalid interface set.')
 
     @property
     def panel(self):
-        """
-        Panel of Launchpad; represents the 9x9 array of buttons,
-        with face buttons included. (See :class:`Panel`.)
+        """Panel of Launchpad; represents the 9x9 array of buttons,
+        with face buttons included.
+
+        See Also
+        --------
+        Panel
         """
         return Panel(self)
 
     @property
     def grid(self):
-        """
-        Grid of Launchpad; represents the 8x8 array of white,
-        faceless buttons. (See :class:`Grid`.)
+        """Grid of Launchpad; represents the 8x8 array of white,
+        faceless buttons.
+
+        See Also
+        --------
+        Grid
         """
         return Grid(self)
 
     @property
     def mode(self):
         """
-        Mode of Launchpad. (See :class:`Mode`.)
+        Mode of Launchpad.
+
+        See Also
+        --------
+        Mode
         """
         self.send_message(SysExMessages.Modes.READBACK)
         return Mode(self.poll_for_event())
 
     @mode.setter
     def mode(self, value):
         if value.lower() == Mode.LIVE:
@@ -218,16 +260,19 @@
         elif value.lower() == Mode.PROG:
             self.send_message(SysExMessages.Modes.PROG)
         else:
             raise ValueError('Invalid mode set.')
 
     @property
     def layout(self):
-        """
-        Layout of Launchpad. (See :class:`Layout`.)
+        """Layout of Launchpad.
+
+        See Also
+        --------
+        Layout
         """
         self.send_message(SysExMessages.Layouts.READBACK)
         return Layout(self.poll_for_event())
 
     @layout.setter
     def layout(self, value):
         if value.lower() == Layout.SESSION:
@@ -242,31 +287,33 @@
             self.send_message(SysExMessages.Layouts.DAW_FADERS)
         elif value.lower() == Layout.PROG:
             self.send_message(SysExMessages.Layouts.PROG)
         else:
             raise ValueError('Invalid layout set.')
 
     def device_inquiry(self):
-        """
-        Sends a "device inquiry" message to this device.
+        """Sends a "device inquiry" message to this device.
 
-        Returns:
-            MidiEvent: MIDI event received.
+        Returns
+        -------
+        MidiEvent
+            MIDI event received.
         """
         self.mode = Mode.PROG
         self.send_message(SysExMessages.DEVICE_INQUIRY)
         return self.poll_for_event()
 
 
 def find_launchpads():
-    """
-    Searches for connected Launchpad Mini MK3 devices.
+    """Searches for connected Launchpad Mini MK3 devices.
 
-    Returns:
-        list of LaunchpadMiniMk3: List of found devices.
+    Returns
+    -------
+    list of LaunchpadMiniMk3
+        List of found devices.
     """
     midi_out = MidiOut()
     out_ports = midi_out.get_ports()
     midi_in = MidiIn()
     in_ports = midi_in.get_ports()
     parser = SystemMidiPortParser(in_ports, out_ports)
```

### Comparing `lpminimk3-0.5.1/lpminimk3/colors/_colors.py` & `lpminimk3-0.6.0/lpminimk3/colors/_colors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+"""Colors for the Launchpad Mini MK3.
+"""
 import re
 
 
 class RgbColor:
-    """
-    An RGB color.
+    """An RGB color.
     """
     _RGB_LENGTH = 3
     _MIN_HEX_LENGTH = 4
     _MAX_HEX_LENGTH = 7
     _MIN_COLOR_VALUE = 0
     _MAX_COLOR_VALUE = 255
 
@@ -23,54 +24,54 @@
         self._parse(value)
 
     def __repr__(self):
         return f'RgbColor(r={self.r}, g={self.g}, b={self.b})'
 
     @staticmethod
     def is_valid(value):
-        """
-        Returns `True` if `value` is a valid (r,g,b) or hex value,
+        """Returns `True` if `value` is a valid (r,g,b) or hex value,
         otherwise returns `False`.
+
+        Returns
+        -------
+        bool
+            `True` if `value` is valid, otherwise `False`.
         """
         if isinstance(value, str):
             match = re.match('^#(?:[0-9a-fA-F]{3}){1,2}$', value)
             return True if match else False
         elif isinstance(value, (tuple, list)):
             valid_values = list(filter(lambda rgb_value: min(RgbColor._MAX_COLOR_VALUE,  # noqa
                                                              max(rgb_value, RgbColor._MIN_COLOR_VALUE)) == rgb_value,  # noqa
                                        value))
             return (len(valid_values) == len(value)
                     and len(value) == RgbColor._RGB_LENGTH)
         return False
 
     @property
     def value(self):
-        """
-        RGB value, as string.
+        """RGB value, as string.
         """
         return self._value
 
     @property
     def r(self):
-        """
-        Red value
+        """Red value.
         """
         return self._r >> 1
 
     @property
     def g(self):
-        """
-        Green value
+        """Green value.
         """
         return self._g >> 1
 
     @property
     def b(self):
-        """
-        Blue value
+        """Blue value.
         """
         return self._b >> 1
 
     def _parse(self, value):
         if (isinstance(value, str)
                 and len(value) == RgbColor._MIN_HEX_LENGTH):
             self._r = int(value[1], 16)
@@ -88,18 +89,17 @@
             self._r = value[0]
             self._g = value[1]
             self._b = value[2]
             self._value = value
 
 
 class ColorShade:
-    """
-    A color shade.
+    """Color shade.
 
-    A color shade is color from the Launchpad's color palette.
+    A color shade is a color from the Launchpad's color palette.
     There are 128 valid color shades, ranging from ID 0 to 127
     (with ID 0 used for OFF).
     """
 
     MIN_COLOR_ID = 0
     MAX_COLOR_ID = 127
     HEX_VALUES = [
@@ -142,43 +142,55 @@
     def __repr__(self):
         return ('ColorShade('
                 f'group={self.color_group}, '
                 f'id={self.color_id})')
 
     @staticmethod
     def is_valid_id(value):
-        """
-        Returns `True` if `value` is a valid color ID,
+        """Returns `True` if `value` is a valid color ID,
         otherwise returns `False`.
+
+        Parameters
+        ----------
+        value : int
+            Color ID.
+
+        Returns
+        -------
+        Boolean
+            `True` if provided value is valid, otherwise
+            `False`.
         """
         return (True
                 if isinstance(value, int)
                 and value >= ColorShade.MIN_COLOR_ID
                 and value <= ColorShade.MAX_COLOR_ID
                 else False)
 
     @property
     def hex(self):
-        """Hex color code."""
+        """Hex color code.
+        """
         return ColorShade.HEX_VALUES[self._color_id]
 
     @property
     def color_id(self):
-        """Unique color ID."""
+        """Unique color ID.
+        """
         return self._color_id
 
     @property
     def color_group(self):
-        """Color group."""
+        """Color group.
+        """
         return self._color_group
 
 
 class ColorPalette:
-    """
-    Color palette of Launchpad.
+    """Color palette of Launchpad.
 
     The color palette contains 127 predefined color shades.
     """
     class Red:
         SHADE_1 = ColorShade(0x04, 'red')
         SHADE_2 = ColorShade(0x05, 'red')
         SHADE_3 = ColorShade(0x06, 'red')
@@ -318,41 +330,56 @@
         SHADE_3 = ColorShade(0x03, 'white')
         SHADE_4 = ColorShade(0x75, 'white')
         SHADE_5 = ColorShade(0x76, 'white')
         SHADE_6 = ColorShade(0x77, 'white')
 
 
 class ColorShadeStore:
-    """
-    Color shade store for the Launchpad.
+    """Color shade store for the Launchpad.
     """
     COLOR_GROUPS = ['red', 'orange', 'yellow', 'green',
                     'blue', 'violet', 'white']
     COLOR_GROUP_SYMBOLS = list(map(lambda color: color[0],
                                    COLOR_GROUPS))
 
     def __iter__(self):
         for color_group in ColorShadeStore.COLOR_GROUPS:
             color_shades_in_group = ColorPalette.__dict__[color_group.capitalize()].__dict__  # noqa
             for _, color_shade in color_shades_in_group.items():
                 if isinstance(color_shade, ColorShade):
                     yield color_shade
 
     def contains(self, value):
-        """
-        Searches for color shade `value` and returns `True` if
+        """Searches for color shade `value` and returns `True` if
         the color shade exists, otherwise returns `False`.
+
+        Parameters
+        ----------
+        value : ColorShadeStore
+            Color shade.
+
+        Returns
+        -------
+            `True` if color shade exists, otherwise `False`.
         """
         color, _ = self._parse(value)
         return True if color else False
 
     def find(self, value):
-        """
-        Searches for color shade `value` and returns the
+        """Searches for color shade `value` and returns the
         `ColorShade` if found, otherwise returns `None`.
+
+        Parameters
+        ----------
+        value : ColorShadeStore
+            Color shade.
+
+        Returns
+        -------
+            `True` if color shade found, otherwise `False`.
         """
         if isinstance(value, ColorShade):
             return value
         return self._find_shade(*self._parse(value))
 
     def _find_shade(self, color, color_shade_id=1):
         if not color:
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/display_character.py` & `lpminimk3-0.6.0/lpminimk3/examples/display_character.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Display characters typed with a QWERTY keyboard on the Launchpad's surface.
+"""Display characters typed with a QWERTY keyboard on the Launchpad's surface.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 import sys
 import termios
 import tty
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/flash.py` & `lpminimk3-0.6.0/lpminimk3/examples/flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Display a random array of colors for 5 seconds.
+"""Display a random array of colors for 5 seconds.
 """
 
 from lpminimk3 import Mode, find_launchpads
 import random
 import time
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/hello.py` & `lpminimk3-0.6.0/lpminimk3/examples/hello.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Scroll text from right to left across the Launchpad's surface.
+"""Scroll text from right to left across the Launchpad's surface.
 """
 
 import sys
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/light_on_push.py` & `lpminimk3-0.6.0/lpminimk3/examples/light_on_push.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Wait for button presses and log events.
+"""Wait for button presses/releases and log events.
 """
 
 from lpminimk3 import ButtonEvent, Mode, find_launchpads
 import random
 import sys
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/party.py` & `lpminimk3-0.6.0/lpminimk3/examples/party.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Random party mode with some interactivity
+"""Random party mode with some interactivity
 
 Author: Matthew Wachter
 """
 
 from lpminimk3 import Mode, find_launchpads, colors
 import random
 import math
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/sync_client.py` & `lpminimk3-0.6.0/lpminimk3/examples/sync_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Sync client for the Launchpad MK3.
+"""
+
 import sys
 import asyncio
 import json
 from collections import namedtuple
 from argparse import ArgumentParser
 from websockets import connect
 from lpminimk3 import find_launchpads, Mode
```

### Comparing `lpminimk3-0.5.1/lpminimk3/examples/text_scroll_region.py` & `lpminimk3-0.6.0/lpminimk3/examples/text_scroll_region.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Scroll text from left to right along the Launchpad's surface,
+"""Scroll text from left to right along the Launchpad's surface,
 lighting a specified region.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 from lpminimk3.region import Labeled as LabeledRegion
 import random
```

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/_graphics.py` & `lpminimk3-0.6.0/lpminimk3/graphics/_graphics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Graphics API.
+"""
 import os
 from ..colors import ColorPalette
 from ._renderable import Renderable,\
                          RenderableColor,\
                          String,\
                          TextScroll,\
                          MovieRoll,\
@@ -10,41 +12,40 @@
 from ._utils import ScrollDirection,\
                     FlipAxis,\
                     Framerate
 from ._renderable import Frame  # noqa
 
 
 class Text(Renderable):
-    """
-    Text renderable on the Launchpad's surface. The text
+    """Text renderable on the Launchpad's surface. The text
     rendered can be transformed by calling any of the
     transformation methods of this class.
 
-
-    EXAMPLES
+    Examples
+    --------
     Render text on Launchpad's surface:
-        lp.grid.render(Text('A'))
+        >>> lp.grid.render(Text('A'))
 
     Print the text in the console:
-        Text('A').print()
+        >>> Text('A').print()
 
     Scroll text and render text on Launchpad's surface:
-        lp.grid.render(Text(' Hello, world!').scroll())
+        >>> lp.grid.render(Text(' Hello, world!').scroll())
 
     Scroll text and render text in the console:
-        Text(' Hello, world!').print()
+        >>> Text(' Hello, world!').print()
 
     Set the foreground color to "blue", rotate the text
     anticlockwise by 90 degrees, flip the text on its 'X'
     axis and scroll once:
-        lp.grid.render(Text(' Hello, world!')
-                       .fg_color.set('blue')
-                       .rotate(-90)
-                       .flip()
-                       .scroll(count=1))
+        >>> lp.grid.render(Text(' Hello, world!')
+                           .fg_color.set('blue')
+                           .rotate(-90)
+                           .flip()
+                           .scroll(count=1))
     """
     def __init__(self,
                  text='', *,
                  fg_color=ColorPalette.Red.SHADE_4,
                  bg_color=None):
         if isinstance(text, Text):
             text = text.text
@@ -67,137 +68,151 @@
         return self._text
 
     def __len__(self):
         return len(self._text)
 
     @Renderable.bits.getter
     def bits(self):
-        """
-        Text as bits (i.e. 0s and 1s).
+        """Text as bits (i.e. 0s and 1s).
         """
         return self._string.bits
 
     @Renderable.word_count.getter
     def word_count(self):
-        """
-        Number of (bit)words.
+        """Number of (bit)words.
         """
         return self._string.word_count
 
     @property
     def fg_color(self):
-        """
-        Foreground color.
+        """Foreground color.
         """
         return self._string.fg_color
 
     @fg_color.setter
     def fg_color(self, color):
         self._string.fg_color = RenderableColor(self, color)
 
     @property
     def bg_color(self):
-        """
-        Background color.
+        """Background color.
         """
         return self._string.bg_color
 
     @bg_color.setter
     def bg_color(self, color):
         self._string.bg_color = RenderableColor(self, color)
 
     def print(self, one='X', zero=' '):
-        """
-        Prints text to the screen as bits, used to give a preview of
+        """Prints text to the screen as bits, used to give a preview of
         how text would be rendered on the Launchpad's surface.
 
-        Keyword Args:
-            one (str): Character to represent bit 1.
-            zero (str): Character to represent bit 0.
-
-        Returns:
-            Text: `Text` reference.
+        Parameters
+        ----------
+        one : str
+            Character to represent bit 1.
+        zero : str
+            Character to represent bit 0.
+
+        Returns
+        -------
+        Text
+            `Text` reference.
         """
         self._string.print(one=one, zero=zero)
 
     def shift(self, count=1, *, circular=True):
-        """
-        Shifts text to the left if `count` is positive, or to the
+        """Shifts text to the left if `count` is positive, or to the
         right if `count` is negative.
 
-        Args:
-            count (int): Number of times to shift.
-
-        Keyword Args:
-            circular (bool): If True, enable text wrapping; else
-                diable text wrapping.
-
-        Returns:
-            Text: `Text` reference.
-
-        Raises:
-            ValueError: When invalid value is set.
+        Parameters
+        ----------
+        count : int
+            Number of times to shift.
+        circular : bool
+            If True, enable text wrapping; else diable text wrapping.
+
+        Returns
+        -------
+        Text
+            `Text` reference.
+
+        Raises
+        ------
+        ValueError
+            When invalid value is set.
         """
         if not isinstance(count, int):
             raise ValueError("'count' must be 'int'.")
         if count > 0:
             self._string.shift_right(count=count, circular=circular)
         elif count < 0:
             self._string.shift_left(count=int(abs(count)), circular=circular)
         return self
 
     def rotate(self, angle):
-        """
-        Rotates rendered text by `angle` degrees. All values
+        """Rotates rendered text by `angle` degrees. All values
         must be a multiples of 90.
 
-        Args:
-            angle (int): Angle of rotation in degrees.
-                A negative `angle` rotates Text in an anticlockwise
-                direction; a positive `angle` clockwise.
-
-        Returns:
-            Text: `Text` reference.
+        Parameters
+        ----------
+        angle : int
+            Angle of rotation in degrees. A negative `angle`
+            rotates Text in an anticlockwise direction; a
+            positive `angle` clockwise.
+
+        Returns
+        -------
+        Text
+            `Text` reference.
         """
         self._string.rotate(angle)
         return self
 
     def scroll(self, *,
                period=.05,
                direction=ScrollDirection.LEFT,
                cycle_func=None,
                count=None,
                timeout=None):
-        """
-        Scrolls rendered text, shifting every `period` seconds in the
+        """Scrolls rendered text, shifting every `period` seconds in the
         `direction` direction; scrolls indefinitely if `count` is not
         set.
 
-        Keyword Args:
-            period (float): Delay before every text render call.
-            direction (str): Direction of scroll, either left or right.
+        Parameters
+        ----------
+        period : float
+            Delay before every text render call.
+        direction : str
+            Direction of scroll, either left or right.
                 (See :class:`ScrollDirection`.)
-            cycle_func (callable): Function to be called right after
-                text render call but before period delay. The function
-                signature is:
+        cycle_func : callable
+            Function to be called right after text render call but
+            before period delay. The function signature is:
                     cycle_func(fraction, launchpad)
-                where `fraction` is the fraction of the scroll (ranging
-                from 0 to 1) and `launchpad` is the Launchpad reference.
-            count (int): Number of complete scrolls. Scrolls
-                indefinitely if `count` and `timeout` are not set.
-            timeout (float): Duration in seconds for scroll. Scrolls
-                indefinitely if `count` and `timeout` are not set.
-                If both `timeout` and `count` are set, the scroll will
-                end depending on which value is reached first.
-
-        Returns:
-            Text: `Text` reference.
-
-        Raises:
-            ValueError: When invalid value is set.
+            where `fraction` is the fraction of the scroll (ranging
+            from 0 to 1) and `launchpad` is the Launchpad reference.
+        count : int
+            Number of complete scrolls. Scrolls
+            indefinitely if `count` and `timeout` are not set.
+        timeout : float
+            Duration in seconds for scroll. Scrolls indefinitely if
+            `count` and `timeout` are not set. If both `timeout`
+            and `count` are set, the scroll will end depending on
+            which value is reached first.
+
+        Returns
+        -------
+        Text
+            `Text` reference.
+
+        Raises
+        ------
+        ValueError
+            When invalid value is set.
         """
         if timeout and timeout <= period:
             raise ValueError("'timeout' must be greater than "
                              "or equal to the period.")
         if cycle_func and not callable(cycle_func):
             raise ValueError("'cycle_func' must be callable.")
         self._string.text_scroll = TextScroll(self._text,
@@ -205,45 +220,59 @@
                                               direction,
                                               cycle_func=cycle_func,
                                               timeout=timeout,
                                               count=count)
         return self
 
     def flip(self, axis=FlipAxis.X):
-        """
-        Flips text on `axis` axis.
+        """Flips text on `axis` axis.
 
-        Args:
-            axis (str): Axis to flip on (X, Y or both).
-                (See :class:`FlipAxis`.)
-
-        Returns:
-            Text: `Text` reference.
+        Parameters
+        ----------
+        axis : str
+            Axis to flip on (X, Y or both).
+            (See :class:`FlipAxis`.)
+
+        Returns
+        -------
+        Text
+            `Text` reference.
         """
         self._string.flip_axis = axis
         return self
 
     def swap_colors(self):
-        """
-        Swaps foreground and background colors.
+        """Swaps foreground and background colors.
 
-        Returns:
-            Text: `Text` reference.
+        Returns
+        -------
+        Text
+            `Text` reference.
         """
         self._string.fg_color, self._string.bg_color = self._string.bg_color, self._string.fg_color  # noqa
         return self
 
     def render(self, matrix):
-        """
-        Renders text on matrix `matrix`. Used for internal purposes only.
+        """Renders text on matrix `matrix`.
+        Used for internal purposes only.
         """
         self._string.render(matrix)
 
 
 class Bitmap(Renderable):
+    """Bitmap renderable on the Launchpad's surface.
+
+    Examples
+    --------
+    Render text on Launchpad's surface:
+        >>> lp.grid.render(Bitmap('path/to/bitmap'))
+
+    Print the text in the console:
+        >>> Bitmap('path/to/bitmap').print()
+    """
     def __init__(self,
                  filename, *,
                  fg_color=None,
                  bg_color=None):
         if not isinstance(filename, str):
             raise TypeError('Must be of type str.')
         if not filename:
@@ -259,54 +288,94 @@
                 f"filename='{os.path.basename(self.filename)}')")
 
     def __str__(self):
         return repr(self)
 
     @Renderable.bits.getter
     def bits(self):
+        """Bits.
+        """
         return self._bitmap.bits
 
     @Renderable.word_count.getter
     def word_count(self):
+        """Word count.
+        """
         return self._bitmap.word_count
 
     @property
     def filename(self):
+        """File name.
+        """
         return self._bitmap.filename
 
     @property
     def fg_color(self):
+        """Foreground color.
+        """
         return self._bitmap.fg_color
 
     @fg_color.setter
     def fg_color(self, color):
         self._bitmap.fg_color = RenderableColor(self, color)
 
     @property
     def bg_color(self):
+        """Background color.
+        """
         return self._bitmap.bg_color
 
     @bg_color.setter
     def bg_color(self, color):
         self._bitmap.bg_color = RenderableColor(self, color)
 
     def render(self, matrix):
+        """Renders text on matrix `matrix`.
+        Used for internal purposes only.
+        """
         self._bitmap.render(matrix)
 
     def print(self, *,
               one='X',
               zero=' '):
+        """Prints text on matrix surface. `one` is the marker
+        for an on bit (1) and `zero` is the marker for an off
+        bit (0).
+
+        Parameters
+        ----------
+        one : str
+            Character that represents 1.
+        zero : str
+            Character that represents 0.
+        """
         self._bitmap.print(one=one, zero=zero)
 
     def swap_colors(self):
         self._bitmap.fg_color, self._bitmap.bg_color = self._bitmap.bg_color, self._bitmap.fg_color  # noqa
         return self
 
 
 class Movie(Renderable):
+    """Movie renderable on the Launchpad's surface.
+
+    Examples
+    --------
+    Render text on Launchpad's surface:
+        >>> lp.grid.render(Movie('path/to/movie'))
+
+    Print the first from of the movie in the console:
+        >>> Movie('path/to/movie').print()
+
+    Play a movie on Launchpad's surface:
+        >>> lp.grid.render(Movie('path/to/movie').play())
+
+    Play movie on the console:
+        >>> Movie('path/to/movie').play().print()
+    """
     def __init__(self,
                  filename, *,
                  fg_color=None,
                  bg_color=None):
         if not isinstance(filename, str):
             raise TypeError('Must be of type str.')
         if not filename:
@@ -322,82 +391,133 @@
                 f"filename='{os.path.basename(self.filename)}')")
 
     def __str__(self):
         return repr(self)
 
     @Renderable.bits.getter
     def bits(self):
+        """Bits.
+        """
         return self._movie.bits
 
     @Renderable.word_count.getter
     def word_count(self):
+        """Word count.
+        """
         return self._movie.word_count
 
     @property
     def filename(self):
+        """File name.
+        """
         return self._movie.filename
 
     @property
     def fg_color(self):
+        """Foreground color.
+        """
         return self._movie.fg_color
 
     @fg_color.setter
     def fg_color(self, color):
         self._movie.fg_color = RenderableColor(self, color)
 
     @property
     def bg_color(self):
+        """Background color.
+        """
         return self._movie.bg_color
 
     @bg_color.setter
     def bg_color(self, color):
         self._movie.bg_color = RenderableColor(self, color)
 
     @property
     def framerate(self):
+        """Frame rate.
+        """
         return Framerate(self, self._movie)
 
     @property
     def frames(self):
+        """Frames.
+        """
         return self._movie.frames
 
     @property
     def first_frame(self):
+        """First frame.
+        """
         return self._movie.first_frame
 
     @property
     def last_frame(self):
+        """Last frame.
+        """
         return self._movie.last_frame
 
     @property
     def position(self):
+        """Position.
+        """
         return self._movie.position
 
     @position.setter
     def position(self, position):
         self._movie.position = position
 
     def render(self, matrix):
+        """Render on matrix `matrix`.
+        """
         self._movie.render(matrix)
 
     def play(self, *,
              count=None,
              cycle_func=None):
+        """Plays movie on the Launchpad's surface.
+
+        Parameters
+        ----------
+        count : int or None
+            Number of times to play movie.
+        cycle_func : callable or None
+            Function to be called each cycle.
+        """
         if cycle_func and not callable(cycle_func):
             raise ValueError("'cycle_func' must be callable.")
         self._movie.roll = MovieRoll(self._movie,
                                      int(self.framerate),
                                      cycle_func=cycle_func,
                                      count=count)
         return self
 
     def skip(self, frame_count=1):
+        """Skips a frame by `frame_count`.
+
+        Parameters
+        ----------
+        frame_count : int
+            Frame count.
+        """
         return self._movie.skip(frame_count, ref=self)
 
     def print(self, *,
               one='X',
               zero=' '):
+        """Prints text on matrix surface. `one` is the marker
+        for an on bit (1) and `zero` is the marker for an off
+        bit (0).
+
+        Parameters
+        ----------
+        one : str
+            Character that represents 1.
+        zero : str
+            Character that represents 0.
+        """
         self._movie.print(one=one, zero=zero)
 
     def swap_colors(self):
+        """Swaps colors.
+        """
         self._movie.fg_color, self._movie.bg_color = self._movie.bg_color, self._movie.fg_color  # noqa
         return self
```

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/_parser.py` & `lpminimk3-0.6.0/lpminimk3/graphics/_parser.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/_renderable.py` & `lpminimk3-0.6.0/lpminimk3/graphics/_renderable.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/_renderer.py` & `lpminimk3-0.6.0/lpminimk3/graphics/_renderer.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/_utils.py` & `lpminimk3-0.6.0/lpminimk3/graphics/_utils.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/bitmaps/smiley.bitmap.json` & `lpminimk3-0.6.0/lpminimk3/graphics/bitmaps/smiley.bitmap.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/glyphs/basic_latin.glyph.json` & `lpminimk3-0.6.0/lpminimk3/graphics/glyphs/basic_latin.glyph.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/movies/ping_pong.movie.json` & `lpminimk3-0.6.0/lpminimk3/graphics/movies/ping_pong.movie.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/render.py` & `lpminimk3-0.6.0/lpminimk3/graphics/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""
-Render script for rendering texts, bitmaps and movies.
+"""Renders texts, bitmaps and movies on the Launchpad's surface.
 """
 
 import json
 import sys
-from argparse import ArgumentParser, FileType
+from argparse import (ArgumentParser,
+                      FileType,
+                      RawDescriptionHelpFormatter)
 from lpminimk3 import find_launchpads, Mode
 from lpminimk3.graphics import Text, Bitmap, Movie
 
 
 def render_character(character,
                      *,
                      on_screen=False,
@@ -85,14 +86,16 @@
 
 def main(args=None):
     args = args if args else sys.argv[1:]
     try:
         parser = ArgumentParser(description="Render texts, bitmaps, "
                                             "and movies on the "
                                             "Launchpad Mini MK3")
+        parser = ArgumentParser(description=__doc__,
+                                formatter_class=RawDescriptionHelpFormatter)
 
         parser.add_argument("-c",
                             type=int,
                             metavar="COUNT",
                             help="Stop after looping COUNT times")
         parser.add_argument("-f",
                             type=FileType('r', encoding='latin-1'),
```

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/schema/bitmap.schema.json` & `lpminimk3-0.6.0/lpminimk3/graphics/schema/bitmap.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/schema/glyph.schema.json` & `lpminimk3-0.6.0/lpminimk3/graphics/schema/glyph.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/schema/movie.schema.json` & `lpminimk3-0.6.0/lpminimk3/graphics/schema/movie.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.1/lpminimk3/graphics/sync.py` & `lpminimk3-0.6.0/lpminimk3/graphics/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-"""
-Sync server for controlling connected Launchpad Mini MK3 clients.
+"""Syncs all Launchpad clients with LP Sketch.
+
+This script starts a sync server for controlling connected
+Launchpad Mini MK3 clients. All changes made with LP Sketch
+will immediately be reflected on the surface of connected
+clients if sync was successful.
 """
 
 import asyncio
 import websockets
 import json
 import sys
 from collections import namedtuple
-from argparse import ArgumentParser
+from argparse import (ArgumentParser,
+                      RawDescriptionHelpFormatter)
 from functools import partial
 from lpminimk3 import find_launchpads, Mode
 from lpminimk3.graphics import Frame
 
 
 _connected_clients = []
 
@@ -41,15 +46,16 @@
         lp.open()
         lp.mode = Mode.PROG
         lps.append(lp)
     return lps
 
 
 def init_parser(ip, port):
-    parser = ArgumentParser(description="Sync server for lpminimk3")
+    parser = ArgumentParser(description=__doc__,
+                            formatter_class=RawDescriptionHelpFormatter)
     parser.add_argument("-a",
                         "--all",
                         action="store_true",
                         help="Listen for all hosts (on 0.0.0.0)")
     parser.add_argument("-i",
                         "--ip",
                         help=f"IP to serve on (Default: {ip})")
```

### Comparing `lpminimk3-0.5.1/lpminimk3/match.py` & `lpminimk3-0.6.0/lpminimk3/match.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-"""
-Match MIDI messages with incoming MIDI events.
+"""Collection of classes for matching MIDI messages with incoming MIDI events.
 """
 
 from abc import ABC
 from .midi_messages import Lighting, Constants
 
 
 class Match(ABC):
-    """
-    A set of rules for filtering MIDI events.
+    """A set of rules for filtering MIDI events.
     """
 
     def contains(self, message):
         return False
 
 
 class ButtonMatch(Match):
-    """
-    A set of rules for filtering button events.
+    """A set of rules for filtering button events.
     """
 
     def __init__(self, buttons, type):
         self._buttons = buttons
         self._type = type.lower().replace('|', '_')
 
     def contains(self, message):
-        """
-        Returns `True` if message `message` is a valid button
+        """Returns `True` if message `message` is a valid button
         message, otherwise returns `False`.
+
+        Returns
+        -------
+        Boolean
+            `True` if provided message is a valid
+            button message, otherwise `False`.
         """
         button_messages = self._determine_messages()
         for button_message in button_messages:
             if message == button_message:
                 return True
         return False
```

### Comparing `lpminimk3-0.5.1/lpminimk3/midi_messages.py` & `lpminimk3-0.6.0/lpminimk3/midi_messages.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,58 @@
-"""
-MIDI messages for the Launchpad Mini MK3.
+"""MIDI messages for the Launchpad Mini MK3.
 """
 
 from abc import ABC
 from functools import reduce
 
 
 class SysExMessages:
+    """SysEx messages.
+    """
     DEVICE_INQUIRY = [0xf0, 0x7e, 0xe7, 0xf0, 0x06, 0x01, 0xf7]
 
     class Interfaces:
+        """SysEx Interface messages.
+        """
         DAW = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x10, 0x00, 0xf7]
         MIDI = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x10, 0x01, 0xf7]
         READBACK = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x10, 0xf7]
 
     class Layouts:
+        """SysEx Layout messages.
+        """
         SESSION = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0x00, 0xf7]
         CUSTOM_1 = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0x04, 0xf7]
         CUSTOM_2 = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0x05, 0xf7]
         CUSTOM_3 = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0x06, 0xf7]
         DAW_FADERS = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0x0d, 0xf7]
         PROG = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0x7f, 0xf7]
         READBACK = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x00, 0xf7]
 
     class Modes:
+        """SysEx Mode messages.
+        """
         LIVE = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x0e, 0x00, 0xf7]
         PROG = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x0e, 0x01, 0xf7]
         READBACK = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x0e, 0xf7]
 
 
 class MidiMessage(ABC):
+    """MIDI message.
+    """
     @property
     def data(self):
+        """Data.
+        """
         return []
 
 
 class Constants:
+    """Constants.
+    """
     DEFAULT_COLOR_ID = 9
     MIDI_MIN_VALUE = 0
     MIDI_MAX_VALUE = 0x7f
 
     class LightingMode:
         OFF = 0x80
         STATIC = 0x90
@@ -53,26 +66,37 @@
 
     class MidiWord:
         NOTE_HEADER = 0x90
         CC_HEADER = 0xb0
 
 
 class ColorspecFragment:
+    """Colorspec fragment.
+    """
     def __init__(self, lighting_type, led_index, *lighting_data):
         self._lighting_type = lighting_type
         self._led_index = led_index
         self._lighting_data = list(lighting_data)
 
     @property
     def data(self):
+        """Data.
+        """
         return ([self._lighting_type,
                 self._led_index]
                 + self._lighting_data)
 
     def append(self, lighting_data):
+        """Append lighting data `lighting_data`.
+
+        Parameters
+        ----------
+        lighting_data : list of int
+            Lighting data.
+        """
         self._lighting_data.extend(lighting_data)
 
     def __repr__(self):
         return ('ColorspecFragment('
                 f'lighting_type={self._lighting_type}, '
                 f'led_index={self._led_index}, '
                 f'lighting_data={self._lighting_data})')
@@ -80,58 +104,83 @@
     def __str__(self):
         fragment_str = str([self._lighting_type, self._led_index]
                            + list(self._lighting_data))
         return fragment_str
 
 
 class Colorspec(MidiMessage):
+    """Colorspec MIDI message.
+    """
     def __init__(self, *fragments):
         self._start_clause = [0xf0, 0x00, 0x20, 0x29, 0x02, 0x0d, 0x03]
         self._fragments = list(fragments)
         self._end_clause = [0xf7]
 
     @MidiMessage.data.getter
     def data(self):
+        """Data.
+        """
         payload = list(reduce(lambda data, fragment: data + fragment.data,
                               self._fragments, []))  # noqa
         return (self._start_clause
                 + payload
                 + self._end_clause)
 
     def append(self, fragment):
+        """Append fragment to colorspec.
+
+        Parameters
+        ----------
+        fragment : ColorspecFragment
+            Colorspec fragment.
+
+        See Also
+        --------
+        ColorspecFragment
+        """
         if not isinstance(fragment, ColorspecFragment):
             raise ValueError('Must be a ColorspecFragment.')
         self._fragments.append(fragment)
 
     def __repr__(self):
         return f'Colorspec({self.data})'
 
 
 class Lighting(MidiMessage):
+    """Lighting MIDI message.
+    """
     def __init__(self, lighting_mode, midi_value, color_id):
         self._lighting_mode = lighting_mode
         self._midi_value = midi_value
         self._color_id = color_id
 
     def __repr__(self):
         return ('Lighting('
                 f'lighting_mode={self._lighting_mode}, '
                 f'midi_value={self._midi_value}, '
                 f'color_id={self.color_id})')
 
     @MidiMessage.data.getter
     def data(self):
+        """Data.
+        """
         return [self._lighting_mode,
                 self._midi_value,
                 self._color_id]
 
     @property
     def lighting_mode(self):
+        """Lighting mode.
+        """
         return self._lighting_mode
 
     @property
     def midi_value(self):
+        """MIDI value.
+        """
         return self._midi_value
 
     @property
     def color_id(self):
+        """Color ID.
+        """
         return self._color_id
```

### Comparing `lpminimk3-0.5.1/lpminimk3/region.py` & `lpminimk3-0.6.0/lpminimk3/region.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-Region of LEDs on a matrix.
+"""Region of LEDs on a matrix.
 """
 
 from abc import ABC
 
 
 class Region(ABC):
-    """
-    A collection of LEDs on a matrix.
+    """A collection of LEDs on a matrix.
     """
 
     def __len__(self):
         return len(self.button_names)
 
     @property
     def button_names(self):
-        """
-        Button names for region.
+        """Button names for region.
         """
         pass
 
 
 class Labeled(Region):
-    """
-    All labeled buttons on a panel.
+    """All labeled buttons on a panel.
     """
 
     @Region.button_names.getter
     def button_names(self):
+        """Button names for labeled region.
+        """
         return ['up',
                 'down',
                 'left',
                 'right',
                 'session',
                 'drums',
                 'keys',
```

### Comparing `lpminimk3-0.5.1/lpminimk3.egg-info/PKG-INFO` & `lpminimk3-0.6.0/lpminimk3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpminimk3
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python API for the Novation Launchpad Mini MK3
 Home-page: https://github.com/obeezzy/lpminimk3
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpminimk3
 Python API for the [Novation Launchpad Mini MK3](https://novationmusic.com/en/launch/launchpad-mini)
 
 [![CI](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml)
-[![CD](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.3.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Documentation Status](https://readthedocs.org/projects/lpminimk3/badge/?version=latest)](https://lpminimk3.readthedocs.io/en/latest/?badge=latest)
 
 The goals of this project are as follows:
 * Intuitive, object-oriented design
 * Convenient for use in script and shell
 * Access to all (or most) of the Launchpad Mini MK3 MIDI features
 
 
@@ -37,16 +38,15 @@
 
 ## Usage example
 Make sure your Launchpad is connected to your computer.
 
 ### In script
 Control LEDs individually:
 ```python
-"""
-Display a random array of colors for 5 seconds.
+"""Display a random array of colors for 5 seconds.
 """
 
 from lpminimk3 import Mode, find_launchpads
 import random
 import time
 
 lp = find_launchpads()[0]  # Get the first available launchpad
@@ -60,16 +60,15 @@
 time.sleep(5)  # Keep LEDs on for a while
 
 for led in lp.panel.led_range():
     del led.color  # Turn off LED
 ```
 Render text on Launchpad's surface:
 ```python
-"""
-Scroll text from right to left across the Launchpad's surface.
+"""Scroll text from right to left across the Launchpad's surface.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
@@ -92,15 +91,15 @@
 >>> lp.open()
 ```
 Query the device to ensure we can read and write to it:
 ```python
 >>> lp.device_inquiry()  # Query device
 MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=150.938086752)
 ```
-Switch to `programmer` mode to start manipulating button LEDs.
+Switch to `programmer` mode to start manipulating button LEDs:
 ```python
 >>> lp.mode = 'prog'  # Switch to programmer mode
 >>> lp.grid.led('0x0').color = 10  # Set color to yellow (Valid values: 0 - 127)
 >>> lp.grid.led(1,0).color = lpminimk3.colors.ColorPalette.Red.SHADE_1  # Set from palette
 >>> lp.panel.led('logo').color = 'violet'  # Set logo LED color to violet
 >>> lp.panel.led('drums').color = 'green2'  # Set 'Drums' LED color to second shade of green
 >>> lp.panel.led('stop').color = 'w1'  # Set 'Stop/Solo/Mute' LED color to first shade of white
@@ -109,15 +108,15 @@
 >>> lp.panel.led('scene_launch_1').color = '#ff0000'  # Set color to red using hex
 >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)  # Set color to blue using rgb
 >>> lp.panel.led('mute').color = 0  # Turn off LED
 >>> lp.panel.led('logo').reset()  # Another way to turn off LED
 >>> del lp.panel.led('stop').color  # Another way to turn off LED
 ```
 Note in the above snippet that `lp.grid` only contains the __*grid*__ buttons
-(i.e. the faceless white buttons) and `lp.panel` contains all buttons
+(i.e. the translucent, faceless buttons) and `lp.panel` contains all buttons
 (including the __*logo*__ LED at the top right corner).  
 
 Wait for and respond to button presses and releases:
 ```python
 >>> ev = lp.panel.buttons().poll_for_event()  # Block until any button is pressed/released
 >>> ev
 ButtonEvent(button='7x5', type='press', deltatime=0.0)
@@ -130,14 +129,15 @@
 ```
 Pass button names as arguments to wait for specific button events:
 ```python
 >>> lp.panel.buttons('up', '0x0', 'stop').poll_for_event()
 ```
 Render `A` on Launchpad's surface:
 ```python
+>>> from lpminimk3.graphics import Text
 >>> lp.grid.render(Text('A'))
 ```
 Print `A` in console:
 ```python
 >>> Text('A').print()
   XX    
  XXXX   
@@ -162,32 +162,30 @@
 $ python -m lpminimk3.graphics.sync
 ```
 Once the server is running, visit the [LP Sketch](https://www.github.com/obeezzy/lpsketch) website to start creating bitmaps and movies live.
 
 ### Rendering bitmaps and movies
 Render `smiley.bitmap.json` on Launchpad's surface:
 ```python
-"""
-Render "Smiley" bitmap.
+"""Render "Smiley" bitmap.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Bitmap
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
 lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))  # Display bitmap
 ```
 Render `ping_pong.movie.json` on Launchpad's surface:
 ```python
-"""
-Render "Ping/Pong" movie.
+"""Render "Ping/Pong" movie.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Movie
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
```

### Comparing `lpminimk3-0.5.1/lpminimk3.egg-info/SOURCES.txt` & `lpminimk3-0.6.0/lpminimk3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 lpminimk3/__init__.py
 lpminimk3/__version__.py
-lpminimk3/_lpminimk3.py
+lpminimk3/_logging.py
+lpminimk3/components.py
+lpminimk3/device.py
 lpminimk3/match.py
 lpminimk3/midi_messages.py
 lpminimk3/region.py
+lpminimk3/utils.py
 lpminimk3.egg-info/PKG-INFO
 lpminimk3.egg-info/SOURCES.txt
 lpminimk3.egg-info/dependency_links.txt
 lpminimk3.egg-info/requires.txt
 lpminimk3.egg-info/top_level.txt
-lpminimk3/_core/__init__.py
-lpminimk3/_core/components.py
-lpminimk3/_core/logging.py
-lpminimk3/_core/utils.py
 lpminimk3/colors/__init__.py
 lpminimk3/colors/_colors.py
 lpminimk3/examples/__init__.py
 lpminimk3/examples/display_character.py
 lpminimk3/examples/flash.py
 lpminimk3/examples/hello.py
 lpminimk3/examples/light_on_push.py
@@ -30,17 +29,16 @@
 lpminimk3/examples/text_scroll_region.py
 lpminimk3/graphics/__init__.py
 lpminimk3/graphics/_graphics.py
 lpminimk3/graphics/_parser.py
 lpminimk3/graphics/_renderable.py
 lpminimk3/graphics/_renderer.py
 lpminimk3/graphics/_utils.py
+lpminimk3/graphics/art.py
 lpminimk3/graphics/render.py
 lpminimk3/graphics/sync.py
-lpminimk3/graphics/art/__init__.py
-lpminimk3/graphics/art/_art.py
 lpminimk3/graphics/bitmaps/smiley.bitmap.json
 lpminimk3/graphics/glyphs/basic_latin.glyph.json
 lpminimk3/graphics/movies/ping_pong.movie.json
 lpminimk3/graphics/schema/bitmap.schema.json
 lpminimk3/graphics/schema/glyph.schema.json
 lpminimk3/graphics/schema/movie.schema.json
```

### Comparing `lpminimk3-0.5.1/setup.py` & `lpminimk3-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="lpminimk3",
-    version="0.5.1",
+    version="0.6.0",
     description="Python API for the Novation Launchpad Mini MK3",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/lpminimk3",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

