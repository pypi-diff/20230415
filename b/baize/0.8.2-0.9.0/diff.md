# Comparing `tmp/baize-0.8.2.tar.gz` & `tmp/baize-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baize-0.8.2.tar", max compression
+gzip compressed data, was "baize-0.9.0.tar", max compression
```

## Comparing `baize-0.8.2.tar` & `baize-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    11341 2021-06-18 03:07:32.288698 baize-0.8.2/LICENSE
--rw-r--r--   0        0        0     3303 2021-06-18 03:07:32.288698 baize-0.8.2/README.md
--rw-r--r--   0        0        0        0 2021-06-18 03:07:32.288698 baize-0.8.2/baize/__init__.py
--rw-r--r--   0        0        0       63 2021-06-18 03:07:32.288698 baize-0.8.2/baize/__version__.py
--rw-r--r--   0        0        0    28023 2021-06-18 03:07:32.288698 baize-0.8.2/baize/asgi.py
--rw-r--r--   0        0        0      301 2021-06-18 03:07:32.288698 baize-0.8.2/baize/concurrency.py
--rw-r--r--   0        0        0    14989 2021-06-18 03:07:32.288698 baize-0.8.2/baize/datastructures.py
--rw-r--r--   0        0        0      768 2021-06-18 03:07:32.288698 baize-0.8.2/baize/exceptions.py
--rw-r--r--   0        0        0     8740 2021-06-18 03:07:32.288698 baize-0.8.2/baize/formparsers.py
--rw-r--r--   0        0        0        0 2021-06-18 03:07:32.288698 baize-0.8.2/baize/py.typed
--rw-r--r--   0        0        0     2349 2021-06-18 03:07:32.288698 baize-0.8.2/baize/requests.py
--rw-r--r--   0        0        0     6773 2021-06-18 03:07:32.288698 baize-0.8.2/baize/responses.py
--rw-r--r--   0        0        0     6275 2021-06-18 03:07:32.288698 baize-0.8.2/baize/routing.py
--rw-r--r--   0        0        0     1503 2021-06-18 03:07:32.288698 baize-0.8.2/baize/typing.py
--rw-r--r--   0        0        0      941 2021-06-18 03:07:32.288698 baize-0.8.2/baize/utils.py
--rw-r--r--   0        0        0    19782 2021-06-18 03:07:32.288698 baize-0.8.2/baize/wsgi.py
--rw-r--r--   0        0        0     1872 2021-06-18 03:07:32.288698 baize-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     4148 2021-06-18 03:07:40.327470 baize-0.8.2/setup.py
--rw-r--r--   0        0        0     4446 2021-06-18 03:07:40.328248 baize-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2021-06-29 15:33:59.466029 baize-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3303 2021-06-29 15:33:59.466029 baize-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2021-06-29 15:33:59.466029 baize-0.9.0/baize/__init__.py
+-rw-r--r--   0        0        0       63 2021-06-29 15:33:59.466029 baize-0.9.0/baize/__version__.py
+-rw-r--r--   0        0        0    28019 2021-06-29 15:33:59.466029 baize-0.9.0/baize/asgi.py
+-rw-r--r--   0        0        0      301 2021-06-29 15:33:59.466029 baize-0.9.0/baize/concurrency.py
+-rw-r--r--   0        0        0    14989 2021-06-29 15:33:59.466029 baize-0.9.0/baize/datastructures.py
+-rw-r--r--   0        0        0      768 2021-06-29 15:33:59.466029 baize-0.9.0/baize/exceptions.py
+-rw-r--r--   0        0        0     8740 2021-06-29 15:33:59.466029 baize-0.9.0/baize/formparsers.py
+-rw-r--r--   0        0        0        0 2021-06-29 15:33:59.466029 baize-0.9.0/baize/py.typed
+-rw-r--r--   0        0        0     2349 2021-06-29 15:33:59.466029 baize-0.9.0/baize/requests.py
+-rw-r--r--   0        0        0     6901 2021-06-29 15:33:59.466029 baize-0.9.0/baize/responses.py
+-rw-r--r--   0        0        0     6318 2021-06-29 15:33:59.466029 baize-0.9.0/baize/routing.py
+-rw-r--r--   0        0        0     2782 2021-06-29 15:33:59.466029 baize-0.9.0/baize/status.py
+-rw-r--r--   0        0        0     1503 2021-06-29 15:33:59.466029 baize-0.9.0/baize/typing.py
+-rw-r--r--   0        0        0      941 2021-06-29 15:33:59.466029 baize-0.9.0/baize/utils.py
+-rw-r--r--   0        0        0    19778 2021-06-29 15:33:59.466029 baize-0.9.0/baize/wsgi.py
+-rw-r--r--   0        0        0     1872 2021-06-29 15:33:59.466029 baize-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4148 2021-06-29 15:34:10.851307 baize-0.9.0/setup.py
+-rw-r--r--   0        0        0     4446 2021-06-29 15:34:10.851818 baize-0.9.0/PKG-INFO
```

### Comparing `baize-0.8.2/LICENSE` & `baize-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/README.md` & `baize-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/asgi.py` & `baize-0.9.0/baize/asgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,16 +758,16 @@
 
     :param routes: A triple composed of path, endpoint, and name. The name is optional. \
         If the name is not given, the corresponding URL cannot be constructed through \
         build_url.
 
     ```python
     applications = Router(
-        ("/static/{filepath:path}", static_files),
-        ("/api/{any:path}", api_app),
+        ("/static/{filepath:any}", static_files),
+        ("/api/{_:any}", api_app),
         ("/about/{name}", about_page, "about"),
         ("/", homepage, "homepage"),
     )
     """
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         path = scope["path"]
```

