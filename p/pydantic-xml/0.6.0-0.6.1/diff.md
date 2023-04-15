# Comparing `tmp/pydantic_xml-0.6.0.tar.gz` & `tmp/pydantic_xml-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-0.6.0.tar", max compression
+gzip compressed data, was "pydantic_xml-0.6.1.tar", max compression
```

## Comparing `pydantic_xml-0.6.0.tar` & `pydantic_xml-0.6.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1211 2023-02-05 07:29:46.152163 pydantic_xml-0.6.0/LICENSE
--rw-r--r--   0        0        0     3182 2023-02-05 07:29:46.152163 pydantic_xml-0.6.0/README.rst
--rw-r--r--   0        0        0      599 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    12576 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      364 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      569 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/errors.py
--rw-r--r--   0        0        0    11265 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/py.typed
--rw-r--r--   0        0        0       73 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0     1445 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/encoder.py
--rw-r--r--   0        0        0      342 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     4246 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4074 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     4732 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0     6781 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     4220 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     6019 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2933 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     6267 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0       48 2023-02-05 07:29:46.156163 pydantic_xml-0.6.0/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-02-05 07:29:46.160163 pydantic_xml-0.6.0/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1850 2023-02-05 07:29:46.160163 pydantic_xml-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 pydantic_xml-0.6.0/setup.py
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 pydantic_xml-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 15:03:55.918234 pydantic_xml-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3182 2023-04-15 15:03:55.918234 pydantic_xml-0.6.1/README.rst
+-rw-r--r--   0        0        0      599 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    12576 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      364 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      569 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    11299 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       73 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0     1445 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/encoder.py
+-rw-r--r--   0        0        0      342 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     4246 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4074 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     4732 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0     6781 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     4220 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     6019 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2933 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     6267 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0       48 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1849 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 pydantic_xml-0.6.1/PKG-INFO
```

### Comparing `pydantic_xml-0.6.0/LICENSE` & `pydantic_xml-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/README.rst` & `pydantic_xml-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/__init__.py` & `pydantic_xml-0.6.1/pydantic_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/element/element.py` & `pydantic_xml-0.6.1/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/element/native/lxml.py` & `pydantic_xml-0.6.1/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/element/native/std.py` & `pydantic_xml-0.6.1/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/errors.py` & `pydantic_xml-0.6.1/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/model.py` & `pydantic_xml-0.6.1/pydantic_xml/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,16 +214,16 @@
 
     def __init_subclass__(
             cls,
             *args: Any,
             tag: Optional[str] = None,
             ns: Optional[str] = None,
             nsmap: Optional[NsMap] = None,
-            ns_attrs: bool = False,
-            search_mode: SearchMode = SearchMode.STRICT,
+            ns_attrs: Optional[bool] = None,
+            search_mode: Optional[SearchMode] = None,
             **kwargs: Any,
     ):
         """
         Initializes a subclass.
 
         :param tag: element tag
         :param ns: element namespace
@@ -233,16 +233,17 @@
         """
 
         super().__init_subclass__(*args, **kwargs)
 
         cls.__xml_tag__ = tag if tag is not None else getattr(cls, '__xml_tag__', None)
         cls.__xml_ns__ = ns if ns is not None else getattr(cls, '__xml_ns__', None)
         cls.__xml_nsmap__ = nsmap if nsmap is not None else getattr(cls, '__xml_nsmap__', None)
-        cls.__xml_ns_attrs__ = ns_attrs if ns_attrs is not None else getattr(cls, '__xml_ns_attrs__', None)
-        cls.__xml_search_mode__ = search_mode if search_mode is not None else getattr(cls, '__xml_search_mode__', None)
+        cls.__xml_ns_attrs__ = ns_attrs if ns_attrs is not None else getattr(cls, '__xml_ns_attrs__', False)
+        cls.__xml_search_mode__ = search_mode if search_mode is not None \
+            else getattr(cls, '__xml_search_mode__', SearchMode.STRICT)
 
         default_xml_encoder: Callable[[Any], Any]
         if xml_encoders := getattr(cls.Config, 'xml_encoders', None):
             default_xml_encoder = ft.partial(pd.json.custom_pydantic_encoder, xml_encoders)
         else:
             default_xml_encoder = pd.json.pydantic_encoder
