# Comparing `tmp/optibot-0.0.1.tar.gz` & `tmp/optibot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optibot-0.0.1.tar", last modified: Mon Apr 10 17:50:44 2023, max compression
+gzip compressed data, was "optibot-0.0.2.tar", last modified: Sat Apr 15 02:14:34 2023, max compression
```

## Comparing `optibot-0.0.1.tar` & `optibot-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-10 17:50:44.268463 optibot-0.0.1/
--rw-r--r--   0 pedro      (501) staff       (20)     1878 2023-04-10 17:50:44.268323 optibot-0.0.1/PKG-INFO
--rw-r--r--   0 pedro      (501) staff       (20)     1476 2023-04-10 17:45:37.000000 optibot-0.0.1/README.md
--rw-r--r--   0 pedro      (501) staff       (20)      104 2023-04-10 17:39:21.000000 optibot-0.0.1/pyproject.toml
--rw-r--r--   0 pedro      (501) staff       (20)       38 2023-04-10 17:50:44.268509 optibot-0.0.1/setup.cfg
--rw-r--r--   0 pedro      (501) staff       (20)      719 2023-04-10 17:38:55.000000 optibot-0.0.1/setup.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-10 17:50:44.266059 optibot-0.0.1/src/
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-10 17:50:44.266667 optibot-0.0.1/src/optibot/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2023-04-10 17:33:11.000000 optibot-0.0.1/src/optibot/__init__.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-10 17:50:44.268106 optibot-0.0.1/src/optibot/core/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2023-04-10 17:32:51.000000 optibot-0.0.1/src/optibot/core/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     5791 2023-04-10 17:32:51.000000 optibot-0.0.1/src/optibot/core/optibot.py
--rw-r--r--   0 pedro      (501) staff       (20)     4262 2023-04-10 17:32:51.000000 optibot-0.0.1/src/optibot/core/renderer.py
--rw-r--r--   0 pedro      (501) staff       (20)      902 2023-04-10 17:32:51.000000 optibot-0.0.1/src/optibot/core/script.py
--rw-r--r--   0 pedro      (501) staff       (20)     1534 2023-04-10 17:32:51.000000 optibot-0.0.1/src/optibot/core/splinter.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-10 17:50:44.267137 optibot-0.0.1/src/optibot.egg-info/
--rw-r--r--   0 pedro      (501) staff       (20)     1878 2023-04-10 17:50:44.000000 optibot-0.0.1/src/optibot.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (501) staff       (20)      339 2023-04-10 17:50:44.000000 optibot-0.0.1/src/optibot.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (501) staff       (20)        1 2023-04-10 17:50:44.000000 optibot-0.0.1/src/optibot.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (501) staff       (20)        8 2023-04-10 17:50:44.000000 optibot-0.0.1/src/optibot.egg-info/top_level.txt
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-15 02:14:34.506504 optibot-0.0.2/
+-rw-r--r--   0 pedro      (501) staff       (20)     1876 2023-04-15 02:14:34.505871 optibot-0.0.2/PKG-INFO
+-rw-r--r--   0 pedro      (501) staff       (20)     1474 2023-04-14 16:27:45.000000 optibot-0.0.2/README.md
+-rw-r--r--   0 pedro      (501) staff       (20)      104 2023-04-10 17:39:21.000000 optibot-0.0.2/pyproject.toml
+-rw-r--r--   0 pedro      (501) staff       (20)       38 2023-04-15 02:14:34.506562 optibot-0.0.2/setup.cfg
+-rw-r--r--   0 pedro      (501) staff       (20)      719 2023-04-15 02:14:11.000000 optibot-0.0.2/setup.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-15 02:14:34.503057 optibot-0.0.2/src/
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-15 02:14:34.503593 optibot-0.0.2/src/optibot/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2023-04-10 17:33:11.000000 optibot-0.0.2/src/optibot/__init__.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-15 02:14:34.505629 optibot-0.0.2/src/optibot/core/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2023-04-10 17:32:51.000000 optibot-0.0.2/src/optibot/core/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)      167 2023-04-12 10:55:36.000000 optibot-0.0.2/src/optibot/core/constants.py
+-rw-r--r--   0 pedro      (501) staff       (20)      138 2023-04-12 10:55:36.000000 optibot-0.0.2/src/optibot/core/errors.py
+-rw-r--r--   0 pedro      (501) staff       (20)     6861 2023-04-12 10:55:36.000000 optibot-0.0.2/src/optibot/core/optibot.py
+-rw-r--r--   0 pedro      (501) staff       (20)     4656 2023-04-14 16:27:45.000000 optibot-0.0.2/src/optibot/core/renderer.py
+-rw-r--r--   0 pedro      (501) staff       (20)     1177 2023-04-14 16:27:45.000000 optibot-0.0.2/src/optibot/core/script.py
+-rw-r--r--   0 pedro      (501) staff       (20)     1726 2023-04-12 10:55:36.000000 optibot-0.0.2/src/optibot/core/splinter.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-04-15 02:14:34.504008 optibot-0.0.2/src/optibot.egg-info/
+-rw-r--r--   0 pedro      (501) staff       (20)     1876 2023-04-15 02:14:34.000000 optibot-0.0.2/src/optibot.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (501) staff       (20)      396 2023-04-15 02:14:34.000000 optibot-0.0.2/src/optibot.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (501) staff       (20)        1 2023-04-15 02:14:34.000000 optibot-0.0.2/src/optibot.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (501) staff       (20)        8 2023-04-15 02:14:34.000000 optibot-0.0.2/src/optibot.egg-info/top_level.txt
```

### Comparing `optibot-0.0.1/PKG-INFO` & `optibot-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optibot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A splinters to scripts generator
 Home-page: https://github.com/pypa/sampleproject
 Author: Zmee
 Author-email: mail.of.zmee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 {{ optiimport("from sklearn.ensemble import RandomForestClassifier")}}
 
 {{ optivar("model")}}
 {{ optivar("X")}}
 {{ optivar("y")}}
 
 {{ optiparam("n_estimators", "int", min=0, max=100) }}
