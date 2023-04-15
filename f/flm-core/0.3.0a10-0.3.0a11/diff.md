# Comparing `tmp/flm_core-0.3.0a10.tar.gz` & `tmp/flm_core-0.3.0a11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flm_core-0.3.0a10.tar", max compression
+gzip compressed data, was "flm_core-0.3.0a11.tar", max compression
```

## Comparing `flm_core-0.3.0a10.tar` & `flm_core-0.3.0a11.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0     1071 2023-04-14 20:38:06.991554 flm_core-0.3.0a10/LICENSE
--rw-r--r--   0        0        0    14576 2023-04-15 13:38:42.712587 flm_core-0.3.0a10/README.md
--rw-r--r--   0        0        0      267 2023-04-15 13:40:44.909762 flm_core-0.3.0a10/flm/__init__.py
--rw-r--r--   0        0        0     5479 2023-04-14 20:38:06.992730 flm_core-0.3.0a10/flm/__main__.py
--rw-r--r--   0        0        0    18048 2023-04-14 22:02:21.948736 flm_core-0.3.0a10/flm/counter.py
--rw-r--r--   0        0        0       83 2023-04-14 20:38:06.992933 flm_core-0.3.0a10/flm/docgen/__init__.py
--rw-r--r--   0        0        0     7332 2023-04-14 20:38:06.992994 flm_core-0.3.0a10/flm/docgen/__main__.py
--rw-r--r--   0        0        0    18252 2023-04-14 20:38:06.993103 flm_core-0.3.0a10/flm/docgen/docgen.py
--rw-r--r--   0        0        0       59 2023-04-14 20:38:06.993196 flm_core-0.3.0a10/flm/feature/__init__.py
--rw-r--r--   0        0        0     4393 2023-04-14 20:38:06.993268 flm_core-0.3.0a10/flm/feature/_base.py
--rw-r--r--   0        0        0     2110 2023-04-14 20:38:06.993331 flm_core-0.3.0a10/flm/feature/baseformatting.py
--rw-r--r--   0        0        0    30750 2023-04-14 20:38:06.993471 flm_core-0.3.0a10/flm/feature/cells.py
--rw-r--r--   0        0        0    21149 2023-04-14 20:38:06.993584 flm_core-0.3.0a10/flm/feature/cite.py
--rw-r--r--   0        0        0     9862 2023-04-14 20:38:06.993682 flm_core-0.3.0a10/flm/feature/defterm.py
--rw-r--r--   0        0        0    18161 2023-04-14 21:53:08.620142 flm_core-0.3.0a10/flm/feature/endnotes.py
--rw-r--r--   0        0        0     9002 2023-04-14 20:38:06.993897 flm_core-0.3.0a10/flm/feature/enumeration.py
--rw-r--r--   0        0        0    22033 2023-04-14 21:43:50.223123 flm_core-0.3.0a10/flm/feature/floats/__init__.py
--rw-r--r--   0        0        0     4908 2023-04-14 20:38:06.994121 flm_core-0.3.0a10/flm/feature/graphics.py
--rw-r--r--   0        0        0     6958 2023-04-14 20:38:06.994207 flm_core-0.3.0a10/flm/feature/headings.py
--rw-r--r--   0        0        0     4536 2023-04-14 20:38:06.994291 flm_core-0.3.0a10/flm/feature/href.py
--rw-r--r--   0        0        0    15940 2023-04-14 21:36:56.296441 flm_core-0.3.0a10/flm/feature/math.py
--rw-r--r--   0        0        0    18659 2023-04-14 20:38:06.994495 flm_core-0.3.0a10/flm/feature/refs.py
--rw-r--r--   0        0        0    26060 2023-04-14 22:00:51.496280 flm_core-0.3.0a10/flm/feature/theorems.py
--rw-r--r--   0        0        0     9622 2023-04-14 20:38:06.994706 flm_core-0.3.0a10/flm/feature/verbatim.py
--rw-r--r--   0        0        0     8314 2023-04-14 20:38:06.994795 flm_core-0.3.0a10/flm/flmdocument.py
--rw-r--r--   0        0        0     7600 2023-04-14 20:38:06.994876 flm_core-0.3.0a10/flm/flmdump.py
--rw-r--r--   0        0        0    37233 2023-04-14 20:38:06.995066 flm_core-0.3.0a10/flm/flmenvironment.py
--rw-r--r--   0        0        0    15840 2023-04-14 20:38:06.995174 flm_core-0.3.0a10/flm/flmfragment.py
--rw-r--r--   0        0        0     4503 2023-04-14 20:38:06.995243 flm_core-0.3.0a10/flm/flmrendercontext.py
--rw-r--r--   0        0        0    12021 2023-04-14 22:05:19.719595 flm_core-0.3.0a10/flm/flmspecinfo.py
--rw-r--r--   0        0        0       46 2023-04-14 20:38:06.995413 flm_core-0.3.0a10/flm/fragmentrenderer/__init__.py
--rw-r--r--   0        0        0    15196 2023-04-14 20:38:06.995513 flm_core-0.3.0a10/flm/fragmentrenderer/_base.py
--rw-r--r--   0        0        0    32467 2023-04-14 20:38:06.995666 flm_core-0.3.0a10/flm/fragmentrenderer/html.py
--rw-r--r--   0        0        0    26435 2023-04-14 21:52:36.579710 flm_core-0.3.0a10/flm/fragmentrenderer/latex.py
--rw-r--r--   0        0        0    12137 2023-04-14 20:38:06.995911 flm_core-0.3.0a10/flm/fragmentrenderer/markdown.py
--rw-r--r--   0        0        0    10011 2023-04-14 20:38:06.996085 flm_core-0.3.0a10/flm/fragmentrenderer/text.py
--rw-r--r--   0        0        0        0 2023-04-14 20:38:06.996155 flm_core-0.3.0a10/flm/main/__init__.py
--rw-r--r--   0        0        0     2942 2023-04-14 20:38:06.996237 flm_core-0.3.0a10/flm/main/_util.py
--rw-r--r--   0        0        0    10169 2023-04-14 20:38:06.996343 flm_core-0.3.0a10/flm/main/configmerger.py
--rw-r--r--   0        0        0     3169 2023-04-14 20:38:06.996416 flm_core-0.3.0a10/flm/main/default_config.yaml
--rw-r--r--   0        0        0     2229 2023-04-14 20:38:06.996492 flm_core-0.3.0a10/flm/main/importclass.py
--rw-r--r--   0        0        0     6915 2023-04-14 20:38:06.996574 flm_core-0.3.0a10/flm/main/main.py
--rw-r--r--   0        0        0      488 2023-04-14 20:38:06.996641 flm_core-0.3.0a10/flm/main/oshelper.py
--rw-r--r--   0        0        0    14442 2023-04-14 20:38:06.996751 flm_core-0.3.0a10/flm/main/run.py
--rw-r--r--   0        0        0     7221 2023-04-14 20:38:06.997067 flm_core-0.3.0a10/flm/main/template.py
--rw-r--r--   0        0        0      646 2023-04-14 20:38:06.997230 flm_core-0.3.0a10/flm/main/templates/html/docgen.yaml
--rw-r--r--   0        0        0       57 2023-04-14 20:38:06.997287 flm_core-0.3.0a10/flm/main/templates/html/none.yaml
--rw-r--r--   0        0        0     1182 2023-04-14 20:38:06.997351 flm_core-0.3.0a10/flm/main/templates/html/simple.html
--rw-r--r--   0        0        0      406 2023-04-14 20:38:06.997411 flm_core-0.3.0a10/flm/main/templates/html/simple.yaml
--rw-r--r--   0        0        0       57 2023-04-14 20:38:06.997497 flm_core-0.3.0a10/flm/main/templates/latex/none.yaml
--rw-r--r--   0        0        0      408 2023-04-14 20:38:06.997571 flm_core-0.3.0a10/flm/main/templates/latex/revtex.tex
--rw-r--r--   0        0        0      478 2023-04-14 20:38:06.997638 flm_core-0.3.0a10/flm/main/templates/latex/revtex.yaml
--rw-r--r--   0        0        0      540 2023-04-14 20:38:06.997705 flm_core-0.3.0a10/flm/main/templates/latex/simple.tex
--rw-r--r--   0        0        0      529 2023-04-14 20:38:06.997772 flm_core-0.3.0a10/flm/main/templates/latex/simple.yaml
--rw-r--r--   0        0        0      159 2023-04-14 20:38:06.998054 flm_core-0.3.0a10/flm/main/templates/markdown/simple.md
--rw-r--r--   0        0        0      237 2023-04-14 20:38:06.998117 flm_core-0.3.0a10/flm/main/templates/markdown/simple.yaml
--rw-r--r--   0        0        0      321 2023-04-14 20:38:06.998207 flm_core-0.3.0a10/flm/main/templates/text/simple.txt
--rw-r--r--   0        0        0      238 2023-04-14 20:38:06.998266 flm_core-0.3.0a10/flm/main/templates/text/simple.yaml
--rw-r--r--   0        0        0       35 2023-04-14 20:38:06.998354 flm_core-0.3.0a10/flm/main/workflow/__init__.py
--rw-r--r--   0        0        0     2669 2023-04-14 20:38:06.998420 flm_core-0.3.0a10/flm/main/workflow/_base.py
--rw-r--r--   0        0        0     7911 2023-04-14 20:38:06.998505 flm_core-0.3.0a10/flm/main/workflow/runlatexpdf.py
--rw-r--r--   0        0        0     4870 2023-04-14 20:38:06.998582 flm_core-0.3.0a10/flm/main/workflow/templatebasedworkflow.py
--rw-r--r--   0        0        0     4057 2023-04-14 20:38:06.998656 flm_core-0.3.0a10/flm/stdfeatures.py
--rw-r--r--   0        0        0      821 2023-04-15 13:40:40.494775 flm_core-0.3.0a10/pyproject.toml
--rw-r--r--   0        0        0    16127 1970-01-01 00:00:00.000000 flm_core-0.3.0a10/setup.py
--rw-r--r--   0        0        0    15192 1970-01-01 00:00:00.000000 flm_core-0.3.0a10/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/LICENSE
+-rw-r--r--   0        0        0    14459 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/README.md
+-rw-r--r--   0        0        0      267 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/__init__.py
+-rw-r--r--   0        0        0     5467 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/__main__.py
+-rw-r--r--   0        0        0    18048 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/counter.py
+-rw-r--r--   0        0        0       83 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/docgen/__init__.py
+-rw-r--r--   0        0        0     7332 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/docgen/__main__.py
+-rw-r--r--   0        0        0    18252 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/docgen/docgen.py
+-rw-r--r--   0        0        0       59 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/feature/__init__.py
+-rw-r--r--   0        0        0     4393 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/feature/_base.py
+-rw-r--r--   0        0        0     2110 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/feature/baseformatting.py
+-rw-r--r--   0        0        0    30762 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/feature/cells.py
+-rw-r--r--   0        0        0    21149 2023-04-15 21:00:06.905522 flm_core-0.3.0a11/flm/feature/cite.py
+-rw-r--r--   0        0        0     9862 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/defterm.py
+-rw-r--r--   0        0        0    18161 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/endnotes.py
+-rw-r--r--   0        0        0     9006 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/enumeration.py
+-rw-r--r--   0        0        0    22049 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/floats/__init__.py
+-rw-r--r--   0        0        0     4912 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/graphics.py
+-rw-r--r--   0        0        0     6958 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/headings.py
+-rw-r--r--   0        0        0     4536 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/href.py
+-rw-r--r--   0        0        0    15946 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/math.py
+-rw-r--r--   0        0        0    18663 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/refs.py
+-rw-r--r--   0        0        0    26064 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/theorems.py
+-rw-r--r--   0        0        0     9622 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/feature/verbatim.py
+-rw-r--r--   0        0        0     8314 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/flmdocument.py
+-rw-r--r--   0        0        0     7600 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/flmdump.py
+-rw-r--r--   0        0        0    37314 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/flmenvironment.py
+-rw-r--r--   0        0        0    15848 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/flmfragment.py
+-rw-r--r--   0        0        0     4503 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/flmrendercontext.py
+-rw-r--r--   0        0        0    12087 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/flmspecinfo.py
+-rw-r--r--   0        0        0       46 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/fragmentrenderer/__init__.py
+-rw-r--r--   0        0        0    15519 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/fragmentrenderer/_base.py
+-rw-r--r--   0        0        0    32467 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/fragmentrenderer/html.py
+-rw-r--r--   0        0        0    26435 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/fragmentrenderer/latex.py
+-rw-r--r--   0        0        0    12137 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/fragmentrenderer/markdown.py
+-rw-r--r--   0        0        0    10011 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/fragmentrenderer/text.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/__init__.py
+-rw-r--r--   0        0        0     2942 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/_util.py
+-rw-r--r--   0        0        0    10169 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/configmerger.py
+-rw-r--r--   0        0        0     3169 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/default_config.yaml
+-rw-r--r--   0        0        0     2229 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/importclass.py
+-rw-r--r--   0        0        0     6915 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/main.py
+-rw-r--r--   0        0        0      488 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/oshelper.py
+-rw-r--r--   0        0        0    14442 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/run.py
+-rw-r--r--   0        0        0     7221 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/template.py
+-rw-r--r--   0        0        0      646 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/html/docgen.yaml
+-rw-r--r--   0        0        0       57 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/html/none.yaml
+-rw-r--r--   0        0        0     1182 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/html/simple.html
+-rw-r--r--   0        0        0      406 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/html/simple.yaml
+-rw-r--r--   0        0        0       57 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/latex/none.yaml
+-rw-r--r--   0        0        0      408 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/latex/revtex.tex
+-rw-r--r--   0        0        0      478 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/latex/revtex.yaml
+-rw-r--r--   0        0        0      540 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/latex/simple.tex
+-rw-r--r--   0        0        0      529 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/latex/simple.yaml
+-rw-r--r--   0        0        0      159 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/markdown/simple.md
+-rw-r--r--   0        0        0      237 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/markdown/simple.yaml
+-rw-r--r--   0        0        0      321 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/text/simple.txt
+-rw-r--r--   0        0        0      238 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/templates/text/simple.yaml
+-rw-r--r--   0        0        0       35 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/workflow/__init__.py
+-rw-r--r--   0        0        0     2669 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/workflow/_base.py
+-rw-r--r--   0        0        0     7911 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/workflow/runlatexpdf.py
+-rw-r--r--   0        0        0     4870 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/main/workflow/templatebasedworkflow.py
+-rw-r--r--   0        0        0     4057 2023-04-15 21:00:06.909522 flm_core-0.3.0a11/flm/stdfeatures.py
+-rw-r--r--   0        0        0      860 2023-04-15 21:00:06.913523 flm_core-0.3.0a11/pyproject.toml
+-rw-r--r--   0        0        0    15080 1970-01-01 00:00:00.000000 flm_core-0.3.0a11/PKG-INFO
```

### Comparing `flm_core-0.3.0a10/LICENSE` & `flm_core-0.3.0a11/LICENSE`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/README.md` & `flm_core-0.3.0a11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -88,30 +88,29 @@
 
 - **Additional HTML Templates:**
   The `--template=` option can be used to change the template used to render the
   document.  See also the
   [*flm-templates*](https://github.com/phfaist/flm-templates) extension package
   for some additional templates and template engines.  You can try:
   ```