```

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/encoder.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/serializers/serializer.py` & `pydantic_xml-0.6.1/pydantic_xml/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pydantic_xml/utils.py` & `pydantic_xml-0.6.1/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.0/pyproject.toml` & `pydantic_xml-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "0.6.0"
+version = "0.6.1"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
@@ -41,15 +41,15 @@
 
 [tool.poetry.dev-dependencies]
 lxml-stubs = "^0.4.0"
 mypy = "^0.971"
 pre-commit = "^2.20.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
-xmldiff = "^2.4"
+xmldiff = "2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 allow_redefinition = true
```

### Comparing `pydantic_xml-0.6.0/setup.py` & `pydantic_xml-0.6.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydantic-xml
+Version: 0.6.1
+Summary: pydantic xml extension
+Home-page: https://github.com/dapper91/pydantic-xml
+License: Unlicense
+Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
+Author: Dmitry Pershin
+Author-email: dapper1291@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: License :: Public Domain
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: docs
+Provides-Extra: lxml
+Requires-Dist: Sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
+Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
+Requires-Dist: lxml (>=4.9.1,<5.0.0) ; extra == "lxml"
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: sphinx-copybutton (>=0.5.1,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) ; extra == "docs"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "docs"
+Project-URL: Documentation, https://github.com/dapper91/pydantic-xml
+Project-URL: Repository, https://github.com/dapper91/pydantic-xml
+Description-Content-Type: text/x-rst
+
+
+pydantic-xml extension
+======================
+
+.. image:: https://static.pepy.tech/personalized-badge/pydantic-xml?period=month&units=international_system&left_color=grey&right_color=orange&left_text=Downloads/month
+    :target: https://pepy.tech/project/pydantic-xml
+    :alt: Downloads/month
+.. image:: https://github.com/dapper91/pydantic-xml/actions/workflows/test.yml/badge.svg?branch=master
+    :target: https://github.com/dapper91/pydantic-xml/actions/workflows/test.yml
+    :alt: Build status
+.. image:: https://img.shields.io/pypi/l/pydantic-xml.svg
+    :target: https://pypi.org/project/pydantic-xml
+    :alt: License
+.. image:: https://img.shields.io/pypi/pyversions/pydantic-xml.svg
+    :target: https://pypi.org/project/pydantic-xml
+    :alt: Supported Python versions
+.. image:: https://codecov.io/gh/dapper91/pydantic-xml/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/dapper91/pydantic-xml
+    :alt: Code coverage
+.. image:: https://readthedocs.org/projects/pydantic-xml/badge/?version=stable&style=flat
+   :alt: ReadTheDocs status
+   :target: https://pydantic-xml.readthedocs.io/en/stable/
+
+
+``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev>`_ extension providing model fields xml binding
+and xml serialization / deserialization.
+It is closely integrated with ``pydantic`` which means it supports most of its features.
+
+
+Features
+--------
+
+- flexable attributes, elements and text binding
+- python collection types support (``Dict``, ``List``, ``Set``, ``Tuple``, ...)
+- ``Union`` type support
+- pydantic `generic <https://pydantic-docs.helpmanual.io/usage/models/#generic-models>`_ models support
+- `lxml <https://lxml.de/>`_ xml parser support
+- ``xml.etree.ElementTree`` standard library xml parser support
+
+What is not supported?
+______________________
+
+- `dynamic model creation <https://docs.pydantic.dev/usage/models/#dynamic-model-creation>`_
+- `dataclasses <https://docs.pydantic.dev/usage/dataclasses/>`_
+- `discriminated unions <https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions>`_
+
+Getting started
+---------------
+
+The following model fields binding:
+
+.. code-block:: python
+
+   class Product(BaseXmlModel):
+       status: Literal['running', 'development'] = attr()  # extracted from the 'status' attribute
+       launched: Optional[int] = attr()  # extracted from the 'launched' attribute
+       title: str  # extracted from the element text
+
+
+   class Company(BaseXmlModel):
+       trade_name: str = attr(name='trade-name')  # extracted from the 'trade-name' attribute
+       website: HttpUrl = element()  # extracted from the 'website' element text
+       products: List[Product] = element(tag='product')  # extracted from the 'website' element
+
+defines the XML document:
+
+.. code-block:: xml
+
+   <Company trade-name="SpaceX">
+       <website>https://www.spacex.com</website>
+       <product status="running" launched="2013">Several launch vehicles</product>
+       <product status="running" launched="2019">Starlink</product>
+       <product status="development">Starship</product>
+   </Company>
 
