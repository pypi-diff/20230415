# Comparing `tmp/dbrief-0.1.1.tar.gz` & `tmp/dbrief-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrief-0.1.1.tar", last modified: Fri Mar 17 19:05:28 2023, max compression
+gzip compressed data, was "dbrief-0.1.2.tar", last modified: Sat Apr 15 02:02:39 2023, max compression
```

## Comparing `dbrief-0.1.1.tar` & `dbrief-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.515550 dbrief-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-17 19:05:11.000000 dbrief-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-17 19:05:11.000000 dbrief-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-17 19:05:11.000000 dbrief-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-17 19:05:28.515550 dbrief-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-17 19:05:11.000000 dbrief-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.511550 dbrief-0.1.1/dbrief/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-17 19:05:11.000000 dbrief-0.1.1/dbrief/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-17 19:05:11.000000 dbrief-0.1.1/dbrief/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.515550 dbrief-0.1.1/dbrief/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-17 19:05:11.000000 dbrief-0.1.1/dbrief/templates/default.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.515550 dbrief-0.1.1/dbrief.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-17 19:05:28.000000 dbrief-0.1.1/dbrief.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-17 19:05:28.000000 dbrief-0.1.1/dbrief.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:05:28.000000 dbrief-0.1.1/dbrief.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:05:28.000000 dbrief-0.1.1/dbrief.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-17 19:05:28.000000 dbrief-0.1.1/dbrief.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-17 19:05:28.000000 dbrief-0.1.1/dbrief.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.511550 dbrief-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.515550 dbrief-0.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-17 19:05:11.000000 dbrief-0.1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-17 19:05:11.000000 dbrief-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-17 19:05:11.000000 dbrief-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:05:28.515550 dbrief-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:28.515550 dbrief-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:11.000000 dbrief-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:05:11.000000 dbrief-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-15 02:02:22.000000 dbrief-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 02:02:22.000000 dbrief-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-15 02:02:22.000000 dbrief-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 02:02:39.795134 dbrief-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-15 02:02:22.000000 dbrief-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/dbrief/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 02:02:22.000000 dbrief-0.1.2/dbrief/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-15 02:02:22.000000 dbrief-0.1.2/dbrief/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/dbrief/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-15 02:02:22.000000 dbrief-0.1.2/dbrief/templates/default.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/dbrief.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 02:02:39.000000 dbrief-0.1.2/dbrief.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-15 02:02:39.000000 dbrief-0.1.2/dbrief.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:02:39.000000 dbrief-0.1.2/dbrief.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:02:39.000000 dbrief-0.1.2/dbrief.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-15 02:02:39.000000 dbrief-0.1.2/dbrief.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 02:02:39.000000 dbrief-0.1.2/dbrief.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-15 02:02:22.000000 dbrief-0.1.2/demo/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-15 02:02:22.000000 dbrief-0.1.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-15 02:02:22.000000 dbrief-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 02:02:22.000000 dbrief-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:02:39.795134 dbrief-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:39.795134 dbrief-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:22.000000 dbrief-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:02:22.000000 dbrief-0.1.2/tests/conftest.py
```

### Comparing `dbrief-0.1.1/LICENSE.txt` & `dbrief-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbrief-0.1.1/PKG-INFO` & `dbrief-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrief
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for quickly creating lightweight HTML reports
 Author-email: Chris Santiago <cjsantiago@gatech.edu>
 License: MIT License
 Project-URL: Sourcecode, https://github.com/chris-santiago/dbrief
 Project-URL: Documentation, https://chris-santiago.github.io/dbrief/
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dbrief-0.1.1/dbrief/report.py` & `dbrief-0.1.2/dbrief/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,41 +18,33 @@
 
 
 def default_id(title: str) -> str:
     """Create a default HTML ID from a given title."""
     return re.sub("[^0-9a-zA-Z]+", "-", title).lower()
 
 
-def make_figure(data: pd.DataFrame, html_id: str, cols: list, file_dir: str = ".html"):
+def make_figure(data: pd.DataFrame, cols: list):
 
     if data.shape[1] >= 2:
         fig = data.hvplot(y=cols, value_label="Value", width=600).opts(
             legend_position=DEFAULT_LEGEND
         )
     else:
         fig = data.hvplot(y=cols, value_label="Value", width=600)
 
     bk_fig = hvplot.render(fig, backend="bokeh")
