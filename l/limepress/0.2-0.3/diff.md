# Comparing `tmp/limepress-0.2.tar.gz` & `tmp/limepress-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/limepress-0.2.tar", last modified: Fri Apr  7 12:39:08 2023, max compression
+gzip compressed data, was "limepress-0.3.tar", last modified: Sat Apr 15 10:33:43 2023, max compression
```

## Comparing `limepress-0.2.tar` & `limepress-0.3.tar`

### file list

```diff
@@ -1,38 +1,50 @@
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1071 2023-01-14 11:53:02.000000 limepress-0.2/LICENSE.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      120 2023-01-14 11:53:02.000000 limepress-0.2/MANIFEST.in
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1690 2023-04-07 12:39:08.000000 limepress-0.2/PKG-INFO
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      822 2023-01-14 11:53:02.000000 limepress-0.2/README.rst
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/bin/
--rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)     1043 2023-04-07 12:37:54.000000 limepress-0.2/bin/limepress
--rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)      397 2023-04-07 12:37:54.000000 limepress-0.2/bin/limepress-build
--rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)     4058 2023-04-07 12:37:54.000000 limepress-0.2/bin/limepress-dev-server
--rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)      380 2023-04-07 12:37:54.000000 limepress-0.2/bin/limepress-shell
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/limepress/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       68 2023-04-07 12:38:14.000000 limepress-0.2/limepress/__init__.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1741 2023-01-14 11:53:02.000000 limepress-0.2/limepress/build_environment.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1030 2023-04-07 12:37:54.000000 limepress-0.2/limepress/command_line.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    13535 2023-04-07 12:37:54.000000 limepress-0.2/limepress/context.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      841 2023-04-07 12:37:54.000000 limepress-0.2/limepress/default_settings.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2692 2023-04-07 12:37:54.000000 limepress-0.2/limepress/dependency_manager.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2882 2023-04-07 12:37:54.000000 limepress-0.2/limepress/file_system.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1475 2023-01-14 11:53:02.000000 limepress-0.2/limepress/parsing.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      320 2023-01-14 11:53:02.000000 limepress-0.2/limepress/plugin_manager.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/limepress/plugins/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-01-14 11:53:02.000000 limepress-0.2/limepress/plugins/__init__.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      695 2023-01-14 11:53:02.000000 limepress-0.2/limepress/plugins/html_parser.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1866 2023-04-07 12:37:54.000000 limepress-0.2/limepress/settings.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/limepress/templates/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      390 2023-01-14 11:53:02.000000 limepress-0.2/limepress/templates/page.html
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/limepress/templates/snippets/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       29 2023-01-14 11:53:02.000000 limepress-0.2/limepress/templates/snippets/pre.html
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     3660 2023-04-07 12:37:54.000000 limepress-0.2/limepress/templating.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     5105 2023-04-07 12:37:54.000000 limepress-0.2/limepress/unit.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-07 12:39:08.000000 limepress-0.2/limepress.egg-info/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1690 2023-04-07 12:39:08.000000 limepress-0.2/limepress.egg-info/PKG-INFO
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      727 2023-04-07 12:39:08.000000 limepress-0.2/limepress.egg-info/SOURCES.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        1 2023-04-07 12:39:08.000000 limepress-0.2/limepress.egg-info/dependency_links.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      118 2023-04-07 12:39:08.000000 limepress-0.2/limepress.egg-info/requires.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       10 2023-04-07 12:39:08.000000 limepress-0.2/limepress.egg-info/top_level.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      518 2023-04-07 12:39:08.000000 limepress-0.2/setup.cfg
--rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)      712 2023-04-07 12:38:08.000000 limepress-0.2/setup.py
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1071 2023-01-14 11:53:02.000000 limepress-0.3/LICENSE.txt
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      120 2023-01-14 11:53:02.000000 limepress-0.3/MANIFEST.in
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2981 2023-04-15 10:33:43.714642 limepress-0.3/PKG-INFO
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      822 2023-01-14 11:53:02.000000 limepress-0.3/README.rst
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.710642 limepress-0.3/bin/
+-rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)     1043 2023-04-12 18:57:53.000000 limepress-0.3/bin/limepress
+-rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)      397 2023-04-12 18:57:54.000000 limepress-0.3/bin/limepress-build
+-rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)     4058 2023-04-07 12:37:54.000000 limepress-0.3/bin/limepress-dev-server
+-rwxrwxr-x   0 fscherf   (1000) fscherf   (1000)      380 2023-04-07 12:37:54.000000 limepress-0.3/bin/limepress-shell
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/limepress/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       68 2023-04-15 10:32:50.000000 limepress-0.3/limepress/__init__.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1784 2023-04-15 10:32:27.000000 limepress-0.3/limepress/build_environment.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1030 2023-04-07 12:37:54.000000 limepress-0.3/limepress/command_line.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    14601 2023-04-15 10:32:27.000000 limepress-0.3/limepress/context.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      841 2023-04-11 20:19:30.000000 limepress-0.3/limepress/default_settings.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2692 2023-04-07 12:37:54.000000 limepress-0.3/limepress/dependency_manager.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2882 2023-04-07 12:37:54.000000 limepress-0.3/limepress/file_system.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1475 2023-01-14 11:53:02.000000 limepress-0.3/limepress/parsing.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      342 2023-04-15 10:32:27.000000 limepress-0.3/limepress/plugin_manager.py
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/limepress/plugins/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-01-14 11:53:02.000000 limepress-0.3/limepress/plugins/__init__.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      689 2023-04-15 10:32:27.000000 limepress-0.3/limepress/plugins/html_parser.py
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.710642 limepress-0.3/limepress/server/
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/limepress/server/views/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-01-14 11:53:02.000000 limepress-0.3/limepress/server/views/__init__.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-01-14 11:53:02.000000 limepress-0.3/limepress/server/views/limepress_console.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-01-14 11:53:02.000000 limepress-0.3/limepress/server/views/limepress_serve.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1866 2023-04-07 12:37:54.000000 limepress-0.3/limepress/settings.py
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/limepress/templates/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      390 2023-01-14 11:53:02.000000 limepress-0.3/limepress/templates/page.html
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/limepress/templates/snippets/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       29 2023-01-14 11:53:02.000000 limepress-0.3/limepress/templates/snippets/pre.html
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     3660 2023-04-07 12:37:54.000000 limepress-0.3/limepress/templating.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     5139 2023-04-15 10:32:27.000000 limepress-0.3/limepress/unit.py
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/limepress.egg-info/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2981 2023-04-15 10:33:43.000000 limepress-0.3/limepress.egg-info/PKG-INFO
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      998 2023-04-15 10:33:43.000000 limepress-0.3/limepress.egg-info/SOURCES.txt
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        1 2023-04-15 10:33:43.000000 limepress-0.3/limepress.egg-info/dependency_links.txt
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      143 2023-04-15 10:33:43.000000 limepress-0.3/limepress.egg-info/requires.txt
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       10 2023-04-15 10:33:43.000000 limepress-0.3/limepress.egg-info/top_level.txt
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1553 2023-04-15 10:32:43.000000 limepress-0.3/pyproject.toml
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       38 2023-04-15 10:33:43.714642 limepress-0.3/setup.cfg
+drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-04-15 10:33:43.714642 limepress-0.3/tests/
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1707 2023-01-14 11:53:02.000000 limepress-0.3/tests/test_context_setup.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2041 2023-04-15 10:32:27.000000 limepress-0.3/tests/test_file_copy.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       49 2023-01-14 11:53:02.000000 limepress-0.3/tests/test_package.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1201 2023-04-15 10:32:27.000000 limepress-0.3/tests/test_path_resolving.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2805 2023-04-15 10:32:27.000000 limepress-0.3/tests/test_rendering.py
+-rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1658 2023-01-14 11:53:02.000000 limepress-0.3/tests/test_unit_parsing.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `limepress-0.2/LICENSE.txt` & `limepress-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limepress-0.2/README.rst` & `limepress-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `limepress-0.2/bin/limepress` & `limepress-0.3/bin/limepress`

 * *Files identical despite different names*

### Comparing `limepress-0.2/bin/limepress-dev-server` & `limepress-0.3/bin/limepress-dev-server`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/build_environment.py` & `limepress-0.3/limepress/build_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,13 +48,14 @@
     def setup(self) -> None:
         self.context = LimepressContext(
             project_root=self.tmp_dir.name,
             settings_overrides=self.settings_overrides,
         )
 
     # helper ##################################################################
-    def build(self) -> None:
-        self.setup()
+    def build(self) -> int:
+        if self.context is None:
+            self.setup()
 
         assert self.context is not None
 
-        self.context.build()
+        return self.context.build()
```

