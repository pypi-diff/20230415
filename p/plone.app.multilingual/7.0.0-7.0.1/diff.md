# Comparing `tmp/plone.app.multilingual-7.0.0.tar.gz` & `tmp/plone.app.multilingual-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.multilingual-7.0.0.tar", last modified: Thu Apr  6 09:51:39 2023, max compression
+gzip compressed data, was "plone.app.multilingual-7.0.1.tar", last modified: Sat Apr 15 08:04:40 2023, max compression
```

## Comparing `plone.app.multilingual-7.0.0.tar` & `plone.app.multilingual-7.0.1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.058045 plone.app.multilingual-7.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)    27236 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      536 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/CREDITS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    42894 2023-04-06 09:51:39.058232 plone.app.multilingual-7.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    14047 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.010219 plone.app.multilingual-7.0.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/LICENSE.gpl
--rw-r--r--   0 maurits    (501) staff       (20)      678 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5620 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/Makefile
--rw-r--r--   0 maurits    (501) staff       (20)     7853 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/conf.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.012313 plone.app.multilingual-7.0.0/docs/images/
--rwxr-xr-x   0 maurits    (501) staff       (20)   135534 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/images/image00.png
--rwxr-xr-x   0 maurits    (501) staff       (20)   136010 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/images/image01.png
--rwxr-xr-x   0 maurits    (501) staff       (20)   136026 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/images/image02.png
--rwxr-xr-x   0 maurits    (501) staff       (20)    99720 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/images/image03.png
--rwxr-xr-x   0 maurits    (501) staff       (20)    36518 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/docs/images/image04.png
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-04-06 09:51:39.058864 plone.app.multilingual-7.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      701 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.002477 plone.app.multilingual-7.0.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.012690 plone.app.multilingual-7.0.0/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.016187 plone.app.multilingual-7.0.0/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.022752 plone.app.multilingual-7.0.0/src/plone/app/multilingual/
--rw-r--r--   0 maurits    (501) staff       (20)      331 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.029124 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7170 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/add.py
--rw-r--r--   0 maurits    (501) staff       (20)    11087 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    10300 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3821 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)    10468 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/helper_views.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.029543 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)     6926 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/images/gtranslate.png
--rw-r--r--   0 maurits    (501) staff       (20)     2511 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.030583 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/
--rw-r--r--   0 maurits    (501) staff       (20)     9666 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/babel_helper.js
--rw-r--r--   0 maurits    (501) staff       (20)   162462 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/jit-yc.js
--rw-r--r--   0 maurits    (501) staff       (20)     9659 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/mmap_helper.js
--rw-r--r--   0 maurits    (501) staff       (20)    22949 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/menu.py
--rw-r--r--   0 maurits    (501) staff       (20)    14571 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/migrator.py
--rw-r--r--   0 maurits    (501) staff       (20)     3352 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/modify.py
--rw-r--r--   0 maurits    (501) staff       (20)     4023 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/selector.py
--rw-r--r--   0 maurits    (501) staff       (20)    10558 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.030956 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/stylesheet/
--rw-r--r--   0 maurits    (501) staff       (20)     2297 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/stylesheet/multilingual.css
--rw-r--r--   0 maurits    (501) staff       (20)     1104 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/switcher.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.037287 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1232 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt
--rw-r--r--   0 maurits    (501) staff       (20)      154 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/alternate-languages.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3714 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/cleanup.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1070 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/cleanup_results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2629 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/dexterity_edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1438 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/disconnect_translation.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1231 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/dx_babel_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      682 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/languages-notice.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1315 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/languageselector.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11049 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/migration.pt
--rw-r--r--   0 maurits    (501) staff       (20)      996 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/migrator-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4613 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/mmap.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4980 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/modify_translations.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2744 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/not_translated_yet.pt
--rw-r--r--   0 maurits    (501) staff       (20)      940 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/reindex-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1006 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/relocate-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3295 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/translate.py
--rw-r--r--   0 maurits    (501) staff       (20)     1084 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/update.py
--rw-r--r--   0 maurits    (501) staff       (20)     6724 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      470 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     5531 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/viewlets.py
--rw-r--r--   0 maurits    (501) staff       (20)     5928 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     6818 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.038929 plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      648 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/lif.py
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/lif.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/lrf.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.043218 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/
--rw-r--r--   0 maurits    (501) staff       (20)       48 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4430 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/cloner.py
--rw-r--r--   0 maurits    (501) staff       (20)     2650 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1640 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3157 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/form.py
--rw-r--r--   0 maurits    (501) staff       (20)      771 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      652 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/language.py
--rw-r--r--   0 maurits    (501) staff       (20)      455 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/languageindependent.py
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     4957 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/subscriber.py
--rw-r--r--   0 maurits    (501) staff       (20)     1100 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2994 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     3350 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/factory.py
--rw-r--r--   0 maurits    (501) staff       (20)      366 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     8439 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1571 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/itg.py
--rw-r--r--   0 maurits    (501) staff       (20)     8502 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/manager.py
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)      218 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.005102 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.046329 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      373 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      171 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       51 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/plone.app.multilingual_default.txt
--rw-r--r--   0 maurits    (501) staff       (20)       96 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/reference_catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1273 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      301 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.047053 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2434 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/LIF.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2464 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/LRF.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      353 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.050378 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      151 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      324 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/cssregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       68 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       51 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/plone.app.multilingual_uninstall.txt
--rw-r--r--   0 maurits    (501) staff       (20)      111 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/reference_catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      154 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      318 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/uninstall/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.005687 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.005362 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.051163 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/
--rw-r--r--   0 maurits    (501) staff       (20)      831 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml
--rw-r--r--   0 maurits    (501) staff       (20)      824 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.051432 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_3/
--rw-r--r--   0 maurits    (501) staff       (20)      253 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_3/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.051728 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_4/
--rw-r--r--   0 maurits    (501) staff       (20)      942 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2988 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/shared_uuid.py
--rw-r--r--   0 maurits    (501) staff       (20)     6529 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/subscriber.py
--rw-r--r--   0 maurits    (501) staff       (20)     9607 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      178 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.056718 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.057856 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3534 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/test_add_translation.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3418 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/test_translate_content.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1434 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_alternates.py
--rw-r--r--   0 maurits    (501) staff       (20)    11045 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_api.py
--rw-r--r--   0 maurits    (501) staff       (20)     2147 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1878 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     8744 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_form.py
--rw-r--r--   0 maurits    (501) staff       (20)     5819 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_helper_views.py
--rw-r--r--   0 maurits    (501) staff       (20)     9471 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_lif.py
--rw-r--r--   0 maurits    (501) staff       (20)     5354 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3299 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_menu.py
--rw-r--r--   0 maurits    (501) staff       (20)      532 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)    39142 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_selector.py
--rw-r--r--   0 maurits    (501) staff       (20)     4552 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     3323 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     6580 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1601 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_uninstall.py
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     7179 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     2432 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone/app/multilingual/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 09:51:39.015869 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    42894 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7004 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      125 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-06 09:51:38.000000 plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.128169 plone.app.multilingual-7.0.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)    27356 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      536 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/CREDITS.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      123 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    42987 2023-04-15 08:04:40.128169 plone.app.multilingual-7.0.1/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)    14047 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.113169 plone.app.multilingual-7.0.1/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/LICENSE.gpl
+-rw-r--r--   0 gil       (1000) gil       (1000)      678 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     5620 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/Makefile
+-rw-r--r--   0 gil       (1000) gil       (1000)     8041 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/conf.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.114169 plone.app.multilingual-7.0.1/docs/images/
+-rwxr-xr-x   0 gil       (1000) gil       (1000)   135534 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/images/image00.png
+-rwxr-xr-x   0 gil       (1000) gil       (1000)   136010 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/images/image01.png
+-rwxr-xr-x   0 gil       (1000) gil       (1000)   136026 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/images/image02.png
+-rwxr-xr-x   0 gil       (1000) gil       (1000)    99720 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/images/image03.png
+-rwxr-xr-x   0 gil       (1000) gil       (1000)    36518 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/docs/images/image04.png
+-rw-r--r--   0 gil       (1000) gil       (1000)     1761 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1187 2023-04-15 08:04:40.129169 plone.app.multilingual-7.0.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1756 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.111169 plone.app.multilingual-7.0.1/src/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.114169 plone.app.multilingual-7.0.1/src/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.115169 plone.app.multilingual-7.0.1/src/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.117169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/
+-rw-r--r--   0 gil       (1000) gil       (1000)      331 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1683 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/api.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.119169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7170 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/add.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    11381 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)    10300 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3821 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/edit.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10414 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/helper_views.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.119169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/images/
+-rw-r--r--   0 gil       (1000) gil       (1000)     6926 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/images/gtranslate.png
+-rw-r--r--   0 gil       (1000) gil       (1000)     2511 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/interfaces.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.120169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/
+-rw-r--r--   0 gil       (1000) gil       (1000)     9667 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/babel_helper.js
+-rw-r--r--   0 gil       (1000) gil       (1000)   162462 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/jit-yc.js
+-rw-r--r--   0 gil       (1000) gil       (1000)     9667 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/mmap_helper.js
+-rw-r--r--   0 gil       (1000) gil       (1000)    22949 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/menu.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14381 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/migrator.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3352 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/modify.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4024 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/selector.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10558 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.120169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/stylesheet/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2297 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/stylesheet/multilingual.css
+-rw-r--r--   0 gil       (1000) gil       (1000)     1104 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/switcher.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.122169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1330 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      157 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/alternate-languages.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     3843 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/cleanup.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1237 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/cleanup_results.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1938 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/controlpanel.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2877 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/dexterity_edit.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1732 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/disconnect_translation.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1563 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/dx_babel_view.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      767 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/languages-notice.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1347 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/languageselector.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    11015 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/migration.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1208 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/migrator-results.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     5387 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/mmap.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     6884 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/modify_translations.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     3307 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/not_translated_yet.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1152 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/reindex-results.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1218 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/relocate-results.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     3295 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/translate.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1084 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/update.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6724 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      470 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5012 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/viewlets.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5962 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/vocabularies.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6674 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.122169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      602 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/lif.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      131 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/lif.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1429 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/lrf.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      131 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/lrf.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.124169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/
+-rw-r--r--   0 gil       (1000) gil       (1000)       48 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4430 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/cloner.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2725 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1640 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/directives.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3157 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/form.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      770 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      652 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/language.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      456 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/languageindependent.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      139 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/meta.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2521 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/schemaeditor.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4955 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/subscriber.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1100 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/supermodel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2994 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3338 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/factory.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      366 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/indexer.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8436 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1571 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/itg.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8502 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/manager.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      151 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/overrides.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)       67 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/permissions.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      234 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/permissions.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.112169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.125169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)      188 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/browserlayer.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      427 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/catalog.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      188 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)       51 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/plone.app.multilingual_default.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      113 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/reference_catalog.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1344 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/registry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      343 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/rolemap.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.125169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2680 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/LIF.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2711 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/LRF.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      240 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      412 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/viewlets.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.126169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/
+-rw-r--r--   0 gil       (1000) gil       (1000)      211 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      418 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/catalog.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      191 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/cssregistry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)       85 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)       51 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/plone.app.multilingual_uninstall.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      139 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/reference_catalog.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      202 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/types.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      362 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/uninstall/viewlets.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.112169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.112169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.126169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1032 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1025 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.126169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_3/
+-rw-r--r--   0 gil       (1000) gil       (1000)      276 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_3/registry.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.126169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_4/
+-rw-r--r--   0 gil       (1000) gil       (1000)      975 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2988 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/setuphandlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1214 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/shared_uuid.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6529 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/subscriber.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9607 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/testing.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      183 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/testing.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.128169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.128169 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3534 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/test_add_translation.robot
+-rw-r--r--   0 gil       (1000) gil       (1000)     3418 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot
+-rw-r--r--   0 gil       (1000) gil       (1000)     2205 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/test_translate_content.robot
+-rw-r--r--   0 gil       (1000) gil       (1000)     1434 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_alternates.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    11045 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_api.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2147 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_catalog.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1878 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_directives.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8744 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_form.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5819 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_helper_views.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9471 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_lif.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5354 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_lrf.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3299 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_menu.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      532 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_robot.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    39142 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_selector.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4419 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3326 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_sitemap.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6580 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_subscribers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1601 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_uninstall.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1288 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_vocabularies.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7095 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/upgrades.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2469 2023-04-15 08:04:39.000000 plone.app.multilingual-7.0.1/src/plone/app/multilingual/upgrades.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:04:40.115169 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    42987 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     7004 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      733 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:04:40.000000 plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/top_level.txt
```

### Comparing `plone.app.multilingual-7.0.0/CHANGES.rst` & `plone.app.multilingual-7.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+7.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (11f0db91)
+
+
 7.0.0 (2023-04-06)
 ------------------
 
 Breaking changes:
 
 
 - Move language independent field declarations from plone.app.event to this package.
@@ -335,15 +345,15 @@
 
 Bug fixes:
 
 
 - Remove deprecation warnings in tests.
   Increase readability
   Add code comments.
-  Remove superfluos reindex of "Language" in manager.
+  Remove superfluous reindex of "Language" in manager.
   [jensens] (#256)
 - wrong check for default addview in addtranslation traverser
   [mauro] (#355)
 - Remove any dependency to ``archetypes.multilingual``, since this is a indirection.
   Remove all dependencies that are already part of ``Products.CMFPlone``.
   All version specifications were reduced to use a recent ``Products.CMFPlone``.
   The ``decorator`` dependency is no longer used.
@@ -613,28 +623,28 @@
 
 5.0.5 (2017-04-27)
 ------------------
 
 Bug fixes:
 
 - Remove travis integration because plone.app.mutlilingual is part of plonecore and should be tested there.
-- Fix bug where formcontrols were overlaped by fields.
+- Fix bug where form controls were overlapped by fields.
   [agitator]
 
 - Fix robot tests to work with improved related items widget.
   [thet]
 
 
 5.0.4 (2017-03-26)
 ------------------
 
 New features:
 
 - Add a new view ``@@tg`` for translatable content. It will return the
-  current translation group of the content, matching the bahavior of ``@@uuid``
+  current translation group of the content, matching the behavior of ``@@uuid``
   of ``plone.app.uuid`` returning UUID of the content.  [datakurre]
 
 
 5.0.3 (2017-02-12)
 ------------------
 
 New features:
@@ -658,15 +668,15 @@
 
 
 5.0.1 (2017-01-02)
 ------------------
 
 Bug fixes:
 
-- Allow to work in an Archtypes free Plone 5.1.
+- Allow to work in an Archetypes free Plone 5.1.
   [jensens]
 
 - Replace unittest2 with unittest.
   [jensens]
 
 
 5.0 (2016-11-17)
@@ -756,15 +766,15 @@
 -------------------
 
 Fixes:
 
 - Wait for visibility of select2 result, instead of time.
   [jensens]
 
-- Workaroud in robot test for TinyMCE overlap bug see
+- Workaround in robot test for TinyMCE overlap bug see
   https://github.com/plone/plone.app.multilingual/issues/227
   for details
   [jensens]
 
 
 3.0.16 (2016-03-31)
 -------------------
@@ -950,18 +960,18 @@
 
 - Add more common api functions and test them.
   [jensens]
 
 - Refactor locations of code in dx to bundle stuff at a sane place.
   [jensens]
 
-- Remove BLACKLIST_IDS, with LIF this is superfluos.
+- Remove BLACKLIST_IDS, with LIF this is superfluous.
   [jensens]
 
-- Remove LanguageTool patch, meanwhile superfluos.
+- Remove LanguageTool patch, meanwhile superfluous.
   [jensens]
 
 - Add new ``bootstrap.py`` to support new parameter ``--setuptools-version``.
   [saily]
 
 - Fixed language independent fields in ++addtranslation++
   requires ``plone.z3cform >= 0.8.1``
@@ -1050,15 +1060,15 @@
 - Fix an import issue in ``upgrades.py``
   [saily]
 
 - Add code analysis to ``plone-test-4.x.cfg`` and ``plone-test-5.x.cfg``
   [saily]
 
 - Huge PEP8 and Flake8 cleanup. Please run ``bin/code-analysis`` before
-  commiting. A git pre-commit hook should be added automatically through
+  committing. A git pre-commit hook should be added automatically through
   buildout.
   [saily]
 
 - Ensure ``plone.app.controlpanel.Language`` permission is present.
   [saily]
 
 - Merge ``add.py`` and ``add_translation_form.py`` into one file
@@ -1110,15 +1120,15 @@
   [ksuess]
 
 - Bugfix: p.a.contentmenu fails if access to translation is not permitted.
   Solution: Introduce restricted access and use it in vocabulary for menu.
   [jensens]
 
 - Added ++add++ and factory support using session var to store where it comes
-  from. It maintains the old programatic way so it's possible to create
+  from. It maintains the old programmatic way so it's possible to create
   translations using code.
   [ramon]
 
 - Extend travis integration to test against Plone 4.1, 4.2, 4.3 and
   include following dependencies into tests:
   - ``plone.multilingual``
   - ``plone.multilingualbehavior``
@@ -1128,15 +1138,15 @@
 - plone.app.contenttypes compatibility on setup
   [sneridagh]
 
 - Added French translation
   [bouchardsyl]
 
 - take care to filter out translated contents
-  wich do no have supported language information
+  which do no have supported language information
   [kiorky]
 
 - added support for language neutral objects with country specific language codes
   by checking _combinedlanguagelist too
   [agitator]
 
 
@@ -1199,15 +1209,15 @@
 
 - Add after migration action on view
   [do3cc]
 
 - Multilingual Map
   [ramon]
 
-- Univeral link
+- Universal link
   [ramon]
 
 - Catalog patch bug solving
   [ramon]
 
 - Language selector bug solving
   [sneridagh]
@@ -1233,15 +1243,15 @@
 - Allow to see all content on adding translation
   [ramon]
 
 
 1.0b2 - 2012-07-08
 ------------------
 
-- change language index to Language to LinguaPlone coexistance
+- change language index to Language to LinguaPlone coexistence
   [ramon]
 
 - don't rebuild the complete catalog on installing
   [pbauer]
 
 - add indexes via setuphandler instead of xml to prevents purging on reinstall
   [pbauer]
```

### Comparing `plone.app.multilingual-7.0.0/CREDITS.rst` & `plone.app.multilingual-7.0.1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/PKG-INFO` & `plone.app.multilingual-7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.multilingual
-Version: 7.0.0
+Version: 7.0.1
 Summary: Multilingual Plone Content package
 Home-page: https://github.com/plone/plone.app.multilingual
 Author: Ramon Navarro, Victor Fernandez de Alba, awello et al
 Author-email: r.navarro@iskra.cat
 Maintainer: Plone Foundation
 Maintainer-email: releasemanager@plone.org
 License: GPL
@@ -19,15 +19,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Provides-Extra: archetypes
 Provides-Extra: test
 
 .. contents::
 
 
 Introduction
 ============
@@ -192,15 +191,15 @@
 
 Dexterity
 ---------
 
 Users should mark a dexterity content type as translatable by assigning a the multilingual behavior to the definition of the content type either via file system, supermodel or through the web.
 
 
-Marking fields as language independant
+Marking fields as language independent
 ======================================
 
 Archetypes
 ----------
 
 The language independent fields on Archetype-based content are marked the same way as in LinguaPlone::
 
@@ -210,15 +209,15 @@
         ....
         ),
         languageIndependent=True
     ),
 
 .. note::
 
