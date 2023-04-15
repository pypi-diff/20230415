# Comparing `tmp/live-fast-api-0.0.1.tar.gz` & `tmp/live-fast-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-fast-api-0.0.1.tar", last modified: Wed Apr 12 14:24:16 2023, max compression
+gzip compressed data, was "live-fast-api-0.0.2.tar", last modified: Sat Apr 15 12:54:27 2023, max compression
```

## Comparing `live-fast-api-0.0.1.tar` & `live-fast-api-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.029597 live-fast-api-0.0.1/
--rw-rw-rw-   0        0        0      215 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2054 2023-04-12 14:24:16.028597 live-fast-api-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.1/build.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.014595 live-fast-api-0.0.1/live_api/
--rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.1/live_api/__init__.py
--rw-rw-rw-   0        0        0     8981 2023-03-09 10:59:33.000000 live-fast-api-0.0.1/live_api/base.py
--rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.1/live_api/document.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.018597 live-fast-api-0.0.1/live_api/endpoints/
--rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.1/live_api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.1/live_api/endpoints/data.py
--rw-rw-rw-   0        0        0    10886 2023-04-12 14:24:12.000000 live-fast-api-0.0.1/live_api/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.1/live_api/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.1/live_api/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.021597 live-fast-api-0.0.1/live_api/service/
--rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.1/live_api/service/__init__.py
--rw-rw-rw-   0        0        0    18136 2023-04-12 14:16:50.000000 live-fast-api-0.0.1/live_api/service/rest.py
--rw-rw-rw-   0        0        0    22076 2023-04-12 14:21:27.000000 live-fast-api-0.0.1/live_api/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.005497 live-fast-api-0.0.1/live_api/source/
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.005643 live-fast-api-0.0.1/live_api/source/assets/
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.022596 live-fast-api-0.0.1/live_api/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.1/live_api/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.1/live_api/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.028597 live-fast-api-0.0.1/live_fast_api.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-04-12 14:23:27.000000 live-fast-api-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       77 2023-03-28 10:14:28.000000 live-fast-api-0.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       68 2023-03-28 10:14:28.000000 live-fast-api-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:24:16.029597 live-fast-api-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1580 2023-04-12 14:23:23.000000 live-fast-api-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.474211 live-fast-api-0.0.2/
+-rw-rw-rw-   0        0        0      215 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2054 2023-04-15 12:54:27.474211 live-fast-api-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.2/build.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.419959 live-fast-api-0.0.2/live_api/
+-rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.2/live_api/__init__.py
+-rw-rw-rw-   0        0        0     8981 2023-03-09 10:59:33.000000 live-fast-api-0.0.2/live_api/base.py
+-rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.2/live_api/document.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.445211 live-fast-api-0.0.2/live_api/endpoints/
+-rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.2/live_api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.2/live_api/endpoints/data.py
+-rw-rw-rw-   0        0        0    10624 2023-04-15 12:51:23.000000 live-fast-api-0.0.2/live_api/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.2/live_api/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.2/live_api/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.452210 live-fast-api-0.0.2/live_api/service/
+-rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.2/live_api/service/__init__.py
+-rw-rw-rw-   0        0        0    17698 2023-04-15 12:53:17.000000 live-fast-api-0.0.2/live_api/service/rest.py
+-rw-rw-rw-   0        0        0    21871 2023-04-15 12:54:04.000000 live-fast-api-0.0.2/live_api/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.390951 live-fast-api-0.0.2/live_api/source/
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.390951 live-fast-api-0.0.2/live_api/source/assets/
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.457223 live-fast-api-0.0.2/live_api/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.2/live_api/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.2/live_api/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-04-15 12:54:27.473210 live-fast-api-0.0.2/live_fast_api.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/live_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/live_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/live_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/live_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/live_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-04-15 12:54:27.000000 live-fast-api-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       77 2023-03-28 10:14:28.000000 live-fast-api-0.0.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       68 2023-03-28 10:14:28.000000 live-fast-api-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 12:54:27.474211 live-fast-api-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-04-15 12:54:20.000000 live-fast-api-0.0.2/setup.py
```

### Comparing `live-fast-api-0.0.1/PKG-INFO` & `live-fast-api-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.1/README.md` & `live-fast-api-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/build.py` & `live-fast-api-0.0.2/build.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_api/base.py` & `live-fast-api-0.0.2/live_api/base.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_api/endpoints/data.py` & `live-fast-api-0.0.2/live_api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_api/endpoints/engine.py` & `live-fast-api-0.0.2/live_api/endpoints/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,24 +38,16 @@
         Defines the class attributes.
 
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
         :param returns: The returned values.
         """
 
-        if args is None:
-            args = ()
-        # end if
-
-        if kwargs is None:
-            kwargs = {}
-        # end if
-
-        self.args = args
-        self.kwargs = kwargs
+        self.args = args or ()
+        self.kwargs = kwargs or {}
         self.returns = returns
     # end __init__
 
     def collect(
             self, *,
             args: Optional[Tuple] = None,
             kwargs: Optional[Dict[str, Any]] = None,
@@ -193,28 +185,20 @@
         :param methods: The endpoint methods.
         :param description: The description of the object.
         :param root: The root to the path.
         :param options: Any keyword arguments.
         :param service: The service object.
         """
 
-        if options is None:
-            options = {}
-        # end if
-
-        if root is None:
-            root = ""
-        # end if
-
         self.record: Requests = []
 
-        self.options = options
+        self.options = options or {}
 
         self.path = str(path)
-        self.root = root
+        self.root = root or ""
         self.description = description
 
         self.methods = methods
 
         self.service = service
     # end __init__
