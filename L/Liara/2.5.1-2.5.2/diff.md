# Comparing `tmp/Liara-2.5.1.tar.gz` & `tmp/Liara-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liara-2.5.1.tar", last modified: Fri Feb 24 19:07:54 2023, max compression
+gzip compressed data, was "Liara-2.5.2.tar", last modified: Sat Apr 15 11:41:51 2023, max compression
```

## Comparing `Liara-2.5.1.tar` & `Liara-2.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-02-24 19:07:54.183312 Liara-2.5.1/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.1/LICENSE.txt
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-02-24 19:07:54.173312 Liara-2.5.1/Liara.egg-info/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-02-24 19:07:54.000000 Liara-2.5.1/Liara.egg-info/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-02-24 19:07:54.000000 Liara-2.5.1/Liara.egg-info/SOURCES.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-02-24 19:07:54.000000 Liara-2.5.1/Liara.egg-info/dependency_links.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-02-24 19:07:54.000000 Liara-2.5.1/Liara.egg-info/entry_points.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-02-24 19:07:54.000000 Liara-2.5.1/Liara.egg-info/requires.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-02-24 19:07:54.000000 Liara-2.5.1/Liara.egg-info/top_level.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-02-24 19:07:54.183312 Liara-2.5.1/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.1/README.md
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-02-24 19:07:54.183312 Liara-2.5.1/liara/
--rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29290 2023-02-24 19:07:41.000000 Liara-2.5.1/liara/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/actions.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    10363 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/cmdline.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/config.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/feeds.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    10879 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    31982 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/nodes.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-02-24 19:07:54.183312 Liara-2.5.1/liara/plugins/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/plugins/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      881 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/plugins/has_pending_document.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1318 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/plugins/series_schedule.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/publish.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/quickstart.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.1/liara/server.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.1/liara/signals.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    28232 2023-02-24 19:07:41.000000 Liara-2.5.1/liara/site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/util.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.1/liara/yaml.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.1/pyproject.toml
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-02-24 19:07:54.183312 Liara-2.5.1/setup.cfg
--rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.1/setup.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-02-24 19:07:54.183312 Liara-2.5.1/test/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.1/test/test_cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1118 2023-02-11 11:15:23.000000 Liara-2.5.1/test/test_md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.1/test/test_nodes.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.1/test/test_query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.1/test/test_site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.1/test/test_template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.1/test/test_util.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.2/LICENSE.txt
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/Liara.egg-info/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/SOURCES.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/dependency_links.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/entry_points.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/requires.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/top_level.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-15 11:41:51.566908 Liara-2.5.2/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.2/README.md
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/liara/
+-rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29291 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/actions.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    10367 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/cmdline.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/config.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/feeds.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    10536 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    31982 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/nodes.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/liara/plugins/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/plugins/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/plugins/has_pending_document.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/plugins/series_schedule.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/publish.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/quickstart.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.2/liara/server.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/signals.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    28210 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/util.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/yaml.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.2/pyproject.toml
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-04-15 11:41:51.566908 Liara-2.5.2/setup.cfg
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.2/setup.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/test/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1118 2023-02-11 11:15:23.000000 Liara-2.5.2/test/test_md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.2/test/test_nodes.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.2/test/test_query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_util.py
```

### Comparing `Liara-2.5.1/LICENSE.txt` & `Liara-2.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/Liara.egg-info/PKG-INFO` & `Liara-2.5.2/Liara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liara
-Version: 2.5.1
+Version: 2.5.2
 Summary: Static page generator
 Home-page: http://shelter13.net/projects/Liara
 Author: Matthäus G. Chajdas
 Author-email: dev@anteru.net
 License: BSD 2-Clause License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Liara-2.5.1/Liara.egg-info/SOURCES.txt` & `Liara-2.5.2/Liara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/PKG-INFO` & `Liara-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liara
-Version: 2.5.1
+Version: 2.5.2
 Summary: Static page generator
 Home-page: http://shelter13.net/projects/Liara
 Author: Matthäus G. Chajdas
 Author-email: dev@anteru.net
 License: BSD 2-Clause License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Liara-2.5.1/liara/__init__.py` & `Liara-2.5.2/liara/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     _process_node_sync
 )
 
 from .cache import Cache, FilesystemCache, NullCache, Sqlite3Cache, RedisCache
 from .util import FilesystemWalker, flatten_dictionary
 from .yaml import load_yaml
 
