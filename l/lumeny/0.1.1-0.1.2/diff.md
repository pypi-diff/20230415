# Comparing `tmp/lumeny-0.1.1.tar.gz` & `tmp/lumeny-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumeny-0.1.1.tar", max compression
+gzip compressed data, was "lumeny-0.1.2.tar", max compression
```

## Comparing `lumeny-0.1.1.tar` & `lumeny-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      652 2023-04-13 12:21:17.181246 lumeny-0.1.1/README.md
--rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.1.1/lumeny/CaldavConnector.py
--rw-r--r--   0        0        0     3765 2023-04-13 12:07:56.836601 lumeny-0.1.1/lumeny/CalendarInteraction.py
--rw-r--r--   0        0        0     1590 2023-04-13 12:16:45.567741 lumeny-0.1.1/lumeny/ConfigLoader.py
--rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.1.1/lumeny/EmbeddingGenerator.py
--rw-r--r--   0        0        0     3001 2023-04-13 12:18:41.544232 lumeny-0.1.1/lumeny/MinifluxConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.1.1/lumeny/QdrantConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.1.1/lumeny/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-13 12:19:59.795216 lumeny-0.1.1/lumeny/ai.py
--rw-r--r--   0        0        0     2003 2023-04-13 12:08:09.609342 lumeny-0.1.1/lumeny/cli.py
--rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.1.1/lumeny/tui.py
--rw-r--r--   0        0        0      912 2023-04-12 20:24:12.954146 lumeny-0.1.1/lumeny/utils.py
--rw-r--r--   0        0        0      623 2023-04-13 12:21:26.562312 lumeny-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 lumeny-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      652 2023-04-13 12:21:17.181246 lumeny-0.1.2/README.md
+-rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.1.2/lumeny/CaldavConnector.py
+-rw-r--r--   0        0        0     1590 2023-04-13 12:16:45.567741 lumeny-0.1.2/lumeny/ConfigLoader.py
+-rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.1.2/lumeny/EmbeddingGenerator.py
+-rw-r--r--   0        0        0     3001 2023-04-13 12:18:41.544232 lumeny-0.1.2/lumeny/MinifluxConnector.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.1.2/lumeny/QdrantConnector.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.1.2/lumeny/__init__.py
+-rw-r--r--   0        0        0     1675 2023-04-14 22:04:00.264026 lumeny-0.1.2/lumeny/ai.py
+-rw-r--r--   0        0        0     4864 2023-04-14 21:57:36.895011 lumeny-0.1.2/lumeny/calendar.py
+-rw-r--r--   0        0        0     1992 2023-04-14 12:09:46.339099 lumeny-0.1.2/lumeny/cli.py
+-rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.1.2/lumeny/tui.py
+-rw-r--r--   0        0        0      912 2023-04-12 20:24:12.954146 lumeny-0.1.2/lumeny/utils.py
+-rw-r--r--   0        0        0      645 2023-04-14 22:02:47.742081 lumeny-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 lumeny-0.1.2/PKG-INFO
```

### Comparing `lumeny-0.1.1/README.md` & `lumeny-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/lumeny/CaldavConnector.py` & `lumeny-0.1.2/lumeny/CaldavConnector.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/lumeny/ConfigLoader.py` & `lumeny-0.1.2/lumeny/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/lumeny/EmbeddingGenerator.py` & `lumeny-0.1.2/lumeny/EmbeddingGenerator.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/lumeny/MinifluxConnector.py` & `lumeny-0.1.2/lumeny/MinifluxConnector.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/lumeny/cli.py` & `lumeny-0.1.2/lumeny/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # cli.py
 import os
 import questionary as q
 import click
 from prompt_toolkit.lexers import PygmentsLexer
 from lumeny.utils import InputLexer
 # from lumen.tui import launch_tui
-from lumeny.CalendarInteraction import generate_command_with_gpt4
+from lumeny.calendar import generate_command_with_gpt4
 
 
 @click.group()
 def cli():
     pass
 
 @click.command()
```

### Comparing `lumeny-0.1.1/lumeny/tui.py` & `lumeny-0.1.2/lumeny/tui.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/lumeny/utils.py` & `lumeny-0.1.2/lumeny/utils.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.1/pyproject.toml` & `lumeny-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lumeny"
-version = "0.1.1"
+version = "0.1.2"
 description = "A cli and tui based personal management app for Lumen Young"
 authors = ["Lumen Young <pip@lumeny.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 caldav = "^1.2.1"
@@ -15,14 +15,15 @@
 qdrant-client = "^1.1.0"
 openai = "^0.27.2"
 docker = "^6.0.1"
 nltk = "^3.8.1"
 pyyaml = "^6.0"
 questionary = "^1.10.0"
 prompt-toolkit = "^3.0.38"
+dateparser = "^1.1.8"
 
 [tool.poetry.scripts]
 lumen = "lumeny.cli:cli"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lumeny-0.1.1/PKG-INFO` & `lumeny-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: lumeny
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cli and tui based personal management app for Lumen Young
 Author: Lumen Young
 Author-email: pip@lumeny.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: caldav (>=1.2.1,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-config-file (>=0.6.0,<0.7.0)
+Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: miniflux (>=0.0.15,<0.0.16)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qdrant-client (>=1.1.0,<2.0.0)
```