-    If you want to completely remove LinguaPlone of your installation, you should make sure that your code are dependant in any way of LP.
+    If you want to completely remove LinguaPlone of your installation, you should make sure that your code are dependent in any way of LP.
 
 
 Dexterity
 ---------
 
 There are four ways of achieve it.
 
@@ -381,14 +380,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+7.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (11f0db91)
+
+
 7.0.0 (2023-04-06)
 ------------------
 
 Breaking changes:
 
 
 - Move language independent field declarations from plone.app.event to this package.
@@ -712,15 +721,15 @@
 
 Bug fixes:
 
 
 - Remove deprecation warnings in tests.
   Increase readability
   Add code comments.
-  Remove superfluos reindex of "Language" in manager.
+  Remove superfluous reindex of "Language" in manager.
   [jensens] (#256)
 - wrong check for default addview in addtranslation traverser
   [mauro] (#355)
 - Remove any dependency to ``archetypes.multilingual``, since this is a indirection.
   Remove all dependencies that are already part of ``Products.CMFPlone``.
   All version specifications were reduced to use a recent ``Products.CMFPlone``.
   The ``decorator`` dependency is no longer used.
@@ -990,28 +999,28 @@
 
 5.0.5 (2017-04-27)
 ------------------
 
 Bug fixes:
 
 - Remove travis integration because plone.app.mutlilingual is part of plonecore and should be tested there.
-- Fix bug where formcontrols were overlaped by fields.
+- Fix bug where form controls were overlapped by fields.
   [agitator]
 
 - Fix robot tests to work with improved related items widget.
   [thet]
 
 
 5.0.4 (2017-03-26)
 ------------------
 
 New features:
 
 - Add a new view ``@@tg`` for translatable content. It will return the
-  current translation group of the content, matching the bahavior of ``@@uuid``
+  current translation group of the content, matching the behavior of ``@@uuid``
   of ``plone.app.uuid`` returning UUID of the content.  [datakurre]
 
 
 5.0.3 (2017-02-12)
 ------------------
 
 New features:
@@ -1035,15 +1044,15 @@
 
 
 5.0.1 (2017-01-02)
 ------------------
 
 Bug fixes:
 
-- Allow to work in an Archtypes free Plone 5.1.
+- Allow to work in an Archetypes free Plone 5.1.
   [jensens]
 
 - Replace unittest2 with unittest.
   [jensens]
 
 
 5.0 (2016-11-17)
@@ -1133,15 +1142,15 @@
 -------------------
 
 Fixes:
 
 - Wait for visibility of select2 result, instead of time.
   [jensens]
 
-- Workaroud in robot test for TinyMCE overlap bug see
+- Workaround in robot test for TinyMCE overlap bug see
   https://github.com/plone/plone.app.multilingual/issues/227
   for details
   [jensens]
 
 
 3.0.16 (2016-03-31)
 -------------------
@@ -1327,18 +1336,18 @@
 
 - Add more common api functions and test them.
   [jensens]
 
 - Refactor locations of code in dx to bundle stuff at a sane place.
   [jensens]
 
-- Remove BLACKLIST_IDS, with LIF this is superfluos.
+- Remove BLACKLIST_IDS, with LIF this is superfluous.
   [jensens]
 
-- Remove LanguageTool patch, meanwhile superfluos.
+- Remove LanguageTool patch, meanwhile superfluous.
   [jensens]
 
 - Add new ``bootstrap.py`` to support new parameter ``--setuptools-version``.
   [saily]
 
 - Fixed language independent fields in ++addtranslation++
   requires ``plone.z3cform >= 0.8.1``
@@ -1427,15 +1436,15 @@
 - Fix an import issue in ``upgrades.py``
   [saily]
 
 - Add code analysis to ``plone-test-4.x.cfg`` and ``plone-test-5.x.cfg``
   [saily]
 
 - Huge PEP8 and Flake8 cleanup. Please run ``bin/code-analysis`` before
-  commiting. A git pre-commit hook should be added automatically through
+  committing. A git pre-commit hook should be added automatically through
   buildout.
   [saily]
 
 - Ensure ``plone.app.controlpanel.Language`` permission is present.
   [saily]
 
 - Merge ``add.py`` and ``add_translation_form.py`` into one file
@@ -1487,15 +1496,15 @@
   [ksuess]
 
 - Bugfix: p.a.contentmenu fails if access to translation is not permitted.
   Solution: Introduce restricted access and use it in vocabulary for menu.
   [jensens]
 
 - Added ++add++ and factory support using session var to store where it comes
-  from. It maintains the old programatic way so it's possible to create
+  from. It maintains the old programmatic way so it's possible to create
   translations using code.
   [ramon]
 
 - Extend travis integration to test against Plone 4.1, 4.2, 4.3 and
   include following dependencies into tests:
   - ``plone.multilingual``
   - ``plone.multilingualbehavior``
@@ -1505,15 +1514,15 @@
 - plone.app.contenttypes compatibility on setup
   [sneridagh]
 
 - Added French translation
   [bouchardsyl]
 
 - take care to filter out translated contents
-  wich do no have supported language information
+  which do no have supported language information
   [kiorky]
 
 - added support for language neutral objects with country specific language codes
   by checking _combinedlanguagelist too
   [agitator]
 
 
@@ -1576,15 +1585,15 @@
 
 - Add after migration action on view
   [do3cc]
 
 - Multilingual Map
   [ramon]
 
-- Univeral link
+- Universal link
   [ramon]
 
 - Catalog patch bug solving
   [ramon]
 
 - Language selector bug solving
   [sneridagh]
@@ -1610,15 +1619,15 @@
 - Allow to see all content on adding translation
   [ramon]
 
 
 1.0b2 - 2012-07-08
 ------------------
 
-- change language index to Language to LinguaPlone coexistance
+- change language index to Language to LinguaPlone coexistence
   [ramon]
 
 - don't rebuild the complete catalog on installing
   [pbauer]
 
 - add indexes via setuphandler instead of xml to prevents purging on reinstall
   [pbauer]
```

### Comparing `plone.app.multilingual-7.0.0/README.rst` & `plone.app.multilingual-7.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
 Dexterity
 ---------
 
 Users should mark a dexterity content type as translatable by assigning a the multilingual behavior to the definition of the content type either via file system, supermodel or through the web.
 
 
-Marking fields as language independant
+Marking fields as language independent
 ======================================
 
 Archetypes
 ----------
 
 The language independent fields on Archetype-based content are marked the same way as in LinguaPlone::
 
@@ -182,15 +182,15 @@
         ....
         ),
         languageIndependent=True
     ),
 
 .. note::
 
-    If you want to completely remove LinguaPlone of your installation, you should make sure that your code are dependant in any way of LP.
+    If you want to completely remove LinguaPlone of your installation, you should make sure that your code are dependent in any way of LP.
 
 
 Dexterity
 ---------
 
 There are four ways of achieve it.
```

### Comparing `plone.app.multilingual-7.0.0/docs/LICENSE.gpl` & `plone.app.multilingual-7.0.1/docs/LICENSE.gpl`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/LICENSE.txt` & `plone.app.multilingual-7.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/Makefile` & `plone.app.multilingual-7.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/conf.py` & `plone.app.multilingual-7.0.1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,238 +6,248 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
-
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'plone.app.multilingual'
-copyright = '2013, Plone Foundation'
+project = "plone.app.multilingual"
+copyright = "2013, Plone Foundation"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.0'
+version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = '1.0'
+release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'ploneappmultilingualdoc'
+htmlhelp_basename = "ploneappmultilingualdoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
+    # The paper size ('letterpaper' or 'a4paper').
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'ploneappmultilingual.tex', 'plone.app.multilingual Documentation',
-   'Plone Foundation', 'manual'),
+    (
+        "index",
+        "ploneappmultilingual.tex",
+        "plone.app.multilingual Documentation",
+        "Plone Foundation",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'ploneappmultilingual', 'plone.app.multilingual Documentation',
-     ['Plone Foundation'], 1)
+    (
+        "index",
+        "ploneappmultilingual",
+        "plone.app.multilingual Documentation",
+        ["Plone Foundation"],
+        1,
+    )
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  ('index', 'ploneappmultilingual', 'plone.app.multilingual Documentation',
-   'Plone Foundation', 'ploneappmultilingual', 'One line description of project.',
-   'Miscellaneous'),
+    (
+        "index",
+        "ploneappmultilingual",
+        "plone.app.multilingual Documentation",
+        "Plone Foundation",
+        "ploneappmultilingual",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
```

### Comparing `plone.app.multilingual-7.0.0/docs/images/image00.png` & `plone.app.multilingual-7.0.1/docs/images/image00.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/images/image01.png` & `plone.app.multilingual-7.0.1/docs/images/image01.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/images/image02.png` & `plone.app.multilingual-7.0.1/docs/images/image02.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/images/image03.png` & `plone.app.multilingual-7.0.1/docs/images/image03.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/docs/images/image04.png` & `plone.app.multilingual-7.0.1/docs/images/image04.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/setup.cfg` & `plone.app.multilingual-7.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 7.0.0
+version = 7.0.1
 name = plone.app.multilingual
 description = Multilingual Plone Content package
 long_description = file: README.rst, CREDITS.rst, CHANGES.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Plone
@@ -26,22 +26,27 @@
 maintainer_email = releasemanager@plone.org
 
 [options]
 python_requires = >=3.8
 
 [check-manifest]
 ignore = 
-	*.cfg
+	.editorconfig
+	.meta.toml
+	.pre-commit-config.yaml
+	tox.ini
 
 [bdist_wheel]
 universal = 0
 
-[isort]
-profile = black
-force_alphabetical_sort = True
-force_single_line = True
-lines_after_imports = 2
+[flake8]
+doctests = 1
+ignore = 
+	E501,
+	W503,
+	E203,
+	E231,
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/api.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         raise ValueError("No translation group found.")
     return tg
 
 
 def get_translation_manager(content):
     """Get the translation manager.
 
-    :param content: Content for which the tranlation manager is needed.
+    :param content: Content for which the translation manager is needed.
     :type content: Content object
     :returns: translation manager instance.
     :raises:
         ValueError
     """
     tm = ITranslationManager(content)
     if tm is None:
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/add.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/configure.zcml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/configure.zcml`

 * *Files 9% similar despite different names*

```diff
@@ -1,295 +1,332 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
-  <include package="plone.app.contentmenu"/>
+  <include package="plone.app.contentmenu" />
 
   <!-- Resource Directories -->
   <browser:resourceDirectory
       name="plone.app.multilingual.javascript"
-      directory="javascript"/>
+      directory="javascript"
+      />
   <browser:resourceDirectory
       name="plone.app.multilingual.stylesheet"
-      directory="stylesheet"/>
+      directory="stylesheet"
+      />
   <browser:resourceDirectory
       name="plone.app.multilingual.images"
-      directory="images"/>
+      directory="images"
+      />
 
   <!-- Vocabulary all languages -->
   <utility
+      name="plone.app.multilingual.vocabularies.AllContentLanguageVocabulary"
       component=".vocabularies.AllContentLanguageVocabularyFactory"
-      name="plone.app.multilingual.vocabularies.AllContentLanguageVocabulary"/>
+      />
 
   <utility
+      name="plone.app.multilingual.vocabularies.AllAvailableLanguageVocabulary"
       component=".vocabularies.AllAvailableLanguageVocabularyFactory"
-      name="plone.app.multilingual.vocabularies.AllAvailableLanguageVocabulary"/>
+      />
 
   <utility
       factory=".vocabularies.RootCatalogVocabularyFactory"
       name="plone.app.multilingual.RootCatalog"
       />
 
   <adapter
+      factory=".add.AddViewTraverser"
       name="addtranslation"
-      factory=".add.AddViewTraverser"/>
+      />
 
   <browser:page
       name="modify_translations"
       for="plone.app.multilingual.interfaces.ITranslatable"
       class=".modify.ModifyTranslationsForm"
       template="templates/modify_translations.pt"
-      permission="plone.app.multilingual.ManageTranslations"/>
+      permission="plone.app.multilingual.ManageTranslations"
+      />
 
   <browser:page
       name="connect_translation"
       for="plone.app.multilingual.interfaces.ITranslatable"
       class=".modify.ConnectTranslation"
-      permission="plone.app.multilingual.ManageTranslations"/>
+      permission="plone.app.multilingual.ManageTranslations"
+      />
 
   <browser:page
       name="disconnect_translation"
       for="plone.app.multilingual.interfaces.ITranslatable"
       class=".modify.DisconnectTranslation"
       template="templates/disconnect_translation.pt"
-      permission="plone.app.multilingual.ManageTranslations"/>
+      permission="plone.app.multilingual.ManageTranslations"
+      />
 
   <browser:page
-      for="plone.app.multilingual.interfaces.ITranslatable"
       name="update_language"
+      for="plone.app.multilingual.interfaces.ITranslatable"
       class=".update.update_language_form"
-      permission="cmf.ModifyPortalContent"/>
+      permission="cmf.ModifyPortalContent"
+      />
 
   <browser:page
-      for="plone.app.multilingual.interfaces.ITranslatable"
       name="create_translation"
+      for="plone.app.multilingual.interfaces.ITranslatable"
       class=".translate.TranslationForm"
-      permission="plone.app.multilingual.ManageTranslations"/>
+      permission="plone.app.multilingual.ManageTranslations"
+      />
 
   <!-- Menu for translations on content -->
   <browser:menu
       id="plone_contentmenu_multilingual"
       title="Translate menu - contains translation-related actions"
-      class=".menu.TranslateMenu"/>
+      class=".menu.TranslateMenu"
+      />
   <adapter
+      factory=".menu.TranslateSubMenuItem"
+      provides="plone.app.contentmenu.interfaces.IContentMenuItem"
       for="plone.app.multilingual.interfaces.ITranslatable
            ..interfaces.IPloneAppMultilingualInstalled"
       name="plone.contentmenu.multilingual"
-      factory=".menu.TranslateSubMenuItem"
-      provides="plone.app.contentmenu.interfaces.IContentMenuItem"/>
+      />
 
   <!-- Control panel -->
   <browser:page
-    name="language-controlpanel"
-    for="plone.base.interfaces.IPloneSiteRoot"
-    class=".controlpanel.LanguageControlPanel"
-    permission="plone.app.controlpanel.Language"
-    layer="..interfaces.IPloneAppMultilingualInstalled"
-    />
+      name="language-controlpanel"
+      for="plone.base.interfaces.IPloneSiteRoot"
+      class=".controlpanel.LanguageControlPanel"
+      permission="plone.app.controlpanel.Language"
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Migration Tab -->
   <browser:page
       name="lp-migration"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".controlpanel.MigrationView"
       permission="plone.app.multilingual.ManageTranslations"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <browser:page
       name="multilingual-map"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".controlpanel.multilingualMapView"
       permission="plone.app.multilingual.ManageTranslations"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Notices Viewlets -->
   <browser:viewlet
-      zcml:condition="installed plone.app.controlpanel"
       name="plone.app.multilingual.supported-languages-notice"
       for="plone.base.interfaces.IPloneSiteRoot"
       view="plone.app.controlpanel.interfaces.IPloneControlPanelView"
       manager="plone.app.layout.viewlets.interfaces.IAboveContent"
       class=".viewlets.OneLanguageConfiguredNoticeViewlet"
       template="templates/languages-notice.pt"
+      permission="cmf.ManagePortal"
       layer="..interfaces.IPloneAppMultilingualInstalled"
-      permission="cmf.ManagePortal"/>
+      zcml:condition="installed plone.app.controlpanel"
+      />
   <browser:viewlet