-  > pip install git+https://github.com/phfaist/flm-templates.git
-  > pip install git+https://github.com/phfaist/flm-htmlplus.git
+  > pip install flm-templates flm-htmlplus
   ```
   and then
   ```
   > flm mydocument.flm -o output.html -w flm_htmlplus -P 'pkg:flm_templates' -t sunset
   ```
   Or try the template `-t oldtextbook`.
 
 - **Citations from arXiv & DOI:**
   Automatically fetch citations from the arXiv, DOI x-references, or other
   sources using the [*flm-citations*](https://github.com/phfaist/flm-citations)
   extension package (see README file there).  Install the extension package
   using pip:
   ```
-  > pip install git+https://github.com/phfaist/flm-citations
+  > pip install flm-citations
   ```
   And then try to compile, e.g., the following FLM document:
   ```yaml
   ---
   $import:
     - pkg:flm_citations
   ---
```

### Comparing `flm_core-0.3.0a10/flm/__main__.py` & `flm_core-0.3.0a11/flm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import logging
 
-from pylatexenc.latexnodes import LatexWalkerParseError
+from pylatexenc.latexnodes import LatexWalkerError
 
 from .main.main import main as _main
 from .main import oshelper as flm_main_oshelper
 from flm import __version__ as flm_version
 
 
 
@@ -123,14 +123,14 @@
     return
 
 
 
 if __name__ == '__main__':
     try:
         run_main()
-    except LatexWalkerParseError as e:
+    except LatexWalkerError as e:
         logging.getLogger('flm').critical(
-            f"Parse Error\n{e}"
+            f"FLM Error\n{e}"
         )
     except Exception as e:
         logging.getLogger('flm').critical('Error.', exc_info=e)
         import pdb; pdb.post_mortem()
```

### Comparing `flm_core-0.3.0a10/flm/counter.py` & `flm_core-0.3.0a11/flm/counter.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/docgen/__main__.py` & `flm_core-0.3.0a11/flm/docgen/__main__.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/docgen/docgen.py` & `flm_core-0.3.0a11/flm/docgen/docgen.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/_base.py` & `flm_core-0.3.0a11/flm/feature/_base.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/baseformatting.py` & `flm_core-0.3.0a11/flm/feature/baseformatting.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/cells.py` & `flm_core-0.3.0a11/flm/feature/cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 from pylatexenc import macrospec
 from pylatexenc.latexnodes import (
     LatexArgumentSpec,
-    LatexWalkerParseError,
+    LatexWalkerLocatedError,
     ParsedArgumentsInfo,
     ParsingStateDelta,
 )
 from pylatexenc.latexnodes import nodes as latexnodes_nodes
 from pylatexenc.latexnodes import parsers as latexnodes_parsers
 
 from ..flmenvironment import (
@@ -589,15 +589,15 @@
         if len(nl) != 1:
             if is_row:
                 PLACEHOLDER = 'ROW'
             elif is_col:
                 PLACEHOLDER = 'COL'
             else:
                 PLACEHOLDER = None
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"Bad cell index or merge range specification, expected ‘{PLACEHOLDER}’ or "
                 f"‘\\merge{'{'}{PLACEHOLDER}-RANGE{'}'}’, got {repr(placement_index_spec)} "
                 f"({len(nl)} nodes)",
                 pos=nl.pos
             )
 
         node = nl[0]
@@ -656,15 +656,15 @@
             elif len(placement_spec_split) == 0:
 
                 # all ok, keep defaults
                 pass
 
             else:
 