-    pathlib.Path(file_dir).mkdir(exist_ok=True)
-    file_path = pathlib.Path(file_dir).joinpath(f"{html_id}.html")
-    with open(file_path, "w") as fp:
-        fp.write(file_html(bk_fig, CDN))
-    return str(file_path)
+    return file_html(bk_fig, CDN)
 
 
 def make_table(
-    data: pd.DataFrame, html_id: str, cols: list, n_rows: int, file_dir: str = ".html"
+    data: pd.DataFrame, cols: list, n_rows: int
 ):
     table = data[cols].tail(n_rows).hvplot.table()
     bk_table = hvplot.render(table, backend="bokeh")
-    pathlib.Path(file_dir).mkdir(exist_ok=True)
-    file_path = pathlib.Path(file_dir).joinpath(f"{html_id}-data.html")
-    with open(file_path, "w") as fp:
-        fp.write(file_html(bk_table, CDN))
-    return str(file_path)
+    return file_html(bk_table, CDN)
 
 
 @dataclasses.dataclass()
 class Section:
     title: str
     html_id: str
     components: list
@@ -128,27 +120,25 @@
         cols: Optional[list] = None,
         html_id: Optional[str] = None,
         include_data: Optional[Union[bool, int]] = None,
         caption: Optional[str] = None,
     ):
         html_id = html_id if html_id else default_id(title)
         fig_path = make_figure(
-            data=data, html_id=html_id, cols=cols if cols else data.columns
+            data=data, cols=cols if cols else data.columns
         )
         if isinstance(include_data, bool):
             table_path = make_table(
                 data=data,
-                html_id=html_id,
                 cols=cols if cols else data.columns,
                 n_rows=DEFAULT_ROWS,
             )
         elif isinstance(include_data, int):
             table_path = make_table(
                 data=data,
-                html_id=html_id,
                 cols=cols if cols else data.columns,
                 n_rows=include_data,
             )
         else:
             table_path = None
         self.add_component(
             section=section,
```

### Comparing `dbrief-0.1.1/dbrief/templates/default.html` & `dbrief-0.1.2/dbrief/templates/default.html`

 * *Files 8% similar despite different names*

```diff
@@ -53,18 +53,18 @@
                                     <h2 class="subtitle">{{ column.title }}</h2>
                                     {% if column.text %}
                                         <div class="block">
                                             {{ column.text }}
                                         </div>
                                     {% endif %}
                                     <iframe class="has-ratio" width="800" height="400"
-                                    src="{{ column.html }}"></iframe>
+                                    srcdoc="{{ column.html.replace('"', "&quot;") }}"></iframe>
                                     {% if column.data %}
                                         <iframe class="has-ratio" width="800" height="400"
-                                        src="{{ column.data }}"></iframe>
+                                        srcdoc="{{ column.data.replace('"', "&quot;") }}"></iframe>
                                     {% endif %}
                                 </div>
                             {% endfor %}
                         </div>
                     {% endfor %}
                 </div>
                 <div class="column">
```

#### html2text {}

```diff
@@ -8,12 +8,14 @@
  {% for section in schema.values() %}
 ****** {{ section.title }} ******
 {% for row in section.components|batch(2) %}
 {% for column in row %}
 ***** {{ column.title }} *****
 {% if column.text %}
 {{ column.text }}
-{% endif %}  {% if column.data %}  {% endif %}
+{% endif %}
+, """) }}"> {% if column.data %}
+, """) }}"> {% endif %}
 {% endfor %}
 {% endfor %}
 Back_to_top
  {% endfor %}
```

### Comparing `dbrief-0.1.1/dbrief.egg-info/PKG-INFO` & `dbrief-0.1.2/dbrief.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrief
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for quickly creating lightweight HTML reports
 Author-email: Chris Santiago <cjsantiago@gatech.edu>
 License: MIT License
 Project-URL: Sourcecode, https://github.com/chris-santiago/dbrief
 Project-URL: Documentation, https://chris-santiago.github.io/dbrief/
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dbrief-0.1.1/docs/source/conf.py` & `dbrief-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbrief-0.1.1/pyproject.toml` & `dbrief-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "dbrief"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python package for quickly creating lightweight HTML reports"
 readme = "README.md"
 license = { text ="MIT License" }
 requires-python = ">=3.9"
 
 authors = [
     { name="Chris Santiago", email="cjsantiago@gatech.edu"}
```

### Comparing `dbrief-0.1.1/requirements.txt` & `dbrief-0.1.2/requirements.txt`

 * *Files identical despite different names*

