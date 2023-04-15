# Comparing `tmp/feynml-0.1.3.tar.gz` & `tmp/feynml-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynml-0.1.3.tar", max compression
+gzip compressed data, was "feynml-0.1.7.tar", max compression
```

## Comparing `feynml-0.1.3.tar` & `feynml-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-12 05:50:36.884966 feynml-0.1.3/LICENSE
--rw-r--r--   0        0        0     2359 2023-04-12 05:50:36.884966 feynml-0.1.3/README.md
--rw-r--r--   0        0        0      179 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/__init__.py
--rw-r--r--   0        0        0      986 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/connector.py
--rw-r--r--   0        0        0     6456 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/feynmandiagram.py
--rw-r--r--   0        0        0     2716 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/feynml.py
--rw-r--r--   0        0        0      651 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/id.py
--rw-r--r--   0        0        0        0 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/interface/__init__.py
--rw-r--r--   0        0        0     1563 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/interface/hepmc.py
--rw-r--r--   0        0        0     1569 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/interface/qgraf.py
--rw-r--r--   0        0        0      385 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/labeled.py
--rw-r--r--   0        0        0     1035 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/leg.py
--rw-r--r--   0        0        0      303 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/line.py
--rw-r--r--   0        0        0      563 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/momentum.py
--rw-r--r--   0        0        0     1385 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/particles.py
--rw-r--r--   0        0        0     3115 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/pdgid.py
--rw-r--r--   0        0        0      846 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/point.py
--rw-r--r--   0        0        0      207 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/propagator.py
--rw-r--r--   0        0        0      363 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/sourcing.py
--rw-r--r--   0        0        0     2749 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/styled.py
--rw-r--r--   0        0        0      364 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/targeting.py
--rw-r--r--   0        0        0     4181 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/types.py
--rw-r--r--   0        0        0      425 2023-04-12 05:50:36.884966 feynml-0.1.3/feynml/vertex.py
--rw-r--r--   0        0        0     1641 2023-04-12 05:50:39.340987 feynml-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 feynml-0.1.3/setup.py
--rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 feynml-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 21:12:25.141286 feynml-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2359 2023-04-15 21:12:25.141286 feynml-0.1.7/README.md
+-rw-r--r--   0        0        0      179 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/__init__.py
+-rw-r--r--   0        0        0      986 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/connector.py
+-rw-r--r--   0        0        0     6932 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/feynmandiagram.py
+-rw-r--r--   0        0        0     3096 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/feynml.py
+-rw-r--r--   0        0        0      651 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/id.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/interface/__init__.py
+-rw-r--r--   0        0        0     1563 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/interface/hepmc.py
+-rw-r--r--   0        0        0     1569 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/interface/qgraf.py
+-rw-r--r--   0        0        0      385 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/labeled.py
+-rw-r--r--   0        0        0     1035 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/leg.py
+-rw-r--r--   0        0        0      303 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/line.py
+-rw-r--r--   0        0        0      563 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/momentum.py
+-rw-r--r--   0        0        0     1385 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/particles.py
+-rw-r--r--   0        0        0     3115 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/pdgid.py
+-rw-r--r--   0        0        0      846 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/point.py
+-rw-r--r--   0        0        0      207 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/propagator.py
+-rw-r--r--   0        0        0      363 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/sourcing.py
+-rw-r--r--   0        0        0     2749 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/styled.py
+-rw-r--r--   0        0        0      364 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/targeting.py
+-rw-r--r--   0        0        0     4182 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/types.py
+-rw-r--r--   0        0        0      425 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/vertex.py
+-rw-r--r--   0        0        0     1641 2023-04-15 21:12:26.821293 feynml-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 feynml-0.1.7/setup.py
+-rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 feynml-0.1.7/PKG-INFO
```

### Comparing `feynml-0.1.3/LICENSE` & `feynml-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/README.md` & `feynml-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/connector.py` & `feynml-0.1.7/feynml/connector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/feynmandiagram.py` & `feynml-0.1.7/feynml/feynmandiagram.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         metadata={
             "name": "style",
             "xml_attribute": True,
             "type": "Attribute",
             "namespace": "",
         },
     )
+    # external_sheet is used to store the sheet from the file
+    # so that we can use it to update the sheet.
+    # It is not saved to the fml file.
+    external_sheet: CSSSheet = None
 
     def add(self, *fd_all: List[Union[Propagator, Vertex, Leg]]):
         for a in fd_all:
             if isinstance(a, Propagator):
                 self.propagators.append(a)
             elif isinstance(a, Vertex):
                 self.vertices.append(a)
@@ -119,14 +123,22 @@
     def with_rule(self, rule: str):
         return self.with_rules(rule)
 
     def with_rules(self, rules: str):
         self.sheet = cssutils.parseString(rules)
         return self
 
+    def get_style_property(self, obj, property_name):
+        style = self.get_style(obj)
+        p = style.getProperty(property_name)
+        if p is None:
+            return None
+        else:
+            return p.value
+
     def get_style(self, obj) -> cssutils.css.CSSStyleDeclaration:
         """Get the style of an object.
 
         This is prefered over accessing the style attribute directly, sicne it includes class and pdgid definitions.
         """
         # selectorText is string
         css = []