-                raise LatexWalkerParseError(
+                raise LatexWalkerLocatedError(
                     f"Bad cell placement specification, expected ‘ROW;COL’ or "
                     f"‘COL’, got ‘{_splfysidews(placement_spec.latex_verbatim())}’",
                     pos=placement_spec.pos
                 )
 
         row_range = self.parse_placement_index_spec(row_spec_nl, is_row=True)
         col_range = self.parse_placement_index_spec(col_spec_nl, is_col=True)
@@ -699,15 +699,15 @@
             if len(nl) != 1:
                 if is_row:
                     PLACEHOLDER = 'ROW-RANGE'
                 elif is_col:
                     PLACEHOLDER = 'COL-RANGE'
                 else:
                     PLACEHOLDER = None
-                raise LatexWalkerParseError(
+                raise LatexWalkerLocatedError(
                     f"Bad cell index or range or merge range specification, "
                     f"expected ‘{PLACEHOLDER}’ or "
                     f"‘\\merge{'{'}{PLACEHOLDER}-RANGE{'}'}’, got {repr(placement_index_spec)} "
                     f"({len(nl)} nodes)",
                     pos=nl.pos
                 )
 
@@ -768,15 +768,15 @@
 
         elif len(placement_mapping_spec_split) == 0:
 
             row_mapping_spec, col_mapping_spec = [], []
 
         else:
 
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"Expected ‘ROWS;COLS’ or ‘COLS’ or ‘’ for placement argument, "
                 f"got ‘{_splfysidews(placement_mapping_spec.latex_verbatim())}’",
                 pos=placement_mapping_spec.pos
             )
 
         row_placements = self.parse_placement_mapping_index_spec(
             row_mapping_spec, index_end=None, is_row=True
@@ -850,15 +850,15 @@
                 continue
 
             if n.isNodeType(latexnodes_nodes.LatexCharsNode) \
                and len(n.chars.strip()) == 0:
                 # okay, ignore pure whitespace
                 continue
 
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"You cannot place ‘{_splfysidews(n.latex_verbatim())}’ here.  Expected: "
                 f"\\cell, \\celldata, \\\\."
             )
 
         cells_model.finalize()
 
         node.flm_cells_model = cells_model
```

### Comparing `flm_core-0.3.0a10/flm/feature/cite.py` & `flm_core-0.3.0a11/flm/feature/cite.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/defterm.py` & `flm_core-0.3.0a11/flm/feature/defterm.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/endnotes.py` & `flm_core-0.3.0a11/flm/feature/endnotes.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/enumeration.py` & `flm_core-0.3.0a11/flm/feature/enumeration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 
-from pylatexenc.latexnodes import ParsedArgumentsInfo, LatexWalkerParseError
+from pylatexenc.latexnodes import ParsedArgumentsInfo, LatexWalkerLocatedError
 import pylatexenc.latexnodes.parsers as latexnodes_parsers
 import pylatexenc.latexnodes.nodes as latexnodes_nodes
 from pylatexenc.macrospec import (
     MacroSpec,
     LatexEnvironmentBodyContentsParser,
     ParsingStateDeltaExtendLatexContextDb,
 )
@@ -119,15 +119,15 @@
                     or (item_macro.isNodeType(latexnodes_nodes.LatexSpecialsNode)
                         and isinstance(item_macro.spec, FLMSpecInfoParagraphBreak))
                 )):
                 # skip leading whitespace
                 continue
             if (not item_macro.isNodeType(latexnodes_nodes.LatexMacroNode)
                 or item_macro.macroname != 'item'):