-{{ optiparam("random_state", "float", min=0, max=40000) }}
+{{ optiparam("random_state", "int", min=0, max=40000) }}
 
 ---
 
 # Train a Lasso model with alpha=0.1
 {{model}} = RandomForestClassifier(n_estimators={{n_estimators}}, random_state={{random_state}})
 {{model}}.fit({{X}}, {{y}})
```

### Comparing `optibot-0.0.1/README.md` & `optibot-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {{ optiimport("from sklearn.ensemble import RandomForestClassifier")}}
 
 {{ optivar("model")}}
 {{ optivar("X")}}
 {{ optivar("y")}}
 
 {{ optiparam("n_estimators", "int", min=0, max=100) }}
-{{ optiparam("random_state", "float", min=0, max=40000) }}
+{{ optiparam("random_state", "int", min=0, max=40000) }}
 
 ---
 
 # Train a Lasso model with alpha=0.1
 {{model}} = RandomForestClassifier(n_estimators={{n_estimators}}, random_state={{random_state}})
 {{model}}.fit({{X}}, {{y}})
```

### Comparing `optibot-0.0.1/setup.py` & `optibot-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="optibot",
-    version="0.0.1",
+    version="0.0.2",
     author="Zmee",
     author_email="mail.of.zmee@gmail.com",
     description="A splinters to scripts generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={},
```

### Comparing `optibot-0.0.1/src/optibot/core/optibot.py` & `optibot-0.0.2/src/optibot/core/optibot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,66 @@
 import os
+import logging
 from glob import glob
 from jinja2 import Environment, BaseLoader
 from .splinter import Splinter
 from .script import Script
 from .renderer import Renderer
+from .errors import DuplicateIdError, MissingIdError, MissingMetaError
+from .constants import MAX_SIZE
 from random import randint