### Comparing `baize-0.8.2/baize/datastructures.py` & `baize-0.9.0/baize/datastructures.py`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/exceptions.py` & `baize-0.9.0/baize/exceptions.py`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/formparsers.py` & `baize-0.9.0/baize/formparsers.py`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/requests.py` & `baize-0.9.0/baize/requests.py`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/responses.py` & `baize-0.9.0/baize/responses.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from hashlib import sha1
 from http import cookies as http_cookies
 from itertools import chain
 from mimetypes import guess_type
 from typing import Iterable, List, Mapping, Sequence, Tuple, Union, overload
 from urllib.parse import quote
 
+from . import status
 from .datastructures import MutableHeaders
 from .exceptions import HTTPException
 from .typing import Literal, ServerSentEvent
 
 
 class BaseResponse:
     def __init__(
-        self, status_code: int = 200, headers: Mapping[str, str] = None
+        self, status_code: int = status.HTTP_200_OK, headers: Mapping[str, str] = None
     ) -> None:
         self.status_code = status_code
         self.headers = MutableHeaders(headers)
         self.cookies: http_cookies.SimpleCookie = http_cookies.SimpleCookie()
 
     def set_cookie(
         self,
@@ -101,15 +102,15 @@
             content_type
             or guess_type(download_name or os.path.basename(filepath))[0]
             or "application/octet-stream"
         )
         self.stat_result = stat_result = stat_result or os.stat(self.filepath)
         if not stat.S_ISREG(stat_result.st_mode):
             raise FileNotFoundError("Filepath exists, but is not a valid file.")
-        super().__init__(status_code=200, headers=headers)
+        super().__init__(status_code=status.HTTP_200_OK, headers=headers)
 
         self.headers["accept-ranges"] = "bytes"
         if download_name is not None or self.content_type == "application/octet-stream":
             download_name = download_name or os.path.basename(self.filepath)
             content_disposition = (
                 "attachment; "
                 f'filename="{download_name}"; '
@@ -139,32 +140,30 @@
     ) -> Sequence[Tuple[int, Union[int, int]]]:
         """
         Parse the Range header and make appropriate merge or cut processing
         """
         try:
             unit, ranges_str = range_raw_line.split("=", maxsplit=1)
         except ValueError:
-            raise HTTPException(status_code=400)
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
         if unit != "bytes":
-            raise HTTPException(status_code=400)
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
 
         ranges = [
             (int(_[0]), int(_[1]) + 1 if _[1] else max_size)
             for _ in self.range_re.findall(ranges_str)
         ]
 
         if any(start > end for start, end in ranges):
-            raise HTTPException(status_code=400)
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST)
 
         if any(end > max_size for _, end in ranges):
             raise HTTPException(
-                status_code=416,
-                headers={
-                    "Content-Range": f"*/{max_size}",
-                },
+                status_code=status.HTTP_416_REQUESTED_RANGE_NOT_SATISFIABLE,
+                headers={"Content-Range": f"*/{max_size}"},
             )
 
         if len(ranges) == 1:
             return ranges
 
         result: List[Tuple[int, int]] = []
         for start, end in ranges:
```

### Comparing `baize-0.8.2/baize/routing.py` & `baize-0.9.0/baize/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def to_python(self, value: str) -> date:
         return date(int(value[0:4]), int(value[5:7]), int(value[8:10]))
 
     def to_string(self, value: date) -> str:
         return value.isoformat()
 
 
-class PathConvertor(Convertor):
+class AnyConvertor(Convertor):
     regex = ".*"
 
     def to_python(self, value: str) -> str:
         return value
 
     def to_string(self, value: str) -> str:
         return value
@@ -95,15 +95,16 @@
 
 CONVERTOR_TYPES = {
     "str": StringConvertor(),
     "int": IntegerConvertor(),
     "decimal": DecimalConvertor(),
     "uuid": UUIDConvertor(),
     "date": DateConvertor(),
-    "path": PathConvertor(),
+    "path": AnyConvertor(),  # will be delete
+    "any": AnyConvertor(),
 }
 
 # Match parameters in URL paths, eg. '{param}', and '{param:int}'
 PARAM_REGEX = re.compile(r"{([^\d]\w*)(:\w+)?}")
 
 
 def compile_path(path: str) -> Tuple[str, Dict[str, Convertor]]:
```

### Comparing `baize-0.8.2/baize/typing.py` & `baize-0.9.0/baize/typing.py`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/utils.py` & `baize-0.9.0/baize/utils.py`

 * *Files identical despite different names*