@@ -152,19 +164,20 @@
             return obj.id in [e.get("id") for e in document.xpath(expression)]
 
         return self._get_style(lambdaselector)
 
     def _get_style(self, lambdaselector) -> cssutils.css.CSSStyleDeclaration:
 
         ret = []
-
+        sheets = []
         if self.default_style:
-            sheets = [get_default_sheet(), self.sheet]
-        else:
-            sheets = [self.sheet]
+            sheets += [get_default_sheet()]
+        sheets += [self.sheet]
+        if self.external_sheet:
+            sheets += [self.external_sheet]
         for sheet in sheets:
             idd = []
             cls = []
             rest = []
             glob = []
             for rule in sheet:
                 if rule.type == rule.STYLE_RULE:
```

### Comparing `feynml-0.1.3/feynml/feynml.py` & `feynml-0.1.7/feynml/feynml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import logging
 import warnings
 from dataclasses import dataclass, field
 from importlib.metadata import version
 from typing import List, Optional
 
 import cssutils
+from smpl_doc import doc
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from feynml.feynmandiagram import FeynmanDiagram
 
 # We don't want to see the cssutils warnings, since we have custom properties
 cssutils.log.setLevel(logging.CRITICAL)
 
 
-feynml_version = "0.0"
+feynml_version = version("feynml")
 
 
 @dataclass
 class Tool:
     class Meta:
         name = "tool"
 
+    # Deprecated to stay closer to html meta tags
+    @doc.deprecated("0.1.3", "Use feynml.feynml.Meta instead.")
+    def __init__(*args, **kwargs):
+        super().__init__(*args, **kwargs)
+
     name: Optional[str] = field(default="feynml", metadata={"type": "Element"})
     version: Optional[str] = field(
         default=version("feynml"), metadata={"type": "Element"}
     )
 
 
 @dataclass
@@ -50,14 +56,20 @@
         default_factory=list,
         metadata={"name": "meta", "namespace": ""},
     )
     description: Optional[str] = field(default="", metadata={"type": "Element"})
 
     style: Optional[str] = field(default="", metadata={"type": "Element"})
 
+    def get_meta_dict(self):
+        """
+        Return a dictionary of meta tags.
+        """
+        return {m.name: m.content for m in self.metas}
+
 
 @dataclass
 class FeynML:
     class Meta:
         name = "feynml"
 
     version: Optional[str] = field(
```

### Comparing `feynml-0.1.3/feynml/id.py` & `feynml-0.1.7/feynml/id.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/interface/hepmc.py` & `feynml-0.1.7/feynml/interface/hepmc.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/interface/qgraf.py` & `feynml-0.1.7/feynml/interface/qgraf.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/leg.py` & `feynml-0.1.7/feynml/leg.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/momentum.py` & `feynml-0.1.7/feynml/momentum.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/particles.py` & `feynml-0.1.7/feynml/particles.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/pdgid.py` & `feynml-0.1.7/feynml/pdgid.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/point.py` & `feynml-0.1.7/feynml/point.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/styled.py` & `feynml-0.1.7/feynml/styled.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.3/feynml/types.py` & `feynml-0.1.7/feynml/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 default_sheet = cssutils.parseString(
     """
         /*************************************************************************/
         /* Diagram */
         /*************************************************************************/
 
         diagram {
-            direction: right;
+            direction : right;
             layout : neato;
         }
 
         /*************************************************************************/
         /* Vertex */
         /*************************************************************************/
```

### Comparing `feynml-0.1.3/pyproject.toml` & `feynml-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynml"
-version = "0.1.3"
+version = "0.1.7"
 description = "Feynman diagram markup language"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynml"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `feynml-0.1.3/setup.py` & `feynml-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'xsdata[cli,lxml,soap]']
 
 extras_require = \
 {'interface': ['pyqgraf>=0.0.3', 'pyhepmc']}
 
 setup_kwargs = {
     'name': 'feynml',
-    'version': '0.1.3',
+    'version': '0.1.7',
     'description': 'Feynman diagram markup language',
     'long_description': '# FeynML\n\nFeynML from <https://feynml.hepforge.org/>\n\nFeynML is a project to develop an XML dialect for describing Feynman diagrams as used in quantum field theory calculations. The primary aim is to unambiguously describe the structure of a diagram in XML, giving a de facto representation for diagram structure which can be easily translated into another representation.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n\n[pypi image]: https://badge.fury.io/py/feynml.svg\n[pypi link]: https://pypi.org/project/feynml/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynml.svg\n\n[a t link]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynml&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynml&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynml?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynml/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynml',
```

### Comparing `feynml-0.1.3/PKG-INFO` & `feynml-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynml
-Version: 0.1.3
+Version: 0.1.7
 Summary: Feynman diagram markup language
 Home-page: https://github.com/APN-Pucky/feynml
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