-from sys import maxsize
 
-MAX_SIZE = int(1e12)
 
 class OptiBot:
     def __init__(self):
         self.splinter_registry : dict[str, Splinter] = dict()
         self.script_registry : dict[str, Script] = dict()
         self.splinters_params = 0
         self.splinter_blocks = 0
 
     def preload_splinters_from_path(self, base_path):
         splinters_paths = glob(base_path)
 
         for splinter_path in splinters_paths:
             with open(splinter_path, "r") as fp:
-                splinter_parts = fp.read().split("---")
+                try:
+                    splinter = self.prepload_splinters_from_string(fp.read())
+                    self._register_splinter(splinter)
+                except MissingMetaError:
+                    logging.error(f"Missing meta splinter in {splinter_path}")
+                except MissingIdError:
+                    logging.error(f"Splinter id not defined in '{splinter_path}'")
+                except DuplicateIdError:
+                    logging.error(f"Splinter id {splinter.id} already exists. Duplicate found in {splinter_path}")
+                
+                    
+    def prepload_splinters_from_string(self, splinter_source) -> Splinter:
+        splinter_parts = splinter_source.split("---")
                 
-                if len(splinter_parts) < 2:
-                    raise SyntaxError(f"Missing meta splinter in {splinter_path}")
+        if len(splinter_parts) < 2:
+            raise MissingMetaError()
 
-                meta, source = splinter_parts[0], splinter_parts[1]
-                splinter = self._build_splinter(meta, source)
-                
-                if splinter.id is None:
-                    raise ValueError(f"Splinter id not defined in '{splinter_path}'")
-
-                if splinter.id in self.splinter_registry:
-                    raise ValueError(f"Splinter id {splinter.id} already exists. Duplicate found in {splinter_path}")
+        meta, source = splinter_parts[0], splinter_parts[1]
+        splinter = self._build_splinter(meta, source)
+        
+        return splinter
 
-                self.splinter_registry[splinter.id] = splinter
     
+    def _register_splinter(self, splinter: Splinter) -> None:
+
+        if splinter.id is None:
+            raise MissingIdError()
+
+        if splinter.id in self.splinter_registry:
+            raise DuplicateIdError()
+
+        self.splinter_registry[splinter.id] = splinter
+
     
-    def _build_splinter(self, splinter_meta, splinter_source):
+    def _build_splinter(self, splinter_meta, splinter_source) -> Splinter:
         splinter = Splinter()
         splinter.source = splinter_source
         env = Environment(loader=BaseLoader)
                 
         env.globals['optiid'] = splinter.optiid_handler
         env.globals['optidesc'] = splinter.optidesc_handler
         env.globals['optitask'] = splinter.optitask_handler
@@ -52,45 +70,55 @@
 
         rtemplate = env.from_string(splinter_meta)
         rtemplate.render()
         
         return splinter
 
     
-    def preload_templates_from_path(self, base_path):
+    def preload_scripts_from_path(self, base_path):
         scripts_path = glob(base_path)
 
         for script_path in scripts_path:
             with open(script_path, "r") as fp:
-                script_source = fp.read()
-                
-                script_id = os.path.basename(script_path)
-                script = self._build_script(script_source)
+                try:
+                    script_id = os.path.basename(script_path)
+                    script = self.preload_templates_from_string(fp.read())
                 
-                if script_id in self.script_registry:
-                    raise ValueError(f"Splinter id {script_id} already exists. Duplicate found in {script_path}")
+                    self._register_script(script_id, script)                
+                except DuplicateIdError:
+                    logging.error(f"Script id {script_id} already exists. Duplicate found in {script_path}")
 