### Comparing `baize-0.8.2/baize/wsgi.py` & `baize-0.9.0/baize/wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,16 +550,16 @@
 
     :param routes: A triple composed of path, endpoint, and name. The name is optional. \
         If the name is not given, the corresponding URL cannot be constructed through \
         build_url.
 
     ```python
     applications = Router(
-        ("/static/{filepath:path}", static_files),
-        ("/api/{any:path}", api_app),
+        ("/static/{filepath:any}", static_files),
+        ("/api/{_:any}", api_app),
         ("/about/{name}", about_page, "about"),
         ("/", homepage, "homepage"),
     )
     ```
     """
 
     def __call__(
```

### Comparing `baize-0.8.2/pyproject.toml` & `baize-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["abersheeran <me@abersheeran.com>"]
 description = "Powerful and exquisite WSGI/ASGI framework/toolkit."
 license = "Apache-2.0"
 name = "baize"
 readme = "README.md"
-version = "0.8.2"
+version = "0.9.0"
 
 homepage = "https://github.com/abersheeran/baize"
 repository = "https://github.com/abersheeran/baize"
 
 classifiers = [
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.6",
```

### Comparing `baize-0.8.2/setup.py` & `baize-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['typing-extensions>=3.7.4,<4.0.0'],
  'multipart': ['python-multipart>=0.0.5,<0.0.6']}
 
 setup_kwargs = {
     'name': 'baize',
-    'version': '0.8.2',
+    'version': '0.9.0',
     'description': 'Powerful and exquisite WSGI/ASGI framework/toolkit.',
     'long_description': '# BáiZé\n\n[![Codecov](https://img.shields.io/codecov/c/github/abersheeran/baize?style=flat-square)](https://codecov.io/gh/abersheeran/baize)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/baize?label=Support%20Python%20Version&style=flat-square)](https://pypi.org/project/baize/)\n\nPowerful and exquisite WSGI/ASGI framework/toolkit.\n\nThe minimize implementation of methods required in the Web framework. No redundant implementation means that you can freely customize functions without considering the conflict with baize\'s own implementation.\n\nUnder the ASGI/WSGI protocol, the interface of the request object and the response object is almost the same, only need to add or delete `await` in the appropriate place. In addition, it should be noted that ASGI supports WebSocket but WSGI does not.\n\n- Support range file response, server-sent event response\n- Support WebSocket (only ASGI)\n- WSGI, ASGI routing to combine any application like [Django(wsgi)](https://docs.djangoproject.com/en/3.0/howto/deployment/wsgi/)/[Pyramid](https://trypyramid.com/)/[Bottle](https://bottlepy.org/)/[Flask](https://flask.palletsprojects.com/) or [Django(asgi)](https://docs.djangoproject.com/en/3.0/howto/deployment/asgi/)/[Index.py](https://index-py.aber.sh/)/[Starlette](https://www.starlette.io/)/[FastAPI](https://fastapi.tiangolo.com/)/[Sanic](https://sanic.readthedocs.io/en/stable/)/[Quart](https://pgjones.gitlab.io/quart/)\n\n## Install\n\n```\npip install -U baize\n```\n\nOr install from GitHub master branch\n\n```\npip install -U git+https://github.com/abersheeran/baize@setup.py\n```\n\n## Document and other website\n\n[BáiZé Document](https://baize.aber.sh/)\n\nIf you have questions or idea, you can send it to [Discussions](https://github.com/abersheeran/baize/discussions).\n\n## Quick Start\n\nA short example for WSGI application, if you don\'t know what is WSGI, please read [PEP3333](https://www.python.org/dev/peps/pep-3333/).\n\n```python\nfrom baize.wsgi import request_response, Router, Request, Response, PlainTextResponse\n\n\n@request_response\ndef sayhi(request: Request) -> Response:\n    return PlainTextResponse("hi, " + request.path_params["name"])\n\n\n@request_response\ndef echo(request: Request) -> Response:\n    return PlainTextResponse(request.body)\n\n\napplication = Router(\n    ("/", PlainTextResponse("homepage")),\n    ("/echo", echo),\n    ("/sayhi/{name}", sayhi),\n)\n\n\nif __name__ == "__main__":\n    import uvicorn\n\n    uvicorn.run(application, interface="wsgi", port=8000)\n```\n\nA short example for ASGI application, if you don\'t know what is ASGI, please read [ASGI Documention](https://asgi.readthedocs.io/en/latest/).\n\n```python\nfrom baize.asgi import request_response, Router, Request, Response, PlainTextResponse\n\n\n@request_response\nasync def sayhi(request: Request) -> Response:\n    return PlainTextResponse("hi, " + request.path_params["name"])\n\n\n@request_response\nasync def echo(request: Request) -> Response:\n    return PlainTextResponse(await request.body)\n\n\napplication = Router(\n    ("/", PlainTextResponse("homepage")),\n    ("/echo", echo),\n    ("/sayhi/{name}", sayhi),\n)\n\n\nif __name__ == "__main__":\n    import uvicorn\n\n    uvicorn.run(application, interface="asgi3", port=8000)\n```\n\n## License\n\nApache-2.0.\n\nYou can do whatever you want with the permission of the license.\n',
     'author': 'abersheeran',
     'author_email': 'me@abersheeran.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/abersheeran/baize',
```

### Comparing `baize-0.8.2/PKG-INFO` & `baize-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baize
-Version: 0.8.2
+Version: 0.9.0
 Summary: Powerful and exquisite WSGI/ASGI framework/toolkit.
 Home-page: https://github.com/abersheeran/baize
 License: Apache-2.0
 Author: abersheeran
 Author-email: me@abersheeran.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