### Comparing `limepress-0.2/limepress/command_line.py` & `limepress-0.3/limepress/command_line.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/context.py` & `limepress-0.3/limepress/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.dependency_manager: LimepressDependencyManager = \
             LimepressDependencyManager(context=self)
 
         self.build_dir: str = ''
         self.source_dirs: List[str] = []
         self.template_dirs: List[str] = []
         self.units: List[LimepressUnit] = []
+        self.errors: List[Exception] = []
 
         # setup
         self.logger.debug('setup context')
 
         self._load_settings()
         self._load_plugins()
         self._run_pre_setup_hook()
@@ -65,14 +66,26 @@
         self._discover_units()
 
         self.logger.debug('setup done')
 
     def __repr__(self) -> str:
         return f'<LimepressContext(project_root={self.project_root!r})>'  # NOQA
 
+    def _run_hook(self, *args, **kwargs):
+        if not self._plugin_manager:
+            raise RuntimeError('plugin manager is not initialized')
+
+        return_values = self._plugin_manager.run_hook(*args, **kwargs)
+
+        for return_value in return_values:
+            if isinstance(return_value, Exception):
+                self.errors.append(return_value)
+
+        return return_values
+
     # setup ###################################################################
     def _load_settings(self) -> None:
         self.logger.debug('load settings')
 
         self.settings = Settings()
 
         self.settings_paths = [
@@ -100,23 +113,23 @@
                 value = getattr(self.settings_overrides, key)
 
                 setattr(self.settings, key, value)
 
     def _load_plugins(self) -> None:
         self.logger.debug('load plugins')
 
-        self.plugin_manager = LimepressPluginManager()
+        self._plugin_manager = LimepressPluginManager()
 
-        self.plugin_manager.load([
+        self._plugin_manager.load([
             *self.settings.DEFAULT_PLUGINS,
             *self.settings.PLUGINS,
         ])
 
     def _run_pre_setup_hook(self) -> None:
-        self.plugin_manager.run_hook(
+        self._run_hook(
             hook_name='pre_setup',
             hook_args=[self],
         )
 
     def _load_template_dirs(self) -> None:
         self.logger.debug('load template dirs')
 
@@ -125,15 +138,15 @@
         # get template dirs from settings
         for template_dir in [*self.settings.TEMPLATE_DIRS,
                              *self.settings.DEFAULT_TEMPLATE_DIRS]:
 
             self.template_dirs.append(str(template_dir))
 
         # get template dirs from plugins
-        return_values = self.plugin_manager.run_hook(
+        return_values = self._run_hook(
             hook_name='get_template_dirs',
             hook_args=[self],
         )
 
         for return_value in return_values:
             self.template_dirs.extend(return_value)
 
@@ -153,15 +166,15 @@
         self.source_dirs.clear()
 
         # get source dirs from settings
         for source_dir in self.settings.SOURCE_DIRS:
             self.source_dirs.append(str(source_dir))
 
         # get source dirs from plugins
-        return_values = self.plugin_manager.run_hook(
+        return_values = self._run_hook(
             hook_name='get_source_dirs',
             hook_args=[self],
         )
 
         for return_value in return_values:
             self.source_dirs.extend(return_value)
 
@@ -195,15 +208,15 @@
             ),
         )
 
         # setup snippet extension
         self.jinja2_env.add_extension(LimepressSnippetTag)
 
     def _run_post_setup_hook(self) -> None:
-        self.plugin_manager.run_hook(
+        self._run_hook(
             hook_name='post_setup',
             hook_args=[self],
         )
 
     def _discover_units(self) -> None:
         self.logger.debug('discover units')
 
@@ -231,19 +244,25 @@
                 unit = self.gen_unit()
 
                 unit.abs_path = abs_path
                 unit.rel_path = rel_path
                 unit.output_rel_path = rel_path
 
                 # run plugin chain
-                self.plugin_manager.run_hook(
-                    hook_name='handle_unit_meta_data',
+                self._run_hook(
+                    hook_name='unit_discovered',
                     hook_args=[unit],
                 )
 
+        # run plugin chain (finish)
+        self._run_hook(
+            hook_name='units_discovered',
+            hook_args=[self],
+        )
+
     def _run_checks(self) -> None:
         # TODO
 
         pass
 
     # templating ##############################################################
     def gen_template_context(self, overrides: Dict[Any, Any] | None) -> dict:
@@ -326,15 +345,15 @@
 
         if os.path.exists(self.build_dir):
             clean_directory(self.build_dir)
 
     def _render_template_unit(self, unit: LimepressUnit) -> None:
 
         # run plugin hook 'render_unit'
-        self.plugin_manager.run_hook(
+        self._run_hook(
             hook_name='render_unit',
             hook_kwargs={
                 'unit': unit,
             },
         )
 
         # setup template context
@@ -342,38 +361,38 @@
             'unit': unit,
             'title': unit.title,
             'body_title': unit.body_title,
             'body_text': unit.body_text,
         })
 
         # pre render title
-        if(unit.meta.get('title_is_template', True) and
-           string_is_template(template_context['title'])):
+        if (unit.meta.get('title_is_template', True) and
+                string_is_template(template_context['title'])):
 
             template_context['title'] = self.render_template_string(
                 string=template_context['title'],
                 context={
                     'unit': unit,
                 },
             )
 
         # pre render body_title
-        if(unit.meta.get('body_title_is_template', True) and
-           string_is_template(template_context['body_title'])):
+        if (unit.meta.get('body_title_is_template', True) and
+                string_is_template(template_context['body_title'])):
 
             template_context['body_title'] = self.render_template_string(
                 string=template_context['body_title'],
                 context={
                     'unit': unit,
                 },
             )
 
         # pre render body_text
-        if(unit.meta.get('body_text_is_template', True) and
-           string_is_template(template_context['body_text'])):
+        if (unit.meta.get('body_text_is_template', True) and
+                string_is_template(template_context['body_text'])):
 
             template_context['body_text'] = self.render_template_string(
                 string=template_context['body_text'],
                 context={
                     'unit': unit,
                 },
             )
@@ -389,14 +408,33 @@
             path=self.gen_output_path(path=unit.output_rel_path),
             text=text,
         )
 
         # discard unit.body_text to save memory
         unit.body_text = ''
 
+    def _write_text_unit(self, unit: LimepressUnit) -> None:
+
+        # run plugin hook 'render_unit'
+        self._run_hook(
+            hook_name='render_unit',
+            hook_kwargs={
+                'unit': unit,
+            },
+        )
+
+        write_file(
+            root_dir='/',  # FIXME
+            path=self.gen_output_path(path=unit.output_rel_path),
+            text=unit.text,
+        )
+
+        # discard unit.text to save memory
+        unit.text = ''
+
     def _render_units(self) -> List[LimepressUnit]:
         self.logger.debug('rendering units')
 
         rendered_units: List[LimepressUnit] = []
         exception_raised: bool = False
 
         for unit in self.units:
@@ -410,16 +448,20 @@
             if not unit.dirty:
                 self.logger.debug('%s is not marked as dirty', unit)
 
                 continue
 
             try:
 
+                # text units
+                if unit.text:
+                    self._write_text_unit(unit=unit)
+
                 # template units
-                if unit.template:
+                elif unit.template:
                     self._render_template_unit(unit=unit)
 
                 # file units
                 else:
                     copy_files(
                         source=unit.abs_path,
                         destination=self.gen_output_path(
@@ -438,21 +480,21 @@
                 )
 
         if len(rendered_units) == 0 and not exception_raised:
             self.logger.info('nothing to do')
 
         return rendered_units
 
-    def build(self, clean: bool = False) -> List[LimepressUnit]:
+    def build(self, clean: bool = False) -> int:
         self.logger.debug('start build')
 
         if clean:
             self._clean_build_dir()
 
         else:
             self.dependency_manager.set_unchanged_units_not_dirty()
 
-        rendered_units = self._render_units()
+        self._render_units()
 
         self.logger.debug('build done')
 
-        return rendered_units
+        return len(self.errors)
```

### Comparing `limepress-0.2/limepress/default_settings.py` & `limepress-0.3/limepress/default_settings.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/dependency_manager.py` & `limepress-0.3/limepress/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/file_system.py` & `limepress-0.3/limepress/file_system.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/parsing.py` & `limepress-0.3/limepress/parsing.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/plugins/html_parser.py` & `limepress-0.3/limepress/plugins/html_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from bs4 import BeautifulSoup
 
 from limepress.unit import LimepressUnit
 
 
 class LimepressHtmlParser:
-    def handle_unit_meta_data(self, unit: LimepressUnit) -> None:
+    def unit_discovered(self, unit: LimepressUnit) -> None:
         if unit.get_file_extension() != 'html':
             return
 
         unit.set_default_template()
         unit.load_meta_data()
 
     def render_unit(self, unit: LimepressUnit) -> None:
```

### Comparing `limepress-0.2/limepress/settings.py` & `limepress-0.3/limepress/settings.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/templating.py` & `limepress-0.3/limepress/templating.py`

 * *Files identical despite different names*

### Comparing `limepress-0.2/limepress/unit.py` & `limepress-0.3/limepress/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # default attributes
     context: LimepressContext = field(repr=False)
     abs_path: str = field(default='')
     rel_path: str = field(default='')
     output_rel_path: str = field(default='')
     disabled: bool = field(default=False)
     dirty: bool = field(default=True)
+    text: str = field(default='')
 
     # templating
     template: str = field(default='')
     title: str = field(default='')
     body_title: str = field(default='')
     body_text: str = field(default='', repr=False)
```

