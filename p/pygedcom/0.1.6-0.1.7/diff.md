# Comparing `tmp/pygedcom-0.1.6.tar.gz` & `tmp/pygedcom-0.1.7.tar.gz`

## Comparing `pygedcom-0.1.6.tar` & `pygedcom-0.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.6/main.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.1.6/requirements.txt
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.6/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/Makefile
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/conf.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/export.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/parsing.rst
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/note.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/submitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_add_elements.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_parse.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_remove_element.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_set_prop.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_verify.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.6/LICENSE
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pygedcom-0.1.6/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pygedcom-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.7/main.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.1.7/requirements.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.7/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/Makefile
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/conf.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/export.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/parsing.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    21491 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_add_elements.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_parse.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_remove_element.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_set_prop.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_verify.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pygedcom-0.1.7/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pygedcom-0.1.7/PKG-INFO
```

### Comparing `pygedcom-0.1.6/requirements.txt` & `pygedcom-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/.github/workflows/python-publish.yml` & `pygedcom-0.1.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/.github/workflows/test_and_doc.yml` & `pygedcom-0.1.7/.github/workflows/test_and_doc.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/Makefile` & `pygedcom-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/conf.py` & `pygedcom-0.1.7/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = 'sphinx_material'
+html_theme = "sphinx_material"
```

### Comparing `pygedcom-0.1.6/docs/index.rst` & `pygedcom-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/make.bat` & `pygedcom-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/sources/export.rst` & `pygedcom-0.1.7/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/sources/gedcomRootElement.rst` & `pygedcom-0.1.7/docs/sources/gedcomRootElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/sources/getting_started.rst` & `pygedcom-0.1.7/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/docs/sources/parsing.rst` & `pygedcom-0.1.7/docs/sources/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/gedcom_parser.py` & `pygedcom-0.1.7/src/pygedcom/gedcom_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,18 +171,20 @@
     def parse(self) -> dict:
         """Parse the GEDCOM file and return a dictionary with the parsed elements
 
         :return: A dictionary with the parsed elements.
         :rtype: dict
         """
         self.head = None
+        self.submitters = []
         self.individuals = []
         self.families = []
         self.sources = []
         self.objects = []
+        self.notes = []
         self.repositories = []
         file = self.__open()
         lines = file.split("\n")
         current_parsed_line = self.__parse_line(lines[0])
         element_lines = []
         if lines != []:
             for line in lines[1:]:
@@ -192,33 +194,38 @@
                         element_lines.append(line)
                     else:
                         self.__create_element(current_parsed_line, element_lines)
                         current_parsed_line = tmp_parsed_line
                         element_lines = []
             self.__create_element(current_parsed_line, element_lines)
         return {
+            "head": self.head,
             "individuals": self.individuals,
+            "submitters": self.submitters,
             "families": self.families,
             "sources": self.sources,
             "objects": self.objects,
+            "notes": self.notes,
             "repositories": self.repositories,
         }
 
     def get_stats(self) -> dict:
         """Get statistics about the GEDCOM file.
 
         :return: A dictionary with the statistics.
         :rtype: dict
         """
         return {
             "head": "OK" if self.head is not None else "None",
+            "submitters": len(self.submitters),
             "individuals": len(self.individuals),
             "families": len(self.families),
             "sources": len(self.sources),
             "objects": len(self.objects),
+            "notes": len(self.notes),
             "repositories": len(self.repositories),
         }
 
     def export(self, format: str = "json", empty_fields=True) -> str:
         """Export the GEDCOM file to another format.
 
         :param format: The format to export to. Default is "json".
```

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/element.py` & `pygedcom-0.1.7/src/pygedcom/elements/element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/mapping.json` & `pygedcom-0.1.7/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/family.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/family.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/head.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/individual.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/note.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/note.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/object.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/repository.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/rootElements/submitter.py` & `pygedcom-0.1.7/src/pygedcom/elements/rootElements/submitter.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.1.7/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.1.7/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.1.7/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.1.7/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/test_add_elements.py` & `pygedcom-0.1.7/test/test_add_elements.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/test_export.py` & `pygedcom-0.1.7/test/test_export.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/test_parse.py` & `pygedcom-0.1.7/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/test_remove_element.py` & `pygedcom-0.1.7/test/test_remove_element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/test_set_prop.py` & `pygedcom-0.1.7/test/test_set_prop.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/test_verify.py` & `pygedcom-0.1.7/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/test/samples/20_complex_sample.ged` & `pygedcom-0.1.7/test/samples/20_complex_sample.ged`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/.gitignore` & `pygedcom-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/LICENSE` & `pygedcom-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/README.md` & `pygedcom-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.6/pyproject.toml` & `pygedcom-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.1.6/PKG-INFO` & `pygedcom-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.1.6
+Version: 0.1.7
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

