# Comparing `tmp/toui-1.0.4b0.tar.gz` & `tmp/toui-1.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-1.0.4b0.tar", last modified: Thu Apr 13 08:28:44 2023, max compression
+gzip compressed data, was "toui-1.1.0b0.tar", last modified: Sat Apr 15 18:13:02 2023, max compression
```

## Comparing `toui-1.0.4b0.tar` & `toui-1.1.0b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.218566 toui-1.0.4b0/
--rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.0.4b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.0.4b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3056 2023-04-13 08:28:44.215569 toui-1.0.4b0/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-04-13 08:05:30.000000 toui-1.0.4b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.024555 toui-1.0.4b0/examples/
--rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-04-13 08:21:09.000000 toui-1.0.4b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.029553 toui-1.0.4b0/images/
--rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.0.4b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 08:28:44.219566 toui-1.0.4b0/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-13 08:27:05.000000 toui-1.0.4b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.123568 toui-1.0.4b0/toui/
--rw-rw-rw-   0        0        0      213 2023-04-13 08:22:36.000000 toui-1.0.4b0/toui/__init__.py
--rw-rw-rw-   0        0        0      429 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1093 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/_helpers.py
--rw-rw-rw-   0        0        0     5234 2023-04-13 06:50:06.000000 toui-1.0.4b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     2380 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/_signals.py
--rw-rw-rw-   0        0        0    20272 2023-04-13 08:21:10.000000 toui-1.0.4b0/toui/apps.py
--rw-rw-rw-   0        0        0    19360 2023-04-13 08:21:10.000000 toui-1.0.4b0/toui/elements.py
--rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    14431 2023-04-13 08:21:10.000000 toui-1.0.4b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.208567 toui-1.0.4b0/toui.egg-info/
--rw-rw-rw-   0        0        0     3056 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.396935 toui-1.1.0b0/
+-rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.1.0b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.1.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3056 2023-04-15 18:13:02.394935 toui-1.1.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2620 2023-04-13 08:05:30.000000 toui-1.1.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.298381 toui-1.1.0b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-04-13 08:21:09.000000 toui-1.1.0b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.301004 toui-1.1.0b0/images/
+-rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.1.0b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:13:02.398404 toui-1.1.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-04-13 08:27:05.000000 toui-1.1.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.346802 toui-1.1.0b0/toui/
+-rw-rw-rw-   0        0        0      213 2023-04-15 17:57:55.000000 toui-1.1.0b0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-04-15 14:31:15.000000 toui-1.1.0b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1093 2023-04-15 17:56:59.000000 toui-1.1.0b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0     7483 2023-04-15 17:49:55.000000 toui-1.1.0b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     3164 2023-04-15 17:30:00.000000 toui-1.1.0b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    20894 2023-04-15 18:09:47.000000 toui-1.1.0b0/toui/apps.py
+-rw-rw-rw-   0        0        0    20399 2023-04-15 16:18:17.000000 toui-1.1.0b0/toui/elements.py
+-rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.1.0b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    15251 2023-04-15 16:14:35.000000 toui-1.1.0b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.1.0b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.391323 toui-1.1.0b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     3056 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/top_level.txt
```

### Comparing `toui-1.0.4b0/LICENSE` & `toui-1.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/PKG-INFO` & `toui-1.1.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.0.4b0
+Version: 1.1.0b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-1.0.4b0/README.md` & `toui-1.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/examples/advanced_example_1_toui_blueprint.py` & `toui-1.1.0b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/examples/example_1_simple_website.py` & `toui-1.1.0b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/examples/example_2_simple_desktop_app.py` & `toui-1.1.0b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/examples/example_3_updating_page.py` & `toui-1.1.0b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/examples/example_4_function_with_arg.py` & `toui-1.1.0b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/examples/example_5_user_variables.py` & `toui-1.1.0b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/images/logo.png` & `toui-1.1.0b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/setup.py` & `toui-1.1.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/toui/_helpers.py` & `toui-1.1.0b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/toui/_javascript_templates.py` & `toui-1.1.0b0/toui/_javascript_templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,66 +7,106 @@
     conn = "ws"
 }}
 const socket = new WebSocket(conn + '://' + location.host + '/toui-communicate')
 socket.addEventListener('message', ev => {{
     _findAndExecute(ev.data)
   }});
 const urlPath = location.pathname
