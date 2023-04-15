# Comparing `tmp/fastapi-soap-0.0.1.tar.gz` & `tmp/fastapi-soap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-soap-0.0.1.tar", max compression
+gzip compressed data, was "fastapi-soap-0.0.2.tar", max compression
```

## Comparing `fastapi-soap-0.0.1.tar` & `fastapi-soap-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1262 2023-04-14 08:52:16.242642 fastapi-soap-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-02-23 10:08:22.933124 fastapi-soap-0.0.1/fastapi_soap/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-13 10:53:08.933885 fastapi-soap-0.0.1/fastapi_soap/exceptions.py
--rw-r--r--   0        0        0     2966 2023-04-13 14:00:36.081413 fastapi-soap-0.0.1/fastapi_soap/models.py
--rw-r--r--   0        0        0     2221 2023-04-13 17:02:01.459950 fastapi-soap-0.0.1/fastapi_soap/request.py
--rw-r--r--   0        0        0     2068 2023-04-13 14:45:44.752264 fastapi-soap-0.0.1/fastapi_soap/response.py
--rw-r--r--   0        0        0     3951 2023-04-13 14:00:36.099063 fastapi-soap-0.0.1/fastapi_soap/routes.py
--rw-r--r--   0        0        0     5390 2023-04-13 17:23:24.456277 fastapi-soap-0.0.1/fastapi_soap/wsdl.py
--rw-r--r--   0        0        0     1204 2023-04-14 09:42:29.737990 fastapi-soap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 fastapi-soap-0.0.1/setup.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 fastapi-soap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1265 2023-04-15 11:15:06.827252 fastapi-soap-0.0.2/README.md
+-rw-r--r--   0        0        0      302 2023-04-15 19:51:41.782214 fastapi-soap-0.0.2/fastapi_soap/__init__.py
+-rw-r--r--   0        0        0     1056 2023-04-15 11:14:45.325982 fastapi-soap-0.0.2/fastapi_soap/exceptions.py
+-rw-r--r--   0        0        0     2966 2023-04-15 11:14:45.326329 fastapi-soap-0.0.2/fastapi_soap/models.py
+-rw-r--r--   0        0        0     2239 2023-04-15 19:52:57.075144 fastapi-soap-0.0.2/fastapi_soap/request.py
+-rw-r--r--   0        0        0     2068 2023-04-15 11:14:45.327064 fastapi-soap-0.0.2/fastapi_soap/response.py
+-rw-r--r--   0        0        0     3951 2023-04-15 11:14:45.327474 fastapi-soap-0.0.2/fastapi_soap/routes.py
+-rw-r--r--   0        0        0     5467 2023-04-15 19:55:00.907192 fastapi-soap-0.0.2/fastapi_soap/wsdl.py
+-rw-r--r--   0        0        0     1204 2023-04-15 19:56:18.090362 fastapi-soap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 fastapi-soap-0.0.2/setup.py
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 fastapi-soap-0.0.2/PKG-INFO
```

### Comparing `fastapi-soap-0.0.1/README.md` & `fastapi-soap-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FastAPI Soap
 
 This package helps to create Soap WebServices using FastAPI (What?!?!)
 
 ## Motivation
-I know, FastAPI is a REST micro framework, but sometimes is needed expose a Soap Interface on a already running FastAPI application for an legacy client/application that only supports, well, the Soap protocol...
+I know, FastAPI is a REST micro framework, but sometimes is needed to expose a Soap Interface on a already running FastAPI application for an legacy client/application that only supports, well, the Soap protocol...
 
 ## Installation and dependencies
 Only FastAPI, Pydantic and Pydantic XML are required.
 
 
 ## First steps
```

### Comparing `fastapi-soap-0.0.1/fastapi_soap/exceptions.py` & `fastapi-soap-0.0.2/fastapi_soap/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-soap-0.0.1/fastapi_soap/models.py` & `fastapi-soap-0.0.2/fastapi_soap/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-soap-0.0.1/fastapi_soap/request.py` & `fastapi-soap-0.0.2/fastapi_soap/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Type, TypeVar, cast
 
 from fastapi import Body, Depends
 from pydantic import ValidationError
+from fastapi_soap.exceptions import ClientFaultException
 
 from fastapi_soap.models import (
     BodyContent,
-    FaultResponse,
     SoapBody,
     SoapEnvelope,
-    SoapHeader,
+    SoapHeader
 )
 
 SoapEnvelopeType = TypeVar('SoapEnvelopeType', bound=SoapEnvelope)
 """Generic type for SoapEnvelope"""
 
 
 def XMLBody(model: Type[BodyContent]) -> Any:
@@ -43,15 +43,15 @@
         try:
             envelope = cast(
                 SoapEnvelope[SoapHeader, SoapBody[model]],
                 model_.from_xml(data),
             )
             return envelope.body.call
         except ValidationError as err:
-            return FaultResponse(faultcode='client', faultstring=str(err))
+            raise ClientFaultException(detail=str(err))
 
     return Depends(parse_model)
 
 
 def XMLHeader(model: Type[SoapHeader]) -> Any:
     """Dependency to load the header from a soap request.
```

### Comparing `fastapi-soap-0.0.1/fastapi_soap/response.py` & `fastapi-soap-0.0.2/fastapi_soap/response.py`

 * *Files identical despite different names*

### Comparing `fastapi-soap-0.0.1/fastapi_soap/routes.py` & `fastapi-soap-0.0.2/fastapi_soap/routes.py`

 * *Files identical despite different names*

### Comparing `fastapi-soap-0.0.1/fastapi_soap/wsdl.py` & `fastapi-soap-0.0.2/fastapi_soap/wsdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,32 +35,36 @@
 ) -> Element:
     element = Element('xs:element')
     model_ = model or getattr(model_field, 'type_')
 
     if model is not None:
         element.set('name', model.__xml_tag__)
     elif model_field and hasattr(model_field.field_info, 'tag'):
-        tag_name = model_field.field_info.tag or model_field.name
+        tag_name = (
+            model_field.field_info.tag
+            or model_field.field_info.alias
+            or model_field.name
+        )
         element.set('name', tag_name)
     elif hasattr(model_, '__xml_tag__'):
         element.set('name', model_.__xml_tag__)
     elif isinstance(getattr(model_, 'field_info', None), XmlElementInfo):
         element.set('name', model_field.name)
     else:
         element.set('name', model_field.name)
 
     if isinstance(model_, XmlModelMeta):
-        complext_type = Element('xs:complexType')
-        sequence = ET.SubElement(complext_type, 'xs:sequence')
+        complex_type = Element('xs:complexType')
+        sequence = ET.SubElement(complex_type, 'xs:sequence')
 
         for model_field_ in model_.__fields__.values():
             tag = generate_xsd_element(model_field=model_field_)
             sequence.append(tag)
 
-        element.append(complext_type)
+        element.append(complex_type)
 
     else:
         element_type = PYTHON_XSD_TYPE_MAP.get(
             display_as_type(model_), 'string'
         )
         element.set('type', f'xs:{element_type}')
```

### Comparing `fastapi-soap-0.0.1/pyproject.toml` & `fastapi-soap-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-soap"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Cleiton Junior Mittmann <mittmannv8@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_soap"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
```

### Comparing `fastapi-soap-0.0.1/setup.py` & `fastapi-soap-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['fastapi>=0.95.0,<0.96.0',
  'lxml>=4.9.2,<5.0.0',
  'pydantic-xml[lxml]>=0.6.0,<0.7.0',
  'pydantic>=1.10.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-soap',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
-    'long_description': '# FastAPI Soap\n\nThis package helps to create Soap WebServices using FastAPI (What?!?!)\n\n## Motivation\nI know, FastAPI is a REST micro framework, but sometimes is needed expose a Soap Interface on a already running FastAPI application for an legacy client/application that only supports, well, the Soap protocol...\n\n## Installation and dependencies\nOnly FastAPI, Pydantic and Pydantic XML are required.\n\n\n## First steps\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_soap.models import BodyContent\n\n\nclass Operands(BodyContent, tag="Operands"):\n    operands: list[float] = element(tag="Operand")\n\nclass Result(BodyContent, tag="Result"):\n    value: float\n\nsoap = SoapRouter(name=\'Calculator\', prefix=\'/Calculator\')\n\n@soap.operation(\n    name="SumOperation",\n    request_model=Operands,\n    response_model=Result\n)\ndef sum_operation(body: Operands = XMLBody(Operands)):\n    result = sum(body.operands)\n    \n    return SoapResponse(\n        Result(value=result)\n    )\n\n\napp = FastAPI()\napp.include_router(soap)\n\nif __name__ == \'__main__\':\n    import uvicorn\n    uvicorn.run("example.main:app")\n```\n_(This script is complete, it should run "as is")_\n\n\nThe WSDL is available on webservice root path for GET method.\n```\nGET http://localhost:8000/Calculator/\n```\n\n',
+    'long_description': '# FastAPI Soap\n\nThis package helps to create Soap WebServices using FastAPI (What?!?!)\n\n## Motivation\nI know, FastAPI is a REST micro framework, but sometimes is needed to expose a Soap Interface on a already running FastAPI application for an legacy client/application that only supports, well, the Soap protocol...\n\n## Installation and dependencies\nOnly FastAPI, Pydantic and Pydantic XML are required.\n\n\n## First steps\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_soap.models import BodyContent\n\n\nclass Operands(BodyContent, tag="Operands"):\n    operands: list[float] = element(tag="Operand")\n\nclass Result(BodyContent, tag="Result"):\n    value: float\n\nsoap = SoapRouter(name=\'Calculator\', prefix=\'/Calculator\')\n\n@soap.operation(\n    name="SumOperation",\n    request_model=Operands,\n    response_model=Result\n)\ndef sum_operation(body: Operands = XMLBody(Operands)):\n    result = sum(body.operands)\n    \n    return SoapResponse(\n        Result(value=result)\n    )\n\n\napp = FastAPI()\napp.include_router(soap)\n\nif __name__ == \'__main__\':\n    import uvicorn\n    uvicorn.run("example.main:app")\n```\n_(This script is complete, it should run "as is")_\n\n\nThe WSDL is available on webservice root path for GET method.\n```\nGET http://localhost:8000/Calculator/\n```\n\n',
     'author': 'Cleiton Junior Mittmann',
     'author_email': 'mittmannv8@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi-soap-0.0.1/PKG-INFO` & `fastapi-soap-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-soap
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Cleiton Junior Mittmann
 Author-email: mittmannv8@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 
 # FastAPI Soap
 
 This package helps to create Soap WebServices using FastAPI (What?!?!)
 
 ## Motivation
-I know, FastAPI is a REST micro framework, but sometimes is needed expose a Soap Interface on a already running FastAPI application for an legacy client/application that only supports, well, the Soap protocol...
+I know, FastAPI is a REST micro framework, but sometimes is needed to expose a Soap Interface on a already running FastAPI application for an legacy client/application that only supports, well, the Soap protocol...
 
 ## Installation and dependencies
 Only FastAPI, Pydantic and Pydantic XML are required.
 
 
 ## First steps
```

