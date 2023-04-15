# Comparing `tmp/pygedcom-0.1.7.tar.gz` & `tmp/pygedcom-0.1.8.tar.gz`

## Comparing `pygedcom-0.1.7.tar` & `pygedcom-0.1.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.7/main.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.1.7/requirements.txt
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.7/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/Makefile
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/conf.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/export.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.1.7/docs/sources/parsing.rst
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    21491 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/note.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/rootElements/submitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.7/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_add_elements.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_parse.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_remove_element.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_set_prop.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/test_verify.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.7/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.7/LICENSE
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pygedcom-0.1.7/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pygedcom-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.8/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygedcom-0.1.8/main.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.8/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/Makefile
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/conf.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/export.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.1.8/docs/sources/parsing.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    21491 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.8/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/test_add_elements.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/test_parse.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/test_remove_element.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/test_set_prop.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/test_verify.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.8/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pygedcom-0.1.8/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pygedcom-0.1.8/PKG-INFO
```

### Comparing `pygedcom-0.1.7/requirements.txt` & `pygedcom-0.1.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/.github/workflows/python-publish.yml` & `pygedcom-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/.github/workflows/test_and_doc.yml` & `pygedcom-0.1.8/.github/workflows/test_and_doc.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/Makefile` & `pygedcom-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/conf.py` & `pygedcom-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/index.rst` & `pygedcom-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/make.bat` & `pygedcom-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/sources/export.rst` & `pygedcom-0.1.8/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/sources/gedcomRootElement.rst` & `pygedcom-0.1.8/docs/sources/gedcomRootElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/sources/getting_started.rst` & `pygedcom-0.1.8/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/docs/sources/parsing.rst` & `pygedcom-0.1.8/docs/sources/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/gedcom_parser.py` & `pygedcom-0.1.8/src/pygedcom/gedcom_parser.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/element.py` & `pygedcom-0.1.8/src/pygedcom/elements/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,9 +203,9 @@
                 if isinstance(export_value, GedcomElement):
                     export_dict[export_key] = export_value.export(
                         empty_fields=empty_fields
                     )
                 elif not export_value and not empty_fields:
                     pass
                 else:
-                    export_dict[export_key] = export_value if export_value else ""
+                    export_dict[export_key] = export_value
         return export_dict
```

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/mapping.json` & `pygedcom-0.1.8/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/family.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/family.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/head.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/individual.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/note.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/note.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/object.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/repository.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/rootElements/submitter.py` & `pygedcom-0.1.8/src/pygedcom/elements/rootElements/submitter.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.1.8/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.1.8/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.1.8/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.1.8/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/test/test_add_elements.py` & `pygedcom-0.1.8/test/test_add_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     assert parser.families[1].get_wife() == "@I2@"
     result = json.loads(parser.export())
     assert result["families"]["@F1@"]["husband"] == "@I1@"
     assert result["families"]["@F1@"]["wife"] == "@I2@"
     assert result["families"]["@F1@"]["children"] == ["@I3@"]
     assert result["families"]["@F2@"]["husband"] == "@I1@"
     assert result["families"]["@F2@"]["wife"] == "@I2@"
-    assert result["families"]["@F2@"]["children"] == ""
+    assert result["families"]["@F2@"]["children"] == []
```

### Comparing `pygedcom-0.1.7/test/test_export.py` & `pygedcom-0.1.8/test/test_export.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/test/test_parse.py` & `pygedcom-0.1.8/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/test/test_remove_element.py` & `pygedcom-0.1.8/test/test_remove_element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/test/test_set_prop.py` & `pygedcom-0.1.8/test/test_set_prop.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/test/test_verify.py` & `pygedcom-0.1.8/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/test/samples/20_complex_sample.ged` & `pygedcom-0.1.8/test/samples/20_complex_sample.ged`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/.gitignore` & `pygedcom-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/LICENSE` & `pygedcom-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.7/README.md` & `pygedcom-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,35 +36,35 @@
 print(parser.get_stats())
 ```
 
 It's a good practice to verify your GEDCOM file before parsing it. You can do this with the following command:
 
 
 ```python
-verif = parser.verify()
-if verif.status == 'ok':
+check = parser.verify()
+if check.status == 'ok':
     print("Your GEDCOM file is valid")
 else:
     print("Your GEDCOM file is not valid")
-    print(verif.errors)
+    print(check.errors)
 ```
 
 Here is the full setup block:
 
 ```python
 import pygedcom
 
 parser = pygedcom.GedcomParser(path="path/to/your/gedcom_file.ged")
-verif = parser.verify()
+check = parser.verify()
 
-if verif.status == 'ok':
+if check.status == 'ok':
     print("Your GEDCOM file is valid")
 else:
     print("Your GEDCOM file is not valid")
-    print(verif.errors)
+    print(check.errors)
 
 print(parser.get_stats())
 ```
 
 ## Parsing
```

### Comparing `pygedcom-0.1.7/pyproject.toml` & `pygedcom-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.1.7/PKG-INFO` & `pygedcom-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.1.7
+Version: 0.1.8
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,35 +50,35 @@
 print(parser.get_stats())
 ```
 
 It's a good practice to verify your GEDCOM file before parsing it. You can do this with the following command:
 
 
 ```python
-verif = parser.verify()
-if verif.status == 'ok':
+check = parser.verify()
+if check.status == 'ok':
     print("Your GEDCOM file is valid")
 else:
     print("Your GEDCOM file is not valid")
-    print(verif.errors)
+    print(check.errors)
 ```
 
 Here is the full setup block:
 
 ```python
 import pygedcom
 
 parser = pygedcom.GedcomParser(path="path/to/your/gedcom_file.ged")
-verif = parser.verify()
+check = parser.verify()
 
-if verif.status == 'ok':
+if check.status == 'ok':
     print("Your GEDCOM file is valid")
 else:
     print("Your GEDCOM file is not valid")
-    print(verif.errors)
+    print(check.errors)
 
 print(parser.get_stats())
 ```
 
 ## Parsing
```