-function _toPy(...arguments) {{
+async function _toPy(...arguments) {{
     var func = arguments.shift()
-    var json = {{func:func,
+    var json = {{type: "page",
+                func:func,
                 args: arguments,
                 url: urlPath}}
+    var properties = _manageProperties()
     json['html'] = _getDoc()
     var jsonstring = JSON.stringify(json)
     if (socket.readyState === 0) {{
         socket.onopen = function() {{
             socket.send(jsonstring);
         }}
     }} else {{
         socket.send(jsonstring)
     }}
 }}
 
+function _send(jsonstring) {{
+    socket.send(jsonstring)
+}}
 """
     
     
 desktop_template = f"""
 function _toPy(...arguments) {{
     var func = arguments.shift()
-    var json = {{func:func,
+    var json = {{type: "page",
+                func: func,
                 args: arguments}}
+    json['properties'] = _manageProperties()
     json['html'] = _getDoc()
     var jsonstring = JSON.stringify(json)
     pywebview.api.communicate(jsonstring)
 }}
+
+function _send(jsonstring) {{
+    return jsonstring
+}}
 """
 
 
 common_template = f"""
 function _getDoc() {{
+    var serializer = new XMLSerializer()
+    const doc = serializer.serializeToString(document)
+    return doc
+    }}
+
+function _setDoc(kwargs) {{
+    document.open()
+    document.write(kwargs['doc'])
+    document.close()
+    }}
+    
+async function _manageProperties() {{
+    var properties = {{files: []}}
     var input_elements = document.getElementsByTagName("input")
     for (var input_element of input_elements) {{
         input_element.setAttribute("value", input_element.value)
         if (input_element.checked == true) {{
             input_element.setAttribute("checked", "")
         }} else {{
             input_element.removeAttribute("checked")
         }}
     }}
-    var serializer = new XMLSerializer()
-    const doc = serializer.serializeToString(document)
-    return doc
-    }}
+    return properties
+}}
 
-function _setDoc(kwargs) {{
-    document.open()
-    document.write(kwargs['doc'])
-    document.close()
+async function _getFiles(kwargs) {{
+    var files = []
+    var element = _getElement(kwargs['selector'])
+    if (element.type == "file") {{
+        for (var file of element.files) {{
+            var selector = _getElementSelector(element)
+            var fileJSON = {{name: file.name,
+                             size: file.size,
+                             type: file.type,
+                             'last-modified': file.lastModified,
+                             'last-modified-date': file.lastModifiedDate,
+                             selector: selector}}
+            if (kwargs['with_content'] == true) {{
+                await file.text().then(function (text) {{
+                    fileJSON['content'] = text
+                }})
+            }}
+            files.push(fileJSON)
+        }}
     }}
+    var jsonstring = JSON.stringify({{data: files, type: "files"}})
+    return _send(jsonstring)
+}}
     
 function _getElement(kwargs) {{
     var number = 0
     if ('number' in kwargs) {{
         var number = parseInt(kwargs['number'])
     }}
     if ('parent' in kwargs) {{
@@ -76,14 +116,40 @@
     }} else {{
         const elements = document.querySelectorAll(kwargs['selector'])
         const element = elements[number]
         return element
     }}
 }}
 
+var _getElementSelector = function(el) {{
+  if (!(el instanceof Element))
+            return;
+        var path = [];
+        while (el.nodeType === Node.ELEMENT_NODE) {{
+            var selector = el.nodeName.toLowerCase();
+            if (el.id) {{
+                selector += '#' + el.id;
+                path.unshift(selector);
+                break;
+            }} else {{
+                var sib = el, nth = 1;
+                while (sib = sib.previousElementSibling) {{
+                    if (sib.nodeName.toLowerCase() == selector)
+                       nth++;
+                }}
+                if (nth != 1)
+                    selector += ":nth-of-type("+nth+")";
+            }}
+            path.unshift(selector);
+            el = el.parentNode;
+        }}
+        path = path.join(" > ");
+        return path;
+     }}
+
 function _replaceElement(kwargs) {{
     var old_element = _getElement(kwargs['selector'])
     old_element.outerHTML = kwargs['element']
     }}
 
 function _replaceElements(kwargs) {{
     var elements = document.querySelectorAll(kwargs['selectors'])
@@ -168,14 +234,17 @@
     }}
     if (func == "_addScript") {{
         _addScript(kwargs)
     }}
     if (func == "_goTo") {{
         _goTo(kwargs)
     }}
+    if (func == "_getFiles") {{
+        _getFiles(kwargs)
+    }}
 }}"""
 
 def custom_func(name):
     text = f"""
     function {name}(...args) {{
         _toPy('{name}', ...args)
     }}
```

### Comparing `toui-1.0.4b0/toui/_signals.py` & `toui-1.1.0b0/toui/_signals.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 """
 A module that creates instructions "signals" to allow communicating with JavaScript.
 """
 import inspect
 import json
-from toui._helpers import debug
+from toui._helpers import debug, info
 from copy import copy
 from functools import wraps
 
 
 class Signal:
 
     included_private_methods = ["_open_another_page"]
     no_return_functions = []
 
-    def __init__(self):
+    def __init__(self, return_type=None):
         self.ws = None
+        self.return_type = return_type
 
     def __call__(decorator, func):
         decorator._func = func
         @wraps(func)
         def new_func(self, *args, **kwargs):
             decorator.object = self
             if self._signal_mode:
                 original_copy = copy(self)
             value = decorator._func(self, *args, **kwargs)
+            real_output = value
             if self._signal_mode:
                 if self.__class__.__name__ == 'Element':
                     decorator.ws = self._parent_page.__dict__.get("_ws")
                     decorator.evaluate_js = self._parent_page._evaluate_js
                 elif self.__class__.__name__ == "Page":
                     decorator.ws = self.__dict__.get("_ws")
                     decorator.evaluate_js = self._evaluate_js
                 kwargs = inspect.signature(decorator._func).bind(self, *args, **kwargs)
                 kwargs.apply_defaults()
                 kwargs = kwargs.arguments
                 kwargs['return_value'] = value
                 kwargs['object'] = kwargs['self']
                 kwargs['original_copy'] = original_copy
                 del kwargs['self']
-                decorator._call_method(decorator._func, **kwargs)
+                real_output = decorator._call_method(decorator._func, **kwargs)
             if func.__name__ in decorator.no_return_functions:
                 return
+            if decorator.return_type == "js":
+                return real_output
             return value
         return new_func
 
     def _call_method(self, func, **kwargs):
         for method_name, method in inspect.getmembers(self, inspect.isfunction):
             if method_name == func.__name__ and (not method_name.startswith("_") or
                                                  method_name in self.included_private_methods):
@@ -54,9 +58,22 @@
                 else:
                     return
 
     def _send(self, signal):
         debug(f"SENT: {signal}")
         if self.ws:
             self.ws.send(json.dumps(signal))
+            data_from_js = self.ws.receive()
+            data_validation = self.object._app._validate_data(data_from_js)
+            if not data_validation:
+                info("Data validation returns `False`. The data will not be used.")
+                return
+            data_dict = json.loads(data_from_js)
+            debug(f"DATA RECEIVED")
+            return data_dict['data']
         else:
-            self.evaluate_js(func=signal['func'], kwargs=signal['kwargs'])
+            out = self.evaluate_js(func=signal['func'], kwargs=signal['kwargs'])
+            try:
+                data_dict = json.loads(out)
+                debug(f"DATA RECEIVED")
+            except: data_dict = {"data": None}
+            return data_dict['data']
```

### Comparing `toui-1.0.4b0/toui/apps.py` & `toui-1.1.0b0/toui/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,34 +179,36 @@
             If ``True``, the `Page` will be copied before adding to the app.
 
         blueprint: toui.structure.ToUIBlueprint, flask.Blueprint, default = None
             If a `flask.Blueprint` or a `ToUIBlueprint` was added, the `Page` view_func will be added
             to the blueprint instead of the `Flask` app.
 
         endpoint
-            `endpoint` parameter in `flask.Flask.route`.
+            `endpoint` parameter in `flask.Flask.route`. If ``None``, the endpoint will be set
+            as the unique id of the `Page`. The unique id is obtained through the ``id()``
+            function and converted to a string.
             
         """
         for page in pages:
             if page.url in self.forbidden_urls:
                 warn(f"The URL '{page.url}' is not allowed and might cause errors.")
             if do_copy:
                 page = copy(page)
             page._add_script()
             page._app = self
             self.pages.append(page)
-            view_func = page.view_func
+            view_func = page._view_func
             if self._auth:
                 view_func = self._auth.required(view_func)
             if not endpoint:
-                endpoint = page.url
+                endpoint = str(id(page))
             if blueprint:
-                route = blueprint.route(page.url, methods=['GET', 'POST'], endpoint=page.url)(view_func)
+                route = blueprint.route(page.url, methods=['GET', 'POST'], endpoint=endpoint)(view_func)
             else:
-                route = self.flask_app.route(page.url, methods=['GET', 'POST'], endpoint=page.url)(view_func)
+                route = self.flask_app.route(page.url, methods=['GET', 'POST'], endpoint=endpoint)(view_func)
             for func in page._functions.values():
                 self._add_functions(func)
 
     def open_new_page(self, url):
         """
         Redirects to another URL.
 
@@ -361,25 +363,36 @@
         Validate data received from JavaScript before using it.
 
         ToUI receives data from JavaScript in the form of a JSON object. To validate this data
         before allowing ToUI to use it, input a function that checks the data. This function
         should have one argument `data` and should either return ``True`` or ``False``.
         If the function returns ``False``, the data will not be used by ToUI.
 
-        Currently, the JSON object contains the following keys:
+        Currently, there are two types of JSON objects that ToUI receives.
+        One of the JSON objects contains the following keys:
 
-        {func: ...,
+        {type: 'page',
+         func: ...,
          args: ...,
          url: ...,
          html: ...}
 
-        `func` contains the name of the Python function that should be called, `args` are the
+        `type` is the type of JSON object, and it always has the value 'page' when JavaScript sends the HTML document
+        as data. `func` contains the name of the Python function that should be called, `args` are the
         arguments of this function, `url` is the URL of the HTML page that sent the data, 'html'
         is the HTML document itself as a string.
-        However, note that the structure of the JSON object might change in future versions of
+
+        Another type of JSON object is a JSON that contains uploaded files:
+
+        {type: 'files',
+         files: ...}
+
+        You can get the uploaded files using the method `Element.get_files()`.
+
+        However, note that the structures of the JSON objects might change in future versions of
         ToUI.
 
         Parameters
         ----------
         func: Callable
             A function that validates data received from JavaScript. It should have one argument
             `data` and should either return ``True`` or ``False``.
@@ -387,15 +400,14 @@
         See Also
         --------
         Website.set_ws_validation
 
         """
         self._validate_data = func
 
-
     def register_toui_blueprint(self, blueprint, **options):
         """
         Registers a `ToUIBlueprint` object. It is similar to `Flask.register_blueprint`.
 
         Parameters
         ----------
         blueprint: toui.structure.ToUIBlueprint
```

### Comparing `toui-1.0.4b0/toui/elements.py` & `toui-1.1.0b0/toui/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         js_func = "_delAttr"
         js_args = []
         js_kwargs = _ElementSignal._default_kwargs(kwargs)
         js_kwargs['name'] = kwargs['name']
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
     @staticmethod
+    def get_files(**kwargs):
+        js_func = "_getFiles"
+        js_args = []
+        js_kwargs = _ElementSignal._default_kwargs(kwargs)
+        js_kwargs['with_content'] = kwargs['with_content']
+        return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
+
+    @staticmethod
     def set_content(**kwargs):
         js_func = "_setContent"
         js_args = []
         js_kwargs = _ElementSignal._default_kwargs(kwargs)
         js_kwargs['content'] = str(kwargs['content'])
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
@@ -68,15 +76,14 @@
         js_args = []
         js_kwargs = _ElementSignal._default_kwargs(kwargs)
         js_kwargs['content'] = str(kwargs['content'])
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
 
 class Element:
-
     """
     Creates an HTML element.
 
     Examples
     --------
 
     Creating a ``<button>`` HTML element:
@@ -109,14 +116,18 @@
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
         return self.to_str()
 
+    @property
+    def _app(self):
+        return self._parent_page._app
+
     @_ElementSignal()
     def from_str(self, html_str):
         """
         Converts HTML code to an `Element` object.
 
         Parameters
         ----------
@@ -308,14 +319,23 @@
         bool
 
         """
         return self.get_attr(name) != None
 
     @_ElementSignal()
     def del_attr(self, name):
+        """
+        Removes an HTML element attribute.
+
+        Parameters
+        ----------
+        name: str
+            The name of the attribute.
+
+        """
         if self.has_attr(name):
             del self._element.attrs[name]
 
     def get_id(self):
         """
         Gets the ``id`` attribute of the HTML element.
 
@@ -365,18 +385,38 @@
         ----------
         value
             The new value of the ``value`` attribute.
 
         """
         self.set_attr("value", value)
 
+    @_ElementSignal(return_type="js")
+    def get_files(self, with_content=True):
+        """
+        Gets uploaded files from element.
+
+        This method is useful when uploading files using ``<input type="file">`` element.
+
+        Parameters
+        ----------
+        with_content: bool, default=True
+            If ``True``, the contents of the files will be included in the output.
+
+        Returns
+        -------
+        list(dict)
+
+        """
+        return []
+
     def get_content(self):
         """
-        Gets the inner HTML content of the element. It is similar to getting the ``Element.innerHTML``
-        property in JavaScript.
+        Gets the inner HTML content of the element.
+
+        It is similar to getting the ``Element.innerHTML`` property in JavaScript.
 
         Returns
         -------
         str
 
         """
         return self._element.decode_contents()
```

### Comparing `toui-1.0.4b0/toui/pages.py` & `toui-1.1.0b0/toui/pages.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,18 +64,14 @@
     url: str
         The URL of the page.
 
     window: pywebview.Window, default = None
         A `pywebview.Window` object. It is automatically created when adding the `Page` to
         `DesktopApp` and running the app.
 
-    view_func: Callable
-        The view function of the `Page`. This is the function that will be decorated by
-        `Flask.route()` when creating web apps.
-
     Examples
     --------
 
     Importing the class:
 
     >>> from toui import Page
 
@@ -144,15 +140,16 @@
         self.window = None
 
         # Other internal attributes
         self._app = None
         self._signal_mode = False
         self._signals = []
         self._functions = {}
-        self._view_func = lambda: view_func(self)
+        self._basic_view_func = lambda: view_func(self)
+        self._view_func = self._basic_view_func
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
         return self.to_str()
 
@@ -263,18 +260,16 @@
 
         do_copy: bool, default = False
             If ``True``, the element will be copied.
 
         Returns
         -------
         element: Element
-            If the element was found, an `Element` object will be returned.
-
-        None
-            If the element was not found.
+            If the element was found, an `Element` object will be returned. Otherwise ``None``
+            will be returned.
 
         """
         bs4_tag = self._html.find(id=element_id)
         if bs4_tag is None:
             return None
         element = Element()
         if do_copy:
@@ -411,21 +406,37 @@
         if func.__name__ in old_functions:
             return ""
         script_element = Element("script")
         script_element.set_content(custom_func(func.__name__))
         self.get_elements(tag_name="html")[0].add_content(script_element)
         return func.__name__
 
-    @property
-    def view_func(self):
-        return self._view_func
-
-    @view_func.setter
-    def view_func(self, func):
-        self._view_func = lambda: func(self)
+    def on_url_request(self, func, display_return_value=False):
+        """
+        Sets a function that will be called when the user types the URL in a browser or when a request is sent to the
+        URL. You can view it as the `view_func` in Flask.
+
+        Parameters
+        ----------
+        func: Callable
+            The function that will be called when a request is sent to the URL.
+
+        display_return_value: bool, default=False
+            If ``True``, the browser will display the return value of the function when the URL is loaded. If ``False``,
+            the return value will be ignored.
+
+        """
+        def new_func():
+            original_return = self._basic_view_func()
+            new_return = func()
+            if display_return_value:
+                return new_return
+            else:
+                return original_return
+        self._view_func = new_func
 
     def _add_script(self, template_type="web"):
         script_tag = Element("script")
         script_content = get_script(template_type)
         script_tag.set_content(script_content)
         self.get_elements(tag_name="html")[0].add_content(script_tag)
 
@@ -443,20 +454,25 @@
             with _TempHTML(directory=assets_folder, html=self.to_str(),
                            win=self.window) as temp_html:
                 time.sleep(1)
         api.window = self.window
         return func
 
     def _evaluate_js(self, func, kwargs):
+        data_from_js = ""
+        def wait_then_get_result(result):
+            nonlocal data_from_js
+            data_from_js = result
         codejs = f"""
         var kwargs = JSON.parse(\'{json.dumps(kwargs)}\')
         {func}(kwargs)
         """
         debug("EVALUATE: " + codejs)
-        out = self.window.evaluate_js(codejs)
+        self.window.evaluate_js(codejs, callback=wait_then_get_result)
+        return data_from_js
 
     @_PageSignal()
     def _open_another_page(self, url):
         return
 
 
 class _TempHTML:
```

### Comparing `toui-1.0.4b0/toui/structure.py` & `toui-1.1.0b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.4b0/toui.egg-info/PKG-INFO` & `toui-1.1.0b0/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.0.4b0
+Version: 1.1.0b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-1.0.4b0/toui.egg-info/SOURCES.txt` & `toui-1.1.0b0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