-__version__ = '2.5.1'
+__version__ = '2.5.2'
 __all__ = [
     'actions',
     'cache',
     'cmdline',
     'config',
     'feeds',
     'md',
@@ -196,15 +196,15 @@
 
     def __setup_cache(self) -> None:
         # Deprecated since version 2.2
         cache_directory = self.__configuration.get('build.cache_directory')
         if cache_directory:
             self.__log.warning(
                 "'build.cache_directory' is deprecated. Please "
-                "use build.cache.<cache_type>.directory' instead.")
+                "use 'build.cache.<cache_type>.directory' instead.")
             cache_directory = pathlib.Path(cache_directory)
 
         # Deprecated since version 2.2
         cache_type = self.__configuration.get('build.cache_type')
         if cache_type:
             self.__log.warning(
                 "'build.cache_type' is deprecated. Please use "
```

### Comparing `Liara-2.5.1/liara/actions.py` & `Liara-2.5.2/liara/actions.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/cache.py` & `Liara-2.5.2/liara/cache.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/cmdline.py` & `Liara-2.5.2/liara/cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     env.config = config
 
 
 def main():
     from .signals import commandline_prepared
 
     Liara.setup_plugins()
-    commandline_prepared.send(cli)
+    commandline_prepared.send(cli=cli)
     cli()
 
 
 def _create_liara(config):
     if os.path.exists(config):
         return Liara(config)
     else:
```

### Comparing `Liara-2.5.1/liara/config.py` & `Liara-2.5.2/liara/config.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/feeds.py` & `Liara-2.5.2/liara/feeds.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/md.py` & `Liara-2.5.2/liara/md.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,25 @@
     title will be provided by a template. This processor replaces each heading
     with the next-lower heading, and adds a ``demoted`` class.
     """
     def run(self, root):
         return self._demote_header(root)
 
     def _demote_header(self, element):
-        if element.tag == 'h1':
-            element.tag = 'h2'
-            element.set('class', 'demoted')
-        elif element.tag == 'h2':
-            element.tag = 'h3'
-            element.set('class', 'demoted')
-        elif element.tag == 'h3':
-            element.tag = 'h4'
-            element.set('class', 'demoted')
-        elif element.tag == 'h4':
-            element.tag = 'h5'
-            element.set('class', 'demoted')
-        elif element.tag == 'h5':
-            element.tag = 'h6'
-            element.set('class', 'demoted')
-        elif element.tag == 'h6':
-            element.tag = 'h6'
+        _demotions = {
+            'h1': 'h2',
+            'h2': 'h3',
+            'h3': 'h4',
+            'h4': 'h5',
+            'h5': 'h6',
+            'h6': 'h6',
+        }
+
+        if demotion := _demotions.get(element.tag):
+            element.tag = demotion
             element.set('class', 'demoted')
 
         for e in element:
             self._demote_header(e)
 
 
 class ShortcodeException(Exception):
```

### Comparing `Liara-2.5.1/liara/nodes.py` & `Liara-2.5.2/liara/nodes.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/plugins/has_pending_document.py` & `Liara-2.5.2/liara/plugins/has_pending_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from liara import signals
 
 
 def register():
     signals.commandline_prepared.connect(_register_cli)
 
 
-def _register_cli(cli):
+def _register_cli(sender, cli):
     from liara.cmdline import pass_environment
     import sys
 
     @cli.command()
     @pass_environment
     def has_pending_document(env):
         """Check if there is a pending document.
```

### Comparing `Liara-2.5.1/liara/plugins/series_schedule.py` & `Liara-2.5.2/liara/plugins/series_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import click
 
 
 def register():
     signals.commandline_prepared.connect(_register_cli)
 
 
-def _register_cli(cli):
+def _register_cli(sender, cli):
     from liara.cmdline import pass_environment
     import sys
 
     @cli.command()
     @click.argument('series')
     @click.option('--day-only', default=False)
     @pass_environment
```

### Comparing `Liara-2.5.1/liara/publish.py` & `Liara-2.5.2/liara/publish.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/query.py` & `Liara-2.5.2/liara/query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/quickstart.py` & `Liara-2.5.2/liara/quickstart.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/server.py` & `Liara-2.5.2/liara/server.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/signals.py` & `Liara-2.5.2/liara/signals.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/site.py` & `Liara-2.5.2/liara/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,20 +164,21 @@
             else:
                 reverse = False
 
             def key_fun(node):
                 accessor = _create_metadata_accessor(ordering)
                 result = accessor(node)
                 if result is None:
-                    logging.error('Node "%s" is missing the metadata '
-                                  'field "%s" which is required by a '
-                                  'order_by statement. Use exclude_without to '
-                                  'excludes nodes which miss certain metadata '
-                                  'fields.',
-                                  node.path, ordering)
+                    self.__log.error(
+                        'Node "%s" is missing the metadata '
+                        'field "%s" which is required by a '
+                        'order_by statement. Use exclude_without to '
+                        'excludes nodes which miss certain metadata '
+                        'fields.',
+                        node.path, ordering)
                     raise Exception(f'Cannot order collection "{self.__name}" '
                                     f'by key "{ordering}"')
                 return result
 
             nodes = sorted(nodes, key=key_fun, reverse=reverse)
 
         # Need to convert to a list here, as we're going to iterate over it
```

### Comparing `Liara-2.5.1/liara/template.py` & `Liara-2.5.2/liara/template.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/util.py` & `Liara-2.5.2/liara/util.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/liara/yaml.py` & `Liara-2.5.2/liara/yaml.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/setup.cfg` & `Liara-2.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/test/test_md.py` & `Liara-2.5.2/test/test_md.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/test/test_nodes.py` & `Liara-2.5.2/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/test/test_query.py` & `Liara-2.5.2/test/test_query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/test/test_site.py` & `Liara-2.5.2/test/test_site.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/test/test_template.py` & `Liara-2.5.2/test/test_template.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.1/test/test_util.py` & `Liara-2.5.2/test/test_util.py`

 * *Files identical despite different names*

