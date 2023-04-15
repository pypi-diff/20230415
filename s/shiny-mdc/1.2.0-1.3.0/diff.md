# Comparing `tmp/shiny_mdc-1.2.0.tar.gz` & `tmp/shiny_mdc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.2.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.3.0.tar", max compression
```

## Comparing `shiny_mdc-1.2.0.tar` & `shiny_mdc-1.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     2246 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/LICENSE
--rw-r--r--   0        0        0       78 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/README.md
--rw-r--r--   0        0        0     2295 2023-04-12 21:01:55.260967 shiny_mdc-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4713 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-12 21:01:55.260967 shiny_mdc-1.2.0/shinymdc/_version.py
--rw-r--r--   0        0        0      337 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      853 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0     3359 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1041 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      426 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    16580 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      977 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1443 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1440 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2187 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      897 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2099 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      511 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2343 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/lines.png
--rw-r--r--   0        0        0     2971 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/references.bib
--rw-r--r--   0        0        0   678733 2023-04-12 21:01:30.044997 shiny_mdc-1.2.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   411241 2023-04-12 21:01:30.044997 shiny_mdc-1.2.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   404508 2023-04-12 21:01:30.048997 shiny_mdc-1.2.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   443714 2023-04-12 21:01:30.048997 shiny_mdc-1.2.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   449285 2023-04-12 21:01:30.052997 shiny_mdc-1.2.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   599001 2023-04-12 21:01:30.056997 shiny_mdc-1.2.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   548590 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   421381 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1619 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/empty.md
--rw-r--r--   0        0        0     1356 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/utils/ext.md
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 shiny_mdc-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2641 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/README.md
+-rw-r--r--   0        0        0     2297 2023-04-15 15:54:00.737400 shiny_mdc-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4713 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-15 15:54:00.737400 shiny_mdc-1.3.0/shinymdc/_version.py
+-rw-r--r--   0        0        0      337 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      853 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      290 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1041 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      426 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19149 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      977 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1443 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1440 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2187 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      897 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     2099 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      511 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2343 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/figures/lines.png
+-rw-r--r--   0        0        0     2971 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/references.bib
+-rw-r--r--   0        0        0   678733 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/samples/basic.pdf
+-rw-r--r--   0        0        0   411241 2023-04-15 15:53:36.724693 shiny_mdc-1.3.0/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   404508 2023-04-15 15:53:36.724693 shiny_mdc-1.3.0/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   443714 2023-04-15 15:53:36.728693 shiny_mdc-1.3.0/test/samples/icml.pdf
+-rw-r--r--   0        0        0   449285 2023-04-15 15:53:36.728693 shiny_mdc-1.3.0/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   599001 2023-04-15 15:53:36.732693 shiny_mdc-1.3.0/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   548590 2023-04-15 15:53:36.732693 shiny_mdc-1.3.0/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   421381 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1619 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/empty.md
+-rw-r--r--   0        0        0     1356 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.3.0/PKG-INFO
```

### Comparing `shiny_mdc-1.2.0/CHANGELOG.md` & `shiny_mdc-1.3.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [1.3.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.2.0...v1.3.0) (2023-04-15)
+
+
+### Features
+
+* improve clean up of tex files directory ([d5b1822](https://github.com/jayanthkoushik/shiny-mdc/commit/d5b182265fbd3884ebc59ca618bd2302df400647))
+* improve command line interface ([58fb232](https://github.com/jayanthkoushik/shiny-mdc/commit/58fb2328e5c59bab3970ee7ff6beea1d4a9af252))
+
 ## [1.2.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.1.0...v1.2.0) (2023-04-12)
 
 
 ### Features
 
 * use more organized tex folder structure ([4296148](https://github.com/jayanthkoushik/shiny-mdc/commit/4296148d049c41634f80e8aa9535a5710d7d7874))
```

### Comparing `shiny_mdc-1.2.0/LICENSE` & `shiny_mdc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/pyproject.toml` & `shiny_mdc-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.2.0"  # managed by `poetry-dynamic-versioning`
+version = "1.3.0"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
@@ -24,15 +24,15 @@
 ]
 
 [tool.poetry.scripts]
 shinymdc = "shinymdc.shinymdc:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-corgy = { version="^7.0", extras = ["colors"] }
+corgy = { version="^8.1.1", extras = ["colors"] }
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.0"
 black = "^22.0"
 isort = "^5.1"
 pylint = "^2.14"
 mypy = "^1.1"
```

### Comparing `shiny_mdc-1.2.0/shinymdc/_latexmk.py` & `shiny_mdc-1.3.0/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/_liquid.py` & `shiny_mdc-1.3.0/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/_pandoc.py` & `shiny_mdc-1.3.0/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/_templates.py` & `shiny_mdc-1.3.0/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.3.0/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.3.0/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.3.0/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.3.0/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.3.0/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.3.0/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.3.0/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.3.0/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.3.0/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.3.0/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.3.0/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/shinymdc.py` & `shiny_mdc-1.3.0/shinymdc/shinymdc.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,122 +2,182 @@
 import shutil
 import sys
 from argparse import ArgumentParser
 from contextlib import ExitStack, redirect_stderr, redirect_stdout
 from pathlib import Path
 from subprocess import CalledProcessError
 from tempfile import NamedTemporaryFile
-from typing import Annotated
+from typing import Annotated, Literal
 
 import yaml
-from corgy import Corgy, CorgyHelpFormatter, corgyparser, NotRequired
-from corgy.types import (
-    KeyValuePairs,
-    LazyOutputDirectory,
-    OutputDirectory,
-    ReadableFile,
-    WritableFile,
-)
+from corgy import Corgy, corgychecker, CorgyHelpFormatter, corgyparser, NotRequired
+from corgy.types import KeyValuePairs
 
 from ._latexmk import run_latexmk
 from ._liquid import run_liquidjs
 from ._pandoc import run_pandoc
 from ._templates import BuiltinTemplate, Template
 from ._version import __version__ as corgy_version
 
 
 class ShinyMDC(Corgy, corgy_required_by_default=True):
+    Flag = Literal[True]
+
+    clean: NotRequired[Annotated[Flag, "do a clean build", ["-c", "--clean"]]]
+    verbose: NotRequired[Annotated[Flag, "enable verbose output", ["-v", "--verbose"]]]
+    quiet: NotRequired[Annotated[Flag, "suppress all output", ["-q", "--quiet"]]]
+
     input_path: NotRequired[
         Annotated[
-            ReadableFile,
+            Path,
             "input markdown file (will read from standard input if not specified)",
             ["-i", "--input"],
         ]
     ]
     output_path: NotRequired[
         Annotated[
-            WritableFile,
+            Path,
             "output file (will write to standard output if not specified)",
             ["-o", "--output"],
         ]
     ]
 
+    template: Annotated[
+        Template,
+        f"LaTeX template (path to custom template file, or name of a builtin "
+        f"template: {'/'.join(BuiltinTemplate.BUILTIN_TEMPLATE_NAMES)})",
+        ["-t", "--template"],
+    ] = BuiltinTemplate("basic")
+
     meta: NotRequired[
         Annotated[
             KeyValuePairs,
             "extra metadata to update the document metadata with",
             ["-m", "--meta"],
         ]
     ]
-
-    template: Annotated[
-        Template,
-        f"LaTeX template (path to custom template file, or name of a builtin "
-        f"template: {'/'.join(BuiltinTemplate.BUILTIN_TEMPLATE_NAMES)})",
-        ["-t", "--template"],
-    ] = BuiltinTemplate("basic")
+    default_img_ext: Annotated[
+        str, "default image extension", ["-x", "--default-img-ext"]
+    ] = "pdf"
+    natbib: Annotated[bool, "whether to use 'natbib' for bibliography"] = True
 
     build_dir: Annotated[
-        OutputDirectory,
+        Path,
         "directory for storing intermediate files and dependencies",
         ["-d", "--build-dir"],
-    ] = LazyOutputDirectory(".shinymdc")
-    tex_files_dir: Annotated[
-        OutputDirectory,
-        "directory for storing final tex files",
-        ["-D", "--tex-files-dir"],
-    ] = LazyOutputDirectory(".shinymdc/main")
-    main_tex: NotRequired[
+    ] = Path(".shinymdc")
+    tex_files_dir: NotRequired[
+        Annotated[
+            Path,
+            "store main tex files in this directory instead of '<build-dir>/main'",
+            ["-D", "--tex-files-dir"],
+        ]
+    ]
+    main_tex_path: NotRequired[
         Annotated[
-            WritableFile,
-            "write main tex to this file instead of '<tex-files-dir>/main.tex'",
+            Path, "write main tex to this file instead of '<tex-files-dir>/main.tex'",
         ]
     ]
-    copy_statics: Annotated[
-        bool, "whether to copy static resources to the tex files directory"
-    ] = False
+    copy_statics: NotRequired[
+        Annotated[Flag, "copy static resources to the tex files directory"]
+    ]
 
-    default_img_ext: Annotated[
-        str, "default image extension", ["-x", "--default-img-ext"]
-    ] = "pdf"
+    @corgychecker("input_path")
+    @staticmethod
+    def _check_is_readable_file(path: Path) -> Path:
+        if not path.exists():
+            raise ValueError(f"no such file: '{path}'")
+        if not path.is_file():
+            raise ValueError(f"not a file: '{path}'")
+        if not os.access(path, os.R_OK):
+            raise ValueError(f"file not readable: '{path}'")
+        return path
 
-    clean: Annotated[bool, "whether to do a clean build", ["-c", "--clean"]] = False
-    verbose: Annotated[
-        bool, "whether to enable verbose output", ["-v", "--verbose"]
-    ] = False
-    quiet: Annotated[bool, "whether to suppress all output", ["-q", "--quiet"]] = False
-    natbib: Annotated[bool, "whether to use 'natbib' for bibliography"] = True
+    @corgychecker("output_path", "main_tex_path")
+    @staticmethod
+    def _check_is_writable_file(path: Path) -> Path:
+        if path.exists():
+            if not path.is_file():
+                raise ValueError(f"not a file: '{path}'")
+            if not os.access(path, os.W_OK):
+                raise ValueError(f"file not writable: '{path}'")
+        else:
+            try:
+                path.parent.mkdir(parents=True, exist_ok=True)
+                path.touch()
+            except OSError as e:
+                raise ValueError(f"failed to create file: '{path}': {e}") from None
+        return path
+
+    @corgychecker("build_dir", "tex_files_dir")
+    @staticmethod
+    def _check_is_writable_dir(path: Path) -> Path:
+        if path.exists():
+            if not path.is_dir():
+                raise ValueError(f"not a directory: '{path}'")
+            if not os.access(path, os.W_OK):
+                raise ValueError(f"directory not writable: '{path}'")
+        else:
+            try:
+                path.mkdir(parents=True, exist_ok=True)
+            except OSError as e:
+                raise ValueError(f"failed to create directory: '{path}': {e}") from None
+        return path
 
     @corgyparser("template", metavar="name|path")
     @staticmethod
     def _parse_template(arg: str) -> Template:
         return Template.make(arg)
 
+    @corgyparser("input_path", metavar="file")
+    @staticmethod
+    def _parse_ifpath(arg: str) -> Path:
+        return ShinyMDC._check_is_readable_file(Path(arg))
+
+    @corgyparser("output_path", "main_tex_path", metavar="file")
+    @staticmethod
+    def _parse_ofpath(arg: str) -> Path:
+        return ShinyMDC._check_is_writable_file(Path(arg))
+
+    @corgyparser("build_dir", "tex_files_dir", metavar="dir")
+    @staticmethod
+    def _parse_odpath(arg: str) -> Path:
+        return ShinyMDC._check_is_writable_dir(Path(arg))
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.build_dir.init()
-        self.tex_files_dir.init()
-        if self.clean:
-            for _f in self.tex_files_dir.glob("*"):
+        if not hasattr(self, "tex_files_dir"):
+            self.tex_files_dir = self.build_dir / "main"
+            self.tex_files_dir.mkdir(exist_ok=True)
+        if not hasattr(self, "main_tex_path"):
+            self.main_tex_path = self.tex_files_dir / "main.tex"
+            self.main_tex_path.touch()
+        if hasattr(self, "clean"):
+            for _f in self.tex_files_dir.glob("*.tex"):
                 if _f.is_file():
+                    print(f"+ rm '{_f}'")
                     _f.unlink()
+            _rescs_dir = self.tex_files_dir / "resources"
+            if _rescs_dir.is_dir():
+                print(f"+ rm -rf '{_rescs_dir}'")
+                shutil.rmtree(_rescs_dir, ignore_errors=True)
         if not hasattr(self, "meta"):
             self.meta = KeyValuePairs("")
 
     def __call__(self) -> int:
         # Wrap the actual call with stdout/stderr redirections.
         # If 'output_path' is not specified, output has to be written to stdout.
         # So, redirect stdout to stderr to prevent subprocesses from writing
         # to stdout. The redirect is done unconditionaly to be consistent.
         # If 'quiet', redirect stderr to a temp file, so that the output can be
         # printed if there is an error.
         true_stdout = sys.stdout
         true_stderr = sys.stderr
         with ExitStack() as stack:
-            if self.quiet:
+            if hasattr(self, "quiet"):
                 # Redirect stderr and stdout to a temp file.
                 temp_file = stack.enter_context(NamedTemporaryFile("r+"))
                 stack.enter_context(redirect_stderr(temp_file))
                 stack.enter_context(redirect_stdout(temp_file))
             else:
                 # Redirect stdout to stderr.
                 temp_file = None
@@ -262,15 +322,15 @@
             combined_tex = run_pandoc(
                 combined_liquified_md_path,
                 stub_template_path,
                 bib_path,
                 None,  # metadata_path
                 self.default_img_ext,
                 self.natbib,
-                self.verbose,
+                hasattr(self, "verbose"),
                 **self.meta,
             )
 
         # Split compiled latex into constituent parts.
         parts = combined_tex.split(primary_sep.strip())
         body_tex = parts[0].strip()
         abstract_tex = parts[1].strip()
@@ -347,15 +407,15 @@
         with self.template.load() as (
             template_path,
             static_resc_paths,
             dynamic_resc_paths,
         ):
             # Add static resources to metadata.
             for resc_name, resc_path in static_resc_paths.items():
-                if self.copy_statics:
+                if hasattr(self, "copy_statics"):
                     # Copy the resource to the tex files dir if it is not already there.
                     copy_resc_path = rescs_dir / f"{resc_name}{resc_path.suffix}"
                     if not copy_resc_path.exists():
                         print(f"+ cp '{resc_path}' '{copy_resc_path}'", file=sys.stderr)
                         shutil.copy(resc_path, copy_resc_path)
                     resc_path = copy_resc_path
                 metadata[resc_name] = str(resc_path.with_suffix(""))
@@ -365,15 +425,15 @@
                 processed_resc_tex = run_pandoc(
                     Path(os.devnull),
                     resc_path,
                     bib_path,
                     metadata_path,
                     self.default_img_ext,
                     self.natbib,
-                    self.verbose,
+                    hasattr(self, "verbose"),
                     **self.meta,
                 )
                 processed_resc_path = rescs_dir / f"{resc_name}{resc_path.suffix}"
                 print(f"+ write '{processed_resc_path}'", file=sys.stderr)
                 processed_resc_path.write_text(processed_resc_tex)
                 metadata[resc_name] = str(processed_resc_path.with_suffix(""))
 
@@ -385,33 +445,35 @@
             main_tex = run_pandoc(
                 Path(os.devnull),
                 template_path,
                 bib_path,
                 metadata_path,
                 self.default_img_ext,
                 self.natbib,
-                self.verbose,
+                hasattr(self, "verbose"),
                 **self.meta,
             )
 
         # Write main tex to file.
-        main_tex_path = getattr(self, "main_tex", self.tex_files_dir / "main.tex")
-        print(f"+ write '{main_tex_path}'", file=sys.stderr)
-        main_tex_path.write_text(main_tex)
+        print(f"+ write '{self.main_tex_path}'", file=sys.stderr)
+        self.main_tex_path.write_text(main_tex)
 
         ############################################################
 
         ## 6. Generate pdf using latexmk.
 
         # Compile main tex with latexmk.
         latexmk_build_dir = self.build_dir / "latexmk"
         print(f"+ mkdir -p '{latexmk_build_dir}'", file=sys.stderr)
         latexmk_build_dir.mkdir(exist_ok=True)
         result_path = run_latexmk(
-            main_tex_path, latexmk_build_dir, self.clean, self.verbose
+            self.main_tex_path,
+            latexmk_build_dir,
+            hasattr(self, "clean"),
+            hasattr(self, "verbose"),
         )
 
         # Copy result to output file or write it to stdout.
         if hasattr(self, "output_path"):
             print(f"+ cp '{result_path}' '{self.output_path}'", file=sys.stderr)
             shutil.copy(result_path, self.output_path)
         else:
```

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.3.0/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.3.0/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.3.0/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.3.0/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.3.0/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.3.0/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.3.0/shinymdc/templates/stylish.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/figures/anscombe.pdf` & `shiny_mdc-1.3.0/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/figures/densities.pdf` & `shiny_mdc-1.3.0/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/figures/diamonds.pdf` & `shiny_mdc-1.3.0/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.3.0/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/figures/lines.png` & `shiny_mdc-1.3.0/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/main.md` & `shiny_mdc-1.3.0/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/references.bib` & `shiny_mdc-1.3.0/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/basic.pdf` & `shiny_mdc-1.3.0/test/samples/basic.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/iccv.pdf` & `shiny_mdc-1.3.0/test/samples/iccv.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/iclr.pdf` & `shiny_mdc-1.3.0/test/samples/iclr.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/icml.pdf` & `shiny_mdc-1.3.0/test/samples/icml.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/neurips.pdf` & `shiny_mdc-1.3.0/test/samples/neurips.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/spacious.pdf` & `shiny_mdc-1.3.0/test/samples/spacious.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/standalone.pdf` & `shiny_mdc-1.3.0/test/samples/standalone.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/samples/stylish.pdf` & `shiny_mdc-1.3.0/test/samples/stylish.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/sections/appendix1.md` & `shiny_mdc-1.3.0/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/sections/appendix2.md` & `shiny_mdc-1.3.0/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/sections/main1.md` & `shiny_mdc-1.3.0/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/sections/main2.md` & `shiny_mdc-1.3.0/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/test/utils/commands.md` & `shiny_mdc-1.3.0/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.2.0/PKG-INFO` & `shiny_mdc-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.2.0
+Version: 1.3.0
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: corgy[colors] (>=7.0,<8.0)
+Requires-Dist: corgy[colors] (>=8.1.1,<9.0.0)
 Project-URL: Repository, https://github.com/jayanthkoushik/shinymdc
 Description-Content-Type: text/markdown
 
 # shiny-mdc
 
 Tool to compile markdown files to tex/pdf using pandoc, latexmk.
```