-                self.script_registry[script_id] = script
+                
+    def preload_templates_from_string(self, script_source: str) -> Script:
+        script = self._build_script(script_source)
+        return script
     
 
+    def _register_script(self, script_id: str, script: Script) -> None:
+        if script_id in self.script_registry:
+            raise DuplicateIdError()
+
+        self.script_registry[script_id] = script
+
+
     def _build_script(self, script_source):
         script = Script(script_source)
 
         env = Environment(loader=BaseLoader)
                 
         env.globals['splinter'] = script.splinter_handler
         env.globals['imports'] = script.imports_handler
         
         rtemplate = env.from_string(script_source)   
         rtemplate.render()
 
         return script
 
 
-    def compile(self):
+    def compile(self) -> None:
         """
         Compiles the script registry by finding the most suitable splinters 
         for each script reference by signature and task.
         Raises ValueError if no suitable splinter is found
         """
 
         # Initialize two variables to keep track of total splinter params and blocks
@@ -133,18 +161,20 @@
                 # Update the total splinter params for each script
                 script.splinters_params += max_param_size
             
             self.splinters_params = max(self.splinters_params, script.splinters_params)
             self.splinter_blocks = max(self.splinter_blocks, script.splinter_blocks)
 
 
-    def generate_script(self):
+    def _generate_script(self):
         for x in range(self.splinter_blocks):
             yield randint(0, MAX_SIZE)
         for x in range(self.splinters_params):
             yield randint(-MAX_SIZE, MAX_SIZE)
     
+    def generate_script(self) -> list[int]:
+        return list(self._generate_script())
     
-    def render(self, script_id, sequence):
+    def render(self, script_id: str, sequence: list[int]):
 
         renderer = Renderer(self.script_registry[script_id], sequence, self.splinter_registry)
         return renderer.render()
```

### Comparing `optibot-0.0.1/src/optibot/core/renderer.py` & `optibot-0.0.2/src/optibot/core/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Optional
 from jinja2 import Environment, BaseLoader
 from .script import Script
 from .splinter import Splinter
+from .constants import MAX_SIZE
+from .constants import INT_TYPE, FLOAT_TYPE, STRING_TYPE
 from random import randint
 
 
 IMPORT_PLACEHOLDER = "##__IMPORTS__##"
 
 class Renderer():
 
@@ -25,21 +27,23 @@
         self.env.globals['splinter'] = self.splinter_handler
         self.env.globals['imports'] = self.imports_handler
         
         rendered_source = self.env.from_string(self.script.source).render()
 
         rendered_source = rendered_source.replace(IMPORT_PLACEHOLDER, "\n".join(self.imports_needed))
 
+        rendered_source = rendered_source.replace("    ", "\t")
+        
         return rendered_source
 
 
     def imports_handler(self):
         return IMPORT_PLACEHOLDER
 
-    def splinter_handler(self, ref_name, splinter_tasks, **kwargs):
+    def splinter_handler(self, ref_name, splinter_tasks, indent=0, **kwargs):
         ref = self.script.refs.get(ref_name)
 
         self.block_at += 1
         splinter_gene = self.script_sequence[self.block_at]
         splinter_gene = int(splinter_gene % len(ref.splinters))
 
         splinter_to_render = list(ref.splinters)[splinter_gene]
@@ -51,35 +55,45 @@
             render_params[var_name] = ref.vars[var_name]
 
         for param_name in splinter.params.keys():
             self.param_at += 1
             param_gene = self.script_sequence[self.script.splinter_blocks + self.param_at]
 
             render_params[param_name] = self.gene_to_value(param_gene, param_name, splinter)
-
-        rendererd_splinter = self.env.from_string(splinter.source) \
-            .render(**render_params)
         
+        source = splinter.source
+        if indent > 0:
+            tabs = "\t" * indent
+            source = source.strip().replace("\n", f"\n{tabs}")
+        
+        rendererd_splinter = self.env.from_string(source) \
+            .render(**render_params)
+
         self.imports_needed = self.imports_needed.union(splinter.imports)
 
         return rendererd_splinter
     
     def gene_to_value(self, value, param_name, splinter):
         param_type = splinter.params[param_name][1]