-      zcml:condition="not-installed plone.app.controlpanel"
       name="plone.app.multilingual.supported-languages-notice"
       for="plone.base.interfaces.IPloneSiteRoot"
       view="plone.base.interfaces.controlpanel.IPloneControlPanelView"
       manager="plone.app.layout.viewlets.interfaces.IAboveContent"
       class=".viewlets.OneLanguageConfiguredNoticeViewlet"
       template="templates/languages-notice.pt"
+      permission="cmf.ManagePortal"
       layer="..interfaces.IPloneAppMultilingualInstalled"
-      permission="cmf.ManagePortal"/>
+      zcml:condition="not-installed plone.app.controlpanel"
+      />
 
   <!-- It comes from a translation DX -->
   <browser:viewlet
       name="plone.app.multilingual.add-form-is-translation"
       for="*"
       view="plone.dexterity.browser.add.DefaultAddView"
       manager="plone.app.layout.viewlets.interfaces.IAboveContent"
       class=".viewlets.AddFormIsATranslationViewlet"
       template="templates/add-form-is-translation.pt"
+      permission="zope.Public"
       layer="..interfaces.IPloneAppMultilingualInstalled"
-      permission="zope.Public"/>
+      />
 
   <!-- Alternate language meta tags -->
   <browser:viewlet
       name="plone.app.multilingual.alternate-languages"
       for="plone.app.multilingual.interfaces.ITranslatable"
       manager="plone.app.layout.viewlets.interfaces.IHtmlHead"
       class=".viewlets.AlternateLanguagesViewlet"
       template="templates/alternate-languages.pt"
+      permission="zope.Public"
       layer="..interfaces.IPloneAppMultilingualInstalled"
-      permission="zope.Public"/>
+      />
 
   <!-- Universal Link -->
   <browser:page
       name="multilingual-universal-link"
       for="*"
       class=".helper_views.universal_link"
       permission="zope.Public"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Translation Group -->
   <browser:page
       name="tg"
       for="plone.app.multilingual.interfaces.ITranslatable"
       class=".helper_views.TGView"
       permission="zope.Public"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Selector -->
   <browser:page
       name="multilingual-selector"
       for="plone.app.layout.navigation.interfaces.INavigationRoot"
       class=".helper_views.selector_view"
       permission="zope.Public"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Not Translated Yet -->
   <browser:page
       name="not_translated_yet"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".helper_views.not_translated_yet"
       permission="zope.Public"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Multilingual Map ajax helper -->
   <browser:page
       name="multilingual-map-ajax"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".controlpanel.multilingualMapViewJSON"
       permission="plone.app.multilingual.ManageTranslations"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Default browser view -->
   <browser:view
+      name="language-switcher"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".switcher.LanguageSwitcher"
-      name="language-switcher"
       permission="zope.Public"
+      layer="..interfaces.IPloneAppMultilingualInstalled"
       menu="plone_displayviews"
       title="Root language switcher"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      />
 
   <!-- Viewlet for switching language -->
   <browser:viewlet
       name="plone.app.multilingual.languageselector"
-      template="templates/languageselector.pt"
+      for="plone.app.multilingual.interfaces.ITranslatable"
       manager="plone.app.layout.viewlets.interfaces.IPortalHeader"
       class=".selector.LanguageSelectorViewlet"
+      template="templates/languageselector.pt"
       permission="zope2.View"
-      for="plone.app.multilingual.interfaces.ITranslatable"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- DEXTERITY -->
   <configure zcml:condition="installed plone.dexterity">
 
     <!-- GTranslate Service -->
     <browser:page
-        for="plone.dexterity.interfaces.IDexterityContent"
         name="gtranslation_service"
+        for="plone.dexterity.interfaces.IDexterityContent"
         class=".translate.gtranslation_service_dexterity"
-        permission="cmf.ModifyPortalContent"/>
+        permission="cmf.ModifyPortalContent"
+        />
 
     <!-- Standard add view and form - invoked from ++addtranslation++ traverser -->
     <adapter
-        name="babel_view"
+        factory=".add.DefaultMultilingualAddView"
+        provides="zope.publisher.interfaces.browser.IBrowserPage"
         for="Products.CMFCore.interfaces.IFolderish
              zope.publisher.interfaces.browser.IDefaultBrowserLayer
-        plone.dexterity.interfaces.IDexterityFTI"
-        provides="zope.publisher.interfaces.browser.IBrowserPage"
-        factory=".add.DefaultMultilingualAddView"/>
+             plone.dexterity.interfaces.IDexterityFTI"
+        name="babel_view"
+        />
     <class class=".add.DefaultMultilingualAddView">
       <require
           permission="cmf.AddPortalContent"
-          interface="zope.publisher.interfaces.browser.IBrowserPage"/>
+          interface="zope.publisher.interfaces.browser.IBrowserPage"
+          />
     </class>
 
     <!-- Edit form -->
     <browser:page
-        for="plone.dexterity.interfaces.IDexterityContent"
         name="babel_edit"
+        for="plone.dexterity.interfaces.IDexterityContent"
         class=".edit.DefaultMultilingualEditView"
-        permission="cmf.ModifyPortalContent"/>
+        permission="cmf.ModifyPortalContent"
+        />
 
 
     <!-- Templates for translation fields info visualization via AJAX -->
     <browser:page
-        for="plone.dexterity.interfaces.IDexterityContent"
         name="babel_view"
+        for="plone.dexterity.interfaces.IDexterityContent"
         class=".view.DexterityBabelView"
         template="templates/dx_babel_view.pt"
-        permission="cmf.ModifyPortalContent"/>
+        permission="cmf.ModifyPortalContent"
+        />
 
   </configure>
 
   <browser:page
-      for="*"
       name="babel_utils"
+      for="*"
       class=".utils.BabelUtils"
-      permission="zope2.View"/>
+      permission="zope2.View"
+      />
 
   <!-- Migration Views -->
 
   <!-- Optional initial step - reindex Language index -->
   <browser:page
       name="reindex-language-index"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".migrator.LP2PAMReindexLanguageIndex"
       permission="cmf.ManagePortal"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Step 1 - Relocates the content if needed -->
   <browser:page
       name="relocate-content"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".migrator.moveContentToProperRLF"
       permission="cmf.ManagePortal"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Step 2 - Migrate multilingual catalog info -->
   <browser:page
       name="transfer-lp-catalog"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".migrator.LP2PAMView"
       permission="cmf.ManagePortal"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- Step 3  - Cleanup tasks after migration -->
   <browser:page
       name="after-migration-cleanup"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".migrator.LP2PAMAfterView"
       permission="cmf.ManagePortal"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
   <!-- For manual folder to LRF migration -->
   <browser:page
       name="migrate-to-language-root-folder"
       for="plone.dexterity.interfaces.IDexterityContainer"
       class=".migrator.MigrateFolderToLRFView"
       permission="cmf.ManagePortal"
@@ -298,10 +335,11 @@
 
   <!-- To delete -->
   <browser:page
       name="lp-migration-after"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".controlpanel.MigrationViewAfter"
       permission="plone.app.multilingual.ManageTranslations"
-      layer="..interfaces.IPloneAppMultilingualInstalled"/>
+      layer="..interfaces.IPloneAppMultilingualInstalled"
+      />
 
 </configure>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/controlpanel.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/edit.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/helper_views.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/helper_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from AccessControl.SecurityManagement import getSecurityManager
 from Acquisition import aq_chain
-from borg.localrole.interfaces import IFactoryTempFolder
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.multilingual.browser.selector import addQuery
 from plone.app.multilingual.browser.selector import NOT_TRANSLATED_YET_TEMPLATE
 from plone.app.multilingual.interfaces import ILanguageRootFolder
 from plone.app.multilingual.interfaces import IMultiLanguageExtraOptionsSchema
 from plone.app.multilingual.interfaces import ITG
 from plone.app.multilingual.interfaces import ITranslatable
@@ -147,17 +146,17 @@
         if len(languages) == 0:
             # If there is no results there are no translations
             # we move to portal root
             return self.wrapDestination(root(), postpath=False)
 
         # We are going to see if there is the preferred language translation
         # Otherwise we get the first as context to look for translation
-        prefered = ltool.getPreferredLanguage(self.request)
-        if prefered in languages:
-            context = languages[prefered]
+        preferred = ltool.getPreferredLanguage(self.request)
+        if preferred in languages:
+            context = languages[preferred]
         else:
             context = languages[list(languages.keys())[0]]
 
         checkPermission = getSecurityManager().checkPermission
         chain = self.getParentChain(context)
         for item in chain:
             if ISiteRoot.providedBy(item) and not ILanguageRootFolder.providedBy(item):
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/images/gtranslate.png` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/images/gtranslate.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/interfaces.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/babel_helper.js` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/babel_helper.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -49,15 +49,15 @@
             } else {
                 original_padding = shift;
             }
 
             // The next calculation of padding is necessary if both elements
             // have to be shifted down.
             if (!first && original.prev().is(":visible")) {
-                // Calulate distance between bottom of prev element and top
+                // Calculate distance between bottom of prev element and top
                 // of current element. add Padding. If > 0, add to more_padding
                 new_distance = distance(original.prev(), original);
                 new_distance += original_padding;
                 if (new_distance < padding) {
                     more_padding += padding - new_distance;
                 }
                 new_distance = distance(destination.prev(), destination);
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/jit-yc.js` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/jit-yc.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/javascript/mmap_helper.js` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/javascript/mmap_helper.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -132,16 +132,16 @@
         //is clicked and its subtree has a smaller depth
         //than the one specified by the levelsToShow parameter.
         //In that case a subtree is requested and is added to the dataset.
         //This method is asynchronous, so you can make an Ajax request for that
         //subtree and then handle it to the onComplete callback.
         //Here we just use a client-side tree generator (the getTree function).
         request: function(nodeId, level, onComplete) {
-            var ans = getTree(nodeId, level);
-            onComplete.onComplete(nodeId, ans);
+            var answer = getTree(nodeId, level);
+            onComplete.onComplete(nodeId, answer);
         },
 
         onBeforeCompute: function(node) {
             Log.write("loading " + node.name);
         },
 
         onAfterCompute: function() {
@@ -196,15 +196,15 @@
                 delete node.data.$color;
             }
         },
 
         //This method is called right before plotting
         //an edge. It's useful for changing an individual edge
         //style properties before plotting it.