-                raise LatexWalkerParseError(
+                raise LatexWalkerLocatedError(
                     msg=f"Expected ‘\\item’ in enumeration environment: {item_macro!r}",
                     pos=item_macro.pos,
                 )
             item_content_nodelist = item_macro.latex_walker.make_nodelist(
                 item_nodelist.nodelist[1:],
                 parsing_state=item_macro.parsing_state,
             )
```

### Comparing `flm_core-0.3.0a10/flm/feature/floats/__init__.py` & `flm_core-0.3.0a11/flm/feature/floats/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 logger = logging.getLogger(__name__)
 
-from pylatexenc.latexnodes import ParsedArgumentsInfo, LatexWalkerParseError
+from pylatexenc.latexnodes import ParsedArgumentsInfo, LatexWalkerLocatedError
 from pylatexenc.latexnodes import nodes as latexnodes_nodes
 from pylatexenc.latexnodes import parsers as latexnodes_parsers
 from pylatexenc.macrospec import (
     LatexEnvironmentBodyContentsParser,
     MacroSpec,
     ParsingStateDeltaExtendLatexContextDb,
 )
@@ -30,15 +30,15 @@
     def float_handle_content_nodes(self, float_node, content_nodes):
         # subclasses can choose to verify the float's content nodes to ensure
         # that it only contains prescribed content nodes (e.g., only a single
         # \includegraphics node)
         #
         # Return a (possibly post-processed) node list to use in place of
         # content_nodes if the nodes were accepted; raise a
-        # LatexWalkerParseError if the nodes were not accepted (unacceptable
+        # LatexWalkerLocatedError if the nodes were not accepted (unacceptable
         # macros, etc.)
         raise RuntimeError(
             f"This method needs to be reimplemented in subclasses!"
         )
 
 
 class FloatContentAnyContent(FloatContentHandlerBase):
@@ -64,15 +64,15 @@
         if len(content_nodes) == 1:
             node = content_nodes[0]
             if node.isNodeType(latexnodes_nodes.LatexMacroNode) \
                and node.macroname == 'includegraphics':
                 # all good!
                 return content_nodes
 
-        raise LatexWalkerParseError(
+        raise LatexWalkerLocatedError(
             f"expected exactly one \\includegraphics command",
             pos=content_nodes.pos
         )
 
 
 class FloatContentCells(FloatContentHandlerBase):
 
@@ -90,15 +90,15 @@
         if len(content_nodes) == 1:
             node = content_nodes[0]
             if node.isNodeType(latexnodes_nodes.LatexEnvironmentNode) \
                and node.environmentname == 'cells':
                 # all good!
                 return content_nodes
 
-        raise LatexWalkerParseError(
+        raise LatexWalkerLocatedError(
             f"expected exactly one "
             f"\\begin{'{'}cells{'}'}...\\end{'{'}cells{'}'} environment",
             pos=content_nodes.pos
         )
 
 
 available_content_handlers = {
@@ -212,25 +212,25 @@
                     ref_label_full = ref_label_node_args['label'].get_content_as_chars()
                     if ':' in ref_label_full:
                         ref_label_prefix, ref_label = ref_label_full.split(':', 1)
                     else:
                         ref_label_prefix, ref_label = None, ref_label_full
 
                     if ref_label_prefix != self.float_type:
-                        raise LatexWalkerParseError(
+                        raise LatexWalkerLocatedError(
                             f"{self.float_type} label must start with the prefix "
                             f"‘{self.float_type}:...’ (got ‘{ref_label_full}’)",
                             pos=n.pos,
                         )
 
                     node.flm_float_label['ref_label_prefix'] = ref_label_prefix
                     node.flm_float_label['ref_label'] = ref_label
 
                     if ref_label_prefix != self.float_type:
-                        raise LatexWalkerParseError(
+                        raise LatexWalkerLocatedError(
                             f"Float's \\label{'{'}...{'}'} must have the "
                             f"prefix ‘{self.float_type}:’",
                             pos=n.pos,
                         )
 
                     continue
 
@@ -258,21 +258,21 @@
         errors = []
         final_content_nodes = None
         for content_handler in self.content_handlers:
             try:
                 final_content_nodes = content_handler.float_handle_content_nodes(
                     node, float_content_nodes
                 )
-            except LatexWalkerParseError as e:
+            except LatexWalkerLocatedError as e:
                 errors.append(f"*** {content_handler.__class__.__name__} error: {str(e)}")
                 #pass # ignore error
 
         if final_content_nodes is None:
             # no content handler accepted this float's content node list
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"Invalid {self.float_type} contents! The following content handler(s) "
                 f"were unable to parse the float's content [other than possible "
                 f"\\caption and \\label commands]:\n"
                 + "\n".join(errors),
                 pos=node.pos
             )
```

### Comparing `flm_core-0.3.0a10/flm/feature/graphics.py` & `flm_core-0.3.0a11/flm/feature/graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 logger = logging.getLogger(__name__)
 
-from pylatexenc.latexnodes import LatexWalkerParseError, ParsedArgumentsInfo
+from pylatexenc.latexnodes import LatexWalkerLocatedError, ParsedArgumentsInfo
 from pylatexenc.latexnodes import parsers as latexnodes_parsers
 
 from ..flmspecinfo import FLMMacroSpecBase
 from ..flmenvironment import FLMArgumentSpec
 from ._base import Feature
 
 
@@ -99,15 +99,15 @@
 
         fragment_renderer = render_context.fragment_renderer
 
         graphics_options_value = node.flmarg_graphics_options_value
         graphics_path = node.flmarg_graphics_path
         
         if graphics_options_value:
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"Graphics options are not supported here: ‘{graphics_options_value}’",
                 pos=node_args['graphics_options'].nodelist.pos,
             )
 
         if not render_context.supports_feature('graphics_resource_provider'):
             raise RuntimeError(
                 "FLM's ‘SimpleIncludeGraphicsSpecInfo’ (‘\\includegraphics’) requires a "
```

### Comparing `flm_core-0.3.0a10/flm/feature/headings.py` & `flm_core-0.3.0a11/flm/feature/headings.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/href.py` & `flm_core-0.3.0a11/flm/feature/href.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/feature/math.py` & `flm_core-0.3.0a11/flm/feature/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 from pylatexenc.latexnodes import (
-    LatexWalkerParseError,
+    LatexWalkerLocatedError,
     ParsedArgumentsInfo,
     ParsingStateDeltaEnterMathMode,
 )
 from pylatexenc.latexnodes import nodes as latexnodes_nodes
 from pylatexenc.latexnodes import parsers as latexnodes_parsers
 from pylatexenc.macrospec import (
     MacroSpec,
@@ -421,15 +421,15 @@
         
         ref_type = None
         ref_label = node_args['ref_label'].get_content_as_chars()
         if ':' in ref_label:
             ref_type, ref_label = ref_label.split(':', 1)
 
         if ref_type != self.ref_type:
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"Equation labels must begin with “{self.ref_type}:” "
                 f"(error in ‘\\{node.macroname}’)",
                 pos=node.pos
             )
 
         node.flmarg_ref = (ref_type, ref_label)
 
@@ -452,15 +452,15 @@
                 resource_info,
                 render_context,
                 counter_with_prefix=False, # no "Eq.~" prefix
             )
         except Exception as e:
             logger.error(f"Failed to resolve reference to ‘{ref_type}:{ref_label}’: {e} "
                          f"in ‘{node.latex_verbatim()}’ @ {node.format_pos()}")
-            raise LatexWalkerParseError(
+            raise LatexWalkerLocatedError(
                 f"Unable to resolve reference to ‘{ref_type}:{ref_label}’. {e}",
                 pos=node.pos,
             )
 
 
 
 # ------------------------------------------------
```

### Comparing `flm_core-0.3.0a10/flm/feature/refs.py` & `flm_core-0.3.0a11/flm/feature/refs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import logging
 logger = logging.getLogger(__name__)
 
 from pylatexenc.latexnodes import parsers as latexnodes_parsers
 from pylatexenc.latexnodes import (
-    LatexWalkerParseError,
+    LatexWalkerLocatedError,
     ParsedArgumentsInfo
 )
 #from pylatexenc import macrospec
 
 from ..flmfragment import FLMFragment
 from ..flmspecinfo import FLMMacroSpecBase
 from ..flmenvironment import FLMArgumentSpec
@@ -500,15 +500,15 @@
                                       display_content_nodelist,
                                       resource_info,
                                       render_context,
                                       counter_prefix_variant=self.counter_prefix_variant)
             except Exception as e:
                 logger.error(f"Failed to resolve reference to ‘{ref_type}:{ref_label}’: {e} "
                              f"in ‘{node.latex_verbatim()}’ @ {node.format_pos()}")
-                raise LatexWalkerParseError(
+                raise LatexWalkerLocatedError(
                     f"Unable to resolve reference to ‘{ref_type}:{ref_label}’: {e}",
                     pos=node.pos,
                 )
 
         # we have multiple ref targets
 
         # can only have one ref target if we have a display string
```

### Comparing `flm_core-0.3.0a10/flm/feature/theorems.py` & `flm_core-0.3.0a11/flm/feature/theorems.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             # parse the theorem title as [*label] or [**label] (as for phfthm.sty)
             if (thmtitle_nodelist is not None and len(thmtitle_nodelist) > 0):
                 chnode = thmtitle_nodelist[0]
                 if (chnode is not None
                     and chnode.isNodeType(latexnodes_nodes.LatexCharsNode)
                     and chnode.chars.startswith('*')):
                     if len(thmtitle_nodelist) != 1:
-                        raise LatexWalkerParseError(
+                        raise LatexWalkerLocatedError(
                             "When specifying a proof-ref target as optional argument "
                             "(‘[*thm:xyz]’), the entire argument must consist of "
                             "regular characters with no special meaning in FLM.  Got: "
                             f"‘{thmtitle_nodelist.latex_verbatim()}’",
                             pos=chnode.pos
                         )
                     if chnode.chars.startswith('**'):
@@ -175,15 +175,15 @@
                 ],
                 parsing_state=node.parsing_state,
             )
 
             # We're not generating target_id's for these elements, so don't pin
             # down labels here...
             if len(flmarg_labels):
-                raise LatexWalkerParseError(
+                raise LatexWalkerLocatedError(
                     r"You cannot use \label{} in unnumbered theorem environment ‘"
                     + self.environmentname + r"’",
                     pos=node.pos
                 )
 
             # for ref_type, ref_label in flmarg_labels:
             #     # register references in refs
```

### Comparing `flm_core-0.3.0a10/flm/feature/verbatim.py` & `flm_core-0.3.0a11/flm/feature/verbatim.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/flmdocument.py` & `flm_core-0.3.0a11/flm/flmdocument.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/flmdump.py` & `flm_core-0.3.0a11/flm/flmdump.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/flmenvironment.py` & `flm_core-0.3.0a11/flm/flmenvironment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import re
 import logging
 logger = logging.getLogger(__name__)
 
 from pylatexenc import latexnodes
 from pylatexenc import macrospec
-from pylatexenc.latexnodes import LatexWalkerParseError, LatexWalkerParseErrorFormatter
+from pylatexenc.latexnodes import (
+    LatexWalkerError, #LatexWalkerLocatedError,
+    LatexWalkerLocatedErrorFormatter,
+    LatexWalkerParseError,
+)
 from pylatexenc.latexnodes import nodes as latexnodes_nodes
 from pylatexenc import latexwalker
 
 from .flmfragment import FLMFragment
 from .flmdocument import FLMDocument
 
 
@@ -763,20 +767,20 @@
         features_ensure_dependencies_are_met(features)
 
         return features
 
 
 
 
-    environment_get_parse_error_message = None
+    environment_get_located_error_message = None
 
-    def get_parse_error_message(self, exception_object):
-        if self.environment_get_parse_error_message is not None:
-            return self.environment_get_parse_error_message(exception_object)
-        return LatexWalkerParseErrorFormatter(exception_object).to_display_string()
+    def get_located_error_message(self, exception_object):
+        if self.environment_get_located_error_message is not None:
+            return self.environment_get_located_error_message(exception_object)
+        return LatexWalkerLocatedErrorFormatter(exception_object).to_display_string()
 
 
 
 
 # ------------------------------------------------------------------------------
 
 
@@ -857,15 +861,15 @@
             )
         )
 
 
 # ------------------------------------------------------------------------------
 
 
-def standard_environment_get_parse_error_message(exception_object):
+def standard_environment_get_located_error_message(exception_object):
     msg = None
     error_type_info = exception_object.error_type_info
     if error_type_info:
         what = error_type_info['what']
         if what == 'token_forbidden_character':
             if error_type_info['forbidden_character'] == '%':
                 msg = (
@@ -877,15 +881,15 @@
                     r"You can't use ‘$’ here. LaTeX math should be typeset using "
                     r"\(...\) for inline math and \[...\] for unnumbered display "
                     r"equations. Use ‘\$’ for a literal dollar sign."
                 )
     if not msg:
         msg = exception_object.msg
 
-    errfmt = latexnodes.LatexWalkerParseErrorFormatter(exception_object)
+    errfmt = latexnodes.LatexWalkerLocatedErrorFormatter(exception_object)
 
     msg += errfmt.format_full_traceback()
 
     return msg
 
 
 
@@ -917,16 +921,16 @@
         parsing_state,
         latex_context,
         **flm_environment_options_2
     )
 
     environment.parsing_state_event_handler = parsing_state_event_handler
 
-    environment.environment_get_parse_error_message = \
-        standard_environment_get_parse_error_message
+    environment.environment_get_located_error_message = \
+        standard_environment_get_located_error_message
 
     return environment
```

### Comparing `flm_core-0.3.0a10/flm/flmfragment.py` & `flm_core-0.3.0a11/flm/flmfragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     A FLM fragment is intended to later be inserted in a document so that it can
     be rendered into the desired output format (HTML, plain text).  If the
     fragment is *standalone* (`standalone_mode=True`), then some FLM features
     are disabled (typically, for instance, cross-references) and the fragment
     can be rendered directly on its own without inserting it in a document, see
     :py:meth:`render_standalone()`.
 
-    .....................
+    Doc .....................
 
     The argument `resource_info` can be set to any custom object that can help
     locate resources called by FLM text.  For instance, a `\includegraphics{}`
     call might wish to look for graphics in the same filesystem folder as a file
     that contained the FLM code; the `resource_info` object can be used to store
     the filesystem folder of the FLM code forming this fragment.
     """
@@ -88,17 +88,17 @@
                     tolerant_parsing=self.tolerant_parsing,
                     is_block_level=self.is_block_level,
                     what=self.what,
                     resource_info=self.resource_info,
                     parsing_mode=self.parsing_mode,
                     input_lineno_colno_offsets=input_lineno_colno_offsets,
                 )
-        except latexnodes.LatexWalkerParseError as e:
+        except latexnodes.LatexWalkerLocatedError as e:
             if not self.silent:
-                error_message = self.environment.get_parse_error_message(e)
+                error_message = self.environment.get_located_error_message(e)
                 logger.error(
                     f"Parse error in latex-like markup ‘{self.what}’: {error_message}\n"
                     f"Given text was:\n‘{self.flm_text}’\n\n"
                 )
             raise
         except Exception as e:
             if not self.silent:
```

### Comparing `flm_core-0.3.0a10/flm/flmrendercontext.py` & `flm_core-0.3.0a11/flm/flmrendercontext.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/flmspecinfo.py` & `flm_core-0.3.0a11/flm/flmspecinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 from pylatexenc import macrospec
 from pylatexenc.latexnodes import parsers as latexnodes_parsers
-from pylatexenc.latexnodes import ParsedArgumentsInfo, LatexWalkerParseError
+from pylatexenc.latexnodes import (
+    LatexWalkerParseError, LatexWalkerLocatedError, ParsedArgumentsInfo
+)
 
 from .flmenvironment import (
     FLMArgumentSpec
 )
 
 
 # ------------------------------------------------------------------------------
@@ -109,22 +111,23 @@
         r"""
         Override this method only if you know what you're doing!
         """
 
         fragment_is_standalone_mode = node.latex_walker.standalone_mode
         if fragment_is_standalone_mode and not self.allowed_in_standalone_mode:
             raise LatexWalkerParseError(
-                f"‘{node.latex_verbatim()}’ is not allowed here (standalone mode)."
+                f"‘{node.latex_verbatim()}’ is not allowed here (standalone mode).",
+                pos=node.pos,
             )
 
         node.flm_specinfo = self
         try:
             self.postprocess_parsed_node(node)
 
-        except LatexWalkerParseError as e:
+        except LatexWalkerLocatedError as e:
             if not hasattr(e, 'pos') or e.pos is None:
                 e.pos = node.pos
             raise e
 
         except ValueError as e:
             raise LatexWalkerParseError(str(e), pos=node.pos)
```

### Comparing `flm_core-0.3.0a10/flm/fragmentrenderer/_base.py` & `flm_core-0.3.0a11/flm/fragmentrenderer/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,30 +92,39 @@
 
         return self.render_inline_content(nodelist, render_context)
 
 
     def render_node(self, node, render_context):
         render_context = self.ensure_render_context(render_context)
 
-        if node.isNodeType(nodes.LatexCharsNode):
-            return self.render_node_chars(node, render_context)
-        if node.isNodeType(nodes.LatexCommentNode):
-            return self.render_node_comment(node, render_context)
-        if node.isNodeType(nodes.LatexGroupNode):
-            return self.render_node_group(node, render_context)
-        if node.isNodeType(nodes.LatexMacroNode):
-            return self.render_node_macro(node, render_context)
-        if node.isNodeType(nodes.LatexEnvironmentNode):
-            return self.render_node_environment(node, render_context)
-        if node.isNodeType(nodes.LatexSpecialsNode):
-            return self.render_node_specials(node, render_context)
-        if node.isNodeType(nodes.LatexMathNode):
-            return self.render_node_math(node, render_context)
+        try:
+            if node.isNodeType(nodes.LatexCharsNode):
+                return self.render_node_chars(node, render_context)
+            if node.isNodeType(nodes.LatexCommentNode):
+                return self.render_node_comment(node, render_context)
+            if node.isNodeType(nodes.LatexGroupNode):
+                return self.render_node_group(node, render_context)
+            if node.isNodeType(nodes.LatexMacroNode):
+                return self.render_node_macro(node, render_context)
+            if node.isNodeType(nodes.LatexEnvironmentNode):
+                return self.render_node_environment(node, render_context)
+            if node.isNodeType(nodes.LatexSpecialsNode):
+                return self.render_node_specials(node, render_context)
+            if node.isNodeType(nodes.LatexMathNode):
+                return self.render_node_math(node, render_context)
+
+            raise ValueError(f"Invalid node type: {node!r}")
+
+        except LatexWalkerLocatedError as e:
+            if not hasattr(e, 'pos') or e.pos is None:
+                e.pos = node.pos
+            raise e
 
-        raise ValueError(f"Invalid node type: {node!r}")
+        except Exception as e:
+            raise LatexWalkerLocatedError(str(e), pos=node.pos)
         
 
     def render_node_chars(self, node, render_context):
         if hasattr(node, 'flm_chars_value'): # transcrypt doesn't like getattr with default arg
             chars_value = node.flm_chars_value
         else:
             chars_value = None
```

### Comparing `flm_core-0.3.0a10/flm/fragmentrenderer/html.py` & `flm_core-0.3.0a11/flm/fragmentrenderer/html.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/fragmentrenderer/latex.py` & `flm_core-0.3.0a11/flm/fragmentrenderer/latex.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/fragmentrenderer/markdown.py` & `flm_core-0.3.0a11/flm/fragmentrenderer/markdown.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/fragmentrenderer/text.py` & `flm_core-0.3.0a11/flm/fragmentrenderer/text.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/_util.py` & `flm_core-0.3.0a11/flm/main/_util.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/configmerger.py` & `flm_core-0.3.0a11/flm/main/configmerger.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/default_config.yaml` & `flm_core-0.3.0a11/flm/main/default_config.yaml`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/importclass.py` & `flm_core-0.3.0a11/flm/main/importclass.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/main.py` & `flm_core-0.3.0a11/flm/main/main.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/run.py` & `flm_core-0.3.0a11/flm/main/run.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/template.py` & `flm_core-0.3.0a11/flm/main/template.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/templates/html/docgen.yaml` & `flm_core-0.3.0a11/flm/main/templates/html/docgen.yaml`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/templates/html/simple.html` & `flm_core-0.3.0a11/flm/main/templates/html/simple.html`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/templates/latex/simple.tex` & `flm_core-0.3.0a11/flm/main/templates/latex/simple.tex`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/templates/latex/simple.yaml` & `flm_core-0.3.0a11/flm/main/templates/latex/simple.yaml`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/workflow/_base.py` & `flm_core-0.3.0a11/flm/main/workflow/_base.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/workflow/runlatexpdf.py` & `flm_core-0.3.0a11/flm/main/workflow/runlatexpdf.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/main/workflow/templatebasedworkflow.py` & `flm_core-0.3.0a11/flm/main/workflow/templatebasedworkflow.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/flm/stdfeatures.py` & `flm_core-0.3.0a11/flm/stdfeatures.py`

 * *Files identical despite different names*

### Comparing `flm_core-0.3.0a10/pyproject.toml` & `flm_core-0.3.0a11/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "flm-core"
-version = "0.3.0alpha000010" # ALSO BUMP IN flm/flm/__init__.py
+version = "0.3.0alpha000011" # ALSO BUMP IN flm/flm/__init__.py
 description = "Flexible Latex-like Markup"
 authors = ["Philippe Faist"]
 license = "MIT"
 readme = "README.md"
 include = ["flm/main/templates/**/*"]
 packages = [
     { include = "flm" },
 ]
 
 [tool.poetry.scripts]
 flm = 'flm.__main__:run_main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pylatexenc = ">=3.0a13"
+pylatexenc = { version = "^3.0a14", allow-prereleases = true }
 python-frontmatter = "^1.0.0"
 PyYAML = ">=5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 ipython = "^8.3.0"
 toml = "^0.10.2"
```

### Comparing `flm_core-0.3.0a10/setup.py` & `flm_core-0.3.0a11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,439 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flm-core
+Version: 0.3.0a11
+Summary: Flexible Latex-like Markup
+License: MIT
+Author: Philippe Faist
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=5.0)
+Requires-Dist: pylatexenc (>=3.0a14,<4.0)
+Requires-Dist: python-frontmatter (>=1.0.0,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['flm',
- 'flm.docgen',
- 'flm.feature',
- 'flm.feature.floats',
- 'flm.fragmentrenderer',
- 'flm.main',
- 'flm.main.workflow']
-
-package_data = \
-{'': ['*'],
- 'flm.main': ['templates/html/*',
-              'templates/latex/*',
-              'templates/markdown/*',
-              'templates/text/*']}
-
-install_requires = \
-['PyYAML>=5.0', 'pylatexenc>=3.0a13', 'python-frontmatter>=1.0.0,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['flm = flm.__main__:run_main']}
-
-setup_kwargs = {
-    'name': 'flm-core',
-    'version': '0.3.0a10',
-    'description': 'Flexible Latex-like Markup',
-    'long_description': '# A Flexible Latex-Like Markup (FLM) language\n\nThis package provides a simple parser and formatter for a custom markup language\nthat is inspired by LaTeX syntax.\n\nThe syntax of FLM is essentially a subset of standard LaTeX commands, including\nmacros, environments, and some characters that have a special meaning; these\nfeatures are parsed in a loosely similar fashion to usual LaTeX code.\n\nThe framework is meant to be very easily extendible and customizable.  The\nparser is based on [*pylatexenc 3*](https://github.com/phfaist/pylatexenc)\n(which is currently still in development).\n\nFLM is used to write the contents of the [Error Correction\nZoo](https://errorcorrectionzoo.org/) in a way that is intuitive for scientists,\nflexible, and robust.  It is easily extensible and closely resembles the LaTeX\nlangauge that many scientists are familiar with.  FLM pushes further one of the\ncore insights of LaTeX, namely, that the code should *describe* document\ncontents in an intuitive way, as a markup language, while disregarding as much\nas possible the details of how that contents will be typeset.  The final\ntypesetting is fully customizable, e.g., through CSS styling of its HTML output\n(including the use of templates).\n\nYou can install FLM with pip:\n```bash\n$ pip install flm-core\n```\n\nExample `mydocument.flm`:\n```latex\n---\ntitle: Kitaev\'s Surface Code\n---\n\\section{Kitaev\'s Surface Code}\n\nThe \\emph{stabilizers} of the \\textit{surface code} on the 2-dimensional\ntorus are generated by star operators \\(A_v\\) and plaquette operators\n\\(B_p\\).  Each star operator is a \\textbf{product} of four Pauli-\\(X\\)\noperators on the edges adjacent to a vertex \\(v\\) of the lattice; each\nplaquette operator is a product of four Pauli-\\(Z\\) operators applied to\nthe edges adjacent to a face, or plaquette, \\(p\\) of the lattice\n(\\ref{figure:toric-code-operators}).\n\n\\begin{figure}\n  \\includegraphics{toric-code-operators}\n  \\caption{Stabilizer generators and logical operators of the 2D surface\n    code on a torus.  The star operators \\(A_v\\) and the plaquette\n    operators \\(B_p\\) generate the stabilizer group of the toric code.\n    The logical operators are strings that wrap around the torus.}\n  \\label{figure:toric-code-operators}\n\\end{figure}\n\n...\n```\n\nTo compile your document into an HTML page, use:\n```bash\n$ flm mydocument.flm -o mydocument.html --format=html --template=simple\n```\n\nYou can then open the `mydocument.html` file in your browser.\n\n# This is work in progress!\n\nThis project is still early in an active development stage, and there might\nstill be a few bugs around. You can expect the API to still change pretty\ndrastically.  Feel free to share ideas!\n\n# Use as a command-line tool\n\nYou can use `flm` in command-line mode to compile your documents:\n```bash\n$ flm mydocument.flm\n```\n\nRun `flm --help` to get a list of options. They should be fairly\nstandard and/or self-explanatory:\n```bash\n# output to file mydocument.html, format HTML, including skeleton\n# HTML structure with minimal CSS.\n$ flm mydocument.flm -o mydocument.html --format=html --template=simple\n```\n\nAvailable formats are `html`, `text`, `latex`, and `markdown`.  Formats\n`text`, `markdown`, and `latex` are very experimental!  (You can also\ngenerate `pdf` output with the options `--workflow=runlatexpdf --format=pdf`\nif your system has a standard LaTeX distribution such as TeXLive installed)\n\n- **Additional HTML Templates:**\n  The `--template=` option can be used to change the template used to render the\n  document.  See also the\n  [*flm-templates*](https://github.com/phfaist/flm-templates) extension package\n  for some additional templates and template engines.  You can try:\n  ```\n  > pip install git+https://github.com/phfaist/flm-templates.git\n  > pip install git+https://github.com/phfaist/flm-htmlplus.git\n  ```\n  and then\n  ```\n  > flm mydocument.flm -o output.html -w flm_htmlplus -P \'pkg:flm_templates\' -t sunset\n  ```\n  Or try the template `-t oldtextbook`.\n\n- **Citations from arXiv & DOI:**\n  Automatically fetch citations from the arXiv, DOI x-references, or other\n  sources using the [*flm-citations*](https://github.com/phfaist/flm-citations)\n  extension package (see README file there).  Install the extension package\n  using pip:\n  ```\n  > pip install git+https://github.com/phfaist/flm-citations\n  ```\n  And then try to compile, e.g., the following FLM document:\n  ```yaml\n  ---\n  $import:\n    - pkg:flm_citations\n  ---\n  \\section{Introduction}\n  Let\'s cite Kitaev\'s surface code~\\cite{doi:10.1070/RM1997v052n06ABEH002155,doi:10.1007/978-1-4615-5923-8_19,arXiv:quant-ph/9707021}. ...\n  ```\n\n- **Theorems and proofs:** Use the environments\n  ``\\begin{theorem}..\\end{theorem}``, ``{lemma}``, ``{proposition}``,\n  ``{definition}``, ``{remark}``, etc. for typesetting theorems.  You can pin\n  labels to theorem statements ``\\label{thm:XYZ}`` (use the `thm:` or `x:`\n  prefixes regardless of the theorem type, so you can easily change it without\n  having to update the label).  These environments accept an optional argument\n  so you can specify a title, e.g. ``\\begin{theorem}[Euler\'s theorem]\n  ... \\end{theorem}``.  Typeset proofs with ``\\begin{proof} ... \\end{proof}``.\n  The proof\'s optional argument enjoys an additional syntax: use\n  ``\\begin{proof}[*thm:XYZ] ...`` to typeset `Proof (Theorem 3)` (with the\n  correct theorem reference using its label, which must match the one specified\n  to the theorem\'s ``\\label`` command).  Use ``\\begin{proof}[**thm:XYZ] ...`` to\n  simply typeset `Proof` as usual, but in this way you have the information about\n  which theorem the proof is directly at hand; if you later move it around there\n  is no ambiguity as to which theorem the proof is associated with.  It is also\n  the same syntax as supported by the [phfthm latex\n  package](https://github.com/phfaist/phfqitltx) which is able to produce\n  hyperlinks between theorems and their proofs.\n\n## Document Front Matter\n\nFLM Documents can contain YAML front matter that specify (i) options for the FLM\nparser, (ii) which features to enable, and (iii) additional document metadata such\nas a title.\n```yaml\n---\ntitle: \'My FLM document\'\nflm:\n   parsing:\n     enable_dollar_math_mode: True\n   features:\n     endnotes:\n       categories:\n         - category_name: footnote\n           counter_formatter: unicodesuperscript\n           heading_title: \'Footnotes\'\n           endnote_command: \'footnote\'\n---\n\n\\section{Greeting}\nHello, \\emph{world}. Inline math can now also be typeset\nas $a$ and $b$.  ...\n\n```\n\n### Imports\n\nYou can use the `$import:` directive to import a configuration from an\nexternal file, URL, or extension package:\n```yaml\n$import:\n  - my-flm-config.yaml # merge my-flm-config.yaml into this config.\n\n# you can still specify configuration to merge with here ...\n...\nflm:\n   ...\n```\n\nThe `$import:` target can specify multiple configurations to import.  Each list\nitem can be a absolute or relative file path (`$import: \'my-flm-config.yaml\'` or\n`$import: /path/to/my/flm-config.yaml`), a URL (`$import:\nhttps://example.com/my/flm-config.yaml`), or a fully qualified python package\nname introduced with ``pkg:package_name`` (e.g., `$import: pkg:flm_citations`).\nIf a package name is specified to the `$import` directive, the package is loaded\nand the default FLM configuration is extracted from it and included (the\n`flm_default_import_config` attribute of the module is read; it is assumed to be\na dictionary or a callable that returns a dictionary).  You can optionally\nfollow the package name by a path to specify submodules/attributes to read\ninstead of `flm_default_import_config`; e.g., ``pkg:mypackage/foo/bar`` will\nimport the module `mypackage` and import the configuration dictionary stored in\n``mypackage.foo.bar``.  FLM extention plugin/package authors can use this\nfeature to offer preset customization configurations that can easily be included\nwith ``pkg:some_flm_extension_package/some/preset/name``.\n\n\n### Parser configuration\n\nHere\'s a basic parser configuration that you can adapt:\n```yaml\nflm:\n  parsing:\n    # Enable/Disable comments as in LaTeX, led by ‘%%’\n    enable_comments: true\n    # This string initiates a comment up to the end of\n    # the line, if comments are enabled.  By default we\n    # require TWO \'%\' signs to avoid accidental comments\n    # (e.g., "... is up 10% from ...")\n    comment_start: \'%%\'\n    # Enable/Disable math mode with $ signs as in LaTeX\n    # in addition to \\( ...\\)\n    dollar_inline_math_mode: false\n    # Force parsing of the content in block-level mode\n    # (paragraphs).  Here ‘null’ means to auto-detect\n    force_block_level: null\n```\n\n### Renderer configuration (`html`, `text`, `latex`, `markdown`)\n\nHere\'s a basic renderer configuration that you can adapt **for HTML output**\n(`--format=html`):\n```yaml\nflm:\n  renderer:\n    html:\n      use_link_target_blank: false\n      html_blocks_joiner: \'\'\n      # use ‘headings_tags_by_level: null’ for defaults\n      heading_tags_by_level:\n        1: h1\n        2: h2\n        3: h3\n        4: span\n        5: span\n        6: span\n      inline_heading_add_space: true\n```\n\nHere\'s a basic renderer configuration that you can adapt **for text output**\n(`--format=text`):\n```yaml\nflm:\n  renderer:\n    text:\n      display_href_urls: true\n```\n\nHere\'s a basic renderer configuration that you can adapt **for LaTeX output**\n(`--format=latex`):\n```yaml\nflm:\n  renderer:\n    latex:\n      heading_commands_by_level:\n        1: "section"\n        2: "subsection"\n        3: "subsubsection"\n        4: "paragraph"\n        5: "subparagraph"\n        6: null\n```\n\nHere\'s a basic renderer configuration that you can adapt **for Markdown output**\n(`--format=markdown`):\n```yaml\nflm:\n  renderer:\n    markdown:\n      use_target_ids: \'github\' # or \'anchor\' or \'pandoc\' or null\n```\n\n\n### Features and their configuration\n\nMany FLM features are organized explicitly into feature classes which can be\nenabled or disabled at wish.  Features include:\n\n- enumeration (`\\begin{enumerate}...\\end{enumerate}`) and itemization\n  (`\\begin{itemize}...\\end{itemize}`) lists\n  \n- floats: figures and tables (`\\begin{figure}...\\end{figure}`)\n\n- headings (`\\section{...}` etc.)\n\n- etc.\n\nFeatures can be selected and configured directly in the FLM config metadata.  For instance\nthe following configuration is extracted from the default feature configuration when you run\nFLM:\n```yaml\nflm:\n  features:\n    # list features that should be available here.\n    enumeration:\n      enumeration_environments:\n        enumerate:\n          # here null means to use defaults\n          counter_formatter: null\n        itemize:\n          counter_formatter:\n            - "\\u2022"\n            - \'-\'\n            - "\\u25B8"\n    refs: {}\n    endnotes:\n      categories:\n        - category_name: footnote\n          counter_formatter: alph\n          endnote_command: footnote\n          heading_title: Footnotes\n      render_options:\n        include_headings_at_level: 1\n        set_headings_target_ids: true\n        endnotes_heading_title: null\n        endnotes_heading_level: 1\n    floats:\n      float_types:\n        - counter_formatter: Roman\n          float_caption_name: Fig.\n          float_type: figure\n          content_handlers: [\'any\', \'includegraphics\', \'cells\']\n        - counter_formatter: Roman\n          float_caption_name: Tab.\n          float_type: table\n          content_handlers: [\'cells\']\n    defterm: {}\n    graphics: {}\n```\n\n## Additional Features such as *Citations*\n\nAdditional features can be imported in the flm config.  They can reside in other\npython packages.  Some day I\'ll properly document how to write new features.\nFor now, check out the examples in `flm/feature/xxx.py` (and keep in mind that\nthe APIs are still likely to change!).\n\nTo include for instance the citations feature provided by the\n[flm-citations](https://github.com/phfaist/flm-citations) package, install that\npackage and use the config:\n```yaml\n$import:\n  - pkg:flm_citations\nbibliography:\n  - bibpreset.yaml\n  - anotherbibtest.json\n```\nCitations are organized by citation prefix and are automatically retrieved\ndepending on the type of citation.  By default:\n- Citations of the form `arxiv:<arXiv ID>` are automatically retrieved from the arXiv API\n- Citations of the form `doi:<DOI>` are automatically retrieved from [doi.org](https://doi.org/)\n- Citations of the form `manual:{Manual citation}` add the manual citation itself as a citation\n- Citations of the form `bib:key` look up `key` in one of the specified bibliography files.  The\n  bibliography files are expected to be CSL-JSON or CSL-YAML files. (Sorry, no bibtex for now.)\n\nYou can of course configure all of that manually. Check out the code in the\n[`flm-citations`](https://github.com/phfaist/flm-citations) repo for more insight.  Doc will\nhopefully come soon.\n\n\n# Using the `flm` package\n\nNeeds doc.\n\n## Example. Converting FLM to HTML\n\nNote: Math is simply marked with `<span class=...>` tags for use with\n[MathJax](https://www.mathjax.org/).\n\nExample:\n```py\nfrom flm.flmenvironment import make_standard_environment\nfrom flm.stdfeatures import standard_features\nfrom flm.fragmentrenderer.html import HtmlFragmentRenderer\n\nenviron = make_standard_environment(features=standard_features())\n\n# suppose we have fragments of FLM text\nfragment_1 = environ.make_fragment(r\'Hello, \\emph{world}.\')\nfragment_2 = environ.make_fragment(\n    r\'\'\'Here\'s a question: \\(1+2=?\\)\n\\begin{enumerate}[(a)]\n\\item 1\n\\item 2\n\\item 3\n\\end{enumerate}\n\'\'\'\n)\n\n# we can define a callback to render these fragments within an\n# HTML page. The advantage of doing so is that different fragments\n# can "see" each other! (E.g., for \\ref\'s, etc.) This feature can\n# be useful especially in combination with template engines.\ndef render_fn(render_context):\n    return (\n        "<main>\\n"\n        + "<div>" + fragment_1.render(render_context) + "</div>\\n"\n        + fragment_2.render(render_context) + "\\n"\n        + "</main>"\n    )\n\ndoc = environ.make_document(render_fn)\n\nfragment_renderer = HtmlFragmentRenderer()\nresult_html, render_context = doc.render(fragment_renderer)\n\nprint(result_html)\n# *** Prints:\n#\n# <main>\n# <div>Hello, <span class="textit">world</span>.</div>\n# <p>Here&#x27;s a question: <span class="inline-math">\\(1+2=?\\)</span></p>\n# <dl class="enumeration enumerate"><dt>(a)</dt><dd><p>1</p></dd><dt>(b)</dt><dd><p>2</p></dd><dt>(c)</dt><dd><p>3</p></dd></dl>\n# </main>\n```\n\n\n# A Javascript FLM library\n\nYou can transpile the core part of this library to Javascript using Transcrypt.\nSee [the `flm-js` subfolder](flm-js/README.md) for more details.\n',
-    'author': 'Philippe Faist',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# A Flexible Latex-Like Markup (FLM) language
 
+This package provides a simple parser and formatter for a custom markup language
+that is inspired by LaTeX syntax.
+
+The syntax of FLM is essentially a subset of standard LaTeX commands, including
+macros, environments, and some characters that have a special meaning; these
+features are parsed in a loosely similar fashion to usual LaTeX code.
+
+The framework is meant to be very easily extendible and customizable.  The
+parser is based on [*pylatexenc 3*](https://github.com/phfaist/pylatexenc)
+(which is currently still in development).
+
+FLM is used to write the contents of the [Error Correction
+Zoo](https://errorcorrectionzoo.org/) in a way that is intuitive for scientists,
+flexible, and robust.  It is easily extensible and closely resembles the LaTeX
+langauge that many scientists are familiar with.  FLM pushes further one of the
+core insights of LaTeX, namely, that the code should *describe* document
+contents in an intuitive way, as a markup language, while disregarding as much
+as possible the details of how that contents will be typeset.  The final
+typesetting is fully customizable, e.g., through CSS styling of its HTML output
+(including the use of templates).
+
+You can install FLM with pip:
+```bash
+$ pip install flm-core
+```
+
+Example `mydocument.flm`:
+```latex
+---
+title: Kitaev's Surface Code
+---
+\section{Kitaev's Surface Code}
+
+The \emph{stabilizers} of the \textit{surface code} on the 2-dimensional
+torus are generated by star operators \(A_v\) and plaquette operators
+\(B_p\).  Each star operator is a \textbf{product} of four Pauli-\(X\)
+operators on the edges adjacent to a vertex \(v\) of the lattice; each
+plaquette operator is a product of four Pauli-\(Z\) operators applied to
+the edges adjacent to a face, or plaquette, \(p\) of the lattice
+(\ref{figure:toric-code-operators}).
+
+\begin{figure}
+  \includegraphics{toric-code-operators}
+  \caption{Stabilizer generators and logical operators of the 2D surface
+    code on a torus.  The star operators \(A_v\) and the plaquette
+    operators \(B_p\) generate the stabilizer group of the toric code.
+    The logical operators are strings that wrap around the torus.}
+  \label{figure:toric-code-operators}
+\end{figure}
+
+...
+```
+
+To compile your document into an HTML page, use:
+```bash
+$ flm mydocument.flm -o mydocument.html --format=html --template=simple
+```
+
+You can then open the `mydocument.html` file in your browser.
+
+# This is work in progress!
+
+This project is still early in an active development stage, and there might
+still be a few bugs around. You can expect the API to still change pretty
+drastically.  Feel free to share ideas!
+
+# Use as a command-line tool
+
+You can use `flm` in command-line mode to compile your documents:
+```bash
+$ flm mydocument.flm
+```
+
+Run `flm --help` to get a list of options. They should be fairly
+standard and/or self-explanatory:
+```bash
+# output to file mydocument.html, format HTML, including skeleton
+# HTML structure with minimal CSS.
+$ flm mydocument.flm -o mydocument.html --format=html --template=simple
+```
+
+Available formats are `html`, `text`, `latex`, and `markdown`.  Formats
+`text`, `markdown`, and `latex` are very experimental!  (You can also
+generate `pdf` output with the options `--workflow=runlatexpdf --format=pdf`
+if your system has a standard LaTeX distribution such as TeXLive installed)
+
+- **Additional HTML Templates:**
+  The `--template=` option can be used to change the template used to render the
+  document.  See also the
+  [*flm-templates*](https://github.com/phfaist/flm-templates) extension package
+  for some additional templates and template engines.  You can try:
+  ```
+  > pip install flm-templates flm-htmlplus
+  ```
+  and then
+  ```
+  > flm mydocument.flm -o output.html -w flm_htmlplus -P 'pkg:flm_templates' -t sunset
+  ```
+  Or try the template `-t oldtextbook`.
+
+- **Citations from arXiv & DOI:**
+  Automatically fetch citations from the arXiv, DOI x-references, or other
+  sources using the [*flm-citations*](https://github.com/phfaist/flm-citations)
+  extension package (see README file there).  Install the extension package
+  using pip:
+  ```
+  > pip install flm-citations
+  ```
+  And then try to compile, e.g., the following FLM document:
+  ```yaml
+  ---
+  $import:
+    - pkg:flm_citations
+  ---
+  \section{Introduction}
+  Let's cite Kitaev's surface code~\cite{doi:10.1070/RM1997v052n06ABEH002155,doi:10.1007/978-1-4615-5923-8_19,arXiv:quant-ph/9707021}. ...
+  ```
+
+- **Theorems and proofs:** Use the environments
+  ``\begin{theorem}..\end{theorem}``, ``{lemma}``, ``{proposition}``,
+  ``{definition}``, ``{remark}``, etc. for typesetting theorems.  You can pin
+  labels to theorem statements ``\label{thm:XYZ}`` (use the `thm:` or `x:`
+  prefixes regardless of the theorem type, so you can easily change it without
+  having to update the label).  These environments accept an optional argument
+  so you can specify a title, e.g. ``\begin{theorem}[Euler's theorem]
+  ... \end{theorem}``.  Typeset proofs with ``\begin{proof} ... \end{proof}``.
+  The proof's optional argument enjoys an additional syntax: use
+  ``\begin{proof}[*thm:XYZ] ...`` to typeset `Proof (Theorem 3)` (with the
+  correct theorem reference using its label, which must match the one specified
+  to the theorem's ``\label`` command).  Use ``\begin{proof}[**thm:XYZ] ...`` to
+  simply typeset `Proof` as usual, but in this way you have the information about
+  which theorem the proof is directly at hand; if you later move it around there
+  is no ambiguity as to which theorem the proof is associated with.  It is also
+  the same syntax as supported by the [phfthm latex
+  package](https://github.com/phfaist/phfqitltx) which is able to produce
+  hyperlinks between theorems and their proofs.
+
+## Document Front Matter
+
+FLM Documents can contain YAML front matter that specify (i) options for the FLM
+parser, (ii) which features to enable, and (iii) additional document metadata such
+as a title.
+```yaml
+---
+title: 'My FLM document'
+flm:
+   parsing:
+     enable_dollar_math_mode: True
+   features:
+     endnotes:
+       categories:
+         - category_name: footnote
+           counter_formatter: unicodesuperscript
+           heading_title: 'Footnotes'
+           endnote_command: 'footnote'
+---
+
+\section{Greeting}
+Hello, \emph{world}. Inline math can now also be typeset
+as $a$ and $b$.  ...
+
+```
+
+### Imports
+
+You can use the `$import:` directive to import a configuration from an
+external file, URL, or extension package:
+```yaml
+$import:
+  - my-flm-config.yaml # merge my-flm-config.yaml into this config.
+
+# you can still specify configuration to merge with here ...
+...
+flm:
+   ...
+```
+
+The `$import:` target can specify multiple configurations to import.  Each list
+item can be a absolute or relative file path (`$import: 'my-flm-config.yaml'` or
+`$import: /path/to/my/flm-config.yaml`), a URL (`$import:
+https://example.com/my/flm-config.yaml`), or a fully qualified python package
+name introduced with ``pkg:package_name`` (e.g., `$import: pkg:flm_citations`).
+If a package name is specified to the `$import` directive, the package is loaded
+and the default FLM configuration is extracted from it and included (the
+`flm_default_import_config` attribute of the module is read; it is assumed to be
+a dictionary or a callable that returns a dictionary).  You can optionally
+follow the package name by a path to specify submodules/attributes to read
+instead of `flm_default_import_config`; e.g., ``pkg:mypackage/foo/bar`` will
+import the module `mypackage` and import the configuration dictionary stored in
+``mypackage.foo.bar``.  FLM extention plugin/package authors can use this
+feature to offer preset customization configurations that can easily be included
+with ``pkg:some_flm_extension_package/some/preset/name``.
+
+
+### Parser configuration
+
+Here's a basic parser configuration that you can adapt:
+```yaml
+flm:
+  parsing:
+    # Enable/Disable comments as in LaTeX, led by ‘%%’
+    enable_comments: true
+    # This string initiates a comment up to the end of
+    # the line, if comments are enabled.  By default we
+    # require TWO '%' signs to avoid accidental comments
+    # (e.g., "... is up 10% from ...")
+    comment_start: '%%'
+    # Enable/Disable math mode with $ signs as in LaTeX
+    # in addition to \( ...\)
+    dollar_inline_math_mode: false
+    # Force parsing of the content in block-level mode
+    # (paragraphs).  Here ‘null’ means to auto-detect
+    force_block_level: null
+```
+
+### Renderer configuration (`html`, `text`, `latex`, `markdown`)
+
+Here's a basic renderer configuration that you can adapt **for HTML output**
+(`--format=html`):
+```yaml
+flm:
+  renderer:
+    html:
+      use_link_target_blank: false
+      html_blocks_joiner: ''
+      # use ‘headings_tags_by_level: null’ for defaults
+      heading_tags_by_level:
+        1: h1
+        2: h2
+        3: h3
+        4: span
+        5: span
+        6: span
+      inline_heading_add_space: true
+```
+
+Here's a basic renderer configuration that you can adapt **for text output**
+(`--format=text`):
+```yaml
+flm:
+  renderer:
+    text:
+      display_href_urls: true
+```
+
+Here's a basic renderer configuration that you can adapt **for LaTeX output**
+(`--format=latex`):
+```yaml
+flm:
+  renderer:
+    latex:
+      heading_commands_by_level:
+        1: "section"
+        2: "subsection"
+        3: "subsubsection"
+        4: "paragraph"
+        5: "subparagraph"
+        6: null
+```
+
+Here's a basic renderer configuration that you can adapt **for Markdown output**
+(`--format=markdown`):
+```yaml
+flm:
+  renderer:
+    markdown:
+      use_target_ids: 'github' # or 'anchor' or 'pandoc' or null
+```
+
+
+### Features and their configuration
+
+Many FLM features are organized explicitly into feature classes which can be
+enabled or disabled at wish.  Features include:
+
+- enumeration (`\begin{enumerate}...\end{enumerate}`) and itemization
+  (`\begin{itemize}...\end{itemize}`) lists
+  
+- floats: figures and tables (`\begin{figure}...\end{figure}`)
+
+- headings (`\section{...}` etc.)
+
+- etc.
+
+Features can be selected and configured directly in the FLM config metadata.  For instance
+the following configuration is extracted from the default feature configuration when you run
+FLM:
+```yaml
+flm:
+  features:
+    # list features that should be available here.
+    enumeration:
+      enumeration_environments:
+        enumerate:
+          # here null means to use defaults
+          counter_formatter: null
+        itemize:
+          counter_formatter:
+            - "\u2022"
+            - '-'
+            - "\u25B8"
+    refs: {}
+    endnotes:
+      categories:
+        - category_name: footnote
+          counter_formatter: alph
+          endnote_command: footnote
+          heading_title: Footnotes
+      render_options:
+        include_headings_at_level: 1
+        set_headings_target_ids: true
+        endnotes_heading_title: null
+        endnotes_heading_level: 1
+    floats:
+      float_types:
+        - counter_formatter: Roman
+          float_caption_name: Fig.
+          float_type: figure
+          content_handlers: ['any', 'includegraphics', 'cells']
+        - counter_formatter: Roman
+          float_caption_name: Tab.
+          float_type: table
+          content_handlers: ['cells']
+    defterm: {}
+    graphics: {}
+```
+
+## Additional Features such as *Citations*
+
+Additional features can be imported in the flm config.  They can reside in other
+python packages.  Some day I'll properly document how to write new features.
+For now, check out the examples in `flm/feature/xxx.py` (and keep in mind that
+the APIs are still likely to change!).
+
+To include for instance the citations feature provided by the
+[flm-citations](https://github.com/phfaist/flm-citations) package, install that
+package and use the config:
+```yaml
+$import:
+  - pkg:flm_citations
+bibliography:
+  - bibpreset.yaml
+  - anotherbibtest.json
+```
+Citations are organized by citation prefix and are automatically retrieved
+depending on the type of citation.  By default:
+- Citations of the form `arxiv:<arXiv ID>` are automatically retrieved from the arXiv API
+- Citations of the form `doi:<DOI>` are automatically retrieved from [doi.org](https://doi.org/)
+- Citations of the form `manual:{Manual citation}` add the manual citation itself as a citation
+- Citations of the form `bib:key` look up `key` in one of the specified bibliography files.  The
+  bibliography files are expected to be CSL-JSON or CSL-YAML files. (Sorry, no bibtex for now.)
+
+You can of course configure all of that manually. Check out the code in the
+[`flm-citations`](https://github.com/phfaist/flm-citations) repo for more insight.  Doc will
+hopefully come soon.
+
+
+# Using the `flm` package
+
+Needs doc.
+
+## Example. Converting FLM to HTML
+
+Note: Math is simply marked with `<span class=...>` tags for use with
+[MathJax](https://www.mathjax.org/).
+
+Example:
+```py
+from flm.flmenvironment import make_standard_environment
+from flm.stdfeatures import standard_features
+from flm.fragmentrenderer.html import HtmlFragmentRenderer
+
+environ = make_standard_environment(features=standard_features())
+
+# suppose we have fragments of FLM text
+fragment_1 = environ.make_fragment(r'Hello, \emph{world}.')
+fragment_2 = environ.make_fragment(
+    r'''Here's a question: \(1+2=?\)
+\begin{enumerate}[(a)]
+\item 1
+\item 2
+\item 3
+\end{enumerate}
+'''
+)
+
+# we can define a callback to render these fragments within an
+# HTML page. The advantage of doing so is that different fragments
+# can "see" each other! (E.g., for \ref's, etc.) This feature can
+# be useful especially in combination with template engines.
+def render_fn(render_context):
+    return (
+        "<main>\n"
+        + "<div>" + fragment_1.render(render_context) + "</div>\n"
+        + fragment_2.render(render_context) + "\n"
+        + "</main>"
+    )
+
+doc = environ.make_document(render_fn)
+
+fragment_renderer = HtmlFragmentRenderer()
+result_html, render_context = doc.render(fragment_renderer)
+
+print(result_html)
+# *** Prints:
+#
+# <main>
+# <div>Hello, <span class="textit">world</span>.</div>
+# <p>Here&#x27;s a question: <span class="inline-math">\(1+2=?\)</span></p>
+# <dl class="enumeration enumerate"><dt>(a)</dt><dd><p>1</p></dd><dt>(b)</dt><dd><p>2</p></dd><dt>(c)</dt><dd><p>3</p></dd></dl>
+# </main>
+```
+
+
+# A Javascript FLM library
+
+You can transpile the core part of this library to Javascript using Transcrypt.
+See [the `flm-js` subfolder](flm-js/README.md) for more details.
 
-setup(**setup_kwargs)
```