-packages = \
-['pydantic_xml',
- 'pydantic_xml.element',
- 'pydantic_xml.element.native',
- 'pydantic_xml.serializers',
- 'pydantic_xml.serializers.factories']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.9.0,<2.0.0']
-
-extras_require = \
-{'docs': ['furo>=2022.12.7,<2023.0.0',
-          'Sphinx>=5.3.0,<6.0.0',
-          'sphinx-copybutton>=0.5.1,<0.6.0',
-          'sphinx_design>=0.3.0,<0.4.0',
-          'toml>=0.10.2,<0.11.0'],
- 'lxml': ['lxml>=4.9.1,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'pydantic-xml',
-    'version': '0.6.0',
-    'description': 'pydantic xml extension',
-    'long_description': '\npydantic-xml extension\n======================\n\n.. image:: https://static.pepy.tech/personalized-badge/pydantic-xml?period=month&units=international_system&left_color=grey&right_color=orange&left_text=Downloads/month\n    :target: https://pepy.tech/project/pydantic-xml\n    :alt: Downloads/month\n.. image:: https://github.com/dapper91/pydantic-xml/actions/workflows/test.yml/badge.svg?branch=master\n    :target: https://github.com/dapper91/pydantic-xml/actions/workflows/test.yml\n    :alt: Build status\n.. image:: https://img.shields.io/pypi/l/pydantic-xml.svg\n    :target: https://pypi.org/project/pydantic-xml\n    :alt: License\n.. image:: https://img.shields.io/pypi/pyversions/pydantic-xml.svg\n    :target: https://pypi.org/project/pydantic-xml\n    :alt: Supported Python versions\n.. image:: https://codecov.io/gh/dapper91/pydantic-xml/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/dapper91/pydantic-xml\n    :alt: Code coverage\n.. image:: https://readthedocs.org/projects/pydantic-xml/badge/?version=stable&style=flat\n   :alt: ReadTheDocs status\n   :target: https://pydantic-xml.readthedocs.io/en/stable/\n\n\n``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev>`_ extension providing model fields xml binding\nand xml serialization / deserialization.\nIt is closely integrated with ``pydantic`` which means it supports most of its features.\n\n\nFeatures\n--------\n\n- flexable attributes, elements and text binding\n- python collection types support (``Dict``, ``List``, ``Set``, ``Tuple``, ...)\n- ``Union`` type support\n- pydantic `generic <https://pydantic-docs.helpmanual.io/usage/models/#generic-models>`_ models support\n- `lxml <https://lxml.de/>`_ xml parser support\n- ``xml.etree.ElementTree`` standard library xml parser support\n\nWhat is not supported?\n______________________\n\n- `dynamic model creation <https://docs.pydantic.dev/usage/models/#dynamic-model-creation>`_\n- `dataclasses <https://docs.pydantic.dev/usage/dataclasses/>`_\n- `discriminated unions <https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions>`_\n\nGetting started\n---------------\n\nThe following model fields binding:\n\n.. code-block:: python\n\n   class Product(BaseXmlModel):\n       status: Literal[\'running\', \'development\'] = attr()  # extracted from the \'status\' attribute\n       launched: Optional[int] = attr()  # extracted from the \'launched\' attribute\n       title: str  # extracted from the element text\n\n\n   class Company(BaseXmlModel):\n       trade_name: str = attr(name=\'trade-name\')  # extracted from the \'trade-name\' attribute\n       website: HttpUrl = element()  # extracted from the \'website\' element text\n       products: List[Product] = element(tag=\'product\')  # extracted from the \'website\' element\n\ndefines the XML document:\n\n.. code-block:: xml\n\n   <Company trade-name="SpaceX">\n       <website>https://www.spacex.com</website>\n       <product status="running" launched="2013">Several launch vehicles</product>\n       <product status="running" launched="2019">Starlink</product>\n       <product status="development">Starship</product>\n   </Company>\n\n\nCheck `documentation <https://pydantic-xml.readthedocs.io/en/latest/>`_ for more information.\n',
-    'author': 'Dmitry Pershin',
-    'author_email': 'dapper1291@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dapper91/pydantic-xml',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
 
+Check `documentation <https://pydantic-xml.readthedocs.io/en/latest/>`_ for more information.
 
-setup(**setup_kwargs)
```