-        //Edge data proprties prefixed with a dollar sign will
+        //Edge data properties prefixed with a dollar sign will
         //override the Edge global style properties.
         onBeforePlotLine: function(adj) {
             if (adj.nodeFrom.selected && adj.nodeTo.selected) {
                 adj.data.$color = "#23A4FF";
                 adj.data.$lineWidth = 3;
             } else {
                 delete adj.data.$color;
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/menu.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/menu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from plone.app.multilingual.interfaces import ILanguageRootFolder
 from plone.app.multilingual.interfaces import IMultiLanguageExtraOptionsSchema
 from plone.app.multilingual.interfaces import IPloneAppMultilingualInstalled
 from plone.app.multilingual.interfaces import ITG
 from plone.app.multilingual.interfaces import ITranslatable
 from plone.app.multilingual.interfaces import LANGUAGE_INDEPENDENT
 from plone.app.multilingual.permissions import ManageTranslations
+from plone.base.defaultpage import is_default_page
 from plone.base.interfaces import ILanguage
+from plone.base.utils import safe_text
 from plone.memoize import view
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.defaultpage import is_default_page
-from plone.base.utils import safe_text
 from zope.browsermenu.menu import BrowserMenu
 from zope.browsermenu.menu import BrowserSubMenuItem
 from zope.component import getUtility
 from zope.component.hooks import getSite
 from zope.interface import implementer
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/migrator.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/migrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,14 @@
     from plone.dexterity.interfaces import IDexterityContent
 except ImportError:
 
     class IDexterityContent(Interface):
         pass
 
 
-try:
-    from Products.Archetypes.interfaces import IBaseObject
-except ImportError:
-
-    class IBaseObject(Interface):
-        pass
-
-
 with warnings.catch_warnings():
     warnings.filterwarnings(
         "ignore",
         message="LanguageRootFolder: LanguageRootFolders should be migrate "
         "to DexterityContainers",
     )
     from plone.app.multilingual.content.lrf import LanguageRootFolder
@@ -141,17 +133,15 @@
 
     template = ViewPageTemplateFile("templates/relocate-results.pt")
     stepinfo = _("Relocate content to the proper root language folder")
     blacklist = list()
 
     def findContent(self, content, depth):
         # only handle portal content
-        if not IDexterityContent.providedBy(content) and not IBaseObject.providedBy(
-            content
-        ):
+        if not IDexterityContent.providedBy(content):
             logger.warning(
                 "SKIP non-portal content %s (%s)"
                 % (content.absolute_url(), content.meta_type)
             )
             return
         if (
             hasattr(aq_base(content), "objectIds")
@@ -212,21 +202,21 @@
             if depth != []:
                 for content in depth:
                     parent = aq_parent(content)
                     target_folder = self.searchNearestTranslatedParent(content)
                     # Test if the id already exist previously
 
                     try:
-                        cutted = parent.manage_cutObjects(content.getId())
+                        obj_cut = parent.manage_cutObjects(content.getId())
                     except ResourceLockedError:
                         lockable = ILockable(content)
                         lockable.unlock()
-                        cutted = parent.manage_cutObjects(content.getId())
+                        obj_cut = parent.manage_cutObjects(content.getId())
                     try:
-                        target_folder.manage_pasteObjects(cutted)
+                        target_folder.manage_pasteObjects(obj_cut)
                         info_str = "Step 2: Moved object {} to folder {}".format(
                             "/".join(content.getPhysicalPath()),
                             "/".join(target_folder.getPhysicalPath()),
                         )
                         log = logger.info
                     except Exception as err:
                         info_str = (
@@ -273,22 +263,22 @@
             )
 
             for brain in objects:
                 if brain.id != lang:
                     old_path = brain.getPath()
 
                     try:
-                        cutted = self.context.manage_cutObjects(brain.id)
+                        obj_cut = self.context.manage_cutObjects(brain.id)
                     except ResourceLockedError:
                         content = brain.getObject()
                         lockable = ILockable(content)
                         lockable.unlock()
-                        cutted = self.context.manage_cutObjects(brain.id)
+                        obj_cut = self.context.manage_cutObjects(brain.id)
                     try:
-                        folder.manage_pasteObjects(cutted)
+                        folder.manage_pasteObjects(obj_cut)
                         info_str = "Moved object %s to language root folder " "%s" % (
                             old_path,
                             lang,
                         )
                         log = logger.info
                     except Exception as err:
                         info_str = (
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/modify.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/selector.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,11 +106,11 @@
                 query_extras["post_path"] = post_path
             site = getSite()
             data["url"] = addQuery(
                 self.request,
                 site.absolute_url().rstrip("/")
                 + "/@@multilingual-selector/%s/%s"
                 % (translation_group, lang_info["code"]),
-                **query_extras
+                **query_extras,
             )
             results.append(data)
         return results
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/setup.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.multilingual import _
 from plone.app.multilingual.interfaces import ITranslatable
 from plone.app.multilingual.interfaces import ITranslationManager
 from plone.app.multilingual.interfaces import LANGUAGE_INDEPENDENT
 from plone.app.multilingual.subscriber import set_recursive_language
 from plone.base.interfaces import ILanguage
+from plone.base.utils import unrestricted_construct_instance
 from plone.dexterity.interfaces import IDexterityFTI
 from plone.i18n.locales.languages import _combinedlanguagelist
 from plone.i18n.locales.languages import _languagelist
 from Products.CMFCore.utils import getToolByName
-from plone.base.utils import unrestricted_construct_instance
 from Products.Five import BrowserView
 from zope.component.hooks import getSite
 from zope.event import notify
 from zope.i18n import translate
 from zope.interface import alsoProvides
 from zope.lifecycleevent import modified
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/stylesheet/multilingual.css` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/stylesheet/multilingual.css`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/switcher.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/switcher.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 00000000: 3c64 6976 2063 6c61 7373 3d22 636f 6e74  <div class="cont
-00000010: 6169 6e65 7222 3e0a 2020 2020 3c64 6976  ainer">.    <div
-00000020: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-00000030: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000040: 3d22 616c 6572 7420 616c 6572 742d 696e  ="alert alert-in
-00000050: 666f 2063 6f6c 2d31 3222 2072 6f6c 653d  fo col-12" role=
-00000060: 2261 6c65 7274 223e 0a20 2020 2020 2020  "alert">.       
-00000070: 2020 2020 203c 7374 726f 6e67 2069 3138       <strong i18
-00000080: 6e3a 7472 616e 736c 6174 653d 2222 2069  n:translate="" i
-00000090: 3138 6e3a 646f 6d61 696e 3d22 706c 6f6e  18n:domain="plon
-000000a0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
-000000b0: 2020 2020 496e 666f 0a20 2020 2020 2020      Info.       
-000000c0: 2020 2020 203c 2f73 7472 6f6e 673e 0a20       </strong>. 
-000000d0: 2020 2020 2020 2020 2020 203c 7461 6c3a             <tal:
-000000e0: 626c 6f63 6b20 6931 386e 3a64 6f6d 6169  block i18n:domai
-000000f0: 6e3d 2270 6c6f 6e65 220a 2020 2020 2020  n="plone".      
-00000100: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000110: 3138 6e3a 7472 616e 736c 6174 653d 2261  18n:translate="a
-00000120: 6464 2d66 6f72 6d2d 6973 2d74 7261 6e73  dd-form-is-trans
-00000130: 6c61 7469 6f6e 223e 0a20 2020 2020 2020  lation">.       
-00000140: 2020 2020 2020 2020 2054 6869 7320 6f62           This ob
-00000150: 6a65 6374 2069 7320 676f 696e 6720 746f  ject is going to
-00000160: 2062 6520 6120 7472 616e 736c 6174 696f   be a translatio
-00000170: 6e20 746f 0a20 2020 2020 2020 2020 2020  n to.           
-00000180: 2020 2020 203c 7370 616e 2069 3138 6e3a       <span i18n:
-00000190: 6e61 6d65 3d22 6c61 6e67 7561 6765 2220  name="language" 
-000001a0: 7461 6c3a 7265 706c 6163 653d 2270 7974  tal:replace="pyt
-000001b0: 686f 6e3a 7669 6577 2e6c 616e 6775 6167  hon:view.languag
-000001c0: 655f 6e61 6d65 2876 6965 772e 6c61 6e67  e_name(view.lang
-000001d0: 7561 6765 2829 2922 3e3c 2f73 7061 6e3e  uage())"></span>
-000001e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000001f0: 2066 726f 6d3a 0a20 2020 2020 2020 2020   from:.         
-00000200: 2020 203c 2f74 616c 3a62 6c6f 636b 3e0a     </tal:block>.
-00000210: 2020 2020 2020 2020 2020 2020 3c75 6c3e              <ul>
-00000220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000230: 203c 6c69 2074 616c 3a72 6570 6561 743d   <li tal:repeat=
-00000240: 226f 7269 6769 6e20 7669 6577 2f6f 7269  "origin view/ori
-00000250: 6769 6e22 3e0a 2020 2020 2020 2020 2020  gin">.          
-00000260: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
-00000270: 7461 6c3a 636f 6e74 656e 743d 2270 7974  tal:content="pyt
-00000280: 686f 6e3a 7669 6577 2e6c 616e 6775 6167  hon:view.languag
-00000290: 655f 6e61 6d65 286f 7269 6769 6e2e 4c61  e_name(origin.La
-000002a0: 6e67 7561 6765 2922 3e3c 2f73 7061 6e3e  nguage)"></span>
-000002b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000002c0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
-000002d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000002e0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-000002f0: 6c69 6e6b 2d6f 7665 726c 6179 2220 7461  link-overlay" ta
-00000300: 6c3a 6174 7472 6962 7574 6573 3d22 6872  l:attributes="hr
-00000310: 6566 206f 7269 6769 6e2f 6765 7455 524c  ef origin/getURL
-00000320: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000330: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00000340: 2074 616c 3a63 6f6e 7465 6e74 3d22 6f72   tal:content="or
-00000350: 6967 696e 2f54 6974 6c65 223e 3c2f 7370  igin/Title"></sp
-00000360: 616e 3e3c 2f61 3e3c 2f6c 693e 0a20 2020  an></a></li>.   
-00000370: 2020 2020 2020 2020 203c 2f75 6c3e 0a20           </ul>. 
-00000380: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00000390: 2069 3138 6e3a 646f 6d61 696e 3d22 706c   i18n:domain="pl
-000003a0: 6f6e 6522 2069 3138 6e3a 7472 616e 736c  one" i18n:transl
-000003b0: 6174 653d 2263 7265 6174 652d 6f62 6a65  ate="create-obje
-000003c0: 6374 2d77 6974 686f 7574 2d74 7261 6e73  ct-without-trans
-000003d0: 6c61 7469 6f6e 223e 0a20 2020 2020 2049  lation">.      I
-000003e0: 6620 796f 7520 7761 6e74 2074 6f20 6372  f you want to cr
-000003f0: 6561 7465 2074 6869 7320 6f62 6a65 6374  eate this object
-00000400: 2077 6974 686f 7574 2062 6569 6e67 2061   without being a
-00000410: 2074 7261 6e73 6c61 7469 6f6e 2070 7265   translation pre
-00000420: 7373 0a20 2020 2020 203c 6120 6872 6566  ss.      <a href
-00000430: 3d22 2322 0a20 2020 2020 2020 2020 636c  ="#".         cl
-00000440: 6173 733d 226c 696e 6b2d 6f76 6572 6c61  ass="link-overla
-00000450: 7922 2069 3138 6e3a 6e61 6d65 3d22 7572  y" i18n:name="ur
-00000460: 6c22 2074 616c 3a61 7474 7269 6275 7465  l" tal:attribute
-00000470: 733d 2268 7265 6620 7669 6577 2f72 6574  s="href view/ret
-00000480: 7572 6e55 524c 2220 6931 386e 3a74 7261  urnURL" i18n:tra
-00000490: 6e73 6c61 7465 3d22 223e 6865 7265 3c2f  nslate="">here</
-000004a0: 613e 0a20 2020 203c 2f73 7061 6e3e 0a20  a>.    </span>. 
-000004b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000004c0: 2020 3c2f 6469 763e 0a3c 2f64 6976 3e0a    </div>.</div>.
+00000010: 6169 6e65 7222 3e0a 2020 3c64 6976 2063  ainer">.  <div c
+00000020: 6c61 7373 3d22 726f 7722 3e0a 2020 2020  lass="row">.    
+00000030: 3c64 6976 2063 6c61 7373 3d22 616c 6572  <div class="aler
+00000040: 7420 616c 6572 742d 696e 666f 2063 6f6c  t alert-info col
+00000050: 2d31 3222 0a20 2020 2020 2020 2020 726f  -12".         ro
+00000060: 6c65 3d22 616c 6572 7422 0a20 2020 203e  le="alert".    >
+00000070: 0a20 2020 2020 203c 7374 726f 6e67 2069  .      <strong i
+00000080: 3138 6e3a 646f 6d61 696e 3d22 706c 6f6e  18n:domain="plon
+00000090: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+000000a0: 2069 3138 6e3a 7472 616e 736c 6174 653d   i18n:translate=
+000000b0: 2222 0a20 2020 2020 203e 0a20 2020 2020  "".      >.     
+000000c0: 2020 2020 2020 2020 2020 2049 6e66 6f0a             Info.
+000000d0: 2020 2020 2020 3c2f 7374 726f 6e67 3e0a        </strong>.
+000000e0: 2020 2020 2020 3c74 616c 3a62 6c6f 636b        <tal:block
+000000f0: 2069 3138 6e3a 646f 6d61 696e 3d22 706c   i18n:domain="pl
+00000100: 6f6e 6522 0a20 2020 2020 2020 2020 2020  one".           
+00000110: 2020 2020 2020 6931 386e 3a74 7261 6e73        i18n:trans
+00000120: 6c61 7465 3d22 6164 642d 666f 726d 2d69  late="add-form-i
+00000130: 732d 7472 616e 736c 6174 696f 6e22 0a20  s-translation". 
+00000140: 2020 2020 203e 0a20 2020 2020 2020 2020       >.         
+00000150: 2020 2020 2020 2054 6869 7320 6f62 6a65         This obje
+00000160: 6374 2069 7320 676f 696e 6720 746f 2062  ct is going to b
+00000170: 6520 6120 7472 616e 736c 6174 696f 6e20  e a translation 
+00000180: 746f 0a20 2020 2020 2020 203c 7370 616e  to.        <span
+00000190: 2074 616c 3a72 6570 6c61 6365 3d22 7079   tal:replace="py
+000001a0: 7468 6f6e 3a76 6965 772e 6c61 6e67 7561  thon:view.langua
+000001b0: 6765 5f6e 616d 6528 7669 6577 2e6c 616e  ge_name(view.lan
+000001c0: 6775 6167 6528 2929 220a 2020 2020 2020  guage())".      
+000001d0: 2020 2020 2020 2020 6931 386e 3a6e 616d          i18n:nam
+000001e0: 653d 226c 616e 6775 6167 6522 0a20 2020  e="language".   
+000001f0: 2020 2020 203e 3c2f 7370 616e 3e0a 2020       ></span>.  
+00000200: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00000210: 6f6d 3a0a 2020 2020 2020 3c2f 7461 6c3a  om:.      </tal:
+00000220: 626c 6f63 6b3e 0a20 2020 2020 203c 756c  block>.      <ul
+00000230: 3e0a 2020 2020 2020 2020 3c6c 6920 7461  >.        <li ta
+00000240: 6c3a 7265 7065 6174 3d22 6f72 6967 696e  l:repeat="origin
+00000250: 2076 6965 772f 6f72 6967 696e 223e 0a20   view/origin">. 
+00000260: 2020 2020 2020 2020 203c 7370 616e 2074           <span t
+00000270: 616c 3a63 6f6e 7465 6e74 3d22 7079 7468  al:content="pyth
+00000280: 6f6e 3a76 6965 772e 6c61 6e67 7561 6765  on:view.language
+00000290: 5f6e 616d 6528 6f72 6967 696e 2e4c 616e  _name(origin.Lan
+000002a0: 6775 6167 6529 223e 3c2f 7370 616e 3e3a  guage)"></span>:
+000002b0: 0a20 2020 2020 2020 2020 203c 6120 636c  .          <a cl
+000002c0: 6173 733d 226c 696e 6b2d 6f76 6572 6c61  ass="link-overla
+000002d0: 7922 0a20 2020 2020 2020 2020 2020 2020  y".             
+000002e0: 6872 6566 3d22 2322 0a20 2020 2020 2020  href="#".       
+000002f0: 2020 2020 2020 7461 6c3a 6174 7472 6962        tal:attrib
+00000300: 7574 6573 3d22 0a20 2020 2020 2020 2020  utes=".         
+00000310: 2020 2020 2020 6872 6566 206f 7269 6769        href origi
+00000320: 6e2f 6765 7455 524c 3b0a 2020 2020 2020  n/getURL;.      
+00000330: 2020 2020 2020 2022 0a20 2020 2020 2020         ".       
+00000340: 2020 203e 0a20 2020 2020 2020 2020 2020     >.           
+00000350: 203c 7370 616e 2074 616c 3a63 6f6e 7465   <span tal:conte
+00000360: 6e74 3d22 6f72 6967 696e 2f54 6974 6c65  nt="origin/Title
+00000370: 223e 3c2f 7370 616e 3e3c 2f61 3e3c 2f6c  "></span></a></l
+00000380: 693e 0a20 2020 2020 203c 2f75 6c3e 0a20  i>.      </ul>. 
+00000390: 2020 2020 203c 7370 616e 2069 3138 6e3a       <span i18n:
+000003a0: 646f 6d61 696e 3d22 706c 6f6e 6522 0a20  domain="plone". 
+000003b0: 2020 2020 2020 2020 2020 2069 3138 6e3a             i18n:
+000003c0: 7472 616e 736c 6174 653d 2263 7265 6174  translate="creat
+000003d0: 652d 6f62 6a65 6374 2d77 6974 686f 7574  e-object-without
+000003e0: 2d74 7261 6e73 6c61 7469 6f6e 220a 2020  -translation".  
+000003f0: 2020 2020 3e0a 2020 2020 2020 4966 2079      >.      If y
+00000400: 6f75 2077 616e 7420 746f 2063 7265 6174  ou want to creat
+00000410: 6520 7468 6973 206f 626a 6563 7420 7769  e this object wi
+00000420: 7468 6f75 7420 6265 696e 6720 6120 7472  thout being a tr
+00000430: 616e 736c 6174 696f 6e20 7072 6573 730a  anslation press.
+00000440: 2020 2020 2020 2020 3c61 2063 6c61 7373          <a class
+00000450: 3d22 6c69 6e6b 2d6f 7665 726c 6179 220a  ="link-overlay".
+00000460: 2020 2020 2020 2020 2020 2068 7265 663d             href=
+00000470: 2223 220a 2020 2020 2020 2020 2020 2074  "#".           t
+00000480: 616c 3a61 7474 7269 6275 7465 733d 220a  al:attributes=".
+00000490: 2020 2020 2020 2020 2020 2020 2068 7265               hre
+000004a0: 6620 7669 6577 2f72 6574 7572 6e55 524c  f view/returnURL
+000004b0: 3b0a 2020 2020 2020 2020 2020 2022 0a20  ;.           ". 
+000004c0: 2020 2020 2020 2020 2020 6931 386e 3a6e            i18n:n
+000004d0: 616d 653d 2275 726c 220a 2020 2020 2020  ame="url".      
+000004e0: 2020 2020 2069 3138 6e3a 7472 616e 736c       i18n:transl
+000004f0: 6174 653d 2222 0a20 2020 2020 2020 203e  ate="".        >
+00000500: 6865 7265 3c2f 613e 0a20 2020 2020 203c  here</a>.      <
+00000510: 2f73 7061 6e3e 0a20 2020 203c 2f64 6976  /span>.    </div
+00000520: 3e0a 2020 3c2f 6469 763e 0a3c 2f64 6976  >.  </div>.</div
+00000530: 3e0a                                     >.
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/cleanup.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/cleanup.pt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/prefs_main_template/macros/master"
-    i18n:domain="plone">
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
 
-<body>
+  <body>
 
-<metal:block metal:fill-slot="prefs_configlet_main">
+    <metal:block metal:fill-slot="prefs_configlet_main">
 
-<script type="text/javascript">
+      <script type="text/javascript">
 (function($) {
 
     $().ready(function() {
         $('.formControls input #resetrelations').click(function (event) {
           event.preventDefault();
           $.get('@@migration-view-after', function(data) {
             $('.results').html(data)
@@ -25,87 +27,105 @@
           $.get('@@relocateContentByLanguage', function(data) {
             $('.results').html(data)
           });
         });
     });
 
 })(jQuery);
-</script>
+      </script>
 
 
-    <div i18n:domain="plone">
-        <ul class="contentViews" id="content-views">
+      <div i18n:domain="plone">
+        <ul class="contentViews"
+            id="content-views"
+        >
           <li>
             <a href=""
-               tal:attributes="href string:${portal_url}/@@language-controlpanel"
-               i18n:translate="label_general">General</a>
+               tal:attributes="
+                 href string:${portal_url}/@@language-controlpanel;
+               "
+               i18n:translate="label_general"
+            >General</a>
           </li>
           <li>
             <a href=""
-               tal:attributes="href string:${portal_url}/@@multilingual-map"
-               i18n:translate="label_translation_map">Translation Map</a>
+               tal:attributes="
+                 href string:${portal_url}/@@multilingual-map;
+               "
+               i18n:translate="label_translation_map"
+            >Translation Map</a>
           </li>
           <li class="selected">
             <a href=""
-              tal:attributes="href string:${portal_url}/@@lp-migration-after"
-              i18n:translate="label_cleanup">Cleanup actions</a>
+               tal:attributes="
+                 href string:${portal_url}/@@lp-migration-after;
+               "
+               i18n:translate="label_cleanup"
+            >Cleanup actions</a>
           </li>
         </ul>
-    </div>
+      </div>
 
 
-        <div metal:use-macro="context/global_statusmessage/macros/portal_message">
+      <div metal:use-macro="context/global_statusmessage/macros/portal_message">
         Portal status message
-        </div>
-
-        <div class="content-core">
+      </div>
 
-            <h1 class="documentFirstHeading"
-                i18n:domain="plone"
-                i18n:translate="heading_migration_after">Products.LinguaPlone After Migration</h1>
+      <div class="content-core">
 
-            <p i18n:translate="description_migrate_after"
-              i18n:domain="plone">
+        <h1 class="documentFirstHeading"
+            i18n:domain="plone"
+            i18n:translate="heading_migration_after"
+        >Products.LinguaPlone After Migration</h1>
+
+        <p i18n:domain="plone"
+           i18n:translate="description_migrate_after"
+        >
                 It can happen that there are relations left that contain
                 LinguaPlone relations. By executing this step, the catalog
                 gets reset and rebuilt. It CAN happen that things go bad.
-                In that case relations get lost. It is therefor important that
+                In that case relations get lost. It is therefore important that
                 you have a backup!
-            </p>
+        </p>
+
+        <form method="post"
+              name="cleanup"
+              tal:attributes="
+                action request/URL;
+              "
+        >
+
+          <div class="formControls">
+
+            <input class="destructive"
+                   id="resetrelations"
+                   name="form.button.Cleanup"
+                   type="submit"
+                   value="Cleanup"
+                   i18n:attributes="value"
+            />
+            <label i18n:translate="label_catalog_reload">Catalog reload</label>
+
+            <span class="clearfix"></span>
+            <input class="destructive"
+                   id="move"
+                   name="form.button.Move"
+                   type="submit"
+                   value="Move"
+                   i18n:attributes="value"
+            />
+            <label i18n:translate="label_move_content_to_languages">Move content to its corresponding language root folder</label>
+          </div>
 
-            <form name="cleanup" tal:attributes="action request/URL" method="post">
+          <input tal:replace="structure context/@@authenticator/authenticator" />
 
-                <div class="formControls">
+        </form>
 
-                  <input
-                        id="resetrelations"
-                        type="submit"
-                        name="form.button.Cleanup"
-                        class="destructive"
-                        value="Cleanup"
-                        i18n:attributes="value" />
-                  <label i18n:translate="label_catalog_reload">Catalog reload</label>
-
-                  <span class="clearfix" />
-                  <input
-                        id="move"
-                        type="submit"
-                        name="form.button.Move"
-                        class="destructive"
-                        value="Move"
-                        i18n:attributes="value" />
-                  <label i18n:translate="label_move_content_to_languages">Move content to its corresponding language root folder</label>
-                </div>
-
-                <input tal:replace="structure context/@@authenticator/authenticator" />
-
-            </form>
-
-            <div class="results">
-              <!-- The migration results -->
-            </div>
+        <div class="results">
+          <!-- The migration results -->
         </div>
+      </div>
 
-</metal:block>
+    </metal:block>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/cleanup_results.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/cleanup_results.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/prefs_main_template/macros/master"
-    i18n:domain="plone">
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
 
-<body>
+  <body>
 
-<metal:prefs fill-slot="prefs_configlet_main">
+    <metal:prefs fill-slot="prefs_configlet_main">
 
-<div id="results">
+      <div id="results">
 
-<div class="resultInfo">
-    <h2 i18n:translate=""
-        tal:content="view/stepinfo">
+        <div class="resultInfo">
+          <h2 tal:content="view/stepinfo"
+              i18n:translate=""
+          >
         After migration relation cleanup
-    </h2>
+          </h2>
 
-    <span i18n:translate="label_total_relations">
+          <span i18n:translate="label_total_relations">
         Number of relations touched:
-    </span>
-    <span tal:content="view/total">Number of objects</span>
-</div>
-<div tal:condition="view/bad">
-    <span i18n:translate="label_bad_relations">
+          </span>
+          <span tal:content="view/total">Number of objects</span>
+        </div>
+        <div tal:condition="view/bad">
+          <span i18n:translate="label_bad_relations">
         Unfortunately a number of relations could not be translated and
         are lost!
         here is some debug information:
-    </span>
-    <span tal:repeat="one_bad view/bad" tal:content="one_bad">
+          </span>
+          <span tal:repeat="one_bad view/bad"
+                tal:content="one_bad"
+          >
         Bad relation
-    </span>
-</div>
-</div>
-</metal:prefs>
-</body>
+          </span>
+        </div>
+      </div>
+    </metal:prefs>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/controlpanel.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/controlpanel.pt`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,67 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="here/prefs_main_template/macros/master"
-      i18n:domain="plone">
-
-<body>
-
-<tal:main metal:fill-slot="prefs_configlet_main">
-
-  <header>
-    <a id="setup-link" class="link-parent"
-       tal:attributes="href string:$portal_url/@@overview-controlpanel"
-       i18n:translate="">
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <body>
+
+    <tal:main metal:fill-slot="prefs_configlet_main">
+
+      <header>
+        <a class="link-parent"
+           id="setup-link"
+           tal:attributes="
+             href string:$portal_url/@@overview-controlpanel;
+           "
+           i18n:translate=""
+        >
         Site Setup
-    </a>
+        </a>
 
-    <h1 class="documentFirstHeading" tal:content="view/label">View Title</h1>
+        <h1 class="documentFirstHeading"
+            tal:content="view/label"
+        >View Title</h1>
 
-    <div metal:use-macro="context/global_statusmessage/macros/portal_message">
+        <div metal:use-macro="context/global_statusmessage/macros/portal_message">
       Portal status message
-    </div>
-  </header>
-  <div id="content-core">
-      <div id="layout-contents">
-          <span tal:replace="structure view/contents" />
-      </div>
-      <div class="mt-4">
-        <p i18n:translate="">
+        </div>
+      </header>
+      <div id="content-core">
+        <div id="layout-contents">
+          <span tal:replace="structure view/contents"></span>
+        </div>
+        <div class="mt-4">
+          <p i18n:translate="">
           The
-          <a i18n:name="url" i18n:translate="" tal:attributes="href string:${context/absolute_url}/multilingual-map">multilingual map view
-          </a>
+            <a tal:attributes="
+                 href string:${context/absolute_url}/multilingual-map;
+               "
+               i18n:name="url"
+               i18n:translate=""
+            >multilingual map view
+            </a>
           allows you to view in a graphical manner the already translated items and its relations.
-        </p>
-        <p i18n:translate=""
-            tal:condition="view/isLPinstalled">
+          </p>
+          <p tal:condition="view/isLPinstalled"
+             i18n:translate=""
+          >
           In case you want to migrate from Products.LinguaPlone access to the
-          <a i18n:name="url" i18n:translate="" tal:attributes="href string:${context/absolute_url}/lp-migration">migration procedure.
-          </a>
-        </p>
+            <a tal:attributes="
+                 href string:${context/absolute_url}/lp-migration;
+               "
+               i18n:name="url"
+               i18n:translate=""
+            >migration procedure.
+            </a>
+          </p>
+        </div>
       </div>
-  </div>
 
-</tal:main>
-</body>
+    </tal:main>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/dexterity_edit.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/dexterity_edit.pt`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,88 @@
-<div class='row' id='babel-edit'
-      xmlns="http://www.w3.org/1999/xhtml"
-      xml:lang="en"
-      lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
-      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone"
-      tal:define="pamutils context/@@babel_utils;">
+<div xmlns="http://www.w3.org/1999/xhtml"
+     xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+     xmlns:metal="http://xml.zope.org/namespaces/metal"
+     xmlns:tal="http://xml.zope.org/namespaces/tal"
+     class="row"
+     id="babel-edit"
+     lang="en"
+     xml:lang="en"
+     tal:define="
+       pamutils context/@@babel_utils;
+     "
+     i18n:domain="plone"
+>
 
-    <script src="++resource++plone.app.multilingual.javascript/babel_helper.js"></script>
-    <input type="hidden" id="url_translate" value="" tal:attributes="value context/absolute_url"/>
-    <input type="hidden" id="gtranslate_service_available" value="" tal:attributes="value pamutils/gtenabled"/>
+  <script src="++resource++plone.app.multilingual.javascript/babel_helper.js"></script>
+  <input id="url_translate"
+         type="hidden"
+         value=""
+         tal:attributes="
+           value context/absolute_url;
+         "
+  />
+  <input id="gtranslate_service_available"
+         type="hidden"
+         value=""
+         tal:attributes="
+           value pamutils/gtenabled;
+         "
+  />
 
-    <div class='col-md-6'>
-        <h2 i18n:translate="heading_available_translations">Available translations for this content</h2>
-        <div id="trans-selector"
-             tal:define="languages pamutils/translated_languages;
-             max_nr_of_buttons view/max_nr_of_buttons">
-          <div class="btn-group"
-            tal:define="use_dropdown python:max_nr_of_buttons and max_nr_of_buttons < len(languages)">
-            <select name="language_selector" tal:condition="use_dropdown">
-              <option tal:repeat="lang languages"
-                tal:attributes="value string:${lang/obj/absolute_url}/babel_view;
-                                      selected python:lang['isDefault'] and 'selected' or '';
-                                      id string:selection-${lang/code}"
-                tal:content="lang/info/native|lang/info/name">Language</option>
-            </select>
-            <tal:block repeat="lang languages" tal:condition="not:use_dropdown">
-              <button class="btn"
-                      tal:attributes="data-url string:${lang/obj/absolute_url}/babel_view;
-                                      class python:lang['isDefault'] and 'btn active' or 'btn';
-                                      name string:button-${lang/info/name}"
-                      tal:content="lang/info/native|lang/info/name">Language</button>
-            </tal:block>
-          </div>
-        </div>
-        <div id="frame-content" i18n:translate="label_translations_should_be_here">
+  <div class="col-md-6">
+    <h2 i18n:translate="heading_available_translations">Available translations for this content</h2>
+    <div id="trans-selector"
+         tal:define="
+           languages pamutils/translated_languages;
+           max_nr_of_buttons view/max_nr_of_buttons;
+         "
+    >
+      <div class="btn-group"
+           tal:define="
+             use_dropdown python:max_nr_of_buttons and max_nr_of_buttons &lt; len(languages);
+           "
+      >
+        <select name="language_selector"
+                tal:condition="use_dropdown"
+        >
+          <option tal:repeat="lang languages"
+                  tal:content="lang/info/native|lang/info/name"
+                  tal:attributes="
+                    value string:${lang/obj/absolute_url}/babel_view;
+                    selected python:lang['isDefault'] and 'selected' or '';
+                    id string:selection-${lang/code};
+                  "
+          >Language</option>
+        </select>
+        <tal:block tal:condition="not:use_dropdown"
+                   repeat="lang languages"
+        >
+          <button class="btn"
+                  tal:content="lang/info/native|lang/info/name"
+                  tal:attributes="
+                    data-url string:${lang/obj/absolute_url}/babel_view;
+                    class python:lang['isDefault'] and 'btn active' or 'btn';
+                    name string:button-${lang/info/name};
+                  "
+          >Language</button>
+        </tal:block>
+      </div>
+    </div>
+    <div id="frame-content"
+         i18n:translate="label_translations_should_be_here"
+    >
             The available translations for this content should be here
-        </div>
     </div>
-    <div class='col-md-6'>
+  </div>
+  <div class="col-md-6">
     <div id="header-translation">
-        <h2 i18n:translate="translation_to">Translation to <span i18n:name="language" tal:content="pamutils/current_language_name" tal:omit-tag="">es</span></h2>
+      <h2 i18n:translate="translation_to">Translation to
+        <span tal:content="pamutils/current_language_name"
+              tal:omit-tag=""
+              i18n:name="language"
+        >es</span></h2>
     </div>
     <div id="form-target">
       <tal:block content="structure view/babel_content">Content edit</tal:block>
     </div>
-    </div>
+  </div>
 </div>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/disconnect_translation.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/disconnect_translation.pt`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,61 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
       metal:use-macro="context/main_template/macros/master"
-      i18n:domain="plone">
-
-    <metal:block fill-slot="top_slot"
-                 tal:define="dummy python:request.set('disable_border',1)" />
-
-    <body>
-
-        <metal:main fill-slot="main">
-
-        <h1 class="documentFirstHeading"
-            i18n:translate="alert_disconnect_translation">
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <metal:block fill-slot="top_slot"
+               tal:define="
+                 dummy python:request.set('disable_border',1);
+               "
+  />
+
+  <body>
+
+    <metal:main fill-slot="main">
+
+      <h1 class="documentFirstHeading"
+          i18n:translate="alert_disconnect_translation"
+      >
             Disconnect translation
-        </h1>
+      </h1>
 
-        <div id="content-core">
+      <div id="content-core">
 
-            <form action="" tal:attributes="action string:${context/absolute_url}/disconnect_translation">
-                <p i18n:translate="confirm_translation_disconnect">Do you really want to disconnect this translation?</p>
-                <input type="hidden" name="came_from" tal:attributes="value context/REQUEST/form/came_from">
-                <input type="hidden" name="language" tal:attributes="value context/REQUEST/form/language">
-                <input type="hidden" name="submitted" value="1">
-                <span tal:replace="structure context/@@authenticator/authenticator"/>
-                <button type="submit" i18n:translate="label_disconnect">Disconnect</button>
-            </form>
+        <form action=""
+              tal:attributes="
+                action string:${context/absolute_url}/disconnect_translation;
+              "
+        >
+          <p i18n:translate="confirm_translation_disconnect">Do you really want to disconnect this translation?</p>
+          <input name="came_from"
+                 type="hidden"
+                 tal:attributes="
+                   value context/REQUEST/form/came_from;
+                 "
+          />
+          <input name="language"
+                 type="hidden"
+                 tal:attributes="
+                   value context/REQUEST/form/language;
+                 "
+          />
+          <input name="submitted"
+                 type="hidden"
+                 value="1"
+          />
+          <span tal:replace="structure context/@@authenticator/authenticator"></span>
+          <button type="submit"
+                  i18n:translate="label_disconnect"
+          >Disconnect</button>
+        </form>
 
-        </div>
+      </div>
 
-        </metal:main>
-    </body>
+    </metal:main>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/dx_babel_view.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/relocate-results.pt`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
-      i18n:domain="plone">
-<body>
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <body>
+
+    <metal:prefs fill-slot="prefs_configlet_main">
+
+      <div id="results">
 
-<div id="view_language" tal:content="context/language">
-</div>
+        <div class="resultInfo"
+             i18n:domain="plone"
+        >
+          <h2 tal:content="view/stepinfo"
+              i18n:translate=""
+          >
+        Relocate content to the proper root language folder
+          </h2>
+          <span i18n:translate="label_total_objects_translated">
+        Total objects handled:
+          </span>
+          <span tal:content="python: len(view.results)">Number of objects</span>
+        </div>
 
-<tal:block repeat="widget view/widgets/values">
-    <div class="field"  id=""
-         tal:attributes="id python:widget.__name__; rel python:widget.__name__">
-        <label tal:content="widget/label" />
-        <br />
-        <div class="value" tal:content="structure widget/render" />
-    </div>
-</tal:block>
-
-<fieldset tal:repeat="group view/groups"
-          tal:attributes="id python:''.join((group.prefix, 'groups.', group.__name__)).replace('.', '-')">
-    <legend tal:content="group/label" />
-    <tal:block repeat="widget group/widgets/values">
-    <div class="field" rel="" id="" tal:attributes="id python:widget.__name__; rel python:widget.__name__" tal:condition="python:widget.__name__!='IDublinCore.language'">
-        <label tal:content="widget/label" />
-        <br />
-        <div tal:content="structure widget/render" />
-    </div>
-  </tal:block>
-</fieldset>
+        <tal:block repeat="result view/results">
+          <div class="result"
+               tal:content="result"
+               tal:attributes="
+                 class python:result.startswith('ERROR') and 'result error' or 'result';
+               "
+          ></div>
+        </tal:block>
 
-</body>
+      </div>
+    </metal:prefs>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,2 @@
-
-
-
-
+***** Relocate content to the proper root language folder *****
+ Total objects handled:  Number of objects
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/languageselector.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/languageselector.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 <tal:language tal:condition="view/available">
-  <ul
-      id="portal-languageselector"
-      tal:define="showFlags view/showFlags;
-                languages view/languages;
-                portal_url view/portal_url;
-                icons python:context.restrictedTraverse('@@iconresolver');">
+  <ul id="portal-languageselector"
+      tal:define="
+        showFlags view/showFlags;
+        languages view/languages;
+        portal_url view/portal_url;
+        icons python:context.restrictedTraverse('@@iconresolver');
+      "
+  >
     <tal:language repeat="lang languages">
-      <li
-          tal:define="code lang/code;
-                    selected lang/selected;
-                    codeclass string:language-${code};
-                    current python: selected and 'currentLanguage ' or '';"
-          tal:attributes="class string:${current}${codeclass}">
-        <a
-            href=""
-            tal:define="flag lang/flag|nothing;
-                       name lang/native|lang/name;
-                       showflag python:showFlags and flag;"
-            tal:attributes="href lang/url;
-                           title name">
+      <li tal:define="
+            code lang/code;
+            selected lang/selected;
+            codeclass string:language-${code};
+            current python: selected and 'currentLanguage ' or '';
+          "
+          tal:attributes="
+            class string:${current}${codeclass};
+          "
+      >
+        <a href=""
+           tal:define="
+             flag lang/flag|nothing;
+             name lang/native|lang/name;
+             showflag python:showFlags and flag;
+           "
+           tal:attributes="
+             href lang/url;
+             title name;
+           "
+        >
           <tal:flag condition="showflag">
             <tal:flag condition="showflag">
               <img tal:replace="structure python:icons.tag(flag, tag_class='plone-icon-flag')" />
             </tal:flag>
           </tal:flag>
-          <tal:nonflag
-              condition="not: showflag"
-              replace="name">language name</tal:nonflag>
+          <tal:nonflag condition="not: showflag"
+                       replace="name"
+          >language name</tal:nonflag>
         </a>
       </li>
     </tal:language>
   </ul>
-</tal:language>
+</tal:language>
```

#### html2text {}

```diff
@@ -1 +1,2 @@
     *   [Image]   language name
+
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/migration.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/migration.pt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/prefs_main_template/macros/master"
-    i18n:domain="plone">
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
 
-<body>
+  <body>
 
-<metal:block metal:fill-slot="prefs_configlet_main">
+    <metal:block metal:fill-slot="prefs_configlet_main">
 
-  <script type="text/javascript">
+      <script type="text/javascript">
   (function($) {
 
       $().ready(function() {
           $('#lp-migration-relocate-content').submit(function () {
             var blacklist = $('textarea#blacklist')[0].value;
             $('html, body').animate({
                 scrollTop: $('.results').offset().top
@@ -52,223 +54,251 @@
             var auth_key = $(this).find('input[name="_authenticator"]').val();
             $('.results').load('@@reindex-language-index?_authenticator=' +  auth_key + ' #results');
             return false;
           });
       });
 
   })(jQuery);
-  </script>
+      </script>
 
-  <style>
+      <style>
   .results {
     border: 1px solid #ccc;
     padding: 10px;
     background-color: #eee;
   }
 
-  </style>
+      </style>
 
-        <div i18n:domain="plone">
-            <ul>
-              <li>
-                <a href=""
-                   tal:attributes="href string:${portal_url}/@@language-controlpanel"
-                   i18n:translate="label_general">General</a>
-              </li>
-              <li>
-                <a href=""
-                   tal:attributes="href string:${portal_url}/@@multilingual-map"
-                   i18n:translate="label_translation_map">Translation Map</a>
-              </li>
-              <li class="selected">
-                <a href=""
-                   tal:attributes="href string:${portal_url}/@@lp-migration"
-                   i18n:translate="label_migration">Migration</a>
-              </li>
-            </ul>
-        </div>
+      <div i18n:domain="plone">
+        <ul>
+          <li>
+            <a href=""
+               tal:attributes="
+                 href string:${portal_url}/@@language-controlpanel;
+               "
+               i18n:translate="label_general"
+            >General</a>
+          </li>
+          <li>
+            <a href=""
+               tal:attributes="
+                 href string:${portal_url}/@@multilingual-map;
+               "
+               i18n:translate="label_translation_map"
+            >Translation Map</a>
+          </li>
+          <li class="selected">
+            <a href=""
+               tal:attributes="
+                 href string:${portal_url}/@@lp-migration;
+               "
+               i18n:translate="label_migration"
+            >Migration</a>
+          </li>
+        </ul>
+      </div>
+
+      <h1 class="documentFirstHeading"
+          i18n:translate="heading_migration"
+      >Products.LinguaPlone Migration</h1>
 
-        <h1 class="documentFirstHeading"
-            i18n:translate="heading_migration">Products.LinguaPlone Migration</h1>
-
-        <div metal:use-macro="context/global_statusmessage/macros/portal_message">
+      <div metal:use-macro="context/global_statusmessage/macros/portal_message">
         Portal status message
-        </div>
+      </div>
 
-        <div id="content-core">
+      <div id="content-core">
 
-            <p i18n:translate="description_migrate">
+        <p i18n:translate="description_migrate">
 
                 The migration process is divided into four steps, listed
                 below. Each one of the steps has a well defined purpose
                 explained. Some of them are destructive, so please read each
                 one of it and do not try to run it on production servers
                 without testing it previously.
 
-            </p>
+        </p>
 
-            <form
-                  id="lp-migration-reindex-content"
-                  tal:attributes="action string:${portal_url}/reindex-language-index"
-                  method="post">
-              <fieldset>
-                <legend i18n:translate="legend_reindex_language_index">
+        <form id="lp-migration-reindex-content"
+              method="post"
+              tal:attributes="
+                action string:${portal_url}/reindex-language-index;
+              "
+        >
+          <fieldset>
+            <legend i18n:translate="legend_reindex_language_index">
                   Optional step - Reindex the Language index
-                </legend>
+            </legend>
 
-                <p i18n:translate="help_reindex_language_index">
+            <p i18n:translate="help_reindex_language_index">
 
                  The migration of LinguaPlone content depends on an up-to-date Language
                  index. Use this step to refresh this index.
                  Warning: Depending on the number of items in your site, this can take
                  a considerable amount of time.
 
-                </p>
+            </p>
+
+            <div class="formControls">
+              <input class="destructive"
+                     name="form.button.reindex-language-index"
+                     type="submit"
+                     value="Reindex"
+                     i18n:attributes="value"
+              />
+            </div>
+
+            <input tal:replace="structure context/@@authenticator/authenticator" />
 
-                <div class="formControls">
-                    <input
-                        type="submit"
-                        name="form.button.reindex-language-index"
-                        class="destructive"
-                        value="Reindex"
-                        i18n:attributes="value" />
-                </div>
-
-                <input tal:replace="structure context/@@authenticator/authenticator" />
-
-              </fieldset>
-            </form>
-
-            <form id="lp-migration-relocate-content"
-                  tal:attributes="action string:${portal_url}/relocate-content"
-                  method="post">
-              <fieldset>
-                <legend i18n:translate="legend_relocate_content">
+          </fieldset>
+        </form>
+
+        <form id="lp-migration-relocate-content"
+              method="post"
+              tal:attributes="
+                action string:${portal_url}/relocate-content;
+              "
+        >
+          <fieldset>
+            <legend i18n:translate="legend_relocate_content">
                   Step 1 - Relocate content to the proper root language folder
-                </legend>
+            </legend>
 
-                <p i18n:translate="description_relocate_content">
+            <p i18n:translate="description_relocate_content">
                   This step will move the site's content to its corresponding
                   root language folder and previously will make a search for
                   misplaced content through the site's content tree and will
                   move them to its nearest translated parent. This step is
                   destructive as it will alter your content tree structure.
                   Make sure you have previously configured your site's
                   languages properly in the 'Site Languages' tab of the
                   'Languages' control panel.
-                </p>
+            </p>
 
-                <div>
-                    <p i18n:translate="description_relocate_blacklist">
+            <div>
+              <p i18n:translate="description_relocate_blacklist">
                         Use this field to define portal types that will not be traversed for finding content to move.
                         All content of those types will be moved with all contained sub-items. This is useful
                         for content types that are themselves translatable, but contain sub-content that is not
-                        translatable or does not have a language set.<br />
+                translatable or does not have a language set.<br />
                         This list is pre-filled with some portal types, but you can add additional ones if needed,
                         one per line.
-                    </p>
-                    <textarea name="blacklist" id="blacklist" rows="5" tal:content="python: '\n'.join(view.portal_types_blacklist)">
-                    </textarea>
-                </div>
-
-                <div class="formControls">
-                    <input
-                        type="submit"
-                        name="form.button.relocate-content"
-                        class="destructive"
-                        value="Relocate"
-                        i18n:attributes="value" />
-                </div>
-
-                <input tal:replace="structure context/@@authenticator/authenticator" />
-
-              </fieldset>
-            </form>
-
-            <form id="lp-migration-transfer-catalog"
-                  tal:attributes="action string:${portal_url}/transfer-lp-catalog"
-                  method="post">
-              <fieldset>
-                <legend i18n:translate="legend_transfer_multilingual_catalog_info">
+              </p>
+              <textarea id="blacklist"
+                        name="blacklist"
+                        rows="5"
+                        tal:content="python: '\n'.join(view.portal_types_blacklist)"
+              >
+              </textarea>
+            </div>
+
+            <div class="formControls">
+              <input class="destructive"
+                     name="form.button.relocate-content"
+                     type="submit"
+                     value="Relocate"
+                     i18n:attributes="value"
+              />
+            </div>
+
+            <input tal:replace="structure context/@@authenticator/authenticator" />
+
+          </fieldset>
+        </form>
+
+        <form id="lp-migration-transfer-catalog"
+              method="post"
+              tal:attributes="
+                action string:${portal_url}/transfer-lp-catalog;
+              "
+        >
+          <fieldset>
+            <legend i18n:translate="legend_transfer_multilingual_catalog_info">
                   Step 2 - Transfer multilingual catalog information
-                </legend>
+            </legend>
 
-                <p i18n:translate="description_transfer_multilingual_catalog_info">
+            <p i18n:translate="description_transfer_multilingual_catalog_info">
 
                   This step will transfer the relations between translations
                   stored by LinguaPlone to the PAM catalog. This step is not
                   destructive and can be executed as many times as needed.
 
-                </p>
+            </p>
 
-                <div class="formControls">
-                    <input
-                        type="submit"
-                        name="form.button.transfer-lp-catalog"
-                        class="destructive"
-                        value="Transfer"
-                        i18n:attributes="value" />
-                </div>
-
-                <input tal:replace="structure context/@@authenticator/authenticator" />
-
-              </fieldset>
-            </form>
-
-            <form id="lp-migration-after-migration"
-                  tal:attributes="action python:not view.isLPinstalled and view.hasRelationCatalog and portal_url + '/after-migration-cleanup'"
-                  method="post">
-              <fieldset>
-                <legend i18n:translate="legend_after_migration_cleanup">
+            <div class="formControls">
+              <input class="destructive"
+                     name="form.button.transfer-lp-catalog"
+                     type="submit"
+                     value="Transfer"
+                     i18n:attributes="value"
+              />
+            </div>
+
+            <input tal:replace="structure context/@@authenticator/authenticator" />
+
+          </fieldset>
+        </form>
+
+        <form id="lp-migration-after-migration"
+              method="post"
+              tal:attributes="
+                action python:not view.isLPinstalled and view.hasRelationCatalog and portal_url + '/after-migration-cleanup';
+              "
+        >
+          <fieldset>
+            <legend i18n:translate="legend_after_migration_cleanup">
                   Step 3 - Cleanup after migration
-                </legend>
+            </legend>
 
-                <p i18n:translate="description_after_migration_cleanup">
+            <p i18n:translate="description_after_migration_cleanup">
 
                   This step will fix some lost dependencies to the
                   ITranslatable interface hidden in the relation catalog and
                   it gets rid of them. It must be run only when LinguaPlone is
                   already uninstalled.
 
-                </p>
+            </p>
 
-                <p tal:condition="view/isLPinstalled"
-                    i18n:translate="relation_migration_with_lp_not_posible">
+            <p tal:condition="view/isLPinstalled"
+               i18n:translate="relation_migration_with_lp_not_posible"
+            >
                     It's not possible to execute this step without
                     uninstalling completely LinguaPlone: uninstall in the
                     add-ons control panel, delete it from your buildout
                     and re-run buildout. Then come here and try again.
-                </p>
+            </p>
 
-                <p tal:condition="python:not view.isLPinstalled and not view.hasRelationCatalog"
-                    i18n:translate="relation_migration_with_not_needed">
+            <p tal:condition="python:not view.isLPinstalled and not view.hasRelationCatalog"
+               i18n:translate="relation_migration_with_not_needed"
+            >
                     Your site has no relation catalog, and therefore this
                     migration step is not needed
-                </p>
+            </p>
 
-                <div class="formControls"
-                     tal:condition="python:not view.isLPinstalled and view.hasRelationCatalog">
-                    <input
-                        type="submit"
-                        name="form.button.after-migration-cleanup"
-                        class="destructive"
-                        value="Cleanup"
-                        i18n:attributes="value" />
-                </div>
-
-                <input tal:replace="structure context/@@authenticator/authenticator" />
-
-              </fieldset>
-            </form>
-
-            <div class="results">
-              <h2 i18n:translate="heading_migration_results">Migration results</h2>
-              <p i18n:translate="description_migration_results">
-                Here you will see the results of the migration process
-              </p>
+            <div class="formControls"
+                 tal:condition="python:not view.isLPinstalled and view.hasRelationCatalog"
+            >
+              <input class="destructive"
+                     name="form.button.after-migration-cleanup"
+                     type="submit"
+                     value="Cleanup"
+                     i18n:attributes="value"
+              />
             </div>
+
+            <input tal:replace="structure context/@@authenticator/authenticator" />
+
+          </fieldset>
+        </form>
+
+        <div class="results">
+          <h2 i18n:translate="heading_migration_results">Migration results</h2>
+          <p i18n:translate="description_migration_results">
+                Here you will see the results of the migration process
+          </p>
         </div>
+      </div>
 
-</metal:block>
+    </metal:block>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/migrator-results.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/migrator-results.pt`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/prefs_main_template/macros/master"
-    i18n:domain="plone">
-
-<body>
-
-<metal:prefs fill-slot="prefs_configlet_main">
-
-<div id="results">
-
-<div class="resultInfo" i18n:domain="plone">
-    <h2 i18n:translate=""
-        tal:content="view/stepinfo">
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <body>
+
+    <metal:prefs fill-slot="prefs_configlet_main">
+
+      <div id="results">
+
+        <div class="resultInfo"
+             i18n:domain="plone"
+        >
+          <h2 tal:content="view/stepinfo"
+              i18n:translate=""
+          >
         Transfer multilingual catalog information
-    </h2>
-    <span i18n:translate="label_total_objects_translated">
+          </h2>
+          <span i18n:translate="label_total_objects_translated">
         Total objects handled:
-    </span>
-    <span tal:content="python: len(view.results)">Number of objects</span>
-</div>
-
-<tal:block repeat="result view/results">
-    <div class="result"
-    tal:attributes="class python:result.startswith('ERROR') and 'result error' or 'result'"
-    tal:content="result"></div>
-</tal:block>
-
-</div>
-</metal:prefs>
-</body>
+          </span>
+          <span tal:content="python: len(view.results)">Number of objects</span>
+        </div>
+
+        <tal:block repeat="result view/results">
+          <div class="result"
+               tal:content="result"
+               tal:attributes="
+                 class python:result.startswith('ERROR') and 'result error' or 'result';
+               "
+          ></div>
+        </tal:block>
+
+      </div>
+    </metal:prefs>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/mmap.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/mmap.pt`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/prefs_main_template/macros/master"
-    i18n:domain="plone">
-
-<body>
-
-<metal:block metal:fill-slot="prefs_configlet_main">
-
-  <script type="text/javascript" src="++resource++plone.app.multilingual.javascript/jit-yc.js"></script>
-  <script type="text/javascript" src="++resource++plone.app.multilingual.javascript/mmap_helper.js"></script>
-  <style>
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <body>
+
+    <metal:block metal:fill-slot="prefs_configlet_main">
+
+      <script src="++resource++plone.app.multilingual.javascript/jit-yc.js"
+              type="text/javascript"
+      ></script>
+      <script src="++resource++plone.app.multilingual.javascript/mmap_helper.js"
+              type="text/javascript"
+      ></script>
+      <style>
   #pam_mmap_toolbar {
     border: 1px solid #000;
     padding: 20px;
     position: relative;
   }
 
   #pam_mmap_language_toolbar {
@@ -47,94 +53,131 @@
     background-color: #ccc;
   }
 
   #pam_language_buttons button.down, #pam_ajax_buttons button.down {
     background-color: #777;
     color: white;
   }
-  </style>
+      </style>
 
-        <a id="setup-link" class="link-parent"
-           tal:attributes="href string:$portal_url/@@overview-controlpanel"
-           i18n:translate="">
+      <a class="link-parent"
+         id="setup-link"
+         tal:attributes="
+           href string:$portal_url/@@overview-controlpanel;
+         "
+         i18n:translate=""
+      >
             Site Setup
-        </a>
+      </a>
 
-        <h1 class="documentFirstHeading"
-            i18n:translate="heading_translation_map">plone.app.multilingual translation map</h1>
+      <h1 class="documentFirstHeading"
+          i18n:translate="heading_translation_map"
+      >plone.app.multilingual translation map</h1>
 
-        <div metal:use-macro="context/global_statusmessage/macros/portal_message">
+      <div metal:use-macro="context/global_statusmessage/macros/portal_message">
         Portal status message
-        </div>
+      </div>
 
-        <div id="content-core">
+      <div id="content-core">
 
-            <p i18n:translate="description_translation_map">
+        <p i18n:translate="description_translation_map">
                 Translation map.
-            </p>
-            <div id="pam_ajax_buttons">
-              <button id="call_missing_translations" i18n:translate="label_missing_translations">Missing translations</button>
-              <button id="call_all_translations" class="down" i18n:translate="label_all_translations">All translations</button>
-            </div>
+        </p>
+        <div id="pam_ajax_buttons">
+          <button id="call_missing_translations"
+                  i18n:translate="label_missing_translations"
+          >Missing translations</button>
+          <button class="down"
+                  id="call_all_translations"
+                  i18n:translate="label_all_translations"
+          >All translations</button>
+        </div>
 
-            <div id="all_translations">
+        <div id="all_translations">
 
-            <div id="pam_mmap_toolbar">
-              <div id="pam_mmap_language_toolbar">
-                <div id="pam_language_buttons" tal:define="data view/languages">
+          <div id="pam_mmap_toolbar">
+            <div id="pam_mmap_language_toolbar">
+              <div id="pam_language_buttons"
+                   tal:define="
+                     data view/languages;
+                   "
+              >
                 <tal:block repeat="languages data/languages">
-                  <button id="" tal:attributes="id languages/value;
-                                                class python: languages.value==data['default'] and 'down' or ''" tal:content="languages/title">Lang</button>
+                  <button id=""
+                          tal:content="languages/title"
+                          tal:attributes="
+                            id languages/value;
+                            class python: languages.value==data['default'] and 'down' or '';
+                          "
+                  >Lang</button>
                 </tal:block>
-                </div>
+              </div>
 
-                <div id="actual_language">
-                </div>
+              <div id="actual_language">
               </div>
+            </div>
 
             <div id="data_translation">
             </div>
           </div>
-            <div id="translation_map_canvas" style="height: 400px; width: 600px;">
-
-            </div>
-            <div id="log">
-            </div>
+          <div id="translation_map_canvas"
+               style="height: 400px; width: 600px;"
+          >
 
           </div>
-          <div id="missing_translations">
-            <div tal:define="not_full_translated view/canonicals">
-              <ul>
+          <div id="log">
+          </div>
+
+        </div>
+        <div id="missing_translations">
+          <div tal:define="
+                 not_full_translated view/canonicals;
+               ">
+            <ul>
               <tal:block repeat="canonical not_full_translated">
                 <li>
-                <span tal:content="canonical/id">Id</span>
-                <ul tal:define="last_url canonical/last_url">
-                  <li>
-                    <span i18n:translate="missing_languages">Missing languages: </span>
-                    <tal:block2 repeat="missing canonical/missing">
-                      <a href="" target="_blank" tal:attributes="href string:$last_url/@@create_translation?language=$missing" tal:content="missing">
+                  <span tal:content="canonical/id">Id</span>
+                  <ul tal:define="
+                        last_url canonical/last_url;
+                      ">
+                    <li>
+                      <span i18n:translate="missing_languages">Missing languages:
+                      </span>
+                      <tal:block2 repeat="missing canonical/missing">
+                        <a href=""
+                           target="_blank"
+                           tal:content="missing"
+                           tal:attributes="
+                             href string:$last_url/@@create_translation?language=$missing;
+                           "
+                        >
                         lang
-                      </a>
-                    </tal:block2>
-                  </li>
-                  <li>
-                    <span i18n:translate="translation">Translations: </span>
-                    <tal:block2 repeat="missing canonical/translated">
-                      <a href="" tal:attributes="href missing/url">
-                        <span tal:content="missing/path">Path</span>
-                        <span tal:content="missing/lang">Lang</span>
-                      </a>
-                    </tal:block2>
-                  </li>
-                </ul>
+                        </a>
+                      </tal:block2>
+                    </li>
+                    <li>
+                      <span i18n:translate="translation">Translations:
+                      </span>
+                      <tal:block2 repeat="missing canonical/translated">
+                        <a href=""
+                           tal:attributes="
+                             href missing/url;
+                           "
+                        >
+                          <span tal:content="missing/path">Path</span>
+                          <span tal:content="missing/lang">Lang</span>
+                        </a>
+                      </tal:block2>
+                    </li>
+                  </ul>
                 </li>
               </tal:block>
-              </ul>
-            </div>
+            </ul>
           </div>
-
         </div>
 
-</metal:block>
+      </div>
+
+    </metal:block>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/not_translated_yet.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/not_translated_yet.pt`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,84 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/main_template/macros/master"
-      i18n:domain="plone">
-<body>
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
 
-<metal:head fill-slot="top_slot"
-            tal:define="dummy python:request.set('disable_border',1);
-                        disable_column_one python:request.set('disable_plone.leftcolumn',1);
-                        disable_column_two python:request.set('disable_plone.rightcolumn',1);">
-</metal:head>
+    <metal:head fill-slot="top_slot"
+                tal:define="
+                  dummy python:request.set('disable_border',1);
+                  disable_column_one python:request.set('disable_plone.leftcolumn',1);
+                  disable_column_two python:request.set('disable_plone.rightcolumn',1);
+                "
+    >
+    </metal:head>
 
-<metal:main fill-slot="main">
-    <metal:main define-macro="main">
+    <metal:main fill-slot="main">
+      <metal:main define-macro="main">
 
-    <h1 class="documentFirstHeading" i18n:translate="heading_not_available_in_language">
-      Not available in <span i18n:name="language" tal:content="view/language_name" tal:omit-tag="">es</span>
-    </h1>
+        <h1 class="documentFirstHeading"
+            i18n:translate="heading_not_available_in_language"
+        >
+      Not available in
+          <span tal:content="view/language_name"
+                tal:omit-tag=""
+                i18n:name="language"
+          >es</span>
+        </h1>
 
-      <div class="documentDescription" id="parent-fieldname-description" i18n:translate="">
+        <div class="documentDescription"
+             id="parent-fieldname-description"
+             i18n:translate=""
+        >
         This content is not translated yet to the language requested.
-      </div>
-      <section>
-        <tal:anytranslation condition="view/has_any_translation">
-          <p i18n:translate="">However, this is the list of the already translated languages for the requested content.</p>
-          <ul>
-            <tal:list repeat="trans_content view/already_translated">
-              <tal:defines define="code python: trans_content[0];
-                              trans_obj python: trans_content[1]">
-              <li tal:condition="python:trans_obj.Title()">
-                <span tal:replace="python:view.language_name(code)" /> - <span tal:replace="code"/>:
-                <a tal:attributes="href python:trans_obj.absolute_url() + '?set_language=' + code"
-                   tal:content="python:trans_obj.Title()">Translation Link</a></li>
-              <li tal:condition="python:not trans_obj.Title()">
-                <span tal:content="python:trans_obj"></span>
-                <a tal:attributes="href python:trans_obj.absolute_url() + '?set_language=' + code"
-                    i18n:translate="label_no_title">
-                  (No Title)</a></li>
-              </tal:defines>
-            </tal:list>
-          </ul>
-        </tal:anytranslation>
-        <tal:anytranslation condition="not: view/has_any_translation">
-          <p i18n:translate="">This item doesn't have any translation yet. You can return to the portal site:</p>
+        </div>
+        <section>
+          <tal:anytranslation condition="view/has_any_translation">
+            <p i18n:translate="">However, this is the list of the already translated languages for the requested content.</p>
+            <ul>
+              <tal:list repeat="trans_content view/already_translated">
+                <tal:defines define="
+                               code python: trans_content[0];
+                               trans_obj python: trans_content[1];
+                             ">
+                  <li tal:condition="python:trans_obj.Title()">
+                    <span tal:replace="python:view.language_name(code)"></span>
+                    -
+                    <span tal:replace="code"></span>:
+                    <a tal:content="python:trans_obj.Title()"
+                       tal:attributes="
+                         href python:trans_obj.absolute_url() + '?set_language=' + code;
+                       "
+                    >Translation Link</a></li>
+                  <li tal:condition="python:not trans_obj.Title()">
+                    <span tal:content="python:trans_obj"></span>
+                    <a tal:attributes="
+                         href python:trans_obj.absolute_url() + '?set_language=' + code;
+                       "
+                       i18n:translate="label_no_title"
+                    >
+                      (No Title)</a></li>
+                </tal:defines>
+              </tal:list>
+            </ul>
+          </tal:anytranslation>
+          <tal:anytranslation condition="not: view/has_any_translation">
+            <p i18n:translate="">This item doesn't have any translation yet. You can return to the portal site:</p>
             <ul>
-              <li><a tal:attributes="href python:context.absolute_url()"
-                     tal:content="python:context.Title()">Content Link</a></li>
+              <li><a tal:content="python:context.Title()"
+                   tal:attributes="
+                     href python:context.absolute_url();
+                   "
+                >Content Link</a></li>
             </ul>
-        </tal:anytranslation>
-      </section>
+          </tal:anytranslation>
+        </section>
+      </metal:main>
     </metal:main>
-  </metal:main>
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/templates/reindex-results.pt` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/templates/reindex-results.pt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/prefs_main_template/macros/master"
-    i18n:domain="plone">
-
-<body>
-
-<metal:prefs fill-slot="prefs_configlet_main">
-
-<div id="results">
-
-<div class="resultInfo">
-    <h2 i18n:translate=""
-        tal:content="view/stepinfo">
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/prefs_main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <body>
+
+    <metal:prefs fill-slot="prefs_configlet_main">
+
+      <div id="results">
+
+        <div class="resultInfo">
+          <h2 tal:content="view/stepinfo"
+              i18n:translate=""
+          >
         Reindex Language Index
-    </h2>
+          </h2>
 
-    <p i18n:translate="migration_reindex_results">
+          <p i18n:translate="migration_reindex_results">
       The "Language" index was re-indexed correctly. Before, it contained
-      <span i18n:name="previous_items_number" tal:content="view/items_before"
-          tal:omit-tag="" /> items, now it contains <span i18n:name="after_items_number"
-          tal:content="view/items_after" tal:omit-tag="" />
-
-    </p>
-</div>
-
-</div>
-</metal:prefs>
-</body>
+            <span tal:content="view/items_before"
+                  tal:omit-tag=""
+                  i18n:name="previous_items_number"
+            ></span>
+            items, now it contains
+            <span tal:content="view/items_after"
+                  tal:omit-tag=""
+                  i18n:name="after_items_number"
+            ></span>
+
+          </p>
+        </div>
+
+      </div>
+    </metal:prefs>
+  </body>
 </html>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/translate.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/translate.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/update.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/update.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/utils.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/viewlets.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/viewlets.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,27 +120,14 @@
         else:
             self.lang = "NaN"
         catalog = getToolByName(self.context, "portal_catalog")
         query = {"TranslationGroup": tg}
         self.origin = catalog.searchResults(query)
 
 
-class AddFormATIsATranslationViewlet(AddFormIsATranslationViewlet):
-    # XXX move this class to archetypes multilingual!
-    # btw., it is not used in here.
-    """Notice the user that this AT add form is a translation"""
-
-    def update(self):
-        """It's only for AT on factory so we check"""
-        factory = getToolByName(self.context, "portal_factory", None)
-        if factory is None or not factory.isTemporary(self.context):
-            return
-        super(AddFormIsATranslationViewlet, self).update()
-
-
 class AlternateLanguagesViewlet(ViewletBase):
     """Notice search engines about alternates languages of current
     content item
     """
 
     alternatives = []
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/browser/vocabularies.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/browser/vocabularies.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 @provider(IContextSourceBinder)
 def translated_languages(context):
     language_tool = getToolByName(context, "portal_languages")
     language_infos = language_tool.getAvailableLanguages()
     manager = ITranslationManager(context)
     # take care to filter out translated contents
-    # wich do no have supported language information
+    # which do no have supported language information
     translated_languages = [
         a for a in manager.get_translated_languages() if a in language_infos
     ]
     content_language = ILanguage(context).get_language()
     if content_language in translated_languages:
         translated_languages.remove(content_language)
     languages = []
@@ -100,16 +100,16 @@
         util = gsm.queryUtility(ILanguageAvailability)
         if ltool.use_combined_language_codes:
             languages = util.getLanguages(combined=True)
         else:
             languages = util.getLanguages()
 
         items = [
-            (l, languages[l].get("native", languages[l].get("name", l)))
-            for l in languages
+            (lang, languages[lang].get("native", languages[lang].get("name", lang)))
+            for lang in languages
         ]
         items.sort(key=sort_key)
         items = [SimpleTerm(i[0], i[0], i[1]) for i in items]
         return SimpleVocabulary(items)
 
 
 AllContentLanguageVocabularyFactory = AllContentLanguageVocabulary()
@@ -127,17 +127,17 @@
         if ltool.use_combined_language_codes:
             languages = util.getLanguages(combined=True)
         else:
             languages = util.getLanguages()
 
         supported_languages = ltool.supported_langs
         items = [
-            (l, languages[l].get("native", languages[l].get("name", l)))
-            for l in languages
-            if l in supported_languages
+            (lang, languages[lang].get("native", languages[lang].get("name", lang)))
+            for lang in languages
+            if lang in supported_languages
         ]
 
         items.sort(key=sort_key)
         items = [SimpleTerm(i[0], i[0], i[1]) for i in items]
         return SimpleVocabulary(items)
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/content/lrf.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/content/lrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/cloner.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/cloner.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from plone.app.multilingual.dx.interfaces import ILanguageIndependentField
 from plone.app.multilingual.interfaces import ILanguageIndependentFieldsManager
 from plone.app.multilingual.interfaces import ITranslationCloner
 from plone.app.multilingual.interfaces import ITranslationManager
 from plone.base.interfaces import ILanguage
-from plone.dexterity.utils import iterSchemata
 from plone.base.utils import safe_text
+from plone.dexterity.utils import iterSchemata
 from z3c.relationfield import RelationValue
 from z3c.relationfield.interfaces import IRelationList
 from z3c.relationfield.interfaces import IRelationValue
 from zope.component import getUtility
 from zope.component import queryAdapter
 from zope.interface import implementer
 from zope.intid.interfaces import IIntIds
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/configure.zcml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:plone="http://namespaces.plone.org/plone"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
   <include file="meta.zcml" />
 
   <!-- Configure plone.schemaeditor adapter -->
   <adapter
+      factory=".schemaeditor.get_li_schema"
       provides="plone.schemaeditor.interfaces.IFieldEditorExtender"
       for="zope.schema.interfaces.IField"
       name="plone.schemaeditor.languageindependent"
-      factory=".schemaeditor.get_li_schema"/>
+      />
 
   <adapter
+      factory=".schemaeditor.FieldLanguageIndependentAdapter"
       provides=".schemaeditor.IFieldLanguageIndependent"
       for="zope.schema.interfaces.IField"
-      factory=".schemaeditor.FieldLanguageIndependentAdapter"/>
+      />
 
 
   <!-- Configure plone.supermodel handler -->
   <utility
       factory=".supermodel.LanguageIndependentFieldMetadataHandler"
-      name="plone.rfc822.lingua"/>
+      name="plone.rfc822.lingua"
+      />
 
   <adapter
       factory=".directives.LanguageIndependentFieldsPlugin"
-      name="plone.rfc822.lingua"/>
+      name="plone.rfc822.lingua"
+      />
 
 
   <plone:behavior
+      name="plone.translatable"
       title="Multilingual Support"
       description="Make this content type multilingual aware"
-      name="plone.translatable"
-      provides=".interfaces.IDexterityTranslatable"/>
+      provides=".interfaces.IDexterityTranslatable"
+      />
 
   <adapter
-      for="plone.app.multilingual.dx.interfaces.IDexterityTranslatable"
+      factory=".cloner.LanguageIndependentFieldsManager"
       provides="plone.app.multilingual.interfaces.ILanguageIndependentFieldsManager"
-      factory=".cloner.LanguageIndependentFieldsManager"/>
+      for="plone.app.multilingual.dx.interfaces.IDexterityTranslatable"
+      />
 
   <adapter
-      for="plone.dexterity.interfaces.IDexterityContent"
+      factory=".language.Language"
       provides="plone.base.interfaces.ILanguage"
-      factory=".language.Language"/>
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
 
   <adapter
+      factory=".form.AddingLanguageIndependentValue"
       for="*
            *
            plone.app.multilingual.dx.interfaces.IMultilingualAddForm
            plone.app.multilingual.dx.interfaces.ILanguageIndependentField
            z3c.form.interfaces.IWidget"
-      factory=".form.AddingLanguageIndependentValue"
-      name="default"/>
+      name="default"
+      />
 
   <adapter
+      factory=".form.LanguageIndependentFieldValidator"
+      provides="z3c.form.interfaces.IValidator"
       for="*
            plone.app.multilingual.interfaces.IPloneAppMultilingualInstalled
            plone.app.multilingual.dx.interfaces.IMultilingualAddForm
            plone.app.multilingual.dx.interfaces.ILanguageIndependentField
            *"
-      provides="z3c.form.interfaces.IValidator"
-      factory=".form.LanguageIndependentFieldValidator"/>
+      />
 
   <adapter
+      factory=".form.LanguageIndependentFieldInputTemplate"
+      provides="zope.pagetemplate.interfaces.IPageTemplate"
       for="*
            plone.app.multilingual.interfaces.IPloneAppMultilingualInstalled
            plone.app.multilingual.dx.interfaces.IMultilingualAddForm
            plone.app.multilingual.dx.interfaces.ILanguageIndependentField
            *"
-      provides="zope.pagetemplate.interfaces.IPageTemplate"
       name="input"
-      factory=".form.LanguageIndependentFieldInputTemplate"/>
+      />
 
 </configure>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/directives.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/form.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/form.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/interfaces.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     """Marker interface for language independent fields"""
 
 
 class IMultilingualAddForm(Interface):
     """Marker Interface for multilingual add forms
 
     This marker is intended to be provided by the main multilingual add form
-    ans to be provided by the groups (aka fieldset) forms
-    (plone.z3cform.fieldsets.group.Group). This is neccessary in order to
+    and to be provided by the groups (aka fieldset) forms
+    (plone.z3cform.fieldsets.group.Group). This is necessary in order to
     make the special template renderer for ILanguageIndependentField fields
     work in fieldset tabs too.
     """
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/language.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/language.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/schemaeditor.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/subscriber.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/subscriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         sm = getSecurityManager()
         try:
             # Do we have permission to sync language independent fields?
             if self.bypass_security_checks():
                 # Clone the current user and assign a new editor role to
                 # allow edition of all translated objects even if the
-                # current user whould not have permission to do that.
+                # current user would not have permission to do that.
                 tmp_user = UnrestrictedUser(
                     sm.getUser().getId(),
                     "",
                     [
                         "Editor",
                     ],
                     "",
@@ -102,15 +102,15 @@
         translation.reindexObject()
 
         fti = getUtility(IDexterityFTI, name=translation.portal_type)
         schema = fti.lookupSchema()
         descriptions = Attributes(schema)
         # where is this information needed?
         # XXX behaviors need to be considered here
-        # use plone.dexterity.utils.iterSchemata or similiar
+        # use plone.dexterity.utils.iterSchemata or similar
 
         # Pass the canonical object as a event description
         notify(ObjectModifiedEvent(translation, descriptions, self.canonical))
 
     def get_all_translations(self, content):
         """Return all translations excluding the just modified content"""
         content_lang = queryAdapter(content, ILanguage).get_language()
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/dx/supermodel.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/dx/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/events.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """Sent after a new translation was registered.
 
     This is meant to be notified on low-level manager level only.
     """
 
     object = Attribute("The base object.")
     target = Attribute("The translated object.")
-    language = Attribute("The language of the translated obejct.")
+    language = Attribute("The language of the translated object.")
 
 
 class ITranslationUpdatedEvent(IObjectEvent):
     """Sent after an translation was moved to point to a different object
 
     This is meant to be notified on low-level manager level only.
     """
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/factory.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,18 @@
 @implementer(ITranslationIdChooser)
 class DefaultTranslationIdChooser:
     def __init__(self, context):
         self.context = context
 
     def __call__(self, parent, language):
         content_id = self.context.getId()
-        splitted = content_id.split("-")
+        parts = content_id.split("-")
         # ugly heuristic (searching for something like 'de', 'en' etc.)
-        if len(splitted) > 1 and len(splitted[-1]) == 2:
-            content_id = "-".join(splitted[:-1])
+        if len(parts) > 1 and len(parts[-1]) == 2:
+            content_id = "-".join(parts[:-1])
         while content_id in parent.objectIds():
             content_id = f"{content_id}-{language}"
         return content_id
 
 
 @implementer(ITranslationFactory)
 class DefaultTranslationFactory:
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/interfaces.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         default=False,
         required=False,
     )
 
     buttons_babel_view_up_to_nr_translations = schema.Int(
         title=_(
             "heading_buttons_babel_view_up_to_nr_translations",
-            default="Use buttons in the bable view for up to how many " "translations?",
+            default="Use buttons in the babel view for up to how many translations?",
         ),
         description=_(
             "description_buttons_babel_view_up_to_nr_translations",
             default="When there are many translations for an item, the "
             "number of displayed buttons for them might get too "
             "large to fit inside the template. Choose here from "
             "which number onwards a drop-down menu will be displayed "
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/itg.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/itg.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/manager.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/manager.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/registry.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/registry.xml`

 * *Files 8% similar despite different names*

#### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/registry.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/registry.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <registry>
-  <records prefix="plone.bundles/multilingual" interface="plone.base.interfaces.IBundleRegistry">
+  <records interface="plone.base.interfaces.IBundleRegistry" prefix="plone.bundles/multilingual">
     <value key="enabled">True</value>
     <value key="csscompilation">++resource++plone.app.multilingual.stylesheet/multilingual.css</value>
   </records>
   <records interface="plone.base.interfaces.ITinyMCEResourceTypesSchema" prefix="plone">
     <value key="contains_objects" purge="false">
       <element>LIF</element>
     </value>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/LIF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/LIF.xml`

 * *Files 21% similar despite different names*

#### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/LIF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/LIF.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="LIF" meta_type="Dexterity FTI" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="LIF" i18n:domain="plone">
   <property name="title" i18n:translate="">Language Independent Folder</property>
   <property name="description" i18n:translate=""/>
   <property name="icon_expr">string:contenttype/folder</property>
   <property name="factory">LIF</property>
   <property name="add_view_expr">string:${folder_url}/++add++LIF</property>
   <property name="link_target"/>
   <property name="immediate_view">view</property>
@@ -32,14 +32,14 @@
   <property name="schema">plone.app.multilingual.interfaces.ILanguageIndependentFolder</property>
   <property name="model_source"/>
   <property name="model_file">plone.app.multilingual.content:lif.xml</property>
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/LRF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/LRF.xml`

 * *Files 21% similar despite different names*

#### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/default/types/LRF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/default/types/LRF.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="LRF" meta_type="Dexterity FTI" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="LRF" i18n:domain="plone">
   <property name="title" i18n:translate="">Language Root Folder</property>
   <property name="description" i18n:translate=""/>
   <property name="icon_expr">string:contenttype/folder</property>
   <property name="factory">LRF</property>
   <property name="add_view_expr">string:${folder_url}/++add++LRF</property>
   <property name="link_target"/>
   <property name="immediate_view">view</property>
@@ -33,14 +33,14 @@
   <property name="schema">plone.app.multilingual.interfaces.ILanguageRootFolder</property>
   <property name="model_source"/>
   <property name="model_file">plone.app.multilingual.content:lrf.xml</property>
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml`

 * *Files 16% similar despite different names*

#### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="LIF" meta_type="Dexterity FTI" i18n:domain="plone">
-  <property name="title" i18n:translate="">Language Independent Folder</property>
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="LRF" i18n:domain="plone">
+  <property name="title" i18n:translate="">Language Root Folder</property>
   <property name="icon_expr">string:contenttype/folder</property>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml`

 * *Files 24% similar despite different names*

#### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="LRF" meta_type="Dexterity FTI" i18n:domain="plone">
-  <property name="title" i18n:translate="">Language Root Folder</property>
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="LIF" i18n:domain="plone">
+  <property name="title" i18n:translate="">Language Independent Folder</property>
   <property name="icon_expr">string:contenttype/folder</property>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" link_target="" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/setuphandlers.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/shared_uuid.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/shared_uuid.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/subscriber.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/subscriber.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/testing.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/test_add_translation.robot` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/test_add_translation.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/robot/test_translate_content.robot` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/robot/test_translate_content.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_alternates.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_alternates.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_api.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_catalog.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_directives.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_form.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_helper_views.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_helper_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_lif.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_lif.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_lrf.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_lrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_menu.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_robot.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_selector.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_selector.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from plone.app.multilingual.browser.selector import NOT_TRANSLATED_YET_TEMPLATE
 from plone.app.multilingual.interfaces import IMultiLanguageExtraOptionsSchema
 from plone.app.multilingual.interfaces import IPloneAppMultilingualInstalled
 from plone.app.multilingual.interfaces import ITG
 from plone.app.multilingual.testing import PAM_FUNCTIONAL_TESTING
 from plone.app.multilingual.testing import PAM_INTEGRATION_PRESET_TESTING
 from plone.app.multilingual.testing import PAM_INTEGRATION_TESTING
+from plone.base.utils import safe_text
 from plone.dexterity.utils import createContentInContainer
 from plone.i18n.interfaces import ILanguageSchema
 from plone.registry.interfaces import IRegistry
 from plone.testing.z2 import Browser
 from Products.CMFCore.utils import getToolByName
-from plone.base.utils import safe_text
 from urllib.parse import parse_qs
 from urllib.parse import urlparse
 from zope.component import getUtility
 from zope.event import notify
 from zope.interface import alsoProvides
 from zope.lifecycleevent import ObjectModifiedEvent
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_setup.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from Acquisition import aq_base
 from plone.app.multilingual.browser.setup import SetupMultilingualSite
-from plone.app.multilingual.browser.vocabularies import (  # noqa: E501
-    AllContentLanguageVocabulary,
-)
+from plone.app.multilingual.browser.vocabularies import AllContentLanguageVocabulary
 from plone.app.multilingual.interfaces import ATTRIBUTE_NAME
 from plone.app.multilingual.interfaces import IPloneAppMultilingualInstalled
-from plone.app.multilingual.interfaces import ITG
-from plone.app.multilingual.interfaces import ITranslatable
 from plone.app.multilingual.testing import PAM_INTEGRATION_PRESET_TESTING
 from plone.app.multilingual.testing import PAM_INTEGRATION_TESTING
 from Products.CMFCore.utils import getToolByName
 from zope.interface import alsoProvides
 
 import unittest
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_sitemap.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_sitemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 
         createContentInContainer(self.portal["es"], "Document", title="Test document")
 
         createContentInContainer(self.portal["en"], "Document", title="Test document")
 
     def uncompress(self, sitemapdata):
         sio = BytesIO(sitemapdata)
-        unziped = GzipFile(fileobj=sio)
-        xml = unziped.read()
-        unziped.close()
+        unzipped = GzipFile(fileobj=sio)
+        xml = unzipped.read()
+        unzipped.close()
         return xml
 
     def test_portalroot_sitemap(self):
         """
         Requests for the sitemap on portalroot return all languages
         """
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_subscribers.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_uninstall.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_uninstall.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/tests/test_vocabularies.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/upgrades.py` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/upgrades.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from Acquisition import aq_base
 from plone.app.multilingual import logger
 from plone.base.interfaces import ILanguage
-from plone.dexterity.interfaces import IDexterityFTI
+from plone.base.utils import unrestricted_construct_instance
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.utils import unrestricted_construct_instance
 from time import time
 from zope.component import getUtility
 
 import transaction
 
 
 SHARED_NAME = "shared"  # old shared folder name
@@ -48,15 +46,15 @@
     for code, name in ltool.listSupportedLanguages():
         if code not in portal:
             continue
 
         older = portal[code]
 
         if older.portal_type == type_name:
-            logger.info(f"'{code}' is alredy a {type_name}, skipping.")
+            logger.info(f"'{code}' is already a {type_name}, skipping.")
             continue
 
         # PHASE 1: rename old language folders
         s2 = time()
         old_id = OLD_PREFIX + older.id
         logger.info(f"{code} - Phase 1: Renaming to '{old_id}' ...")
         portal.manage_renameObject(older.id, old_id)
```

### Comparing `plone.app.multilingual-7.0.0/src/plone/app/multilingual/upgrades.zcml` & `plone.app.multilingual-7.0.1/src/plone/app/multilingual/upgrades.zcml`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,86 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
   <genericsetup:upgradeStep
-      source="1"
-      destination="2"
       title="Update css_registry to render styles for authenticated users only."
       description=""
       profile="plone.app.multilingual:default"
+      source="1"
+      destination="2"
       handler=".upgrades.reimport_css_registry"
       />
 
   <genericsetup:upgradeStep
       title="Migration for new LRF type"
       description="Rename old language folders and copy content into new LRF. Migrate shared folder to portal root."
+      profile="plone.app.multilingual:default"
       source="1"
       destination="2"
       handler="plone.app.multilingual.upgrades.migration_pam_1_to_2"
-      profile="plone.app.multilingual:default"/>
+      />
 
   <genericsetup:registerProfile
       name="to_3"
       title="Update new registry key"
-      directory="profiles/upgrades/to_3"
-      for="plone.base.interfaces.IMigratingPloneSiteRoot"
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="plone.base.interfaces.IMigratingPloneSiteRoot"
+      directory="profiles/upgrades/to_3"
       />
 
   <genericsetup:upgradeStep
+      title="Add new registry entry"
       profile="plone.app.multilingual:default"
       source="2"
       destination="3"
-      title="Add new registry entry"
       handler=".upgrades.upgrade_to_3"
       />
 
   <genericsetup:registerProfile
       name="to_4"
       title="Update bundle registration"
-      directory="profiles/upgrades/to_4"
-      for="plone.base.interfaces.IMigratingPloneSiteRoot"
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="plone.base.interfaces.IMigratingPloneSiteRoot"
+      directory="profiles/upgrades/to_4"
       />
 
   <genericsetup:upgradeStep
+      title="Update bundle registration"
       profile="plone.app.multilingual:default"
       source="3"
       destination="4"
-      title="Update bundle registration"
       handler=".upgrades.upgrade_to_4"
       />
 
   <genericsetup:registerProfile
       name="to_1000"
       title="Update to 1000"
-      directory="profiles/upgrades/to_1000"
-      for="plone.base.interfaces.IMigratingPloneSiteRoot"
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="plone.base.interfaces.IMigratingPloneSiteRoot"
+      directory="profiles/upgrades/to_1000"
       />
 
-  <genericsetup:upgradeSteps source="4"
+  <genericsetup:upgradeSteps
+      profile="plone.app.multilingual:default"
+      source="4"
       destination="1000"
-      profile="plone.app.multilingual:default">
+      >
 
-      <genericsetup:upgradeDepends
+    <genericsetup:upgradeDepends
         title="Add icon expressions"
-        import_profile="plone.app.multilingual:to_1000" />
+        import_profile="plone.app.multilingual:to_1000"
+        />
 
   </genericsetup:upgradeSteps>
 
   <genericsetup:upgradeStep
+      title="Update old layouts"
+      profile="plone.app.multilingual:default"
       source="1000"
       destination="1001"
-      profile="plone.app.multilingual:default"
-      title="Update old layouts"
-      handler=".upgrades.update_old_layouts" />
+      handler=".upgrades.update_old_layouts"
+      />
 
 </configure>
```

### Comparing `plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/PKG-INFO` & `plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.multilingual
-Version: 7.0.0
+Version: 7.0.1
 Summary: Multilingual Plone Content package
 Home-page: https://github.com/plone/plone.app.multilingual
 Author: Ramon Navarro, Victor Fernandez de Alba, awello et al
 Author-email: r.navarro@iskra.cat
 Maintainer: Plone Foundation
 Maintainer-email: releasemanager@plone.org
 License: GPL
@@ -19,15 +19,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Provides-Extra: archetypes
 Provides-Extra: test
 
 .. contents::
 
 
 Introduction
 ============
@@ -192,15 +191,15 @@
 
 Dexterity
 ---------
 
 Users should mark a dexterity content type as translatable by assigning a the multilingual behavior to the definition of the content type either via file system, supermodel or through the web.
 
 
-Marking fields as language independant
+Marking fields as language independent
 ======================================
 
 Archetypes
 ----------
 
 The language independent fields on Archetype-based content are marked the same way as in LinguaPlone::
 
@@ -210,15 +209,15 @@
         ....
         ),
         languageIndependent=True
     ),
 
 .. note::
 
-    If you want to completely remove LinguaPlone of your installation, you should make sure that your code are dependant in any way of LP.
+    If you want to completely remove LinguaPlone of your installation, you should make sure that your code are dependent in any way of LP.
 
 
 Dexterity
 ---------
 
 There are four ways of achieve it.
 
@@ -381,14 +380,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+7.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (11f0db91)
+
+
 7.0.0 (2023-04-06)
 ------------------
 
 Breaking changes:
 
 
 - Move language independent field declarations from plone.app.event to this package.
@@ -712,15 +721,15 @@
 
 Bug fixes:
 
 
 - Remove deprecation warnings in tests.
   Increase readability
   Add code comments.
-  Remove superfluos reindex of "Language" in manager.
+  Remove superfluous reindex of "Language" in manager.
   [jensens] (#256)
 - wrong check for default addview in addtranslation traverser
   [mauro] (#355)
 - Remove any dependency to ``archetypes.multilingual``, since this is a indirection.
   Remove all dependencies that are already part of ``Products.CMFPlone``.
   All version specifications were reduced to use a recent ``Products.CMFPlone``.
   The ``decorator`` dependency is no longer used.
@@ -990,28 +999,28 @@
 
 5.0.5 (2017-04-27)
 ------------------
 
 Bug fixes:
 
 - Remove travis integration because plone.app.mutlilingual is part of plonecore and should be tested there.
-- Fix bug where formcontrols were overlaped by fields.
+- Fix bug where form controls were overlapped by fields.
   [agitator]
 
 - Fix robot tests to work with improved related items widget.
   [thet]
 
 
 5.0.4 (2017-03-26)
 ------------------
 
 New features:
 
 - Add a new view ``@@tg`` for translatable content. It will return the
-  current translation group of the content, matching the bahavior of ``@@uuid``
+  current translation group of the content, matching the behavior of ``@@uuid``
   of ``plone.app.uuid`` returning UUID of the content.  [datakurre]
 
 
 5.0.3 (2017-02-12)
 ------------------
 
 New features:
@@ -1035,15 +1044,15 @@
 
 
 5.0.1 (2017-01-02)
 ------------------
 
 Bug fixes:
 
-- Allow to work in an Archtypes free Plone 5.1.
+- Allow to work in an Archetypes free Plone 5.1.
   [jensens]
 
 - Replace unittest2 with unittest.
   [jensens]
 
 
 5.0 (2016-11-17)
@@ -1133,15 +1142,15 @@
 -------------------
 
 Fixes:
 
 - Wait for visibility of select2 result, instead of time.
   [jensens]
 
-- Workaroud in robot test for TinyMCE overlap bug see
+- Workaround in robot test for TinyMCE overlap bug see
   https://github.com/plone/plone.app.multilingual/issues/227
   for details
   [jensens]
 
 
 3.0.16 (2016-03-31)
 -------------------
@@ -1327,18 +1336,18 @@
 
 - Add more common api functions and test them.
   [jensens]
 
 - Refactor locations of code in dx to bundle stuff at a sane place.
   [jensens]
 
-- Remove BLACKLIST_IDS, with LIF this is superfluos.
+- Remove BLACKLIST_IDS, with LIF this is superfluous.
   [jensens]
 
-- Remove LanguageTool patch, meanwhile superfluos.
+- Remove LanguageTool patch, meanwhile superfluous.
   [jensens]
 
 - Add new ``bootstrap.py`` to support new parameter ``--setuptools-version``.
   [saily]
 
 - Fixed language independent fields in ++addtranslation++
   requires ``plone.z3cform >= 0.8.1``
@@ -1427,15 +1436,15 @@
 - Fix an import issue in ``upgrades.py``
   [saily]
 
 - Add code analysis to ``plone-test-4.x.cfg`` and ``plone-test-5.x.cfg``
   [saily]
 
 - Huge PEP8 and Flake8 cleanup. Please run ``bin/code-analysis`` before
-  commiting. A git pre-commit hook should be added automatically through
+  committing. A git pre-commit hook should be added automatically through
   buildout.
   [saily]
 
 - Ensure ``plone.app.controlpanel.Language`` permission is present.
   [saily]
 
 - Merge ``add.py`` and ``add_translation_form.py`` into one file
@@ -1487,15 +1496,15 @@
   [ksuess]
 
 - Bugfix: p.a.contentmenu fails if access to translation is not permitted.
   Solution: Introduce restricted access and use it in vocabulary for menu.
   [jensens]
 
 - Added ++add++ and factory support using session var to store where it comes
-  from. It maintains the old programatic way so it's possible to create
+  from. It maintains the old programmatic way so it's possible to create
   translations using code.
   [ramon]
 
 - Extend travis integration to test against Plone 4.1, 4.2, 4.3 and
   include following dependencies into tests:
   - ``plone.multilingual``
   - ``plone.multilingualbehavior``
@@ -1505,15 +1514,15 @@
 - plone.app.contenttypes compatibility on setup
   [sneridagh]
 
 - Added French translation
   [bouchardsyl]
 
 - take care to filter out translated contents
-  wich do no have supported language information
+  which do no have supported language information
   [kiorky]
 
 - added support for language neutral objects with country specific language codes
   by checking _combinedlanguagelist too
   [agitator]
 
 
@@ -1576,15 +1585,15 @@
 
 - Add after migration action on view
   [do3cc]
 
 - Multilingual Map
   [ramon]
 
-- Univeral link
+- Universal link
   [ramon]
 
 - Catalog patch bug solving
   [ramon]
 
 - Language selector bug solving
   [sneridagh]
@@ -1610,15 +1619,15 @@
 - Allow to see all content on adding translation
   [ramon]
 
 
 1.0b2 - 2012-07-08
 ------------------
 
-- change language index to Language to LinguaPlone coexistance
+- change language index to Language to LinguaPlone coexistence
   [ramon]
 
 - don't rebuild the complete catalog on installing
   [pbauer]
 
 - add indexes via setuphandler instead of xml to prevents purging on reinstall
   [pbauer]
```

### Comparing `plone.app.multilingual-7.0.0/src/plone.app.multilingual.egg-info/SOURCES.txt` & `plone.app.multilingual-7.0.1/src/plone.app.multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