```

### Comparing `live-fast-api-0.0.1/live_api/endpoints/exceptions.py` & `live-fast-api-0.0.2/live_api/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_api/endpoints/process.py` & `live-fast-api-0.0.2/live_api/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_api/service/rest.py` & `live-fast-api-0.0.2/live_api/service/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,58 +115,38 @@
         :param description: The description of the object.
         :param icon: The icon path.
         :param root: The root to the path.
         :param home: The home endpoint.
         :param debug: The value to create the docs' endpoint for the home endpoint.
         """
 
-        if version is None:
-            version = self.VERSION
-        # end if
-
-        if description is None:
-            description = self.DESCRIPTION
-        # end if
-
-        if icon is None:
-            icon = self.ICON
-        # end if
-
-        if name is None:
-            name = self.NAME
-        # end if
-
         self._root = None
 
         self.endpoints = {}
 
-        if root is None:
-            root = ""
-        # end if
-
         if (
             (isinstance(home, bool) and home) or
             (debug and (home is None))
         ):
             home = True
         # end if
 
         self.app = None
 
         self.service_process = None
         self.timeout_process = None
 
         self.block = False
 
-        self.description = description
-        self.root = root
-        self.icon = icon
+        self.description = description or self.DESCRIPTION
+        self.root = root or ""
+        self.icon = icon or self.ICON
         self.home = home
-        self.name = name
-        self.version = version
+        self.name = name or self.NAME
+        self.version = version or self.VERSION
 
         self.endpoints.update(
             self.valid_endpoints(endpoints)
         )
 
         for endpoint in self.endpoints.values():
             endpoint.service = self
@@ -278,19 +258,15 @@
         """
         Adds the endpoint to the service.
 
         :param path: The path for the endpoint.
         :param endpoint: The command to run.
         """
 
-        if path is None:
-            path = endpoint.path
-        # end if
-
-        self.endpoints[path] = endpoint
+        self.endpoints[path or endpoint.path] = endpoint
     # end add_endpoint
 
     def add_endpoints(self, endpoints: EndpointsContainer) -> None:
         """
         Adds the endpoint to the service.
 
         :param endpoints: The commands to run.
@@ -305,17 +281,15 @@
         """
         Adds the endpoint to the service.
 
         :param path: The path for the endpoint.
         :param endpoint: The command to run.
         """
 
-        if path is None:
-            path = endpoint.path
-        # end if
+        path = path or endpoint.path
 
         if path not in self.endpoints:
             raise ValueError(
                 f"The path was not initialized for a different "
                 f"endpoint beforehand. Consider using "
                 f"'{self.add_endpoint.__name__}' method instead, "
                 f"to add endpoints with new path. Given path: {path}. "
```

### Comparing `live-fast-api-0.0.1/live_api/service/sockets.py` & `live-fast-api-0.0.2/live_api/service/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,19 +267,15 @@
     def __init__(self, clients: Optional[dict] = None) -> None:
         """
         Defines the base data class to contain the clients.
 
         :param clients: The base dictionary to contain the clients' data.
         """
 
-        if clients is None:
-            clients = {}
-        # end if
-
-        self.clients = clients
+        self.clients = clients or {}
     # end __init__
 
     # defines a method to set a client
     def set_client(
             self, address: Address, connection: Optional[Socket] = None
     ) -> None:
         """
@@ -703,19 +699,15 @@
     def __init__(self, endpoints: Optional[EndpointsContainer] = None) -> None:
         """
         Defines the server datasets for clients and client commands.
 
         :param endpoints: The commands to run for specific requests of the clients.
         """
 
-        if endpoints is None:
-            endpoints = {}
-        # end if
-
-        self.endpoints = self.valid_endpoints(endpoints)
+        self.endpoints = self.valid_endpoints(endpoints or {})
 
         SocketServer.__init__(self)
     # end __init__
 
     @staticmethod
     def valid_endpoints(endpoints: Optional[Any] = None) -> Endpoints:
         """
@@ -768,32 +760,28 @@
     :param endpoint: The path to the endpoint.
     :param port: The sending port.
     :param parameters: The request parameters.
 
     :return: The returned value.
     """
 
-    if parameters is None:
-        parameters = {}
-    # end if
-
     # noinspection PyUnresolvedReferences
     connection = socket.socket(
         socket.AF_BLUETOOTH, socket.SOCK_STREAM,
         socket.BTPROTO_RFCOMM
     )
 
     client = SocketClient(connection=connection)
     client.connect(host=host, port=port)
 
     # noinspection HttpUrlsUsage
     url = f"http://127.0.0.1:5555/{endpoint}"
 
     req = PreparedRequest()
-    req.prepare_url(url, parameters)
+    req.prepare_url(url, parameters or {})
 
     client.send(message=req.url.encode())
     content = client.receive()
 
     connection.close()
 
     return decode(content.decode())
```

### Comparing `live-fast-api-0.0.1/live_api/source/assets/icon/icon.ico` & `live-fast-api-0.0.2/live_api/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_api/source/assets/icon/icon.png` & `live-fast-api-0.0.2/live_api/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/live_fast_api.egg-info/PKG-INFO` & `live-fast-api-0.0.2/live_fast_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.1/live_fast_api.egg-info/SOURCES.txt` & `live-fast-api-0.0.2/live_fast_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.1/pyproject.toml` & `live-fast-api-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'live-fast-api'
-version = '0.0.1'
+version = '0.0.2'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `live-fast-api-0.0.1/setup.py` & `live-fast-api-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "live_api/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='live-fast-api',
-        version='0.0.1',
+        version='0.0.2',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

