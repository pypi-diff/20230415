# Comparing `tmp/pygedcom-0.1.5.tar.gz` & `tmp/pygedcom-0.1.6.tar.gz`

## Comparing `pygedcom-0.1.5.tar` & `pygedcom-0.1.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.5/main.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.1.5/requirements.txt
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.5/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/Makefile
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/conf.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/export.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.1.5/docs/sources/parsing.rst
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/note.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/rootElements/submitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.5/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_add_elements.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_parse.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_remove_element.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_set_prop.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/test_verify.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.5/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.5/LICENSE
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.1.5/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.6/main.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.1.6/requirements.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.6/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/conf.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/export.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.1.6/docs/sources/parsing.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.6/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_add_elements.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_parse.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_remove_element.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_set_prop.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/test_verify.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.6/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pygedcom-0.1.6/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pygedcom-0.1.6/PKG-INFO
```

### Comparing `pygedcom-0.1.5/requirements.txt` & `pygedcom-0.1.6/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 alabaster==0.7.13
 attrs==22.2.0
 Babel==2.12.1
+beautifulsoup4==4.12.2
 black==23.1.0
 certifi==2022.12.7
 charset-normalizer==3.1.0
 click==8.1.3
+css-html-js-minify==2.5.5
 docutils==0.18.1
 exceptiongroup==1.1.1
 idna==3.4
 imagesize==1.4.1
 iniconfig==2.0.0
 Jinja2==3.1.2
+lxml==4.9.2
 MarkupSafe==2.1.2
 mypy-extensions==1.0.0
 packaging==23.0
 pathspec==0.11.1
 platformdirs==3.1.1
 pluggy==1.0.0
 py==1.11.0
 Pygments==2.14.0
 pytest==7.2.2
 pytest-html==3.2.0
 pytest-metadata==2.0.4
+python-slugify==8.0.1
 requests==2.28.2
 snowballstemmer==2.2.0
+soupsieve==2.4
 Sphinx==6.1.3
+sphinx-material==0.0.35
 sphinx-rtd-theme==1.2.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
+text-unidecode==1.3
 tomli==2.0.1
+Unidecode==1.3.6
 urllib3==1.26.15
```

### Comparing `pygedcom-0.1.5/.github/workflows/python-publish.yml` & `pygedcom-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/.github/workflows/test_and_doc.yml` & `pygedcom-0.1.6/.github/workflows/test_and_doc.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/docs/Makefile` & `pygedcom-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/docs/conf.py` & `pygedcom-0.1.6/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = "sphinx_rtd_theme"
+html_theme = 'sphinx_material'
```

### Comparing `pygedcom-0.1.5/docs/index.rst` & `pygedcom-0.1.6/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    contain the root `toctree` directive.
 
 Welcome to pygedcom's documentation!
 =========================================
 
 .. toctree::
    :maxdepth: 2
-   :caption: Introduction:
+   :caption: Introduction
 
    ./sources/getting_started.rst
    ./sources/parsing.rst
    ./sources/export.rst
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `pygedcom-0.1.5/docs/make.bat` & `pygedcom-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/docs/sources/export.rst` & `pygedcom-0.1.6/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/docs/sources/gedcomRootElement.rst` & `pygedcom-0.1.6/docs/sources/gedcomRootElement.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 GedcomRootElement
 =================
 
 .. autoclass:: src.pygedcom.elements.rootElements.rootElement.GedcomRootElement
     :show-inheritance:
-    :inherited-members:
     :members:
 
 
 .. autoclass:: src.pygedcom.elements.rootElements.head.GedcomHead
     :show-inheritance:
-    :inherited-members:
     :members:
 
 
 .. autoclass:: src.pygedcom.elements.rootElements.individual.GedcomIndividual
     :show-inheritance:
-    :inherited-members:
     :members:
 
 
 .. autoclass:: src.pygedcom.elements.rootElements.family.GedcomFamily
     :show-inheritance:
-    :inherited-members:
     :members:
 
 
 .. autoclass:: src.pygedcom.elements.rootElements.object.GedcomObject
     :show-inheritance:
-    :inherited-members:
     :members:
 
 
 .. autoclass:: src.pygedcom.elements.rootElements.repository.GedcomRepository
     :show-inheritance:
-    :inherited-members:
     :members:
 
 
 .. autoclass:: src.pygedcom.elements.rootElements.source.GedcomSource
     :show-inheritance:
-    :inherited-members:
     :members:
```

### Comparing `pygedcom-0.1.5/docs/sources/getting_started.rst` & `pygedcom-0.1.6/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/docs/sources/parsing.rst` & `pygedcom-0.1.6/docs/sources/parsing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,12 +6,14 @@
 .. code-block:: python
 
     # Initialize the parser
     data = parser.parse()
 
 Now the `data` object contains the parsed data. This is a dictionary with the following fields:
     - **head**: the :class:`GedcomHead` object.