-        if param_type == "int":
+        opts = splinter.params[param_name][-1]
+
+        if "choices" in opts:
+            return self._gene_to_value_choices(value, param_name, splinter)
+
+        if param_type == INT_TYPE:
             return self._gene_to_value_int(value, param_name, splinter)
-        if param_type == "float":
+        if param_type == FLOAT_TYPE:
             return self._gene_to_value_float(value, param_name, splinter)
-        if param_type == "str":
-            return self._gene_to_value_str(value, param_name, splinter)
+        if param_type == STRING_TYPE:
+            return self._gene_to_value_choices(value, param_name, splinter)
+        
         
         return value
     
     def _gene_to_value_int(self, value, param_name, splinter):
-        from .optibot import MAX_SIZE
 
         opts = splinter.params[param_name][-1]
 
         lowest_possible = -MAX_SIZE
         highest_possible = MAX_SIZE
         max_range = highest_possible - lowest_possible
         original_delta = (value - lowest_possible) / max_range
@@ -93,15 +107,14 @@
         scaled_range = highest_possible - lowest_possible
         
         scaled_value = lowest_possible + (scaled_range * original_delta)
 
         return int(scaled_value)
 
     def _gene_to_value_float(self, value, param_name, splinter):
-        from .optibot import MAX_SIZE
 
         opts = splinter.params[param_name][-1]
 
         lowest_possible = -MAX_SIZE
         highest_possible = MAX_SIZE
         max_range = highest_possible - lowest_possible
         original_delta = (value - lowest_possible) / max_range
@@ -118,15 +131,14 @@
 
         scaled_range = highest_possible - lowest_possible
         
         scaled_value = lowest_possible + (scaled_range * original_delta)
 
         return scaled_value
 
-    def _gene_to_value_str(self, value, param_name, splinter):
-        from .optibot import MAX_SIZE
+    def _gene_to_value_choices(self, value, param_name, splinter):
 
         opts = splinter.params[param_name][-1]
         
         value = value % len(opts["choices"])
 
         return f'\"{opts["choices"][value]}\"'
```

### Comparing `optibot-0.0.1/src/optibot/core/splinter.py` & `optibot-0.0.2/src/optibot/core/splinter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import cached_property
+from .constants import KNOWN_PARAM_TYPES
 
 class Splinter:
     
     def __init__(self):
         self.id = None
         self.vars = dict()
         self.params = dict()
@@ -42,13 +43,15 @@
             raise ValueError(f"Splinter '{self.id}' already has var '{var_name}' defined ")
 
         self.vars[var_name] = (var_name, required)
 
     def optiparam_handler(self, param_name: str, param_type: str, param_values: list = None, **kwargs):
         if param_name in self.params:
             raise ValueError(f"Splinter '{self.id}' already has param '{param_name}' defined ")
-
+        if param_type not in KNOWN_PARAM_TYPES:
+            raise ValueError(f"Splinter '{self.id}' has an invalid param type '{param_type}'")
+        
         self.params[param_name] = (param_name, param_type, param_values, kwargs)
```

### Comparing `optibot-0.0.1/src/optibot.egg-info/PKG-INFO` & `optibot-0.0.2/src/optibot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optibot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A splinters to scripts generator
 Home-page: https://github.com/pypa/sampleproject
 Author: Zmee
 Author-email: mail.of.zmee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 {{ optiimport("from sklearn.ensemble import RandomForestClassifier")}}
 
 {{ optivar("model")}}
 {{ optivar("X")}}
 {{ optivar("y")}}
 
 {{ optiparam("n_estimators", "int", min=0, max=100) }}
-{{ optiparam("random_state", "float", min=0, max=40000) }}
+{{ optiparam("random_state", "int", min=0, max=40000) }}
 
 ---
 
 # Train a Lasso model with alpha=0.1
 {{model}} = RandomForestClassifier(n_estimators={{n_estimators}}, random_state={{random_state}})
 {{model}}.fit({{X}}, {{y}})
```