+    - **submitters**: a list of :class:`GedcomSubmitter` objects.
     - **individuals**: a list of :class:`GedcomIndividual` objects.
     - **families**: a list of :class:`GedcomFamily` objects.
     - **objects**: a list of :class:`GedcomObject` objects.
+    - **notes**: a list of :class:`GedcomNote` objects.
     - **repository**: a list of :class:`GedcomRepository` objects.
     - **source**: a list of :class:`GedcomSource` objects.
```

### Comparing `pygedcom-0.1.5/src/pygedcom/gedcom_parser.py` & `pygedcom-0.1.6/src/pygedcom/gedcom_parser.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/element.py` & `pygedcom-0.1.6/src/pygedcom/elements/element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/mapping.json` & `pygedcom-0.1.6/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/family.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/family.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/head.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/individual.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/note.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/note.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/object.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/repository.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/rootElements/submitter.py` & `pygedcom-0.1.6/src/pygedcom/elements/rootElements/submitter.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.1.6/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.1.6/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.1.6/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.1.6/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/test_add_elements.py` & `pygedcom-0.1.6/test/test_add_elements.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/test_export.py` & `pygedcom-0.1.6/test/test_export.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/test_parse.py` & `pygedcom-0.1.6/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/test_remove_element.py` & `pygedcom-0.1.6/test/test_remove_element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/test_set_prop.py` & `pygedcom-0.1.6/test/test_set_prop.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/test_verify.py` & `pygedcom-0.1.6/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/test/samples/20_complex_sample.ged` & `pygedcom-0.1.6/test/samples/20_complex_sample.ged`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/.gitignore` & `pygedcom-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/LICENSE` & `pygedcom-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.5/README.md` & `pygedcom-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 ```bash
 pip install pygedcom
 ```
 
 ## Getting started
 
-First, you need to import the `gedcom_parser` module.
+First, you need to import the `pygedcom` module.
 
 ```python
 import pygedcom
 ```
 
 
-To get started with the `gedcom_parser` module, you'll need to initialize a `GedcomParser` object:
+To get started with the `parser` module, you'll need to initialize a `GedcomParser` object:
 
 
 ```python
-parser = gedcom_parser.GedcomParser(path="path/to/your/gedcom_file.ged")
+parser = pygedcom.GedcomParser(path="path/to/your/gedcom_file.ged")
 ```
 
 You can check the parsing statistics to ensure that you've parsed the file correctly:
 
 
 ```python
 print(parser.get_stats())
@@ -73,17 +73,19 @@
 ```python
     # Initialize the parser
     data = parser.parse()
 ```
 
 Now the `data` object contains the parsed data. This is a dictionary with the following fields:
 - **head**: the `GedcomHead` object.
+- **submitters**: a list of `GedcomSubmitter` objects.
 - **individuals**: a list of `GedcomIndividual` objects.
 - **families**: a list of `GedcomFamily` objects.
 - **objects**: a list of `GedcomObject` objects.
+- **notes**: a list of `GedcomNote` objects.
 - **repository**: a list of `GedcomRepository` objects.
 - **source**: a list of `GedcomSource` objects.
 
 
 ## Export
 
 The export function is used to export the GedcomParser object to a file. The export function takes two arguments:
```

### Comparing `pygedcom-0.1.5/pyproject.toml` & `pygedcom-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.1.5/PKG-INFO` & `pygedcom-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.1.5
+Version: 0.1.6
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,26 +25,26 @@
 
 ```bash
 pip install pygedcom
 ```
 
 ## Getting started
 
-First, you need to import the `gedcom_parser` module.
+First, you need to import the `pygedcom` module.
 
 ```python
 import pygedcom
 ```
 
 
-To get started with the `gedcom_parser` module, you'll need to initialize a `GedcomParser` object:
+To get started with the `parser` module, you'll need to initialize a `GedcomParser` object:
 
 
 ```python
-parser = gedcom_parser.GedcomParser(path="path/to/your/gedcom_file.ged")
+parser = pygedcom.GedcomParser(path="path/to/your/gedcom_file.ged")
 ```
 
 You can check the parsing statistics to ensure that you've parsed the file correctly:
 
 
 ```python
 print(parser.get_stats())
@@ -87,17 +87,19 @@
 ```python
     # Initialize the parser
     data = parser.parse()
 ```
 
 Now the `data` object contains the parsed data. This is a dictionary with the following fields:
 - **head**: the `GedcomHead` object.
+- **submitters**: a list of `GedcomSubmitter` objects.
 - **individuals**: a list of `GedcomIndividual` objects.
 - **families**: a list of `GedcomFamily` objects.
 - **objects**: a list of `GedcomObject` objects.
+- **notes**: a list of `GedcomNote` objects.
 - **repository**: a list of `GedcomRepository` objects.
 - **source**: a list of `GedcomSource` objects.
 
 
 ## Export
 
 The export function is used to export the GedcomParser object to a file. The export function takes two arguments:
```

