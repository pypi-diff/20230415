# Comparing `tmp/plone.app.layout-4.0.2.tar.gz` & `tmp/plone.app.layout-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.layout-4.0.2.tar", last modified: Tue Mar 14 01:06:27 2023, max compression
+gzip compressed data, was "plone.app.layout-4.0.3.tar", last modified: Sat Apr 15 09:04:32 2023, max compression
```

## Comparing `plone.app.layout-4.0.2.tar` & `plone.app.layout-4.0.3.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.979813 plone.app.layout-4.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    60689 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    62357 2023-03-14 01:06:27.979947 plone.app.layout-4.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      740 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.945069 plone.app.layout-4.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      678 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.945374 plone.app.layout-4.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.948000 plone.app.layout-4.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.949588 plone.app.layout-4.0.2/plone/app/layout/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.950712 plone.app.layout-4.0.2/plone/app/layout/analytics/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      329 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.951546 plone.app.layout-4.0.2/plone/app/layout/analytics/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1695 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/tests/analytics.txt
--rw-r--r--   0 maurits    (501) staff       (20)      637 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1025 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/analytics/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      577 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.952342 plone.app.layout-4.0.2/plone/app/layout/dashboard/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/dashboard/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      100 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/dashboard/dashboard.py
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/dashboard/user_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      886 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/favicon_handler.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.954541 plone.app.layout-4.0.2/plone/app/layout/globals/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1404 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9179 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/context.py
--rw-r--r--   0 maurits    (501) staff       (20)     4083 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     6503 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    12280 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     3812 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.956267 plone.app.layout-4.0.2/plone/app/layout/globals/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.956558 plone.app.layout-4.0.2/plone/app/layout/globals/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)       29 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10563 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_context.py
--rw-r--r--   0 maurits    (501) staff       (20)     3885 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     8496 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     6321 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_tools.py
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/globals/tools.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.957659 plone.app.layout-4.0.2/plone/app/layout/icons/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/icons/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1606 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/icons/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5640 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/icons/icons.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/icons/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.959550 plone.app.layout-4.0.2/plone/app/layout/links/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      494 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/author.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1231 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      227 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/favicon.pt
--rw-r--r--   0 maurits    (501) staff       (20)      241 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/rsslink.pt
--rw-r--r--   0 maurits    (501) staff       (20)      320 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/search.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.960653 plone.app.layout-4.0.2/plone/app/layout/links/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      804 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/tests/test_canonical_url.py
--rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/tests/test_favicon_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1402 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/tests/test_rssviewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     7022 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/links/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.961977 plone.app.layout-4.0.2/plone/app/layout/navigation/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      247 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1749 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    14358 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/navtree.py
--rw-r--r--   0 maurits    (501) staff       (20)     2186 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/root.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.962443 plone.app.layout-4.0.2/plone/app/layout/navigation/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      525 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/navigation/tests/test_root.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.963970 plone.app.layout-4.0.2/plone/app/layout/nextprevious/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/nextprevious/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1024 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/nextprevious/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      856 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/nextprevious/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      843 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/nextprevious/links.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/nextprevious/nextprevious.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1611 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/nextprevious/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      322 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.965270 plone.app.layout-4.0.2/plone/app/layout/sitemap/
--rw-r--r--   0 maurits    (501) staff       (20)      159 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      295 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4491 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)      783 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/sitemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.965730 plone.app.layout-4.0.2/plone/app/layout/sitemap/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    11358 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/sitemap/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     1234 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.977074 plone.app.layout-4.0.2/plone/app/layout/viewlets/
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      363 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/anontools.pt
--rw-r--r--   0 maurits    (501) staff       (20)      384 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/colophon.pt
--rw-r--r--   0 maurits    (501) staff       (20)    20548 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    10592 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18946 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     5298 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)      627 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/contentviews.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1390 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/document_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1886 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/document_byline.pt
--rw-r--r--   0 maurits    (501) staff       (20)      980 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/document_contributors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1541 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/document_relateditems.pt
--rw-r--r--   0 maurits    (501) staff       (20)      308 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/document_rights.pt
--rw-r--r--   0 maurits    (501) staff       (20)      114 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/dublin_core.pt
--rw-r--r--   0 maurits    (501) staff       (20)      763 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/globalstatusmessage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1579 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/globalstatusmessage.py
--rw-r--r--   0 maurits    (501) staff       (20)      617 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/history_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      953 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/httpheaders.py
--rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      758 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/keywords.pt
--rw-r--r--   0 maurits    (501) staff       (20)      364 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1243 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/membertools.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1721 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/menu.pt
--rw-r--r--   0 maurits    (501) staff       (20)      698 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/path_bar.pt
--rw-r--r--   0 maurits    (501) staff       (20)      490 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/popup_content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2922 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/review_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1428 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/searchbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      564 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/sections.pt
--rw-r--r--   0 maurits    (501) staff       (20)      587 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/site_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5450 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/social.py
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/social_tags.pt
--rw-r--r--   0 maurits    (501) staff       (20)      252 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/social_tags_body.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.979526 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      667 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2620 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/history.txt
--rw-r--r--   0 maurits    (501) staff       (20)    27918 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_common.py
--rw-r--r--   0 maurits    (501) staff       (20)    14062 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)      590 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5391 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_history.py
--rw-r--r--   0 maurits    (501) staff       (20)     5488 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_social.py
--rw-r--r--   0 maurits    (501) staff       (20)      174 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/tiny_logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)       66 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)      336 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/toc.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2290 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/toolbar.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1779 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/toolbar.py
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone/app/layout/viewlets/viewport.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 01:06:27.947630 plone.app.layout-4.0.2/plone.app.layout.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    62357 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4974 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      552 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/plone.app.layout.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      361 2023-03-14 01:06:27.980594 plone.app.layout-4.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2326 2023-03-14 01:06:27.000000 plone.app.layout-4.0.2/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.489205 plone.app.layout-4.0.3/
+-rw-r--r--   0 gil       (1000) gil       (1000)    60894 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      122 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    62562 2023-04-15 09:04:32.489205 plone.app.layout-4.0.3/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      740 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.477204 plone.app.layout-4.0.3/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      678 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.477204 plone.app.layout-4.0.3/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.478204 plone.app.layout-4.0.3/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.478204 plone.app.layout-4.0.3/plone/app/layout/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.479204 plone.app.layout-4.0.3/plone/app/layout/analytics/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      322 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.479204 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1695 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/analytics.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      637 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/test_doctests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      199 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/view.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1024 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      550 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.479204 plone.app.layout-4.0.3/plone/app/layout/dashboard/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/dashboard/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      100 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/dashboard/dashboard.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      103 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/dashboard/user_actions.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      885 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/favicon_handler.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.480204 plone.app.layout-4.0.3/plone/app/layout/globals/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1327 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     9179 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/context.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4098 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/interface.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6502 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    12280 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/layout.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3805 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/portal.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.481204 plone.app.layout-4.0.3/plone/app/layout/globals/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.481204 plone.app.layout-4.0.3/plone/app/layout/globals/tests/data/
+-rw-r--r--   0 gil       (1000) gil       (1000)       30 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    10563 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_context.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3885 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_interface.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8497 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_layout.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6321 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_portal.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1375 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_tools.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1060 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tools.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.481204 plone.app.layout-4.0.3/plone/app/layout/icons/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1553 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5639 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/icons.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      759 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/interfaces.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.482205 plone.app.layout-4.0.3/plone/app/layout/links/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      523 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/author.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1166 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      284 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/favicon.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      249 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/rsslink.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      363 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/search.pt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.482205 plone.app.layout-4.0.3/plone/app/layout/links/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      803 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/test_canonical_url.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2707 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/test_favicon_viewlet.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1402 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/test_rssviewlet.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7019 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/viewlets.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.483204 plone.app.layout-4.0.3/plone/app/layout/navigation/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      244 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1749 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14357 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/navtree.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2186 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/root.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.483204 plone.app.layout-4.0.3/plone/app/layout/navigation/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      524 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/tests/test_root.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.484204 plone.app.layout-4.0.3/plone/app/layout/nextprevious/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      989 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      856 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      909 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/links.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/nextprevious.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1611 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      323 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/permissions.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.484204 plone.app.layout-4.0.3/plone/app/layout/sitemap/
+-rw-r--r--   0 gil       (1000) gil       (1000)      159 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/README.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      301 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     4491 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      820 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.484204 plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    11362 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/test_sitemap.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1184 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.488205 plone.app.layout-4.0.3/plone/app/layout/viewlets/
+-rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      409 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/anontools.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      445 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/colophon.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    20134 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/common.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10010 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)    18971 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/content.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6137 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/content_history.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      782 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/contentviews.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1239 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_actions.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1978 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_byline.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      980 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_contributors.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1833 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_relateditems.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      375 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_rights.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      139 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/dublin_core.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      793 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1579 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      620 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/history_view.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      953 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/httpheaders.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2331 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      920 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/keywords.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      361 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/logo.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1318 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/membertools.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1816 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/menu.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      811 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/path_bar.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      515 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/popup_content_history.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     3320 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/review_history.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1621 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/searchbox.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      661 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/sections.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      552 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/site_actions.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     5451 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/social.py
+-rw-r--r--   0 gil       (1000) gil       (1000)       80 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/social_tags.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      294 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/social_tags_body.pt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.489205 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      665 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/base.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2621 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/history.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    27962 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_common.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14111 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_content.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      590 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_functional.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5391 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_history.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5586 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_social.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      192 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tiny_logo.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)       66 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/title.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      382 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/toc.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2484 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1779 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.py
+-rw-r--r--   0 gil       (1000) gil       (1000)       79 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/viewport.pt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.478204 plone.app.layout-4.0.3/plone.app.layout.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    62562 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     4974 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      486 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1690 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 09:04:32.490204 plone.app.layout-4.0.3/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2193 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/setup.py
```

### Comparing `plone.app.layout-4.0.2/CHANGES.rst` & `plone.app.layout-4.0.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-04-15)
+------------------
+
+Bug fixes:
+
+
+- Remove Archetypes code from TOC viewlet.
+  @jensens (rm-at-code-from-toc)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (11f0db91)
+
+
 4.0.2 (2023-03-14)
 ------------------
 
 Bug fixes:
 
 
 - Move interface plone.app.layout.navigation.interfaces.INavigationRoot to plone.base.interfaces.siteroot and add a deprecated import to plone.app.layout.
@@ -388,15 +405,15 @@
 3.4.1 (2020-03-09)
 ------------------
 
 Bug fixes:
 
 
 - Analytics viewlet: make webstats_js a property, so that it does not rely on an a call to the update method to be correctly evaluated [ale-rt] (#227)
-- Code formating according to Plone standards (black, isort).
+- Code formatting according to Plone standards (black, isort).
   [thet] (#230)
 - Remove selectedTabs and update method from GlobalSectionsViewlet as both are now unused.
   [thet] (#231)
 - Remove deprecation warnings [ale-rt] (#233)
 - Integrate Plone20200121 hotfix: prevent XSS in title.
   Part of https://plone.org/security/hotfix/20200121/xss-in-the-title-field-on-plone-5-0-and-higher
   [maurits] (#3021)
@@ -423,15 +440,15 @@
 
 3.3.0 (2019-10-12)
 ------------------
 
 New features:
 
 
-- Add a sorrounding div to the webstats js. Fixes #157
+- Add a surrounding div to the webstats js. Fixes #157
   [erral] (#157)
 
 
 Bug fixes:
 
 
 - Fix memory leak on getUserInfo [avoinea] (#204) (#210)
@@ -572,15 +589,15 @@
 ------------------
 
 New features:
 
 - Allow addition of extra body classes via multiple IBodyClassAdapter adapter registrations without the need to overload the ILayoutPolicy view.
   [thet, jensens, agitator]
 
-- Make it easier to override seperator in title viewlet
+- Make it easier to override separator in title viewlet
   [tomgross]
 
 Bug fixes:
 
 - Do not use ``rel="tag"`` attribute on the keywords viewlet as the referenced document is not a tag definition but a search result;
   use ``rel="nofollow"`` instead to avoid search crawlers hammering our sites.
   [hvelarde]
@@ -638,15 +655,15 @@
 New features:
 
 - Added membertools viewlet. If user is not anonymous and toolbar is not visible according to ``is_toolbar_visible`` the viewlet will show at the location of anontools.
   [agitator]
 
 Bug fixes:
 
-- show 'in current section only' before seach input field for a11y reasons. https://github.com/plone/Products.CMFPlone/issues/1619 [polyester]
+- show 'in current section only' before search input field for a11y reasons. https://github.com/plone/Products.CMFPlone/issues/1619 [polyester]
 
 
 2.7.1 (2017-07-03)
 ------------------
 
 Bug fixes:
 
@@ -747,15 +764,15 @@
 
 
 2.6.1 (2016-06-07)
 ------------------
 
 Bug fixes:
 
-- Document byline viewlet is now displayed only to anonymous users if permited by the `Allow anyone to view 'about' information` option in the `Security Settings` of `Site Setup` (closes `CMFPlone#1556`_).
+- Document byline viewlet is now displayed only to anonymous users if permitted by the `Allow anyone to view 'about' information` option in the `Security Settings` of `Site Setup` (closes `CMFPlone#1556`_).
   Code used to show the lock status and history view was removed from the document byline as this information was not available to anonymous users anyway.
   [hvelarde]
 
 
 2.6.0 (2016-05-10)
 ------------------
 
@@ -964,15 +981,15 @@
 
 - always show site root syndication links if enabled
   [vangheem]
 
 - by default, show site logo in social settings
   [vangheem]
 
-- Add aria hidden role to avoid screenreaders to nonesense stop by at the
+- Add aria hidden role to avoid screenreaders to nonsense stop by at the
   toolbar tiny logo [sneridagh]
 
 - Get rid completely of the plone.skip_links viewlet because it already doesn't
   worked OOTB since always and this does not follow modern a11y methods and we
   are dropping support for outdated ways [sneridagh]
 
 - Remove all references to "accesskeys" attributes on templates [sneridagh]
@@ -1295,15 +1312,15 @@
 
 2.3.4 (2013-03-05)
 ------------------
 
 - handle missing feed type so it doesn't throw an error
   [vangheem]
 
-- handle absense of ACTUAL_URL on request.
+- handle absence of ACTUAL_URL on request.
   Fixes https://dev.plone.org/ticket/13173
   [vangheem]
 
 - Also show history on the folder contents view
   [vangheem]
 
 
@@ -1359,28 +1376,28 @@
 2.3 (2012-08-11)
 ----------------
 
 - Change breadcrumb separator to / (slash character) for accessibility, and added SEO benefits.
   see https://dev.plone.org/ticket/12904
   [polyester]
 
-- Add language atribute to presentation.pt for WCAG 2.0 compliance.
+- Add language attribute to presentation.pt for WCAG 2.0 compliance.
   See https://dev.plone.org/ticket/12902
   [rmatt, polyester]
 
 - Display publication date in author byline:
   https://dev.plone.org/ticket/8699
   [vipod]
 
 - Remove hard dependency on ATContentTypes.
   [davisagli]
 
 - Correctly hand action URLs not ending / [phrearch]
 
-- Removed obsolete 'define-macro' and 'define-slot' from viewlet page tempates.
+- Removed obsolete 'define-macro' and 'define-slot' from viewlet page templates.
   Fixes http://dev.plone.org/ticket/11541.
   [kleist]
 
 - nextprevious/nextprevious.pt: Use "view/site_url" instead of deprecated "view/portal_url".
   Closes http://dev.plone.org/ticket/12720.
   [kleist]
 
@@ -1391,15 +1408,15 @@
 2.2.7 (2012-08-11)
 ------------------
 
 - Change breadcrumb separator to / (slash character) for accessibility, and added SEO benefits.
   see https://dev.plone.org/ticket/12904
   [polyester]
 
-- Add language atribute to presentation.pt for WCAG 2.0 compliance.
+- Add language attribute to presentation.pt for WCAG 2.0 compliance.
   See https://dev.plone.org/ticket/12902
   [rmatt, polyester]
 
 - Remove hard dependency on ATContentTypes.
   [davisagli]
 
 - Add body class for each part of url path. plip12905
@@ -1431,15 +1448,15 @@
 - Added a page as a not-js fallback for the user dropdown menu
   [giacomos]
 
 
 2.2.4 (2011-12-03)
 ------------------
 
-- Add the ability for the navtree strategy to suppliment the query.
+- Add the ability for the navtree strategy to supplement the query.
   Fixes a problem where the listing of default pages in navigation
   trees could no longer be enabled.
   [rossp]
 
 
 2.2.3 (2011-10-17)
 ------------------
```

### Comparing `plone.app.layout-4.0.2/PKG-INFO` & `plone.app.layout-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.2
+Version: 4.0.3
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -49,14 +49,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-04-15)
+------------------
+
+Bug fixes:
+
+
+- Remove Archetypes code from TOC viewlet.
+  @jensens (rm-at-code-from-toc)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (11f0db91)
+
+
 4.0.2 (2023-03-14)
 ------------------
 
 Bug fixes:
 
 
 - Move interface plone.app.layout.navigation.interfaces.INavigationRoot to plone.base.interfaces.siteroot and add a deprecated import to plone.app.layout.
@@ -433,15 +450,15 @@
 3.4.1 (2020-03-09)
 ------------------
 
 Bug fixes:
 
 
 - Analytics viewlet: make webstats_js a property, so that it does not rely on an a call to the update method to be correctly evaluated [ale-rt] (#227)
-- Code formating according to Plone standards (black, isort).
+- Code formatting according to Plone standards (black, isort).
   [thet] (#230)
 - Remove selectedTabs and update method from GlobalSectionsViewlet as both are now unused.
   [thet] (#231)
 - Remove deprecation warnings [ale-rt] (#233)
 - Integrate Plone20200121 hotfix: prevent XSS in title.
   Part of https://plone.org/security/hotfix/20200121/xss-in-the-title-field-on-plone-5-0-and-higher
   [maurits] (#3021)
@@ -468,15 +485,15 @@
 
 3.3.0 (2019-10-12)
 ------------------
 
 New features:
 
 
-- Add a sorrounding div to the webstats js. Fixes #157
+- Add a surrounding div to the webstats js. Fixes #157
   [erral] (#157)
 
 
 Bug fixes:
 
 
 - Fix memory leak on getUserInfo [avoinea] (#204) (#210)
@@ -617,15 +634,15 @@
 ------------------
 
 New features:
 
 - Allow addition of extra body classes via multiple IBodyClassAdapter adapter registrations without the need to overload the ILayoutPolicy view.
   [thet, jensens, agitator]
 
-- Make it easier to override seperator in title viewlet
+- Make it easier to override separator in title viewlet
   [tomgross]
 
 Bug fixes:
 
 - Do not use ``rel="tag"`` attribute on the keywords viewlet as the referenced document is not a tag definition but a search result;
   use ``rel="nofollow"`` instead to avoid search crawlers hammering our sites.
   [hvelarde]
@@ -683,15 +700,15 @@
 New features:
 
 - Added membertools viewlet. If user is not anonymous and toolbar is not visible according to ``is_toolbar_visible`` the viewlet will show at the location of anontools.
   [agitator]
 
 Bug fixes:
 
-- show 'in current section only' before seach input field for a11y reasons. https://github.com/plone/Products.CMFPlone/issues/1619 [polyester]
+- show 'in current section only' before search input field for a11y reasons. https://github.com/plone/Products.CMFPlone/issues/1619 [polyester]
 
 
 2.7.1 (2017-07-03)
 ------------------
 
 Bug fixes:
 
@@ -792,15 +809,15 @@
 
 
 2.6.1 (2016-06-07)
 ------------------
 
 Bug fixes:
 
-- Document byline viewlet is now displayed only to anonymous users if permited by the `Allow anyone to view 'about' information` option in the `Security Settings` of `Site Setup` (closes `CMFPlone#1556`_).
+- Document byline viewlet is now displayed only to anonymous users if permitted by the `Allow anyone to view 'about' information` option in the `Security Settings` of `Site Setup` (closes `CMFPlone#1556`_).
   Code used to show the lock status and history view was removed from the document byline as this information was not available to anonymous users anyway.
   [hvelarde]
 
 
 2.6.0 (2016-05-10)
 ------------------
 
@@ -1009,15 +1026,15 @@
 
 - always show site root syndication links if enabled
   [vangheem]
 
 - by default, show site logo in social settings
   [vangheem]
 
-- Add aria hidden role to avoid screenreaders to nonesense stop by at the
+- Add aria hidden role to avoid screenreaders to nonsense stop by at the
   toolbar tiny logo [sneridagh]
 
 - Get rid completely of the plone.skip_links viewlet because it already doesn't
   worked OOTB since always and this does not follow modern a11y methods and we
   are dropping support for outdated ways [sneridagh]
 
 - Remove all references to "accesskeys" attributes on templates [sneridagh]
@@ -1340,15 +1357,15 @@
 
 2.3.4 (2013-03-05)
 ------------------
 
 - handle missing feed type so it doesn't throw an error
   [vangheem]
 
-- handle absense of ACTUAL_URL on request.
+- handle absence of ACTUAL_URL on request.
   Fixes https://dev.plone.org/ticket/13173
   [vangheem]
 
 - Also show history on the folder contents view
   [vangheem]
 
 
@@ -1404,28 +1421,28 @@
 2.3 (2012-08-11)
 ----------------
 
 - Change breadcrumb separator to / (slash character) for accessibility, and added SEO benefits.
   see https://dev.plone.org/ticket/12904
   [polyester]
 
-- Add language atribute to presentation.pt for WCAG 2.0 compliance.
+- Add language attribute to presentation.pt for WCAG 2.0 compliance.
   See https://dev.plone.org/ticket/12902
   [rmatt, polyester]
 
 - Display publication date in author byline:
   https://dev.plone.org/ticket/8699
   [vipod]
 
 - Remove hard dependency on ATContentTypes.
   [davisagli]
 
 - Correctly hand action URLs not ending / [phrearch]
 
-- Removed obsolete 'define-macro' and 'define-slot' from viewlet page tempates.
+- Removed obsolete 'define-macro' and 'define-slot' from viewlet page templates.
   Fixes http://dev.plone.org/ticket/11541.
   [kleist]
 
 - nextprevious/nextprevious.pt: Use "view/site_url" instead of deprecated "view/portal_url".
   Closes http://dev.plone.org/ticket/12720.
   [kleist]
 
@@ -1436,15 +1453,15 @@
 2.2.7 (2012-08-11)
 ------------------
 
 - Change breadcrumb separator to / (slash character) for accessibility, and added SEO benefits.
   see https://dev.plone.org/ticket/12904
   [polyester]
 
-- Add language atribute to presentation.pt for WCAG 2.0 compliance.
+- Add language attribute to presentation.pt for WCAG 2.0 compliance.
   See https://dev.plone.org/ticket/12902
   [rmatt, polyester]
 
 - Remove hard dependency on ATContentTypes.
   [davisagli]
 
 - Add body class for each part of url path. plip12905
@@ -1476,15 +1493,15 @@
 - Added a page as a not-js fallback for the user dropdown menu
   [giacomos]
 
 
 2.2.4 (2011-12-03)
 ------------------
 
-- Add the ability for the navtree strategy to suppliment the query.
+- Add the ability for the navtree strategy to supplement the query.
   Fixes a problem where the listing of default pages in navigation
   trees could no longer be enabled.
   [rossp]
 
 
 2.2.3 (2011-10-17)
 ------------------
```

### Comparing `plone.app.layout-4.0.2/README.rst` & `plone.app.layout-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/docs/LICENSE.GPL` & `plone.app.layout-4.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/docs/LICENSE.txt` & `plone.app.layout-4.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/analytics/tests/analytics.txt` & `plone.app.layout-4.0.3/plone/app/layout/analytics/tests/analytics.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/analytics/tests/test_doctests.py` & `plone.app.layout-4.0.3/plone/app/layout/analytics/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/analytics/view.py` & `plone.app.layout-4.0.3/plone/app/layout/analytics/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from plone.registry.interfaces import IRegistry
 from plone.base.interfaces import ISiteSchema
+from plone.registry.interfaces import IRegistry
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.viewlet.interfaces import IViewlet
 
 
 @implementer(IViewlet)
 class AnalyticsViewlet(BrowserView):
-
     render = ViewPageTemplateFile("view.pt")
 
     def __init__(self, context, request, view, manager):
         super().__init__(context, request)
         self.__parent__ = view
         self.view = view
         self.manager = manager
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/configure.zcml` & `plone.app.layout-4.0.3/plone/app/layout/configure.zcml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
-    <include package=".globals" />
-    <include package=".navigation" />
-    <include package=".viewlets" />
-    <include package=".nextprevious" />
-    <include package=".icons" />
-    <include package=".links" />
-    <include package=".sitemap" />
-    <include package=".analytics" />
+  <include package=".globals" />
+  <include package=".navigation" />
+  <include package=".viewlets" />
+  <include package=".nextprevious" />
+  <include package=".icons" />
+  <include package=".links" />
+  <include package=".sitemap" />
+  <include package=".analytics" />
 
-    <include file="permissions.zcml" />
+  <include file="permissions.zcml" />
 
-    <subscriber
-        handler=".favicon_handler.updateMimetype"
-    />
+  <subscriber handler=".favicon_handler.updateMimetype" />
 
 </configure>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/favicon_handler.py` & `plone.app.layout-4.0.3/plone/app/layout/favicon_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+from plone.base.interfaces import ISiteSchema
 from plone.formwidget.namedfile.converter import b64decode_file
 from plone.registry.interfaces import IRecordModifiedEvent
 from plone.registry.recordsproxy import RecordsProxy
-from plone.base.interfaces import ISiteSchema
 from zope.component import adapter
 
 import mimetypes
 
 
 @adapter(ISiteSchema, IRecordModifiedEvent)
 def updateMimetype(settings: RecordsProxy, event: IRecordModifiedEvent = None):
-
     if event.record.fieldName != "site_favicon" or not event.record.value:
         return
 
     filename = b64decode_file(event.newValue)[0]
     mimetype = mimetypes.guess_type(filename)[0] if filename else None
     if mimetype in ("image/x-icon", None):
         # Override incorrect MIME type registered in both PIL and the
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/configure.zcml` & `plone.app.layout-4.0.3/plone/app/layout/globals/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser">
+    xmlns:browser="http://namespaces.zope.org/browser"
+    >
 
-    <!-- Views with global constants -->
+  <!-- Views with global constants -->
 
-    <browser:page
-        name="plone_interface_info"
-        for="*"
-        permission="zope.Public"
-        class=".interface.InterfaceInformation"
-        allowed_interface=".interfaces.IInterfaceInformation"
-        />
-
-    <browser:page
-        name="plone_layout"
-        for="*"
-        permission="zope.Public"
-        class=".layout.LayoutPolicy"
-        allowed_interface=".interfaces.ILayoutPolicy"
-        />
-
-    <browser:page
-        name="plone_tools"
-        for="*"
-        permission="zope.Public"
-        class=".tools.Tools"
-        allowed_interface=".interfaces.ITools"
-        />
-
-    <browser:page
-        name="plone_context_state"
-        for="*"
-        permission="zope.Public"
-        class=".context.ContextState"
-        allowed_interface=".interfaces.IContextState"
-        />
-
-    <browser:page
-        name="plone_portal_state"
-        for="*"
-        permission="zope.Public"
-        class=".portal.PortalState"
-        allowed_interface=".interfaces.IPortalState"
-        />
-
-    <!-- We need to make the request annotatable for this to work -->
-
-    <class class="ZPublisher.BaseRequest.BaseRequest">
-        <implements interface="zope.annotation.interfaces.IAttributeAnnotatable" />
-    </class>
+  <browser:page
+      name="plone_interface_info"
+      for="*"
+      class=".interface.InterfaceInformation"
+      allowed_interface=".interfaces.IInterfaceInformation"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="plone_layout"
+      for="*"
+      class=".layout.LayoutPolicy"
+      allowed_interface=".interfaces.ILayoutPolicy"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="plone_tools"
+      for="*"
+      class=".tools.Tools"
+      allowed_interface=".interfaces.ITools"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="plone_context_state"
+      for="*"
+      class=".context.ContextState"
+      allowed_interface=".interfaces.IContextState"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="plone_portal_state"
+      for="*"
+      class=".portal.PortalState"
+      allowed_interface=".interfaces.IPortalState"
+      permission="zope.Public"
+      />
+
+  <!-- We need to make the request annotatable for this to work -->
+
+  <class class="ZPublisher.BaseRequest.BaseRequest">
+    <implements interface="zope.annotation.interfaces.IAttributeAnnotatable" />
+  </class>
 
 </configure>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/context.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/context.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .interfaces import IContextState
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from plone.base.interfaces import INavigationRoot
+from plone.base.interfaces import INonStructuralFolder
 from plone.base.utils import pretty_title_or_id
 from plone.memoize.view import memoize
 from plone.portlets.interfaces import ILocalPortletAssignable
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.interfaces import IDynamicType
 from Products.CMFCore.interfaces import ISiteRoot
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDynamicViewFTI.interfaces import IBrowserDefault
-from plone.base.interfaces import INonStructuralFolder
 from Products.Five.browser import BrowserView
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.component import queryAdapter
 from zope.component import queryMultiAdapter
 from zope.interface import implementer
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/interface.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         return iface.providedBy(aq_base(self.context).__class__)
 
     @memoize
     def names_and_descriptions(self, dotted_name, all=0):
         """Returns a list of pairs (name, description) for a given
         interface"""
         iface = resolveInterface(dotted_name)
-        nd = iface.namesAndDescriptions(all=all)
-        return [(n, d.getDoc()) for n, d in nd]
+        data = iface.namesAndDescriptions(all=all)
+        return [(name, desc.getDoc()) for name, desc in data]
 
     @memoize
     def get_interfaces(self):
         """Returns the list of interfaces which are implemented by the object"""
         return tuple(providedBy(aq_base(self.context)).flattened())
 
     def get_base_interface(self):
@@ -82,15 +82,15 @@
         ifaces = self.get_interfaces()
         bases = []
         for iface in ifaces:
             visitBaseInterfaces(iface, bases)
         return [biface for biface in bases if biface not in ifaces]
 
     def get_interface_informations(self, iface):
-        """Gets all useful informations from an iface
+        """Gets all useful information from an iface
 
         * name
         * dotted name
         * trimmed doc string
         * base interfaces
         * methods with signature and trimmed doc string
         * attributes with trimemd doc string
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/interfaces.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """Returns all base interfaces of an object but no direct interfaces
 
         Base interfaces are the interfaces which are the super interfaces of
         the direct interfaces
         """
 
     def get_interface_informations(self, iface):
-        """Gets all useful informations from an iface
+        """Gets all useful information from an iface
 
         * name
         * dotted name
         * trimmed doc string
         * base interfaces
         * methods with signature and trimmed doc string
         * attributes with trimemd doc string
@@ -166,15 +166,15 @@
         called, instead of with /view appended.  We want to avoid that.
         """
 
     def view_template_id():
         """The id of the view template of the context"""
 
     def is_view_template():
-        """Return True if the currentl URL (in the request) refers to the
+        """Return True if the current URL (in the request) refers to the
         standard "view" of the context (i.e. the "view" tab).
         """
 
     def object_url():
         """The URL of the current object"""
 
     def object_title():
@@ -204,15 +204,15 @@
     def is_editable():
         """Whether or not the current object is editable"""
 
     def is_locked():
         """Whether or not the current object is locked"""
 
     def is_toolbar_visible():
-        """Wether toolbar is visible or not in the actual context"""
+        """Whether toolbar is visible or not in the actual context"""
 
     def actions(category):
         """The filtered actions in the context. You can restrict the actions
         to just one category.
         """
 
     def portlet_assignable():
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/layout.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/layout.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from AccessControl import getSecurityManager
 from plone.app.layout.globals.interfaces import IBodyClassAdapter
 from plone.app.layout.globals.interfaces import ILayoutPolicy
 from plone.app.layout.globals.interfaces import IViewView
+from plone.base.interfaces.controlpanel import ILinkSchema
+from plone.base.interfaces.controlpanel import ISiteSchema
 from plone.i18n.normalizer.interfaces import IIDNormalizer
 from plone.memoize.view import memoize
 from plone.portlets.interfaces import IPortletManager
 from plone.portlets.interfaces import IPortletManagerRenderer
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.interfaces.controlpanel import ILinkSchema
-from plone.base.interfaces.controlpanel import ISiteSchema
 from Products.Five.browser.metaconfigure import ViewMixinForTemplates
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.browserpage.viewpagetemplatefile import (
     ViewPageTemplateFile as ZopeViewPageTemplateFile,
 )
 from zope.component import adapter
 from zope.component import getAdapters
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/portal.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/portal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .interfaces import IPortalState
 from Acquisition import aq_inner
 from plone.app.layout.navigation.root import getNavigationRoot
 from plone.app.layout.navigation.root import getNavigationRootObject
+from plone.base.interfaces import IPloneSiteRoot
+from plone.base.interfaces import ISearchSchema
+from plone.base.interfaces import ISiteSchema
 from plone.i18n.interfaces import ILanguageSchema
 from plone.memoize.view import memoize
 from plone.memoize.view import memoize_contextless
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.interfaces import ISiteRoot
 from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.interfaces import IPloneSiteRoot
-from plone.base.interfaces import ISearchSchema
-from plone.base.interfaces import ISiteSchema
 from Products.Five.browser import BrowserView
 from zope.component import getUtility
 from zope.component import providedBy
 from zope.component.hooks import getSite
 from zope.interface import implementer
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_context.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_context.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from plone.base.interfaces import INavigationRoot
 from plone.app.layout.testing import INTEGRATION_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing.helpers import logout
-from plone.locking.interfaces import ILockable
-from Products.CMFDynamicViewFTI.interfaces import IBrowserDefault
+from plone.base.interfaces import INavigationRoot
 from plone.base.interfaces import INonStructuralFolder
 from plone.base.utils import unrestricted_construct_instance
+from plone.locking.interfaces import ILockable
+from Products.CMFDynamicViewFTI.interfaces import IBrowserDefault
 from zope.interface import alsoProvides
 from zope.interface import directlyProvides
 
 import unittest
 
 
 class TestContextStateView(unittest.TestCase):
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_interface.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_layout.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from plone.base.interfaces import INavigationRoot
 from plone.app.layout.testing import INTEGRATION_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing.helpers import logout
+from plone.base.interfaces import INavigationRoot
+from plone.base.interfaces.controlpanel import ILinkSchema
 from plone.portlets.interfaces import IPortletType
 from plone.registry.interfaces import IRegistry
-from plone.base.interfaces.controlpanel import ILinkSchema
 from zope.component import getUtility
 
 import os
 import unittest
 import zope.interface
 
 
@@ -40,15 +40,15 @@
         self.assertEqual(True, self.view.have_portlets("plone.leftcolumn"))
 
     def testDisableColumns(self):
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.app = self.layer["app"]
         # Now add some portlets to be sure we have columns.  For
         # simplicity we want a portlet that has no add form.  Note
-        # that apparently the Calender had no add form until Plone
+        # that apparently the Calendar had no add form until Plone
         # 4.3, but since 4.4 it does, so it is not fit to use here.
         portlet = getUtility(IPortletType, name="portlets.Login")
         mapping_left = self.portal.restrictedTraverse(
             "++contextportlets++plone.leftcolumn"
         )
         mapping_right = self.portal.restrictedTraverse(
             "++contextportlets++plone.rightcolumn"
@@ -106,15 +106,15 @@
         body_class = layout_view.bodyClass(template, view)
         self.assertIn("template-document_view", body_class)
 
         # case 2: even w/o second parameter it has to work
         body_class = layout_view.bodyClass(template, None)
         self.assertIn("template-document_view", body_class)
 
-        # case 3: if theres no template get name from view
+        # case 3: if there's no template get name from view
         body_class = layout_view.bodyClass(None, view)
         self.assertIn("template-view", body_class)
 
     def testBodyClassWithNavigationRoot(self):
         # mark a folder "between" self.folder and self.portal with
         # INavigationRoot
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_portal.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_portal.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from plone.base.interfaces import INavigationRoot
 from plone.app.layout.navigation.root import getNavigationRoot
 from plone.app.layout.testing import INTEGRATION_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing.helpers import logout
-from plone.i18n.interfaces import ILanguageSchema
-from plone.registry.interfaces import IRegistry
+from plone.base.interfaces import INavigationRoot
 from plone.base.interfaces import ISearchSchema
 from plone.base.interfaces import ISiteSchema
+from plone.i18n.interfaces import ILanguageSchema
+from plone.registry.interfaces import IRegistry
 from zope.component import getUtility
 from zope.event import notify
 from zope.i18n.locales import locales
 from zope.traversing.interfaces import BeforeTraverseEvent
 
 import unittest
 import zope.interface
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/tests/test_tools.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/globals/tools.py` & `plone.app.layout-4.0.3/plone/app/layout/globals/tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/icons/configure.zcml` & `plone.app.layout-4.0.3/plone/app/layout/icons/configure.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:browser="http://namespaces.zope.org/browser"
-           xmlns:five="http://namespaces.zope.org/five">
-
-  <adapter for="*
-                zope.publisher.interfaces.browser.IBrowserRequest
-                Products.ZCatalog.CatalogBrains.AbstractCatalogBrain"
-           factory=".icons.CatalogBrainContentIcon"
-           provides=".interfaces.IContentIcon" />
-
-  <adapter for="*
-                zope.publisher.interfaces.browser.IBrowserRequest
-                Products.CMFCore.interfaces.IDynamicType"
-           factory=".icons.CMFContentIcon"
-           provides=".interfaces.IContentIcon" />
-
-  <adapter for="*
-                zope.publisher.interfaces.browser.IBrowserRequest
-                plone.dexterity.interfaces.IDexterityContent"
-           factory=".icons.DefaultContentIcon"
-           provides=".interfaces.IContentIcon" />
-
-
-  <adapter for="*
-                zope.publisher.interfaces.browser.IBrowserRequest
-                Products.CMFCore.TypesTool.FactoryTypeInformation"
-           factory=".icons.FTIContentIcon"
-           provides=".interfaces.IContentIcon" />
-
-  <adapter for="*
-                zope.publisher.interfaces.browser.IBrowserRequest
-                plone.base.interfaces.IPloneSiteRoot"
-           factory=".icons.PloneSiteContentIcon"
-           provides=".interfaces.IContentIcon" />
-
-  <adapter for="*
-                zope.publisher.interfaces.browser.IBrowserRequest
-                *"
-           factory=".icons.DefaultContentIcon"
-           provides=".interfaces.IContentIcon" />
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:browser="http://namespaces.zope.org/browser"
+    xmlns:five="http://namespaces.zope.org/five"
+    >
+
+  <adapter
+      factory=".icons.CatalogBrainContentIcon"
+      provides=".interfaces.IContentIcon"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest
+           Products.ZCatalog.CatalogBrains.AbstractCatalogBrain"
+      />
+
+  <adapter
+      factory=".icons.CMFContentIcon"
+      provides=".interfaces.IContentIcon"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest
+           Products.CMFCore.interfaces.IDynamicType"
+      />
+
+  <adapter
+      factory=".icons.DefaultContentIcon"
+      provides=".interfaces.IContentIcon"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest
+           plone.dexterity.interfaces.IDexterityContent"
+      />
+
+
+  <adapter
+      factory=".icons.FTIContentIcon"
+      provides=".interfaces.IContentIcon"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest
+           Products.CMFCore.TypesTool.FactoryTypeInformation"
+      />
+
+  <adapter
+      factory=".icons.PloneSiteContentIcon"
+      provides=".interfaces.IContentIcon"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest
+           plone.base.interfaces.IPloneSiteRoot"
+      />
+
+  <adapter
+      factory=".icons.DefaultContentIcon"
+      provides=".interfaces.IContentIcon"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest
+           *"
+      />
 
 </configure>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/icons/icons.py` & `plone.app.layout-4.0.3/plone/app/layout/icons/icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     __allow_access_to_unprotected_subobjects__ = True
 
     def __call__(self):
         return self.html_tag()
 
     @memoize
     def html_tag(self):
-
         if not self.url:
             return None
 
         tag = '<img width="{}" height="{}" src="{}"'.format(
             self.width,
             self.height,
             self.url,
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/icons/interfaces.py` & `plone.app.layout-4.0.3/plone/app/layout/icons/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/links/configure.zcml` & `plone.app.layout-4.0.3/plone/app/layout/links/configure.zcml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:browser="http://namespaces.zope.org/browser"
-           xmlns:five="http://namespaces.zope.org/five">
-
-    <browser:viewlet
-        name="plone.links.favicon"
-        manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
-        class=".viewlets.FaviconViewlet"
-        permission="zope2.View"
-        />
-
-    <browser:viewlet
-        name="plone.links.search"
-        manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
-        class=".viewlets.SearchViewlet"
-        permission="zope2.View"
-        />
-
-    <browser:viewlet
-        name="plone.links.author"
-        manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
-        class=".viewlets.AuthorViewlet"
-        permission="zope2.View"
-        />
-
-    <browser:viewlet
-        name="plone.links.RSS"
-        manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
-        class=".viewlets.RSSViewlet"
-        permission="zope2.View"
-        />
-
-    <browser:viewlet
-        name="plone.links.canonical_url"
-        manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
-        class=".viewlets.CanonicalURL"
-        permission="zope2.View"
-        />
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:browser="http://namespaces.zope.org/browser"
+    xmlns:five="http://namespaces.zope.org/five"
+    >
+
+  <browser:viewlet
+      name="plone.links.favicon"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
+      class=".viewlets.FaviconViewlet"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.links.search"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
+      class=".viewlets.SearchViewlet"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.links.author"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
+      class=".viewlets.AuthorViewlet"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.links.RSS"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
+      class=".viewlets.RSSViewlet"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.links.canonical_url"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
+      class=".viewlets.CanonicalURL"
+      permission="zope2.View"
+      />
 
 </configure>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/links/tests/test_canonical_url.py` & `plone.app.layout-4.0.3/plone/app/layout/links/tests/test_canonical_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from plone.app.layout.testing import FUNCTIONAL_TESTING
 from plone.testing.zope import Browser
 
 import unittest
 
 
 class ViewletTestCase(unittest.TestCase):
-
     layer = FUNCTIONAL_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
 
     def test_canonical_url_viewlet(self):
         portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/links/tests/test_favicon_viewlet.py` & `plone.app.layout-4.0.3/plone/app/layout/links/tests/test_favicon_viewlet.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from plone.app.layout.links.viewlets import FaviconViewlet
 from plone.app.layout.testing import FUNCTIONAL_TESTING
 from plone.app.layout.viewlets.tests.base import ViewletsTestCase
+from plone.base.interfaces import ISiteSchema
 from plone.formwidget.namedfile.converter import b64encode_file
 from plone.registry.interfaces import IRegistry
-from plone.base.interfaces import ISiteSchema
 from zope.component import getUtility
 
 
 class TestFaviconViewletView(ViewletsTestCase, FaviconViewlet):
     layer = FUNCTIONAL_TESTING
 
     def setUp(self):
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/links/tests/test_rssviewlet.py` & `plone.app.layout-4.0.3/plone/app/layout/links/tests/test_rssviewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/links/viewlets.py` & `plone.app.layout-4.0.3/plone/app/layout/links/viewlets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from Acquisition import aq_inner
 from plone.app.layout.viewlets import ViewletBase
 from plone.app.uuid.utils import uuidToObject
+from plone.base.interfaces import ISecuritySchema
+from plone.base.interfaces import ISiteSchema
 from plone.base.interfaces import ISiteSyndicationSettings
 from plone.base.interfaces.syndication import IFeedSettings
 from plone.base.utils import safe_bytes
 from plone.formwidget.namedfile.converter import b64decode_file
 from plone.memoize import ram
 from plone.memoize import view
 from plone.memoize.compress import xhtml_compress
 from plone.registry.interfaces import IRegistry
-from plone.base.interfaces import ISecuritySchema
-from plone.base.interfaces import ISiteSchema
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from typing import NoReturn
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.schema.interfaces import IVocabularyFactory
 
 
@@ -32,15 +32,14 @@
             self.site_url,
             get_language(aq_inner(self.context), self.request),
         ]
     )
 
 
 class FaviconViewlet(ViewletBase):
-
     _template = ViewPageTemplateFile("favicon.pt")
     mimetype: str
     favicon_path: str
 
     def init_favicon(self) -> NoReturn:
         registry = getUtility(IRegistry)
         settings: ISiteSchema = registry.forInterface(ISiteSchema, prefix="plone")
@@ -77,24 +76,22 @@
 
     def render(self) -> ViewPageTemplateFile:
         self.init_favicon()
         return xhtml_compress(self._template())
 
 
 class SearchViewlet(ViewletBase):
-
     _template = ViewPageTemplateFile("search.pt")
 
     @ram.cache(render_cachekey)
     def render(self):
         return xhtml_compress(self._template())
 
 
 class AuthorViewlet(ViewletBase):
-
     _template = ViewPageTemplateFile("author.pt")
 
     def update(self):
         super().update()
         self.tools = getMultiAdapter((self.context, self.request), name="plone_tools")
 
     def show(self):
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/navigation/interfaces.py` & `plone.app.layout-4.0.3/plone/app/layout/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/navigation/navtree.py` & `plone.app.layout-4.0.3/plone/app/layout/navigation/navtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     pruneRoot = False
     if strategy is not None:
         rootObject = portalObject.unrestrictedTraverse(rootPath, None)
         if rootObject is not None:
             pruneRoot = not strategy.showChildrenOf(rootObject)
 
-    # Allow the strategy to suppliment the query for keys not already
+    # Allow the strategy to supplement the query for keys not already
     # present in the query such as sorting and omitting default pages
     for key, value in strategy.supplimentQuery.items():
         if key not in query:
             query[key] = value
 
     results = portal_catalog.searchResults(query)
 
@@ -256,15 +256,14 @@
             "currentParent": isCurrentParent,
         }
 
         insert = True
         if not forceInsert and strategy is not None:
             insert = strategy.nodeFilter(newNode)
         if insert:
-
             if strategy is not None:
                 newNode = strategy.decoratorFactory(newNode)
 
             # Tell parent about this item, unless an earlier subtree filter
             # told us not to. If we're forcing the insert, ignore the
             # pruning, but avoid inserting the node twice
             if parentPath in itemPaths:
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/navigation/root.py` & `plone.app.layout-4.0.3/plone/app/layout/navigation/root.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/navigation/tests/test_root.py` & `plone.app.layout-4.0.3/plone/app/layout/navigation/tests/test_root.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from plone.app.layout.navigation.root import getNavigationRootObject
 from plone.app.layout.testing import INTEGRATION_TESTING
 
 import unittest
 
 
 class NavigationRootTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def test_getNavigationRootObject_no_context(self):
         """
         If you don't know the context then you also don't know what the
         navigation root is.
         """
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/nextprevious/configure.zcml` & `plone.app.layout-4.0.3/plone/app/layout/nextprevious/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser">
+    xmlns:browser="http://namespaces.zope.org/browser"
+    >
 
-    <!-- We need this both in the viewlet and in Plone's header for rel links,
+  <!-- We need this both in the viewlet and in Plone's header for rel links,
          so define a view and use it in both places. Note that the actual
          values are request memoized, so the calculations will only be
          performed once.
      -->
 
-    <browser:page
-        for="*"
-        name="plone_nextprevious_view"
-        class=".view.NextPreviousView"
-        permission="zope.Public"
-        allowed_attributes="next previous enabled"
-        />
+  <browser:page
+      name="plone_nextprevious_view"
+      for="*"
+      class=".view.NextPreviousView"
+      allowed_attributes="next previous enabled"
+      permission="zope.Public"
+      />
 
-    <browser:viewlet
-        name="plone.nextprevious"
-        manager="plone.app.layout.viewlets.interfaces.IBelowContent"
-        class=".view.NextPreviousViewlet"
-        permission="zope2.View"
-        />
+  <browser:viewlet
+      name="plone.nextprevious"
+      manager="plone.app.layout.viewlets.interfaces.IBelowContent"
+      class=".view.NextPreviousViewlet"
+      permission="zope2.View"
+      />
 
-    <browser:viewlet
-        name="plone.nextprevious.links"
-        manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
-        class=".view.NextPreviousLinksViewlet"
-        permission="zope2.View"
-        />
+  <browser:viewlet
+      name="plone.nextprevious.links"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHeadLinks"
+      class=".view.NextPreviousLinksViewlet"
+      permission="zope2.View"
+      />
 
 </configure>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/nextprevious/interfaces.py` & `plone.app.layout-4.0.3/plone/app/layout/nextprevious/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/nextprevious/nextprevious.pt` & `plone.app.layout-4.0.3/plone/app/layout/nextprevious/nextprevious.pt`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 <section id="section-next-prev"
-     tal:define="enabled view/enabled|nothing;
-                 isViewTemplate view/isViewTemplate|nothing"
-     tal:condition="python:enabled and isViewTemplate"
-     i18n:domain="plone">
-
-  <tal:block define="portal_url view/site_url;">
+         tal:define="
+           enabled view/enabled|nothing;
+           isViewTemplate view/isViewTemplate|nothing;
+         "
+         tal:condition="python:enabled and isViewTemplate"
+         i18n:domain="plone"
+>
+
+  <tal:block define="
+               portal_url view/site_url;
+             ">
 
     <nav class="pagination justify-content-between"
-         tal:define="next view/next;
-                     previous view/previous"
-         tal:condition="python:previous is not None or next is not None">
-
-          <a class="btn btn-sm btn-outline-secondary align-self-start previous" tal:condition="previous"
-              title="Go to previous item"
-              i18n:attributes="title title_previous_item"
-              tal:attributes="href previous/url">
-            <span class="arrow"></span>
-            <span i18n:translate="label_previous_item" class="label">
+         tal:define="
+           next view/next;
+           previous view/previous;
+         "
+         tal:condition="python:previous is not None or next is not None"
+    >
+
+      <a class="btn btn-sm btn-outline-secondary align-self-start previous"
+         title="Go to previous item"
+         tal:condition="previous"
+         tal:attributes="
+           href previous/url;
+         "
+         i18n:attributes="title title_previous_item"
+      >
+        <span class="arrow"></span>
+        <span class="label"
+              i18n:translate="label_previous_item"
+        >
               Previous:
-              <span i18n:name="itemtitle" tal:replace="previous/title" />
-            </span>
-          </a>
-
-          <a class="btn btn-sm btn-outline-secondary align-self-end next" tal:condition="next" title="Go to next item"
-              i18n:attributes="title title_next_item"
-              tal:attributes="href next/url">
-            <span i18n:translate="label_next_item" class="label">
+          <span tal:replace="previous/title"
+                i18n:name="itemtitle"
+          ></span>
+        </span>
+      </a>
+
+      <a class="btn btn-sm btn-outline-secondary align-self-end next"
+         title="Go to next item"
+         tal:condition="next"
+         tal:attributes="
+           href next/url;
+         "
+         i18n:attributes="title title_next_item"
+      >
+        <span class="label"
+              i18n:translate="label_next_item"
+        >
               Next:
-              <span i18n:name="itemtitle" tal:replace="next/title" />
-            </span>
-            <span class="arrow"></span>
-          </a>
+          <span tal:replace="next/title"
+                i18n:name="itemtitle"
+          ></span>
+        </span>
+        <span class="arrow"></span>
+      </a>
 
 
     </nav>
 
   </tal:block>
 
 </section>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/nextprevious/view.py` & `plone.app.layout-4.0.3/plone/app/layout/nextprevious/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/sitemap/sitemap.py` & `plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from BTrees.OOBTree import OOBTree
 from gzip import GzipFile
 from io import BytesIO
+from plone.base.interfaces import IPloneSiteRoot
+from plone.base.interfaces import ISiteSchema
 from plone.memoize import ram
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.interfaces import IPloneSiteRoot
-from plone.base.interfaces import ISiteSchema
 from Products.Five import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.component import getUtility
 from zope.publisher.interfaces import NotFound
 
 
 def _render_cachekey(fun, self):
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/sitemap/sitemap.xml` & `plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 7572 6c73 6574 2078  F-8"?>.<urlset x
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
+00000020: 662d 3822 3f3e 0a3c 7572 6c73 6574 2078  f-8"?>.<urlset x
 00000030: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
 00000040: 2e73 6974 656d 6170 732e 6f72 672f 7363  .sitemaps.org/sc
 00000050: 6865 6d61 732f 7369 7465 6d61 702f 302e  hemas/sitemap/0.
 00000060: 3922 0a20 2020 2020 2020 2078 6d6c 6e73  9".        xmlns
 00000070: 3a74 616c 3d22 6874 7470 3a2f 2f78 6d6c  :tal="http://xml
 00000080: 2e7a 6f70 652e 6f72 672f 6e61 6d65 7370  .zope.org/namesp
 00000090: 6163 6573 2f74 616c 220a 2020 2020 2020  aces/tal".      
@@ -15,35 +15,38 @@
 000000e0: 7873 693a 7363 6865 6d61 4c6f 6361 7469  xsi:schemaLocati
 000000f0: 6f6e 3d22 6874 7470 3a2f 2f77 7777 2e73  on="http://www.s
 00000100: 6974 656d 6170 732e 6f72 672f 7363 6865  itemaps.org/sche
 00000110: 6d61 732f 7369 7465 6d61 702f 302e 3920  mas/sitemap/0.9 
 00000120: 6874 7470 3a2f 2f77 7777 2e73 6974 656d  http://www.sitem
 00000130: 6170 732e 6f72 672f 7363 6865 6d61 732f  aps.org/schemas/
 00000140: 7369 7465 6d61 702f 302e 392f 7369 7465  sitemap/0.9/site
-00000150: 6d61 702e 7873 6422 3e0a 3c75 726c 2074  map.xsd">.<url t
-00000160: 616c 3a72 6570 6561 743d 226f 626a 2076  al:repeat="obj v
-00000170: 6965 772f 6f62 6a65 6374 7322 3e0a 2020  iew/objects">.  
-00000180: 3c6c 6f63 2074 616c 3a63 6f6e 7465 6e74  <loc tal:content
-00000190: 3d22 6f62 6a2f 6c6f 6322 3e75 726c 3c2f  ="obj/loc">url</
-000001a0: 6c6f 633e 0a20 203c 6c61 7374 6d6f 6420  loc>.  <lastmod 
-000001b0: 7461 6c3a 636f 6e64 6974 696f 6e3d 226f  tal:condition="o
-000001c0: 626a 2f6c 6173 746d 6f64 207c 206e 6f74  bj/lastmod | not
-000001d0: 6869 6e67 220a 2020 2020 2020 2020 2020  hing".          
-000001e0: 7461 6c3a 636f 6e74 656e 743d 226f 626a  tal:content="obj
-000001f0: 2f6c 6173 746d 6f64 223e 6461 7465 206d  /lastmod">date m
-00000200: 6f64 6966 6965 643c 2f6c 6173 746d 6f64  odified</lastmod
-00000210: 3e0a 2020 3c63 6861 6e67 6566 7265 7120  >.  <changefreq 
-00000220: 7461 6c3a 636f 6e64 6974 696f 6e3d 226f  tal:condition="o
-00000230: 626a 2f63 6861 6e67 6566 7265 7120 7c20  bj/changefreq | 
-00000240: 6e6f 7468 696e 6722 0a20 2020 2020 2020  nothing".       
-00000250: 2020 2020 2020 7461 6c3a 636f 6e74 656e        tal:conten
-00000260: 743d 226f 626a 2f63 6861 6e67 6566 7265  t="obj/changefre
-00000270: 7122 3e63 6861 6e67 6520 6672 6571 7565  q">change freque
-00000280: 6e63 793c 2f63 6861 6e67 6566 7265 713e  ncy</changefreq>
-00000290: 0a20 203c 7072 696f 7269 7479 2074 616c  .  <priority tal
-000002a0: 3a63 6f6e 6469 7469 6f6e 3d22 6f62 6a2f  :condition="obj/
-000002b0: 7072 696f 7269 7479 207c 206e 6f74 6869  priority | nothi
-000002c0: 6e67 220a 2020 2020 2020 2020 2020 2074  ng".           t
-000002d0: 616c 3a63 6f6e 7465 6e74 3d22 6f62 6a2f  al:content="obj/
-000002e0: 7072 696f 7269 7479 223e 7072 696f 7269  priority">priori
-000002f0: 7479 3c2f 7072 696f 7269 7479 3e0a 3c2f  ty</priority>.</
-00000300: 7572 6c3e 0a3c 2f75 726c 7365 743e 0a    url>.</urlset>.
+00000150: 6d61 702e 7873 6422 0a3e 0a20 203c 7572  map.xsd".>.  <ur
+00000160: 6c20 7461 6c3a 7265 7065 6174 3d22 6f62  l tal:repeat="ob
+00000170: 6a20 7669 6577 2f6f 626a 6563 7473 223e  j view/objects">
+00000180: 0a20 2020 203c 6c6f 6320 7461 6c3a 636f  .    <loc tal:co
+00000190: 6e74 656e 743d 226f 626a 2f6c 6f63 223e  ntent="obj/loc">
+000001a0: 7572 6c3c 2f6c 6f63 3e0a 2020 2020 3c6c  url</loc>.    <l
+000001b0: 6173 746d 6f64 2074 616c 3a63 6f6e 6469  astmod tal:condi
+000001c0: 7469 6f6e 3d22 6f62 6a2f 6c61 7374 6d6f  tion="obj/lastmo
+000001d0: 6420 7c20 6e6f 7468 696e 6722 0a20 2020  d | nothing".   
+000001e0: 2020 2020 2020 2020 2020 7461 6c3a 636f            tal:co
+000001f0: 6e74 656e 743d 226f 626a 2f6c 6173 746d  ntent="obj/lastm
+00000200: 6f64 220a 2020 2020 3e64 6174 6520 6d6f  od".    >date mo
+00000210: 6469 6669 6564 3c2f 6c61 7374 6d6f 643e  dified</lastmod>
+00000220: 0a20 2020 203c 6368 616e 6765 6672 6571  .    <changefreq
+00000230: 2074 616c 3a63 6f6e 6469 7469 6f6e 3d22   tal:condition="
+00000240: 6f62 6a2f 6368 616e 6765 6672 6571 207c  obj/changefreq |
+00000250: 206e 6f74 6869 6e67 220a 2020 2020 2020   nothing".      
+00000260: 2020 2020 2020 2020 2020 7461 6c3a 636f            tal:co
+00000270: 6e74 656e 743d 226f 626a 2f63 6861 6e67  ntent="obj/chang
+00000280: 6566 7265 7122 0a20 2020 203e 6368 616e  efreq".    >chan
+00000290: 6765 2066 7265 7175 656e 6379 3c2f 6368  ge frequency</ch
+000002a0: 616e 6765 6672 6571 3e0a 2020 2020 3c70  angefreq>.    <p
+000002b0: 7269 6f72 6974 7920 7461 6c3a 636f 6e64  riority tal:cond
+000002c0: 6974 696f 6e3d 226f 626a 2f70 7269 6f72  ition="obj/prior
+000002d0: 6974 7920 7c20 6e6f 7468 696e 6722 0a20  ity | nothing". 
+000002e0: 2020 2020 2020 2020 2020 2020 2074 616c               tal
+000002f0: 3a63 6f6e 7465 6e74 3d22 6f62 6a2f 7072  :content="obj/pr
+00000300: 696f 7269 7479 220a 2020 2020 3e70 7269  iority".    >pri
+00000310: 6f72 6974 793c 2f70 7269 6f72 6974 793e  ority</priority>
+00000320: 0a20 203c 2f75 726c 3e0a 3c2f 7572 6c73  .  </url>.</urls
+00000330: 6574 3e0a                                et>.
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/sitemap/tests/test_sitemap.py` & `plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/test_sitemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from DateTime import DateTime
 from gzip import GzipFile
 from io import BytesIO
-from plone.base.interfaces import INavigationRoot
 from plone.app.layout.testing import INTEGRATION_TESTING
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
+from plone.base.interfaces import INavigationRoot
+from plone.base.interfaces import ISearchSchema
+from plone.base.interfaces import ISiteSchema
 from plone.base.utils import safe_text
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.interfaces import ISearchSchema
-from plone.base.interfaces import ISiteSchema
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.interface import alsoProvides
 from zope.publisher.interfaces import INotFound
 
 import unittest
 
@@ -32,15 +32,15 @@
         self.site_settings = registry.forInterface(ISiteSchema, prefix="plone")
         self.site_settings.enable_sitemap = True
         self.sitemap = getMultiAdapter(
             (self.portal, self.portal.REQUEST), name="sitemap.xml.gz"
         )
         self.wftool = getToolByName(self.portal, "portal_workflow")
 
-        # we need to explizitly set a workflow cause we can't rely on the
+        # we need to explicitly set a workflow cause we can't rely on the
         # test environment.
         # `instance test -m plone.app.layout`:
         # wftool._default_chain == 'simple_publication_workflow'
         # `instance test -m plone.app`:
         # wftool._default_chain == 'plone_workflow'
         self.wftool.setChainForPortalTypes(["Document"], "simple_publication_workflow")
 
@@ -67,17 +67,17 @@
         pending = self.portal.pending
         self.wftool.doActionFor(pending, "submit")
         self.assertTrue("pending" == self.wftool.getInfoFor(pending, "review_state"))
         logout()
 
     def uncompress(self, sitemapdata):
         sio = BytesIO(sitemapdata)
-        unziped = GzipFile(fileobj=sio)
-        xml = unziped.read()
-        unziped.close()
+        unzipped = GzipFile(fileobj=sio)
+        xml = unzipped.read()
+        unzipped.close()
         return safe_text(xml)
 
     def test_disabled(self):
         """
         If the sitemap is disabled throws a 404 error.
         """
         self.site_settings.enable_sitemap = False
@@ -262,10 +262,10 @@
             self.portal.published, idxs=["modified", "is_default_page", "effective"]
         )
         logout()
 
         xml = self.uncompress(self.sitemap())
         self.assertFalse("<loc>http://nohost/plone/folder/default</loc>" in xml)
         self.assertTrue("<loc>http://nohost/plone/folder</loc>" in xml)
-        self.assertTrue("<lastmod>2001-01-01T" in xml)
+        self.assertTrue("<lastmod >2001-01-01T" in xml)
         self.assertTrue("<loc>http://nohost/plone</loc>" in xml)
         self.assertFalse("<loc>http://nohost/plone/published</loc>" in xml)
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/testing.py` & `plone.app.layout-4.0.3/plone/app/layout/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import TEST_USER_ID
-from plone.app.testing import TEST_USER_PASSWORD
 from plone.base.utils import unrestricted_construct_instance
 
 
 class Fixture(PloneSandboxLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load ZCML
         import plone.app.layout
 
         self.loadZCML(package=plone.app.layout)
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/common.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from Acquisition import aq_inner
 from collections import defaultdict
 from functools import total_ordering
 from html import escape
 from plone.app.layout.globals.interfaces import IViewView
 from plone.app.layout.navigation.root import getNavigationRoot
 from plone.base import PloneMessageFactory as _
+from plone.base.interfaces import IPloneSiteRoot
+from plone.base.interfaces import ISearchSchema
+from plone.base.interfaces import ISiteSchema
+from plone.base.interfaces.controlpanel import INavigationSchema
 from plone.base.utils import safe_text
 from plone.i18n.interfaces import ILanguageSchema
 from plone.memoize.view import memoize
 from plone.protect.utils import addTokenToUrl
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
-from plone.base.interfaces import IPloneSiteRoot
-from plone.base.interfaces import ISearchSchema
-from plone.base.interfaces import ISiteSchema
-from plone.base.interfaces.controlpanel import INavigationSchema
 from Products.CMFPlone.utils import getSiteLogo
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from urllib.parse import unquote
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
@@ -80,15 +80,15 @@
         """Check for equality"""
         return id(self) == id(other)
 
 
 class TitleViewlet(ViewletBase):
     index = ViewPageTemplateFile("title.pt")
 
-    # seperator of page- and portal-title
+    # separator of page- and portal-title
     sep = " &mdash; "
 
     @property
     @memoize
     def site_title_setting(self):
         registry = getUtility(IRegistry)
         site_settings = registry.forInterface(ISiteSchema, prefix="plone", check=False)
@@ -154,27 +154,15 @@
         self.metatags = plone_utils.listMetaTags(context).items()
 
 
 class TableOfContentsViewlet(ViewletBase):
     index = ViewPageTemplateFile("toc.pt")
 
     def update(self):
-        obj = aq_base(self.context)
-        getTableContents = getattr(obj, "getTableContents", None)
-        self.enabled = False
-        if getTableContents is not None:
-            try:
-                self.enabled = getTableContents()
-            except KeyError:
-                # schema not updated yet
-                self.enabled = False
-        # handle dexterity-behavior
-        toc = getattr(obj, "table_of_contents", None)
-        if toc is not None:
-            self.enabled = toc
+        self.enabled = getattr(aq_base(self.context), "table_of_contents", False)
 
 
 class SiteActionsViewlet(ViewletBase):
     index = ViewPageTemplateFile("site_actions.pt")
 
     def update(self):
         context_state = getMultiAdapter(
@@ -405,15 +393,14 @@
         portal_tabs_view = getMultiAdapter(
             (self.context, self.request), name="portal_tabs_view"
         )
         return portal_tabs_view.topLevelTabs()
 
 
 class PersonalBarViewlet(ViewletBase):
-
     homelink_url = ""
     user_name = ""
 
     def update(self):
         super().update()
         context = aq_inner(self.context)
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/configure.zcml` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/configure.zcml`

 * *Files 9% similar despite different names*

```diff
@@ -1,357 +1,361 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
-    <include package="Products.CMFCore" file="permissions.zcml"/>
-
-    <!-- Register viewlet managers - used in plone's main_template -->
-
-    <browser:viewletManager
-        name="plone.httpheaders"
-        provides=".interfaces.IHTTPHeaders"
-        permission="zope.Public"
-        class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.htmlhead"
-        provides=".interfaces.IHtmlHead"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.scripts"
-        provides=".interfaces.IScripts"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.htmlhead.links"
-        provides=".interfaces.IHtmlHeadLinks"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.portaltop"
-        provides=".interfaces.IPortalTop"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.mainnavigation"
-        provides=".interfaces.IMainNavigation"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.globalstatusmessage"
-        provides=".interfaces.IGlobalStatusMessage"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.portalheader"
-        provides=".interfaces.IPortalHeader"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.toolbar"
-        provides=".interfaces.IToolbar"
-        permission="zope2.View"
-        class=".toolbar.ToolbarViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.abovecontent"
-        provides=".interfaces.IAboveContent"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.abovecontenttitle"
-        provides=".interfaces.IAboveContentTitle"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.belowcontenttitle"
-        provides=".interfaces.IBelowContentTitle"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.belowcontentdescription"
-        provides=".interfaces.IBelowContentDescription"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.abovecontentbody"
-        provides=".interfaces.IAboveContentBody"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.belowcontentbody"
-        provides=".interfaces.IBelowContentBody"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.belowcontent"
-        provides=".interfaces.IBelowContent"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <browser:viewletManager
-        name="plone.portalfooter"
-        provides=".interfaces.IPortalFooter"
-        permission="zope2.View"
-        class="plone.app.viewletmanager.manager.OrderedViewletManager"
-        />
-
-    <!-- Define some viewlets -->
-
-    <!-- HTTPHeaders -->
-    <browser:viewlet
-        name="plone.httpcachingheaders"
-        manager=".interfaces.IHTTPHeaders"
-        class=".httpheaders.HTTPCachingHeaders"
-        permission="zope.Public"
-        />
-
-    <!-- The site actions -->
-    <browser:viewlet
-        name="plone.site_actions"
-        manager=".interfaces.IPortalFooter"
-        class=".common.SiteActionsViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- The search box -->
-    <browser:viewlet
-        name="plone.searchbox"
-        manager=".interfaces.IPortalHeader"
-        class=".common.SearchBoxViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- The anontools (login, register) -->
-    <browser:viewlet
-        name="plone.anontools"
-        manager=".interfaces.IPortalHeader"
-        class=".common.PersonalBarViewlet"
-        permission="zope2.View"
-        template="anontools.pt"
-        />
-
-    <!-- The member panel (logout, user actions) -->
-    <browser:viewlet
-        name="plone.membertools"
-        manager=".interfaces.IPortalHeader"
-        class=".common.PersonalBarViewlet"
-        permission="zope2.View"
-        template="membertools.pt"
-        />
-
-    <!-- The logo -->
-    <browser:viewlet
-        name="plone.logo"
-        manager=".interfaces.IPortalHeader"
-        class=".common.LogoViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- The global sections -->
-    <browser:viewlet
-        name="plone.global_sections"
-        manager=".interfaces.IMainNavigation"
-        class=".common.GlobalSectionsViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- Content views (tabs) -->
-    <browser:viewlet
-        name="plone.contentviews"
-        manager=".interfaces.IToolbar"
-        class=".common.ContentViewsViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- Render the browser title -->
-    <browser:viewlet
-        name="plone.htmlhead.title"
-        manager=".interfaces.IHtmlHead"
-        class=".common.TitleViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- Render the Dublin Core metadata -->
-    <browser:viewlet
-        name="plone.htmlhead.dublincore"
-        manager=".interfaces.IHtmlHead"
-        class=".common.DublinCoreViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- Render the social media metadata -->
-    <browser:viewlet
-        name="plone.htmlhead.socialtags"
-        manager=".interfaces.IHtmlHead"
-        class=".social.SocialTagsViewlet"
-        template="social_tags.pt"
-        permission="zope2.View"
-        />
-
-    <!-- Render the social media body tags -->
-    <browser:viewlet
-        name="plone.socialtags"
-        manager=".interfaces.IAboveContentTitle"
-        class=".social.SocialTagsViewlet"
-        template="social_tags_body.pt"
-        permission="zope2.View"
-        />
-
-    <!-- Render the viewport -->
-    <browser:viewlet
-        name="plone.htmlhead.viewport"
-        manager=".interfaces.IHtmlHead"
-        template="viewport.pt"
-        permission="zope2.View"
-        />
-
-    <!-- The related items -->
-    <browser:viewlet
-        name="plone.relateditems"
-        manager=".interfaces.IBelowContentBody"
-        class=".content.ContentRelatedItems"
-        view="plone.app.layout.globals.interfaces.IViewView"
-        permission="zope2.View"
-        />
-
-    <!-- Render the document actions -->
-    <browser:viewlet
-        name="plone.documentactions"
-        manager="plone.app.layout.viewlets.interfaces.IBelowContent"
-        class=".content.DocumentActionsViewlet"
-        permission="zope2.View"
-        />
-
-
-    <!-- Render the workflow history as a view -->
-    <browser:view
-        for="*"
-        name="contenthistory"
-        class=".content.ContentHistoryView"
-        permission="zope2.View"
-        />
-
-    <!-- Render the workflow history for popup -->
-    <browser:page
-        for="*"
-        name="contenthistorypopup"
-        template="popup_content_history.pt"
-        permission="zope2.View"
-        />
-
-    <!-- Render the workflow history contents as a page-->
-    <browser:page
-        for="*"
-        name="historyview"
-        class=".content.HistoryByLineView"
-        permission="cmf.ModifyPortalContent"
-        />
-
-    <!-- The breadcrumbs -->
-    <browser:viewlet
-        name="plone.path_bar"
-        manager=".interfaces.IAboveContent"
-        class=".common.PathBarViewlet"
-        permission="zope2.View"
-        />
-
-    <browser:viewlet
-        name="plone.globalstatusmessage"
-        manager=".interfaces.IGlobalStatusMessage"
-        class=".globalstatusmessage.GlobalStatusMessage"
-        permission="zope2.View"
-        />
-
-    <!-- Render the document byline -->
-    <browser:viewlet
-        name="plone.documentbyline"
-        manager=".interfaces.IBelowContentTitle"
-        class=".content.DocumentBylineViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- Render the contributors section -->
-    <browser:viewlet
-        name="plone.contributors"
-        manager=".interfaces.IBelowContentBody"
-        class=".content.DocumentBylineViewlet"
-        template="document_contributors.pt"
-        permission="zope2.View"
-        />
-
-    <!-- Render the rights section -->
-    <browser:viewlet
-        name="plone.rights"
-        manager=".interfaces.IBelowContentBody"
-        template="document_rights.pt"
-        permission="zope2.View"
-        />
-
-    <!-- Render the keywords -->
-    <browser:viewlet
-        name="plone.keywords"
-        manager=".interfaces.IBelowContentBody"
-        view="plone.app.layout.globals.interfaces.IViewView"
-        template="keywords.pt"
-        permission="zope2.View"
-        />
-
-    <!-- Render lock info -->
-    <browser:viewlet
-        name="plone.lockinfo"
-        manager=".interfaces.IAboveContent"
-        class="plone.locking.browser.info.LockInfoViewlet"
-        permission="cmf.ModifyPortalContent"
-        for="plone.locking.interfaces.ITTWLockable"
-        />
-
-    <!-- Render table of contents -->
-    <browser:viewlet
-        name="plone.tableofcontents"
-        for="plone.app.contenttypes.behaviors.tableofcontents.ITableOfContents"
-        manager=".interfaces.IAboveContentBody"
-        class=".common.TableOfContentsViewlet"
-        permission="zope2.View"
-        />
-
-    <!-- Colophon -->
-    <browser:viewlet
-        name="plone.colophon"
-        for="*"
-        manager=".interfaces.IPortalFooter"
-        template="colophon.pt"
-        permission="zope.Public"
-        />
+  <include
+      package="Products.CMFCore"
+      file="permissions.zcml"
+      />
+
+  <!-- Register viewlet managers - used in plone's main_template -->
+
+  <browser:viewletManager
+      name="plone.httpheaders"
+      provides=".interfaces.IHTTPHeaders"
+      class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
+      permission="zope.Public"
+      />
+
+  <browser:viewletManager
+      name="plone.htmlhead"
+      provides=".interfaces.IHtmlHead"
+      class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.scripts"
+      provides=".interfaces.IScripts"
+      class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.htmlhead.links"
+      provides=".interfaces.IHtmlHeadLinks"
+      class="plone.app.viewletmanager.manager.BaseOrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.portaltop"
+      provides=".interfaces.IPortalTop"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.mainnavigation"
+      provides=".interfaces.IMainNavigation"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.globalstatusmessage"
+      provides=".interfaces.IGlobalStatusMessage"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.portalheader"
+      provides=".interfaces.IPortalHeader"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.toolbar"
+      provides=".interfaces.IToolbar"
+      class=".toolbar.ToolbarViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.abovecontent"
+      provides=".interfaces.IAboveContent"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.abovecontenttitle"
+      provides=".interfaces.IAboveContentTitle"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.belowcontenttitle"
+      provides=".interfaces.IBelowContentTitle"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.belowcontentdescription"
+      provides=".interfaces.IBelowContentDescription"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.abovecontentbody"
+      provides=".interfaces.IAboveContentBody"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.belowcontentbody"
+      provides=".interfaces.IBelowContentBody"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.belowcontent"
+      provides=".interfaces.IBelowContent"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <browser:viewletManager
+      name="plone.portalfooter"
+      provides=".interfaces.IPortalFooter"
+      class="plone.app.viewletmanager.manager.OrderedViewletManager"
+      permission="zope2.View"
+      />
+
+  <!-- Define some viewlets -->
+
+  <!-- HTTPHeaders -->
+  <browser:viewlet
+      name="plone.httpcachingheaders"
+      manager=".interfaces.IHTTPHeaders"
+      class=".httpheaders.HTTPCachingHeaders"
+      permission="zope.Public"
+      />
+
+  <!-- The site actions -->
+  <browser:viewlet
+      name="plone.site_actions"
+      manager=".interfaces.IPortalFooter"
+      class=".common.SiteActionsViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- The search box -->
+  <browser:viewlet
+      name="plone.searchbox"
+      manager=".interfaces.IPortalHeader"
+      class=".common.SearchBoxViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- The anontools (login, register) -->
+  <browser:viewlet
+      name="plone.anontools"
+      manager=".interfaces.IPortalHeader"
+      class=".common.PersonalBarViewlet"
+      template="anontools.pt"
+      permission="zope2.View"
+      />
+
+  <!-- The member panel (logout, user actions) -->
+  <browser:viewlet
+      name="plone.membertools"
+      manager=".interfaces.IPortalHeader"
+      class=".common.PersonalBarViewlet"
+      template="membertools.pt"
+      permission="zope2.View"
+      />
+
+  <!-- The logo -->
+  <browser:viewlet
+      name="plone.logo"
+      manager=".interfaces.IPortalHeader"
+      class=".common.LogoViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- The global sections -->
+  <browser:viewlet
+      name="plone.global_sections"
+      manager=".interfaces.IMainNavigation"
+      class=".common.GlobalSectionsViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Content views (tabs) -->
+  <browser:viewlet
+      name="plone.contentviews"
+      manager=".interfaces.IToolbar"
+      class=".common.ContentViewsViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Render the browser title -->
+  <browser:viewlet
+      name="plone.htmlhead.title"
+      manager=".interfaces.IHtmlHead"
+      class=".common.TitleViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Render the Dublin Core metadata -->
+  <browser:viewlet
+      name="plone.htmlhead.dublincore"
+      manager=".interfaces.IHtmlHead"
+      class=".common.DublinCoreViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Render the social media metadata -->
+  <browser:viewlet
+      name="plone.htmlhead.socialtags"
+      manager=".interfaces.IHtmlHead"
+      class=".social.SocialTagsViewlet"
+      template="social_tags.pt"
+      permission="zope2.View"
+      />
+
+  <!-- Render the social media body tags -->
+  <browser:viewlet
+      name="plone.socialtags"
+      manager=".interfaces.IAboveContentTitle"
+      class=".social.SocialTagsViewlet"
+      template="social_tags_body.pt"
+      permission="zope2.View"
+      />
+
+  <!-- Render the viewport -->
+  <browser:viewlet
+      name="plone.htmlhead.viewport"
+      manager=".interfaces.IHtmlHead"
+      template="viewport.pt"
+      permission="zope2.View"
+      />
+
+  <!-- The related items -->
+  <browser:viewlet
+      name="plone.relateditems"
+      view="plone.app.layout.globals.interfaces.IViewView"
+      manager=".interfaces.IBelowContentBody"
+      class=".content.ContentRelatedItems"
+      permission="zope2.View"
+      />
+
+  <!-- Render the document actions -->
+  <browser:viewlet
+      name="plone.documentactions"
+      manager="plone.app.layout.viewlets.interfaces.IBelowContent"
+      class=".content.DocumentActionsViewlet"
+      permission="zope2.View"
+      />
+
+
+  <!-- Render the workflow history as a view -->
+  <browser:view
+      name="contenthistory"
+      for="*"
+      class=".content.ContentHistoryView"
+      permission="zope2.View"
+      />
+
+  <!-- Render the workflow history for popup -->
+  <browser:page
+      name="contenthistorypopup"
+      for="*"
+      template="popup_content_history.pt"
+      permission="zope2.View"
+      />
+
+  <!-- Render the workflow history contents as a page-->
+  <browser:page
+      name="historyview"
+      for="*"
+      class=".content.HistoryByLineView"
+      permission="cmf.ModifyPortalContent"
+      />
+
+  <!-- The breadcrumbs -->
+  <browser:viewlet
+      name="plone.path_bar"
+      manager=".interfaces.IAboveContent"
+      class=".common.PathBarViewlet"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.globalstatusmessage"
+      manager=".interfaces.IGlobalStatusMessage"
+      class=".globalstatusmessage.GlobalStatusMessage"
+      permission="zope2.View"
+      />
+
+  <!-- Render the document byline -->
+  <browser:viewlet
+      name="plone.documentbyline"
+      manager=".interfaces.IBelowContentTitle"
+      class=".content.DocumentBylineViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Render the contributors section -->
+  <browser:viewlet
+      name="plone.contributors"
+      manager=".interfaces.IBelowContentBody"
+      class=".content.DocumentBylineViewlet"
+      template="document_contributors.pt"
+      permission="zope2.View"
+      />
+
+  <!-- Render the rights section -->
+  <browser:viewlet
+      name="plone.rights"
+      manager=".interfaces.IBelowContentBody"
+      template="document_rights.pt"
+      permission="zope2.View"
+      />
+
+  <!-- Render the keywords -->
+  <browser:viewlet
+      name="plone.keywords"
+      view="plone.app.layout.globals.interfaces.IViewView"
+      manager=".interfaces.IBelowContentBody"
+      template="keywords.pt"
+      permission="zope2.View"
+      />
+
+  <!-- Render lock info -->
+  <browser:viewlet
+      name="plone.lockinfo"
+      for="plone.locking.interfaces.ITTWLockable"
+      manager=".interfaces.IAboveContent"
+      class="plone.locking.browser.info.LockInfoViewlet"
+      permission="cmf.ModifyPortalContent"
+      />
+
+  <!-- Render table of contents -->
+  <browser:viewlet
+      name="plone.tableofcontents"
+      for="plone.app.contenttypes.behaviors.tableofcontents.ITableOfContents"
+      manager=".interfaces.IAboveContentBody"
+      class=".common.TableOfContentsViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Colophon -->
+  <browser:viewlet
+      name="plone.colophon"
+      for="*"
+      manager=".interfaces.IPortalFooter"
+      template="colophon.pt"
+      permission="zope.Public"
+      />
 
 </configure>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/content.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/content.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 from plone.app.multilingual.browser.vocabularies import translated_languages
 from plone.app.multilingual.interfaces import ITranslatable
 from plone.app.multilingual.interfaces import ITranslationManager
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import ISecuritySchema
 from plone.base.interfaces import ISiteSchema
 from plone.base.utils import base_hasattr
+from plone.base.utils import logger
 from plone.memoize.instance import memoize
 from plone.memoize.view import memoize_contextless
 from plone.protect.authenticator import createToken
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import _checkPermission
 from Products.CMFCore.utils import getToolByName
 from Products.CMFCore.WorkflowCore import WorkflowException
 from Products.CMFEditions.Permissions import AccessPreviousVersions
-from Products.CMFPlone.utils import log
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from urllib.parse import urlencode
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
 from zope.deprecation import deprecation
 
-import logging
 import pkg_resources
 
 
 try:
     pkg_resources.get_distribution("plone.app.relationfield")
 except pkg_resources.DistributionNotFound:
     HAS_RELATIONFIELD = False
@@ -42,41 +41,43 @@
     HAS_RELATIONFIELD = True
 
 # XXX needs refactoring, since Plone 5 we have PAM in core.
 HAS_PAM = True
 
 
 class DocumentActionsViewlet(ViewletBase):
-
     index = ViewPageTemplateFile("document_actions.pt")
 
     def update(self):
         super().update()
 
         self.context_state = getMultiAdapter(
             (self.context, self.request), name="plone_context_state"
         )
         self.actions = self.context_state.actions("document_actions")
 
 
 class DocumentBylineViewlet(ViewletBase):
-
     index = ViewPageTemplateFile("document_byline.pt")
 
     def update(self):
         super().update()
         self.anonymous = self.portal_state.anonymous()
 
     @property
-    @deprecation.deprecate("The context_state property is unused and will be removed in Plone 7")
+    @deprecation.deprecate(
+        "The context_state property is unused and will be removed in Plone 7"
+    )
     def context_state(self):
         return getMultiAdapter((self.context, self.request), name="plone_context_state")
 
     @property
-    @deprecation.deprecate("The has_pam property is unused and will be removed in Plone 7")
+    @deprecation.deprecate(
+        "The has_pam property is unused and will be removed in Plone 7"
+    )
     def has_pam(self):
         return HAS_PAM
 
     @property
     @memoize_contextless
     def portal_membership(self):
         return getToolByName(self.context, "portal_membership")
@@ -93,24 +94,28 @@
         registry = getUtility(IRegistry)
         settings = registry.forInterface(
             ISecuritySchema,
             prefix="plone",
         )
         return not self.anonymous or settings.allow_anon_views_about
 
-    @deprecation.deprecate("The creator method is unused and will be removed in Plone 7")
+    @deprecation.deprecate(
+        "The creator method is unused and will be removed in Plone 7"
+    )
     def creator(self):
         return self.context.Creator()
 
     @deprecation.deprecate("The author method is unused and will be removed in Plone 7")
     def author(self):
         membership = getToolByName(self.context, "portal_membership")
         return membership.getMemberInfo(self.creator())
 
-    @deprecation.deprecate("The authorname method is unused and will be removed in Plone 7")
+    @deprecation.deprecate(
+        "The authorname method is unused and will be removed in Plone 7"
+    )
     def authorname(self):
         author = self.author()
         return author and author["fullname"] or self.creator()
 
     @memoize
     def get_member_info(self, user_id):
         return self.portal_membership.getMemberInfo(user_id)
@@ -135,15 +140,17 @@
         )
 
     def isExpired(self):
         if base_hasattr(self.context, "expires"):
             return self.context.expires().isPast()
         return False
 
-    @deprecation.deprecate("The toLocalizedTime method is unused and will be removed in Plone 7")
+    @deprecation.deprecate(
+        "The toLocalizedTime method is unused and will be removed in Plone 7"
+    )
     def toLocalizedTime(self, time, long_format=None, time_only=None):
         """Convert time to localized time"""
         util = getToolByName(self.context, "translation_service")
         return util.ulocalized_time(
             time, long_format, time_only, self.context, domain="plonelocales"
         )
 
@@ -163,15 +170,17 @@
         # check if we have Effective Date set
         date = self.context.EffectiveDate()
         if not date or date == "None":
             return None
 
         return DateTime(date)
 
-    @deprecation.deprecate("The get_translations method is unused and will be removed in Plone 7")
+    @deprecation.deprecate(
+        "The get_translations method is unused and will be removed in Plone 7"
+    )
     def get_translations(self):
         cts = []
         if ITranslatable.providedBy(self.context):
             t_langs = translated_languages(self.context)
             context_translations = ITranslationManager(self.context).get_translations()
             for lang in t_langs:
                 cts.append(
@@ -304,15 +313,14 @@
                     )
                 )
 
         return cts
 
 
 class ContentRelatedItems(ViewletBase):
-
     index = ViewPageTemplateFile("document_relateditems.pt")
 
     def related_items(self):
         context = aq_inner(self.context)
         res = ()
 
         # Archetypes
@@ -361,15 +369,14 @@
             # the query will return an empty list if the user
             # has no permission to see the target object
             brains.extend(catalog(path=dict(query=path, depth=0)))
         return brains
 
 
 class WorkflowHistoryViewlet(ViewletBase):
-
     index = ViewPageTemplateFile("review_history.pt")
 
     @memoize
     def getUserInfo(self, userid):
         actor = dict(fullname=userid)
         mt = getToolByName(self.context, "portal_membership")
         info = mt.getMemberInfo(userid)
@@ -426,25 +433,23 @@
                     r["actor"] = {"username": anon, "fullname": anon}
                     r["actor_home"] = ""
                 else:
                     r.update(self.getUserInfo(actorid))
             review_history.reverse()
 
         except WorkflowException:
-            log(
-                "plone.app.layout.viewlets.content: "
-                "%s has no associated workflow" % context.absolute_url(),
-                severity=logging.DEBUG,
+            logger.debug(
+                "plone.app.layout.viewlets.content: %s has no associated workflow",
+                context.absolute_url(),
             )
 
         return review_history
 
 
 class ContentHistoryViewlet(WorkflowHistoryViewlet):
-
     index = ViewPageTemplateFile("content_history.pt")
 
     def revisionHistory(self):
         context = aq_inner(self.context)
         if not _checkPermission(AccessPreviousVersions, context):
             return []
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/content_history.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/content_history.pt`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,162 @@
-<div i18n:domain="plone"
-     tal:define="history view/fullHistory;"
-     tal:omit-tag="">
-     <div tal:condition="not: history">—</div>
+<div tal:define="
+       history view/fullHistory;
+     "
+     tal:omit-tag=""
+     i18n:domain="plone"
+>
+  <div tal:condition="not: history">&mdash;</div>
 
-    <table class="table" id="history-list" tal:condition="history"
-        summary="Content history"
-        i18n:attributes="summary summary_content_history;">
-        <tbody>
-            <tr class="odd">
-                <th i18n:translate="">What</th>
-                <th i18n:translate="">View</th>
-                <th colspan="2" i18n:translate="">Compare</th>
-                <th i18n:translate="">Revert</th>
-            </tr>
-            <tal:block repeat="item history">
-            <tal:historyItem
-                define="rhComments item/comments|nothing;
-                        actor item/actor;
-                        actor_name python:actor and actor.get('fullname','username') or item['actorid'];
-                        actor_home item/actor_home;
-                        action item/transition_title;
-                        action_id python:item['action'] or item['review_state'];
-                        effective item/effective_date|nothing;
-                        effectiveDate python:effective and view.toLocalizedTime(item['effective_date'],long_format=True);
-                        isVersion python:item['type']=='versioning';
-                        icons python:context.restrictedTraverse('@@iconresolver')">
-            <tr class="historyRecord ${python:'table-secondary' if not isVersion else ''}">
-                <td>
-                    <span class="historyByLine">
-                        <tal:action i18n:translate="history_action">
-                            <span class="historyAction" tal:content="action" i18n:translate="" i18n:name="action"
-                               tal:attributes="class string:historyAction state-${action_id}"/>
-                            —
-                            <tal:actor i18n:name="actor">
-                             <a href=""
-                                tal:condition="actor_home"
-                                tal:attributes="href actor_home"
-                                tal:content="actor_name"> runyaga </a>
-                             <span tal:condition="not: actor_home"
-                                   tal:replace="actor_name"/>
-                            </tal:actor>
+  <table class="table"
+         id="history-list"
+         summary="Content history"
+         tal:condition="history"
+         i18n:attributes="summary summary_content_history;"
+  >
+    <tbody>
+      <tr class="odd">
+        <th i18n:translate="">What</th>
+        <th i18n:translate="">View</th>
+        <th colspan="2"
+            i18n:translate=""
+        >Compare</th>
+        <th i18n:translate="">Revert</th>
+      </tr>
+      <tal:block repeat="item history">
+        <tal:historyitem define="
+                           rhComments item/comments|nothing;
+                           actor item/actor;
+                           actor_name python:actor and actor.get('fullname','username') or item['actorid'];
+                           actor_home item/actor_home;
+                           action item/transition_title;
+                           action_id python:item['action'] or item['review_state'];
+                           effective item/effective_date|nothing;
+                           effectiveDate python:effective and view.toLocalizedTime(item['effective_date'],long_format=True);
+                           isVersion python:item['type']=='versioning';
+                           icons python:context.restrictedTraverse('@@iconresolver');
+                         ">
+          <tr class="historyRecord ${python:'table-secondary' if not isVersion else ''}">
+            <td>
+              <span class="historyByLine">
+                <tal:action i18n:translate="history_action">
+                  <span class="historyAction"
+                        tal:content="action"
+                        tal:attributes="
+                          class string:historyAction state-${action_id};
+                        "
+                        i18n:name="action"
+                        i18n:translate=""
+                  ></span>
+                            &mdash;
+                  <tal:actor i18n:name="actor">
+                    <a href=""
+                       tal:condition="actor_home"
+                       tal:content="actor_name"
+                       tal:attributes="
+                         href actor_home;
+                       "
+                    >
+                      runyaga
+                    </a>
+                    <span tal:condition="not: actor_home"
+                          tal:replace="actor_name"
+                    ></span>
+                  </tal:actor>
                             on
-                            <span i18n:translate="" i18n:name="time" tal:content="python:view.toLocalizedTime(item['time'],long_format=True)"/>
-                        </tal:action>
-                        <tal:effective tal:condition="effective|nothing">
-                            (<span i18n:translate="label_publishing_effective" tal:omit-tag="">effective</span>: ${effectiveDate})
-                        </tal:effective>
+                  <span tal:content="python:view.toLocalizedTime(item['time'],long_format=True)"
+                        i18n:name="time"
+                        i18n:translate=""
+                  ></span>
+                </tal:action>
+                <tal:effective tal:condition="effective|nothing">
+                  (<span tal:omit-tag=""
+                        i18n:translate="label_publishing_effective"
+                  >effective</span>: ${effectiveDate})
+                </tal:effective>
 
-                    </span>
-                    <p class="text-muted" tal:condition="rhComments">
-                        <span i18n:translate="label_change_note">Change Note</span>:
-                        <span i18n:translate="" tal:content="rhComments" />
-                    </p>
-                </td>
-                <td>
-                    <span class="historyLinks" tal:condition="isVersion">
-                        <a class="btn btn-primary" href=""
-                            tal:attributes="href item/preview_url"
-                            i18n:translate="title_view_revision">View</a>
-                    </span>
-                </td>
-                <td>
-                    <span class="historyLinks" tal:condition="isVersion">
-                        <a class="btn btn-secondary" href="" tal:attributes="href item/diff_current_url"
-                            tal:condition="exists:item/diff_current_url">
-                            <tal:icon replace="structure python:icons.tag('arrow-up')" />
-                            <span i18n:translate="title_compare_revision">Compare to current</span>
-                        </a>
-                    </span>
-                </td>
-                <td>
-                    <a class="btn btn-secondary" tal:condition="exists:item/diff_previous_url"
-                        tal:attributes="href item/diff_previous_url"
-                        title="Compare with previous revision"
-                        i18n:attributes="title title_compare_previous_revision">
-                        <tal:icon replace="structure python:icons.tag('arrow-down')" />
-                        <span i18n:translate="label_compare" tal:omit-tag="">Compare</span>
-                    </a>
-                </td>
-                <td>
-                    <span class="historyTools" tal:condition="isVersion">
-                    <form action="" method="post" tal:condition="item/revert_url" tal:attributes="action item/revert_url">
-                        <input type="hidden" name="version_id" value="" tal:attributes="value item/version_id" />
-                        <button class="btn btn-warning" type="submit"
-                                tal:condition="exists:item/diff_current_url"
-                                i18n:translate="title_revert_revision">Revert to this revision</button>
-                    </form>
-                    </span>
-                </td>
-            </tr>
-            </tal:historyItem>
-            </tal:block>
-        </tbody>
-    </table>
+              </span>
+              <p class="text-muted"
+                 tal:condition="rhComments"
+              >
+                <span i18n:translate="label_change_note">Change Note</span>:
+                <span tal:content="rhComments"
+                      i18n:translate=""
+                ></span>
+              </p>
+            </td>
+            <td>
+              <span class="historyLinks"
+                    tal:condition="isVersion"
+              >
+                <a class="btn btn-primary"
+                   href=""
+                   tal:attributes="
+                     href item/preview_url;
+                   "
+                   i18n:translate="title_view_revision"
+                >View</a>
+              </span>
+            </td>
+            <td>
+              <span class="historyLinks"
+                    tal:condition="isVersion"
+              >
+                <a class="btn btn-secondary"
+                   href=""
+                   tal:condition="exists:item/diff_current_url"
+                   tal:attributes="
+                     href item/diff_current_url;
+                   "
+                >
+                  <tal:icon replace="structure python:icons.tag('arrow-up')" />
+                  <span i18n:translate="title_compare_revision">Compare to current</span>
+                </a>
+              </span>
+            </td>
+            <td>
+              <a class="btn btn-secondary"
+                 title="Compare with previous revision"
+                 tal:condition="exists:item/diff_previous_url"
+                 tal:attributes="
+                   href item/diff_previous_url;
+                 "
+                 i18n:attributes="title title_compare_previous_revision"
+              >
+                <tal:icon replace="structure python:icons.tag('arrow-down')" />
+                <span tal:omit-tag=""
+                      i18n:translate="label_compare"
+                >Compare</span>
+              </a>
+            </td>
+            <td>
+              <span class="historyTools"
+                    tal:condition="isVersion"
+              >
+                <form action=""
+                      method="post"
+                      tal:condition="item/revert_url"
+                      tal:attributes="
+                        action item/revert_url;
+                      "
+                >
+                  <input name="version_id"
+                         type="hidden"
+                         value=""
+                         tal:attributes="
+                           value item/version_id;
+                         "
+                  />
+                  <button class="btn btn-warning"
+                          type="submit"
+                          tal:condition="exists:item/diff_current_url"
+                          i18n:translate="title_revert_revision"
+                  >Revert to this revision</button>
+                </form>
+              </span>
+            </td>
+          </tr>
+        </tal:historyitem>
+      </tal:block>
+    </tbody>
+  </table>
 
 </div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-â
-What                                                       View  Compare          Revert
-                                                                                   Revert
-   â  runyaga   on    (effective: ${effectiveDate})    View Compare  Compare to this
-Change Note:                                                     to               revision
-                                                                 current
+—
+What                                                    View  Compare          Revert
+                                                                                Revert
+   —  runyaga   on    (effective: ${effectiveDate})    View Compare  Compare to this
+Change Note:                                                  to               revision
+                                                              current
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/contentviews.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/contentviews.pt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-<tal:contentviews tal:define="ploneview context/@@plone;"
+<tal:contentviews tal:define="
+                    ploneview context/@@plone;
+                  "
                   tal:condition="ploneview/showToolbar"
-                  i18n:domain="plone">
+                  i18n:domain="plone"
+>
 
-  <tal:block define="actions view/tabSet1;">
-    <div tal:replace="structure python: view.menu_template(actions=actions)" />
+  <tal:block define="
+               actions view/tabSet1;
+             ">
+    <div tal:replace="structure python: view.menu_template(actions=actions)"></div>
   </tal:block>
 
   <li class="border-top my-2">
 
-  <tal:contentmenus>
-    <div tal:replace="structure provider:plone.contentmenu" />
-  </tal:contentmenus>
+    <tal:contentmenus>
+      <div tal:replace="structure provider:plone.contentmenu"></div>
+    </tal:contentmenus>
+
+    <li class="border-top my-2">
+
+      <tal:block define="
+                   actions view/tabSet2;
+                 ">
+        <div tal:replace="structure python: view.menu_template(actions=actions)"></div>
+      </tal:block>
 
-  <li class="border-top my-2">
-
-  <tal:block define="actions view/tabSet2;">
-    <div tal:replace="structure python: view.menu_template(actions=actions)" />
-  </tal:block>
-
-</tal:contentviews>
+    </li></li></tal:contentviews>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/document_actions.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_actions.pt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 <section id="section-document-actions"
-    i18n:domain="plone"
-    tal:condition="view/actions">
+         tal:condition="view/actions"
+         i18n:domain="plone"
+>
 
-    <div class="viewlet viewlet-document-actions">
-        <tal:docactions>
+  <div class="viewlet viewlet-document-actions">
+    <tal:docactions>
 
-            <div class="d-none" i18n:translate="heading_document_actions">
+      <div class="d-none"
+           i18n:translate="heading_document_actions"
+      >
               Document Actions
-            </div>
+      </div>
 
-            <ul class="list-inline"
-                tal:define="normalizeString nocall: context/@@plone/normalizeString;
-                            icons python:context.restrictedTraverse('@@iconresolver');
-                            ">
-                  <li tal:repeat="daction view/actions"
-                      tal:attributes="id python:'document-action-' + normalizeString(daction['id'])">
-                      <a href=""
-                         tal:attributes="href daction/url;
-                                         target daction/link_target|nothing;
-                                         title daction/description|nothing"
-                        >
-                        <tal:icon tal:replace="structure python:icons.tag(daction.get('icon'))" />
-                        <span
-                            i18n:translate=""
-                            tal:replace="daction/title">
+      <ul class="list-inline"
+          tal:define="
+            normalizeString nocall: context/@@plone/normalizeString;
+            icons python:context.restrictedTraverse('@@iconresolver');
+          "
+      >
+        <li tal:repeat="daction view/actions"
+            tal:attributes="
+              id python:'document-action-' + normalizeString(daction['id']);
+            "
+        >
+          <a href=""
+             tal:attributes="
+               href daction/url;
+               target daction/link_target|nothing;
+               title daction/description|nothing;
+             "
+          >
+            <tal:icon tal:replace="structure python:icons.tag(daction.get('icon'))" />
+            <span tal:replace="daction/title"
+                  i18n:translate=""
+            >
                             Menu Title
-                        </span>
-                      </a>
-                  </li>
-            </ul>
-        </tal:docactions>
+            </span>
+          </a>
+        </li>
+      </ul>
+    </tal:docactions>
 
-    </div>
+  </div>
 </section>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/document_byline.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_byline.pt`

 * *Files 18% similar despite different names*

```diff
@@ -19,34 +19,42 @@
            tal:condition="url_path"
         >${fullname}</a>
         <span class="badge rounded-pill bg-light text-dark fw-normal fs-6"
               tal:condition="not:url_path"
         >${fullname}</span>
       </tal:user>
     </tal:for>
-    —
+    &mdash;
   </tal:creators>
 
-  <tal:dates define="published view/pub_date;
-                     modified context/ModificationDate;
-                     show_modification_date python:view.show_modification_date()">
-  <span class="documentPublished" tal:condition="published">
-    <span i18n:translate="box_published">published</span>
-    <span tal:content="python:context.toLocalizedTime(published)">Published</span><tal:sep condition="show_modification_date">,</tal:sep>
-  </span>
+  <tal:dates define="
+               published view/pub_date;
+               modified context/ModificationDate;
+               show_modification_date python:view.show_modification_date();
+             ">
+    <span class="documentPublished"
+          tal:condition="published"
+    >
+      <span i18n:translate="box_published">published</span>
+      <span tal:content="python:context.toLocalizedTime(published)">Published</span><tal:sep condition="show_modification_date">,</tal:sep>
+    </span>
 
-  <span class="documentModified" tal:condition="show_modification_date">
-    <span i18n:translate="box_last_modified">
+    <span class="documentModified"
+          tal:condition="show_modification_date"
+    >
+      <span i18n:translate="box_last_modified">
       last modified
-    </span>
-    <span tal:content="python:context.toLocalizedTime(modified)">
+      </span>
+      <span tal:content="python:context.toLocalizedTime(modified)">
       Modified
+      </span>
     </span>
-  </span>
   </tal:dates>
 
   <tal:expired tal:condition="view/isExpired">
-    —
-    <span class="state-expired" i18n:translate="time_expired">expired</span>
+    &mdash;
+    <span class="state-expired"
+          i18n:translate="time_expired"
+    >expired</span>
   </tal:expired>
 
 </section>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/document_contributors.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_contributors.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/globalstatusmessage.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.pt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-<tal:statusmsg tal:define="icons nocall: context/@@iconresolver"
-               tal:repeat="message python:view.messages">
+<tal:statusmsg tal:define="
+                 icons nocall: context/@@iconresolver;
+               "
+               tal:repeat="message python:view.messages"
+>
 
-    <div tal:define="mtype message/type | nothing;
-                     display_info python:view.display_info_for_mtype(mtype);"
-         tal:condition="mtype"
-         class="portalMessage ${python:display_info['cssclass']}"
-         role="alert">
-        <tal:icon tal:replace="structure python:icons.tag(display_info['icon'], tag_alt=display_info['msg'], tag_class='statusmessage-icon mb-1 me-2')" />
-        <strong>${python:display_info['msg']}</strong>
-        <span class="content"
-              tal:replace="message/message | nothing" i18n:translate="">
+  <div class="portalMessage ${python:display_info['cssclass']}"
+       role="alert"
+       tal:define="
+         mtype message/type | nothing;
+         display_info python:view.display_info_for_mtype(mtype);
+       "
+       tal:condition="mtype"
+  >
+    <tal:icon tal:replace="structure python:icons.tag(display_info['icon'], tag_alt=display_info['msg'], tag_class='statusmessage-icon mb-1 me-2')" />
+    <strong>${python:display_info['msg']}</strong>
+    <span class="content"
+          tal:replace="message/message | nothing"
+          i18n:translate=""
+    >
             The status message.
-        </span>
-    </div>
+    </span>
+  </div>
 
 </tal:statusmsg>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/globalstatusmessage.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/history_view.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/history_view.pt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
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
+      xml:lang="en"
+      i18n:domain="plone"
+>
 
-<body>
+  <body>
 
     <metal:description fill-slot="content-description" />
-    
+
     <metal:content fill-slot="content-core">
-        <h3 i18n:translate="label_history">History</h3>
-        <div tal:replace="structure here/@@contenthistory">Content History</div>
+      <h3 i18n:translate="label_history">History</h3>
+      <div tal:replace="structure here/@@contenthistory">Content History</div>
     </metal:content>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/httpheaders.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/httpheaders.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/interfaces.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/keywords.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/keywords.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 00000000: 3c73 6563 7469 6f6e 2069 643d 2273 6563  <section id="sec
-00000010: 7469 6f6e 2d63 6174 6567 6f72 7922 2069  tion-category" i
-00000020: 3138 6e3a 646f 6d61 696e 3d22 706c 6f6e  18n:domain="plon
-00000030: 6522 2074 616c 3a64 6566 696e 653d 2263  e" tal:define="c
-00000040: 6174 6567 6f72 6965 7320 636f 6e74 6578  ategories contex
-00000050: 742f 5375 626a 6563 747c 6e6f 7468 696e  t/Subject|nothin
-00000060: 673b 2075 726c 5f71 756f 7465 206e 6f63  g; url_quote noc
-00000070: 616c 6c3a 6d6f 6475 6c65 732f 5072 6f64  all:modules/Prod
-00000080: 7563 7473 2e50 7974 686f 6e53 6372 6970  ucts.PythonScrip
-00000090: 7473 2e73 7461 6e64 6172 642f 7572 6c5f  ts.standard/url_
-000000a0: 7175 6f74 6522 2074 616c 3a63 6f6e 6469  quote" tal:condi
-000000b0: 7469 6f6e 3d22 6361 7465 676f 7269 6573  tion="categories
-000000c0: 223e 0a0a 2020 3c64 6976 2063 6c61 7373  ">..  <div class
-000000d0: 3d22 7669 6577 6c65 7420 6b65 7977 6f72  ="viewlet keywor
-000000e0: 6473 2d76 6965 776c 6574 223e 0a0a 2020  ds-viewlet">..  
-000000f0: 2020 3c68 6561 6465 7220 636c 6173 733d    <header class=
-00000100: 2263 6172 642d 7469 746c 6520 7365 6374  "card-title sect
-00000110: 696f 6e2d 6865 6164 696e 6720 642d 6e6f  ion-heading d-no
-00000120: 6e65 2220 6931 386e 3a74 7261 6e73 6c61  ne" i18n:transla
-00000130: 7465 3d22 7365 6374 696f 6e5f 6b65 7977  te="section_keyw
-00000140: 6f72 6473 5f68 6561 6469 6e67 223e 0a20  ords_heading">. 
-00000150: 2020 2020 204b 6579 776f 7264 730a 2020       Keywords.  
-00000160: 2020 3c2f 6865 6164 6572 3e0a 0a20 2020    </header>..   
-00000170: 203c 7461 6c3a 7265 7065 6174 2074 616c   <tal:repeat tal
-00000180: 3a72 6570 6561 743d 2263 6174 6567 6f72  :repeat="categor
-00000190: 7920 6361 7465 676f 7269 6573 223e 0a20  y categories">. 
-000001a0: 2020 203c 6120 6872 6566 3d22 2322 2072     <a href="#" r
-000001b0: 656c 3d22 6e6f 666f 6c6c 6f77 2220 636c  el="nofollow" cl
-000001c0: 6173 733d 2262 746e 2062 746e 2d73 6d20  ass="btn btn-sm 
-000001d0: 6274 6e2d 6f75 746c 696e 652d 7072 696d  btn-outline-prim
-000001e0: 6172 7922 0a20 2020 2020 2074 616c 3a64  ary".      tal:d
-000001f0: 6566 696e 653d 2271 756f 7465 6443 6174  efine="quotedCat
-00000200: 2070 7974 686f 6e3a 7572 6c5f 7175 6f74   python:url_quot
-00000210: 6528 6361 7465 676f 7279 2922 0a20 2020  e(category)".   
-00000220: 2020 2074 616c 3a61 7474 7269 6275 7465     tal:attribute
-00000230: 733d 2268 7265 6620 7374 7269 6e67 3a24  s="href string:$
-00000240: 7b63 6f6e 7465 7874 2f40 4070 6c6f 6e65  {context/@@plone
-00000250: 5f70 6f72 7461 6c5f 7374 6174 652f 6e61  _portal_state/na
-00000260: 7669 6761 7469 6f6e 5f72 6f6f 745f 7572  vigation_root_ur
-00000270: 6c7d 2f40 4073 6561 7263 683f 5375 626a  l}/@@search?Subj
-00000280: 6563 7425 3341 6c69 7374 3d24 7b71 756f  ect%3Alist=${quo
-00000290: 7465 6443 6174 7d22 3e0a 2020 2020 2020  tedCat}">.      
-000002a0: 3c73 7061 6e20 7461 6c3a 636f 6e74 656e  <span tal:conten
-000002b0: 743d 2263 6174 6567 6f72 7922 3e3c 2f73  t="category"></s
-000002c0: 7061 6e3e 0a20 2020 203c 2f61 3e0a 2020  pan>.    </a>.  
-000002d0: 2020 3c2f 7461 6c3a 7265 7065 6174 3e0a    </tal:repeat>.
-000002e0: 0a20 203c 2f64 6976 3e0a 0a3c 2f73 6563  .  </div>..</sec
-000002f0: 7469 6f6e 3e0a                           tion>.
+00000010: 7469 6f6e 2d63 6174 6567 6f72 7922 0a20  tion-category". 
+00000020: 2020 2020 2020 2020 7461 6c3a 6465 6669          tal:defi
+00000030: 6e65 3d22 0a20 2020 2020 2020 2020 2020  ne=".           
+00000040: 6361 7465 676f 7269 6573 2063 6f6e 7465  categories conte
+00000050: 7874 2f53 7562 6a65 6374 7c6e 6f74 6869  xt/Subject|nothi
+00000060: 6e67 3b0a 2020 2020 2020 2020 2020 2075  ng;.           u
+00000070: 726c 5f71 756f 7465 206e 6f63 616c 6c3a  rl_quote nocall:
+00000080: 6d6f 6475 6c65 732f 5072 6f64 7563 7473  modules/Products
+00000090: 2e50 7974 686f 6e53 6372 6970 7473 2e73  .PythonScripts.s
+000000a0: 7461 6e64 6172 642f 7572 6c5f 7175 6f74  tandard/url_quot
+000000b0: 653b 0a20 2020 2020 2020 2020 220a 2020  e;.         ".  
+000000c0: 2020 2020 2020 2074 616c 3a63 6f6e 6469         tal:condi
+000000d0: 7469 6f6e 3d22 6361 7465 676f 7269 6573  tion="categories
+000000e0: 220a 2020 2020 2020 2020 2069 3138 6e3a  ".         i18n:
+000000f0: 646f 6d61 696e 3d22 706c 6f6e 6522 0a3e  domain="plone".>
+00000100: 0a0a 2020 3c64 6976 2063 6c61 7373 3d22  ..  <div class="
+00000110: 7669 6577 6c65 7420 6b65 7977 6f72 6473  viewlet keywords
+00000120: 2d76 6965 776c 6574 223e 0a0a 2020 2020  -viewlet">..    
+00000130: 3c68 6561 6465 7220 636c 6173 733d 2263  <header class="c
+00000140: 6172 642d 7469 746c 6520 7365 6374 696f  ard-title sectio
+00000150: 6e2d 6865 6164 696e 6720 642d 6e6f 6e65  n-heading d-none
+00000160: 220a 2020 2020 2020 2020 2020 2020 6931  ".            i1
+00000170: 386e 3a74 7261 6e73 6c61 7465 3d22 7365  8n:translate="se
+00000180: 6374 696f 6e5f 6b65 7977 6f72 6473 5f68  ction_keywords_h
+00000190: 6561 6469 6e67 220a 2020 2020 3e0a 2020  eading".    >.  
+000001a0: 2020 2020 4b65 7977 6f72 6473 0a20 2020      Keywords.   
+000001b0: 203c 2f68 6561 6465 723e 0a0a 2020 2020   </header>..    
+000001c0: 3c74 616c 3a72 6570 6561 7420 7461 6c3a  <tal:repeat tal:
+000001d0: 7265 7065 6174 3d22 6361 7465 676f 7279  repeat="category
+000001e0: 2063 6174 6567 6f72 6965 7322 3e0a 2020   categories">.  
+000001f0: 2020 2020 3c61 2063 6c61 7373 3d22 6274      <a class="bt
+00000200: 6e20 6274 6e2d 736d 2062 746e 2d6f 7574  n btn-sm btn-out
+00000210: 6c69 6e65 2d70 7269 6d61 7279 220a 2020  line-primary".  
+00000220: 2020 2020 2020 2068 7265 663d 2223 220a         href="#".
+00000230: 2020 2020 2020 2020 2072 656c 3d22 6e6f           rel="no
+00000240: 666f 6c6c 6f77 220a 2020 2020 2020 2020  follow".        
+00000250: 2074 616c 3a64 6566 696e 653d 220a 2020   tal:define=".  
+00000260: 2020 2020 2020 2020 2071 756f 7465 6443           quotedC
+00000270: 6174 2070 7974 686f 6e3a 7572 6c5f 7175  at python:url_qu
+00000280: 6f74 6528 6361 7465 676f 7279 293b 0a20  ote(category);. 
+00000290: 2020 2020 2020 2020 220a 2020 2020 2020          ".      
+000002a0: 2020 2074 616c 3a61 7474 7269 6275 7465     tal:attribute
+000002b0: 733d 220a 2020 2020 2020 2020 2020 2068  s=".           h
+000002c0: 7265 6620 7374 7269 6e67 3a24 7b63 6f6e  ref string:${con
+000002d0: 7465 7874 2f40 4070 6c6f 6e65 5f70 6f72  text/@@plone_por
+000002e0: 7461 6c5f 7374 6174 652f 6e61 7669 6761  tal_state/naviga
+000002f0: 7469 6f6e 5f72 6f6f 745f 7572 6c7d 2f40  tion_root_url}/@
+00000300: 4073 6561 7263 683f 5375 626a 6563 7425  @search?Subject%
+00000310: 3341 6c69 7374 3d24 7b71 756f 7465 6443  3Alist=${quotedC
+00000320: 6174 7d3b 0a20 2020 2020 2020 2020 220a  at};.         ".
+00000330: 2020 2020 2020 3e0a 2020 2020 2020 2020        >.        
+00000340: 3c73 7061 6e20 7461 6c3a 636f 6e74 656e  <span tal:conten
+00000350: 743d 2263 6174 6567 6f72 7922 3e3c 2f73  t="category"></s
+00000360: 7061 6e3e 0a20 2020 2020 203c 2f61 3e0a  pan>.      </a>.
+00000370: 2020 2020 3c2f 7461 6c3a 7265 7065 6174      </tal:repeat
+00000380: 3e0a 0a20 203c 2f64 6976 3e0a 0a3c 2f73  >..  </div>..</s
+00000390: 6563 7469 6f6e 3e0a                      ection>.
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/membertools.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/membertools.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 00000000: 3c64 6976 2069 643d 2270 6f72 7461 6c2d  <div id="portal-
 00000010: 6d65 6d62 6572 746f 6f6c 732d 7772 6170  membertools-wrap
-00000020: 7065 7222 0a20 2020 2020 6931 386e 3a64  per".     i18n:d
-00000030: 6f6d 6169 6e3d 2270 6c6f 6e65 220a 2020  omain="plone".  
-00000040: 2020 2074 616c 3a64 6566 696e 653d 2274     tal:define="t
-00000050: 6f6f 6c62 6172 5f76 6973 6962 6c65 2068  oolbar_visible h
-00000060: 6572 652f 4040 706c 6f6e 655f 636f 6e74  ere/@@plone_cont
-00000070: 6578 745f 7374 6174 652f 6973 5f74 6f6f  ext_state/is_too
-00000080: 6c62 6172 5f76 6973 6962 6c65 3b0a 2020  lbar_visible;.  
-00000090: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000000a0: 7341 6e6f 6e20 7669 6577 2f61 6e6f 6e79  sAnon view/anony
-000000b0: 6d6f 7573 3b22 0a20 2020 2020 7461 6c3a  mous;".     tal:
-000000c0: 636f 6e64 6974 696f 6e3d 2270 7974 686f  condition="pytho
-000000d0: 6e3a 6e6f 7420 6973 416e 6f6e 2061 6e64  n:not isAnon and
-000000e0: 206e 6f74 2074 6f6f 6c62 6172 5f76 6973   not toolbar_vis
-000000f0: 6962 6c65 223e 0a0a 2020 3c70 2063 6c61  ible">..  <p cla
-00000100: 7373 3d22 6869 6464 656e 5374 7275 6374  ss="hiddenStruct
-00000110: 7572 6522 2069 3138 6e3a 7472 616e 736c  ure" i18n:transl
-00000120: 6174 653d 2268 6561 6469 6e67 5f6d 656d  ate="heading_mem
-00000130: 6265 725f 746f 6f6c 7322 3e4d 656d 6265  ber_tools">Membe
-00000140: 7220 746f 6f6c 733c 2f70 3e0a 0a20 203c  r tools</p>..  <
-00000150: 6469 7620 636c 6173 733d 2264 726f 7064  div class="dropd
-00000160: 6f77 6e20 6472 6f70 646f 776e 2d6d 656e  own dropdown-men
-00000170: 752d 656e 6422 2069 643d 2270 6f72 7461  u-end" id="porta
-00000180: 6c2d 6d65 6d62 6572 746f 6f6c 7322 0a20  l-membertools". 
-00000190: 2020 2020 2074 616c 3a63 6f6e 6469 7469       tal:conditi
-000001a0: 6f6e 3d22 7079 7468 6f6e 3a76 6965 772e  on="python:view.
-000001b0: 7573 6572 5f61 6374 696f 6e73 2061 6e64  user_actions and
-000001c0: 206e 6f74 2076 6965 772e 616e 6f6e 796d   not view.anonym
-000001d0: 6f75 7322 3e0a 2020 2020 2020 3c61 2069  ous">.      <a i
-000001e0: 643d 2275 7365 722d 6e61 6d65 220a 2020  d="user-name".  
-000001f0: 2020 2020 2020 2063 6c61 7373 3d22 6472         class="dr
-00000200: 6f70 646f 776e 2d74 6f67 676c 6522 2064  opdown-toggle" d
-00000210: 6174 612d 6273 2d74 6f67 676c 653d 2264  ata-bs-toggle="d
-00000220: 726f 7064 6f77 6e22 0a20 2020 2020 2020  ropdown".       
-00000230: 2020 7461 6c3a 6174 7472 6962 7574 6573    tal:attributes
-00000240: 3d22 6872 6566 2076 6965 772f 686f 6d65  ="href view/home
-00000250: 6c69 6e6b 5f75 726c 223e 0a20 2020 2020  link_url">.     
-00000260: 2020 2020 3c73 7061 6e20 7461 6c3a 7265      <span tal:re
-00000270: 706c 6163 653d 2276 6965 772f 7573 6572  place="view/user
-00000280: 5f6e 616d 6522 3e4a 6f68 6e3c 2f73 7061  _name">John</spa
-00000290: 6e3e 0a20 2020 2020 2020 2020 3c73 7061  n>.         <spa
-000002a0: 6e20 636c 6173 733d 2263 6172 6574 223e  n class="caret">
-000002b0: 3c2f 7370 616e 3e0a 2020 2020 2020 3c2f  </span>.      </
-000002c0: 613e 0a20 2020 2020 203c 756c 2063 6c61  a>.      <ul cla
-000002d0: 7373 3d22 6472 6f70 646f 776e 2d6d 656e  ss="dropdown-men
-000002e0: 7522 2072 6f6c 653d 226d 656e 7522 2061  u" role="menu" a
-000002f0: 7269 612d 6c61 6265 6c6c 6564 6279 3d22  ria-labelledby="
-00000300: 6472 6f70 646f 776e 4d65 6e75 223e 0a20  dropdownMenu">. 
-00000310: 2020 2020 2020 2020 203c 6c69 2074 616c           <li tal
-00000320: 3a72 6570 6561 743d 2261 6374 696f 6e20  :repeat="action 
-00000330: 7669 6577 2f75 7365 725f 6163 7469 6f6e  view/user_action
-00000340: 7322 0a20 2020 2020 2020 2020 2020 2020  s".             
-00000350: 2074 616c 3a61 7474 7269 6275 7465 733d   tal:attributes=
-00000360: 2269 6420 7374 7269 6e67 3a6d 656d 6265  "id string:membe
-00000370: 7274 6f6f 6c73 2d24 7b61 6374 696f 6e2f  rtools-${action/
-00000380: 6964 7d22 3e0a 2020 2020 2020 2020 2020  id}">.          
-00000390: 2020 2020 3c61 2068 7265 663d 2222 2063      <a href="" c
-000003a0: 6c61 7373 3d22 6472 6f70 646f 776e 2d69  lass="dropdown-i
-000003b0: 7465 6d22 0a20 2020 2020 2020 2020 2020  tem".           
-000003c0: 2020 2020 2020 7461 6c3a 6174 7472 6962        tal:attrib
-000003d0: 7574 6573 3d22 6872 6566 2061 6374 696f  utes="href actio
-000003e0: 6e2f 6872 6566 3b0a 2020 2020 2020 2020  n/href;.        
-000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000400: 2020 2020 2020 2020 2074 6172 6765 7420           target 
-00000410: 6163 7469 6f6e 2f6c 696e 6b5f 7461 7267  action/link_targ
-00000420: 6574 7c6e 6f74 6869 6e67 220a 2020 2020  et|nothing".    
-00000430: 2020 2020 2020 2020 2020 2020 2074 616c               tal
-00000440: 3a63 6f6e 7465 6e74 3d22 6163 7469 6f6e  :content="action
-00000450: 2f74 6974 6c65 220a 2020 2020 2020 2020  /title".        
-00000460: 2020 2020 2020 2020 2069 3138 6e3a 7472           i18n:tr
-00000470: 616e 736c 6174 653d 2222 3e0a 2020 2020  anslate="">.    
-00000480: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00000490: 7469 6f6e 2074 6974 6c65 0a20 2020 2020  tion title.     
-000004a0: 2020 2020 2020 2020 203c 2f61 3e0a 2020           </a>.  
-000004b0: 2020 2020 2020 2020 3c2f 6c69 3e0a 2020          </li>.  
-000004c0: 2020 2020 3c2f 756c 3e0a 2020 3c2f 6469      </ul>.  </di
-000004d0: 763e 0a0a 3c2f 6469 763e 0a              v>..</div>.
+00000020: 7065 7222 0a20 2020 2020 7461 6c3a 6465  per".     tal:de
+00000030: 6669 6e65 3d22 0a20 2020 2020 2020 746f  fine=".       to
+00000040: 6f6c 6261 725f 7669 7369 626c 6520 6865  olbar_visible he
+00000050: 7265 2f40 4070 6c6f 6e65 5f63 6f6e 7465  re/@@plone_conte
+00000060: 7874 5f73 7461 7465 2f69 735f 746f 6f6c  xt_state/is_tool
+00000070: 6261 725f 7669 7369 626c 653b 0a20 2020  bar_visible;.   
+00000080: 2020 2020 6973 416e 6f6e 2076 6965 772f      isAnon view/
+00000090: 616e 6f6e 796d 6f75 733b 0a20 2020 2020  anonymous;.     
+000000a0: 220a 2020 2020 2074 616c 3a63 6f6e 6469  ".     tal:condi
+000000b0: 7469 6f6e 3d22 7079 7468 6f6e 3a6e 6f74  tion="python:not
+000000c0: 2069 7341 6e6f 6e20 616e 6420 6e6f 7420   isAnon and not 
+000000d0: 746f 6f6c 6261 725f 7669 7369 626c 6522  toolbar_visible"
+000000e0: 0a20 2020 2020 6931 386e 3a64 6f6d 6169  .     i18n:domai
+000000f0: 6e3d 2270 6c6f 6e65 220a 3e0a 0a20 203c  n="plone".>..  <
+00000100: 7020 636c 6173 733d 2268 6964 6465 6e53  p class="hiddenS
+00000110: 7472 7563 7475 7265 220a 2020 2020 2069  tructure".     i
+00000120: 3138 6e3a 7472 616e 736c 6174 653d 2268  18n:translate="h
+00000130: 6561 6469 6e67 5f6d 656d 6265 725f 746f  eading_member_to
+00000140: 6f6c 7322 0a20 203e 4d65 6d62 6572 2074  ols".  >Member t
+00000150: 6f6f 6c73 3c2f 703e 0a0a 2020 3c64 6976  ools</p>..  <div
+00000160: 2063 6c61 7373 3d22 6472 6f70 646f 776e   class="dropdown
+00000170: 2064 726f 7064 6f77 6e2d 6d65 6e75 2d65   dropdown-menu-e
+00000180: 6e64 220a 2020 2020 2020 2069 643d 2270  nd".       id="p
+00000190: 6f72 7461 6c2d 6d65 6d62 6572 746f 6f6c  ortal-membertool
+000001a0: 7322 0a20 2020 2020 2020 7461 6c3a 636f  s".       tal:co
+000001b0: 6e64 6974 696f 6e3d 2270 7974 686f 6e3a  ndition="python:
+000001c0: 7669 6577 2e75 7365 725f 6163 7469 6f6e  view.user_action
+000001d0: 7320 616e 6420 6e6f 7420 7669 6577 2e61  s and not view.a
+000001e0: 6e6f 6e79 6d6f 7573 220a 2020 3e0a 2020  nonymous".  >.  
+000001f0: 2020 3c61 2063 6c61 7373 3d22 6472 6f70    <a class="drop
+00000200: 646f 776e 2d74 6f67 676c 6522 0a20 2020  down-toggle".   
+00000210: 2020 2020 6964 3d22 7573 6572 2d6e 616d      id="user-nam
+00000220: 6522 0a20 2020 2020 2020 6461 7461 2d62  e".       data-b
+00000230: 732d 746f 6767 6c65 3d22 6472 6f70 646f  s-toggle="dropdo
+00000240: 776e 220a 2020 2020 2020 2074 616c 3a61  wn".       tal:a
+00000250: 7474 7269 6275 7465 733d 220a 2020 2020  ttributes=".    
+00000260: 2020 2020 2068 7265 6620 7669 6577 2f68       href view/h
+00000270: 6f6d 656c 696e 6b5f 7572 6c3b 0a20 2020  omelink_url;.   
+00000280: 2020 2020 220a 2020 2020 3e0a 2020 2020      ".    >.    
+00000290: 2020 3c73 7061 6e20 7461 6c3a 7265 706c    <span tal:repl
+000002a0: 6163 653d 2276 6965 772f 7573 6572 5f6e  ace="view/user_n
+000002b0: 616d 6522 3e4a 6f68 6e3c 2f73 7061 6e3e  ame">John</span>
+000002c0: 0a20 2020 2020 203c 7370 616e 2063 6c61  .      <span cla
+000002d0: 7373 3d22 6361 7265 7422 3e3c 2f73 7061  ss="caret"></spa
+000002e0: 6e3e 0a20 2020 203c 2f61 3e0a 2020 2020  n>.    </a>.    
+000002f0: 3c75 6c20 636c 6173 733d 2264 726f 7064  <ul class="dropd
+00000300: 6f77 6e2d 6d65 6e75 220a 2020 2020 2020  own-menu".      
+00000310: 2020 6172 6961 2d6c 6162 656c 6c65 6462    aria-labelledb
+00000320: 793d 2264 726f 7064 6f77 6e4d 656e 7522  y="dropdownMenu"
+00000330: 0a20 2020 2020 2020 2072 6f6c 653d 226d  .        role="m
+00000340: 656e 7522 0a20 2020 203e 0a20 2020 2020  enu".    >.     
+00000350: 203c 6c69 2074 616c 3a72 6570 6561 743d   <li tal:repeat=
+00000360: 2261 6374 696f 6e20 7669 6577 2f75 7365  "action view/use
+00000370: 725f 6163 7469 6f6e 7322 0a20 2020 2020  r_actions".     
+00000380: 2020 2020 2074 616c 3a61 7474 7269 6275       tal:attribu
+00000390: 7465 733d 220a 2020 2020 2020 2020 2020  tes=".          
+000003a0: 2020 6964 2073 7472 696e 673a 6d65 6d62    id string:memb
+000003b0: 6572 746f 6f6c 732d 247b 6163 7469 6f6e  ertools-${action
+000003c0: 2f69 647d 3b0a 2020 2020 2020 2020 2020  /id};.          
+000003d0: 220a 2020 2020 2020 3e0a 2020 2020 2020  ".      >.      
+000003e0: 2020 3c61 2063 6c61 7373 3d22 6472 6f70    <a class="drop
+000003f0: 646f 776e 2d69 7465 6d22 0a20 2020 2020  down-item".     
+00000400: 2020 2020 2020 6872 6566 3d22 220a 2020        href="".  
+00000410: 2020 2020 2020 2020 2074 616c 3a63 6f6e           tal:con
+00000420: 7465 6e74 3d22 6163 7469 6f6e 2f74 6974  tent="action/tit
+00000430: 6c65 220a 2020 2020 2020 2020 2020 2074  le".           t
+00000440: 616c 3a61 7474 7269 6275 7465 733d 220a  al:attributes=".
+00000450: 2020 2020 2020 2020 2020 2020 2068 7265               hre
+00000460: 6620 6163 7469 6f6e 2f68 7265 663b 0a20  f action/href;. 
+00000470: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00000480: 6574 2061 6374 696f 6e2f 6c69 6e6b 5f74  et action/link_t
+00000490: 6172 6765 747c 6e6f 7468 696e 673b 0a20  arget|nothing;. 
+000004a0: 2020 2020 2020 2020 2020 220a 2020 2020            ".    
+000004b0: 2020 2020 2020 2069 3138 6e3a 7472 616e         i18n:tran
+000004c0: 736c 6174 653d 2222 0a20 2020 2020 2020  slate="".       
+000004d0: 203e 0a20 2020 2020 2020 2020 2020 2020   >.             
+000004e0: 2020 2020 2061 6374 696f 6e20 7469 746c       action titl
+000004f0: 650a 2020 2020 2020 2020 3c2f 613e 0a20  e.        </a>. 
+00000500: 2020 2020 203c 2f6c 693e 0a20 2020 203c       </li>.    <
+00000510: 2f75 6c3e 0a20 203c 2f64 6976 3e0a 0a3c  /ul>.  </div>..<
+00000520: 2f64 6976 3e0a                           /div>.
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/menu.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/menu.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,114 @@
 00000000: 3c74 616c 3a63 6f6e 7465 6e74 7669 6577  <tal:contentview
-00000010: 7320 7461 6c3a 6465 6669 6e65 3d22 706c  s tal:define="pl
-00000020: 6f6e 6576 6965 7720 636f 6e74 6578 742f  oneview context/
-00000030: 4040 706c 6f6e 653b 0a20 2020 2020 2020  @@plone;.       
-00000040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000050: 2020 2020 2020 206c 6f63 6b65 6420 7669         locked vi
-00000060: 6577 2f6c 6f63 6b65 645f 6963 6f6e 3b0a  ew/locked_icon;.
-00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000080: 2020 2020 2020 2020 2020 2020 2020 6963                ic
-00000090: 6f6e 7320 7079 7468 6f6e 3a63 6f6e 7465  ons python:conte
-000000a0: 7874 2e72 6573 7472 6963 7465 6454 7261  xt.restrictedTra
-000000b0: 7665 7273 6528 2740 4069 636f 6e72 6573  verse('@@iconres
-000000c0: 6f6c 7665 7227 293b 220a 2020 2020 2020  olver');".      
-000000d0: 2020 2020 2020 2020 2020 2020 7461 6c3a              tal:
-000000e0: 636f 6e64 6974 696f 6e3d 2270 6c6f 6e65  condition="plone
-000000f0: 7669 6577 2f73 686f 7754 6f6f 6c62 6172  view/showToolbar
-00000100: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000110: 2020 2020 6931 386e 3a64 6f6d 6169 6e3d      i18n:domain=
-00000120: 2270 6c6f 6e65 223e 0a20 203c 7461 6c3a  "plone">.  <tal:
-00000130: 6163 7469 6f6e 7320 7461 6c3a 7265 7065  actions tal:repe
-00000140: 6174 3d22 6163 7469 6f6e 206f 7074 696f  at="action optio
-00000150: 6e73 2f61 6374 696f 6e73 223e 0a20 2020  ns/actions">.   
-00000160: 203c 6c69 2069 643d 2263 6f6e 7465 6e74   <li id="content
-00000170: 7669 6577 2d24 7b61 6374 696f 6e2f 6964  view-${action/id
-00000180: 7d22 2063 6c61 7373 3d22 6e61 762d 6974  }" class="nav-it
-00000190: 656d 220a 2020 2020 2020 2020 7461 6c3a  em".        tal:
-000001a0: 6465 6669 6e65 3d22 6163 7469 6f6e 6964  define="actionid
-000001b0: 2061 6374 696f 6e2f 6964 3b0a 2020 2020   action/id;.    
-000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001d0: 7365 6c65 6374 6564 2061 6374 696f 6e2f  selected action/
-000001e0: 7365 6c65 6374 6564 207c 2070 7974 686f  selected | pytho
-000001f0: 6e3a 4661 6c73 6522 3e0a 0a20 2020 2020  n:False">..     
-00000200: 2020 203c 6120 6872 6566 3d22 2322 2063     <a href="#" c
-00000210: 6c61 7373 3d22 6e61 762d 6c69 6e6b 2024  lass="nav-link $
-00000220: 7b70 7974 686f 6e3a 276c 6f63 6b65 6427  {python:'locked'
-00000230: 2069 6620 6c6f 636b 6564 2061 6e64 2061   if locked and a
-00000240: 6374 696f 6e69 6420 3d3d 2027 6869 7374  ctionid == 'hist
-00000250: 6f72 7927 2065 6c73 6520 2727 7d20 247b  ory' else ''} ${
-00000260: 6163 7469 6f6e 2f63 7373 436c 6173 7320  action/cssClass 
-00000270: 7c20 6e6f 7468 696e 677d 2024 7b70 7974  | nothing} ${pyt
-00000280: 686f 6e3a 2761 6374 6976 6527 2069 6620  hon:'active' if 
-00000290: 7365 6c65 6374 6564 2065 6c73 6520 4e6f  selected else No
-000002a0: 6e65 7d22 0a20 2020 2020 2020 2020 2020  ne}".           
-000002b0: 7461 6c3a 6174 7472 6962 7574 6573 3d22  tal:attributes="
-000002c0: 6872 6566 2061 6374 696f 6e2f 7572 6c3b  href action/url;
-000002d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000002e0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-000002f0: 6574 2061 6374 696f 6e2f 6c69 6e6b 5f74  et action/link_t
-00000300: 6172 6765 747c 6e6f 7468 696e 673b 223e  arget|nothing;">
-00000310: 0a0a 2020 2020 2020 2020 2020 3c74 616c  ..          <tal
-00000320: 3a69 6620 636f 6e64 6974 696f 6e3d 2270  :if condition="p
-00000330: 7974 686f 6e3a 6163 7469 6f6e 6964 2021  ython:actionid !
-00000340: 3d20 2768 6973 746f 7279 2722 3e0a 2020  = 'history'">.  
-00000350: 2020 2020 2020 2020 2020 3c74 616c 3a69            <tal:i
-00000360: 636f 6e20 7461 6c3a 636f 6e64 6974 696f  con tal:conditio
-00000370: 6e3d 2270 7974 686f 6e3a 6163 7469 6f6e  n="python:action
-00000380: 5b27 6963 6f6e 275d 220a 2020 2020 2020  ['icon']".      
-00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003a0: 7461 6c3a 7265 706c 6163 653d 2273 7472  tal:replace="str
-000003b0: 7563 7475 7265 2070 7974 686f 6e3a 6963  ucture python:ic
-000003c0: 6f6e 732e 7461 6728 6163 7469 6f6e 5b27  ons.tag(action['
-000003d0: 6963 6f6e 275d 206f 7220 2774 6f6f 6c62  icon'] or 'toolb
-000003e0: 6172 2d61 6374 696f 6e27 2c20 7461 675f  ar-action', tag_
-000003f0: 636c 6173 733d 276d 652d 3127 2922 202f  class='me-1')" /
-00000400: 3e0a 2020 2020 2020 2020 2020 2020 3c73  >.            <s
-00000410: 7061 6e20 636c 6173 733d 2274 6f6f 6c62  pan class="toolb
-00000420: 6172 2d6c 6162 656c 2220 7461 6c3a 636f  ar-label" tal:co
-00000430: 6e74 656e 743d 2261 6374 696f 6e2f 7469  ntent="action/ti
-00000440: 746c 6522 2069 3138 6e3a 7472 616e 736c  tle" i18n:transl
-00000450: 6174 653d 2222 3e56 6965 7720 6e61 6d65  ate="">View name
-00000460: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
-00000470: 2020 3c2f 7461 6c3a 6966 3e0a 0a20 2020    </tal:if>..   
-00000480: 2020 2020 2020 203c 7461 6c3a 6966 2074         <tal:if t
-00000490: 616c 3a63 6f6e 6469 7469 6f6e 3d22 7079  al:condition="py
-000004a0: 7468 6f6e 3a61 6374 696f 6e69 6420 3d3d  thon:actionid ==
-000004b0: 2027 6869 7374 6f72 7927 223e 0a20 2020   'history'">.   
-000004c0: 2020 2020 2020 2020 203c 7461 6c3a 6963           <tal:ic
-000004d0: 6f6e 2074 616c 3a72 6570 6c61 6365 3d22  on tal:replace="
-000004e0: 7374 7275 6374 7572 6520 7079 7468 6f6e  structure python
-000004f0: 3a69 636f 6e73 2e74 6167 2827 6c6f 636b  :icons.tag('lock
-00000500: 2720 6966 206c 6f63 6b65 6420 656c 7365  ' if locked else
-00000510: 2061 6374 696f 6e5b 2769 636f 6e27 5d2c   action['icon'],
-00000520: 2074 6167 5f63 6c61 7373 3d27 6d65 2d31   tag_class='me-1
-00000530: 2729 2220 2f3e 0a20 2020 2020 2020 2020  ')" />.         
-00000540: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
-00000550: 746f 6f6c 6261 722d 6c61 6265 6c22 3e0a  toolbar-label">.
-00000560: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00000570: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
-00000580: 2020 2020 636c 6173 733d 2270 6174 2d64      class="pat-d
-00000590: 6973 706c 6179 2d74 696d 6522 0a20 2020  isplay-time".   
-000005a0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-000005b0: 612d 7061 742d 6469 7370 6c61 792d 7469  a-pat-display-ti
-000005c0: 6d65 3d22 6f75 7470 7574 2d66 6f72 6d61  me="output-forma
-000005d0: 743a 204c 204c 5453 220a 2020 2020 2020  t: L LTS".      
-000005e0: 2020 2020 2020 2020 2020 6461 7465 7469            dateti
-000005f0: 6d65 3d22 247b 636f 6e74 6578 742f 4d6f  me="${context/Mo
-00000600: 6469 6669 6361 7469 6f6e 4461 7465 7d22  dificationDate}"
-00000610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000620: 2074 616c 3a63 6f6e 7465 6e74 3d22 223e   tal:content="">
-00000630: 247b 636f 6e74 6578 742f 4d6f 6469 6669  ${context/Modifi
-00000640: 6361 7469 6f6e 4461 7465 7d3c 2f74 696d  cationDate}</tim
-00000650: 653e 0a20 2020 2020 2020 2020 2020 203c  e>.            <
-00000660: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
-00000670: 203c 2f74 616c 3a69 663e 0a0a 2020 2020   </tal:if>..    
-00000680: 2020 2020 3c2f 613e 0a0a 2020 2020 3c2f      </a>..    </
-00000690: 6c69 3e0a 2020 3c2f 7461 6c3a 6163 7469  li>.  </tal:acti
-000006a0: 6f6e 733e 0a3c 2f74 616c 3a63 6f6e 7465  ons>.</tal:conte
-000006b0: 6e74 7669 6577 733e 0a                   ntviews>.
+00000010: 7320 7461 6c3a 6465 6669 6e65 3d22 0a20  s tal:define=". 
+00000020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000030: 2020 2070 6c6f 6e65 7669 6577 2063 6f6e     ploneview con
+00000040: 7465 7874 2f40 4070 6c6f 6e65 3b0a 2020  text/@@plone;.  
+00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000060: 2020 6c6f 636b 6564 2076 6965 772f 6c6f    locked view/lo
+00000070: 636b 6564 5f69 636f 6e3b 0a20 2020 2020  cked_icon;.     
+00000080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000090: 636f 6e73 2070 7974 686f 6e3a 636f 6e74  cons python:cont
+000000a0: 6578 742e 7265 7374 7269 6374 6564 5472  ext.restrictedTr
+000000b0: 6176 6572 7365 2827 4040 6963 6f6e 7265  averse('@@iconre
+000000c0: 736f 6c76 6572 2729 3b0a 2020 2020 2020  solver');.      
+000000d0: 2020 2020 2020 2020 2020 2020 220a 2020              ".  
+000000e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000000f0: 7461 6c3a 636f 6e64 6974 696f 6e3d 2270  tal:condition="p
+00000100: 6c6f 6e65 7669 6577 2f73 686f 7754 6f6f  loneview/showToo
+00000110: 6c62 6172 220a 2020 2020 2020 2020 2020  lbar".          
+00000120: 2020 2020 2020 2020 6931 386e 3a64 6f6d          i18n:dom
+00000130: 6169 6e3d 2270 6c6f 6e65 220a 3e0a 2020  ain="plone".>.  
+00000140: 3c74 616c 3a61 6374 696f 6e73 2074 616c  <tal:actions tal
+00000150: 3a72 6570 6561 743d 2261 6374 696f 6e20  :repeat="action 
+00000160: 6f70 7469 6f6e 732f 6163 7469 6f6e 7322  options/actions"
+00000170: 3e0a 2020 2020 3c6c 6920 636c 6173 733d  >.    <li class=
+00000180: 226e 6176 2d69 7465 6d22 0a20 2020 2020  "nav-item".     
+00000190: 2020 2069 643d 2263 6f6e 7465 6e74 7669     id="contentvi
+000001a0: 6577 2d24 7b61 6374 696f 6e2f 6964 7d22  ew-${action/id}"
+000001b0: 0a20 2020 2020 2020 2074 616c 3a64 6566  .        tal:def
+000001c0: 696e 653d 220a 2020 2020 2020 2020 2020  ine=".          
+000001d0: 6163 7469 6f6e 6964 2061 6374 696f 6e2f  actionid action/
+000001e0: 6964 3b0a 2020 2020 2020 2020 2020 7365  id;.          se
+000001f0: 6c65 6374 6564 2061 6374 696f 6e2f 7365  lected action/se
+00000200: 6c65 6374 6564 207c 2070 7974 686f 6e3a  lected | python:
+00000210: 4661 6c73 653b 0a20 2020 2020 2020 2022  False;.        "
+00000220: 0a20 2020 203e 0a0a 2020 2020 2020 3c61  .    >..      <a
+00000230: 2063 6c61 7373 3d22 6e61 762d 6c69 6e6b   class="nav-link
+00000240: 2024 7b70 7974 686f 6e3a 276c 6f63 6b65   ${python:'locke
+00000250: 6427 2069 6620 6c6f 636b 6564 2061 6e64  d' if locked and
+00000260: 2061 6374 696f 6e69 6420 3d3d 2027 6869   actionid == 'hi
+00000270: 7374 6f72 7927 2065 6c73 6520 2727 7d20  story' else ''} 
+00000280: 247b 6163 7469 6f6e 2f63 7373 436c 6173  ${action/cssClas
+00000290: 7320 7c20 6e6f 7468 696e 677d 2024 7b70  s | nothing} ${p
+000002a0: 7974 686f 6e3a 2761 6374 6976 6527 2069  ython:'active' i
+000002b0: 6620 7365 6c65 6374 6564 2065 6c73 6520  f selected else 
+000002c0: 4e6f 6e65 7d22 0a20 2020 2020 2020 2020  None}".         
+000002d0: 6872 6566 3d22 2322 0a20 2020 2020 2020  href="#".       
+000002e0: 2020 7461 6c3a 6174 7472 6962 7574 6573    tal:attributes
+000002f0: 3d22 0a20 2020 2020 2020 2020 2020 6872  =".           hr
+00000300: 6566 2061 6374 696f 6e2f 7572 6c3b 0a20  ef action/url;. 
+00000310: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00000320: 2061 6374 696f 6e2f 6c69 6e6b 5f74 6172   action/link_tar
+00000330: 6765 747c 6e6f 7468 696e 673b 0a20 2020  get|nothing;.   
+00000340: 2020 2020 2020 220a 2020 2020 2020 3e0a        ".      >.
+00000350: 0a20 2020 2020 2020 203c 7461 6c3a 6966  .        <tal:if
+00000360: 2063 6f6e 6469 7469 6f6e 3d22 7079 7468   condition="pyth
+00000370: 6f6e 3a61 6374 696f 6e69 6420 213d 2027  on:actionid != '
+00000380: 6869 7374 6f72 7927 223e 0a20 2020 2020  history'">.     
+00000390: 2020 2020 203c 7461 6c3a 6963 6f6e 2074       <tal:icon t
+000003a0: 616c 3a63 6f6e 6469 7469 6f6e 3d22 7079  al:condition="py
+000003b0: 7468 6f6e 3a61 6374 696f 6e5b 2769 636f  thon:action['ico
+000003c0: 6e27 5d22 0a20 2020 2020 2020 2020 2020  n']".           
+000003d0: 2020 2020 2020 2020 2074 616c 3a72 6570           tal:rep
+000003e0: 6c61 6365 3d22 7374 7275 6374 7572 6520  lace="structure 
+000003f0: 7079 7468 6f6e 3a69 636f 6e73 2e74 6167  python:icons.tag
+00000400: 2861 6374 696f 6e5b 2769 636f 6e27 5d20  (action['icon'] 
+00000410: 6f72 2027 746f 6f6c 6261 722d 6163 7469  or 'toolbar-acti
+00000420: 6f6e 272c 2074 6167 5f63 6c61 7373 3d27  on', tag_class='
+00000430: 6d65 2d31 2729 220a 2020 2020 2020 2020  me-1')".        
+00000440: 2020 2f3e 0a20 2020 2020 2020 2020 203c    />.          <
+00000450: 7370 616e 2063 6c61 7373 3d22 746f 6f6c  span class="tool
+00000460: 6261 722d 6c61 6265 6c22 0a20 2020 2020  bar-label".     
+00000470: 2020 2020 2020 2020 2020 2074 616c 3a63             tal:c
+00000480: 6f6e 7465 6e74 3d22 6163 7469 6f6e 2f74  ontent="action/t
+00000490: 6974 6c65 220a 2020 2020 2020 2020 2020  itle".          
+000004a0: 2020 2020 2020 6931 386e 3a74 7261 6e73        i18n:trans
+000004b0: 6c61 7465 3d22 220a 2020 2020 2020 2020  late="".        
+000004c0: 2020 3e56 6965 7720 6e61 6d65 3c2f 7370    >View name</sp
+000004d0: 616e 3e0a 2020 2020 2020 2020 3c2f 7461  an>.        </ta
+000004e0: 6c3a 6966 3e0a 0a20 2020 2020 2020 203c  l:if>..        <
+000004f0: 7461 6c3a 6966 2074 616c 3a63 6f6e 6469  tal:if tal:condi
+00000500: 7469 6f6e 3d22 7079 7468 6f6e 3a61 6374  tion="python:act
+00000510: 696f 6e69 6420 3d3d 2027 6869 7374 6f72  ionid == 'histor
+00000520: 7927 223e 0a20 2020 2020 2020 2020 203c  y'">.          <
+00000530: 7461 6c3a 6963 6f6e 2074 616c 3a72 6570  tal:icon tal:rep
+00000540: 6c61 6365 3d22 7374 7275 6374 7572 6520  lace="structure 
+00000550: 7079 7468 6f6e 3a69 636f 6e73 2e74 6167  python:icons.tag
+00000560: 2827 6c6f 636b 2720 6966 206c 6f63 6b65  ('lock' if locke
+00000570: 6420 656c 7365 2061 6374 696f 6e5b 2769  d else action['i
+00000580: 636f 6e27 5d2c 2074 6167 5f63 6c61 7373  con'], tag_class
+00000590: 3d27 6d65 2d31 2729 2220 2f3e 0a20 2020  ='me-1')" />.   
+000005a0: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
+000005b0: 7373 3d22 746f 6f6c 6261 722d 6c61 6265  ss="toolbar-labe
+000005c0: 6c22 3e0a 2020 2020 2020 2020 2020 2020  l">.            
+000005d0: 3c74 696d 6520 636c 6173 733d 2270 6174  <time class="pat
+000005e0: 2d64 6973 706c 6179 2d74 696d 6522 0a20  -display-time". 
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 2064 6174 6574 696d 653d 2224 7b63 6f6e   datetime="${con
+00000610: 7465 7874 2f4d 6f64 6966 6963 6174 696f  text/Modificatio
+00000620: 6e44 6174 657d 220a 2020 2020 2020 2020  nDate}".        
+00000630: 2020 2020 2020 2020 2020 6461 7461 2d70            data-p
+00000640: 6174 2d64 6973 706c 6179 2d74 696d 653d  at-display-time=
+00000650: 226f 7574 7075 742d 666f 726d 6174 3a20  "output-format: 
+00000660: 4c20 4c54 5322 0a20 2020 2020 2020 2020  L LTS".         
+00000670: 2020 2020 2020 2020 2074 616c 3a63 6f6e           tal:con
+00000680: 7465 6e74 3d22 220a 2020 2020 2020 2020  tent="".        
+00000690: 2020 2020 3e24 7b63 6f6e 7465 7874 2f4d      >${context/M
+000006a0: 6f64 6966 6963 6174 696f 6e44 6174 657d  odificationDate}
+000006b0: 3c2f 7469 6d65 3e0a 2020 2020 2020 2020  </time>.        
+000006c0: 2020 3c2f 7370 616e 3e0a 2020 2020 2020    </span>.      
+000006d0: 2020 3c2f 7461 6c3a 6966 3e0a 0a20 2020    </tal:if>..   
+000006e0: 2020 203c 2f61 3e0a 0a20 2020 203c 2f6c     </a>..    </l
+000006f0: 693e 0a20 203c 2f74 616c 3a61 6374 696f  i>.  </tal:actio
+00000700: 6e73 3e0a 3c2f 7461 6c3a 636f 6e74 656e  ns>.</tal:conten
+00000710: 7476 6965 7773 3e0a                      tviews>.
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/path_bar.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/path_bar.pt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 
-<nav id="portal-breadcrumbs" i18n:attributes="label_breadcrumb" aria-label="breadcrumb" i18n:domain="plone" tal:define="breadcrumbs python:view.breadcrumbs">
+<nav id="portal-breadcrumbs"
+     aria-label="breadcrumb"
+     tal:define="
+       breadcrumbs python:view.breadcrumbs;
+     "
+     i18n:attributes="label_breadcrumb"
+     i18n:domain="plone"
+>
   <div class="container">
     <ol class="breadcrumb">
-      <li class="breadcrumb-item"><a i18n:translate="tabs_home" href="${python:view.navigation_root_url}">Home</a></li>
+      <li class="breadcrumb-item"><a href="${python:view.navigation_root_url}"
+           i18n:translate="tabs_home"
+        >Home</a></li>
       <tal:loop tal:repeat="crumb breadcrumbs">
-      <li tal:condition="not: repeat/crumb/end" class="breadcrumb-item" ><a href="${python:crumb['absolute_url']}">${python:crumb['Title']}</a></li>
-      <li tal:condition="repeat/crumb/end" class="breadcrumb-item active" aria-current="page">${python:crumb['Title']}</li>
+        <li class="breadcrumb-item"
+            tal:condition="not: repeat/crumb/end"
+        ><a href="${python:crumb['absolute_url']}">${python:crumb['Title']}</a></li>
+        <li class="breadcrumb-item active"
+            aria-current="page"
+            tal:condition="repeat/crumb/end"
+        >${python:crumb['Title']}</li>
       </tal:loop>
     </ol>
   </div>
 </nav>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/review_history.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/review_history.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,99 @@
 <div class="reviewHistory"
      id="review-history"
+     tal:define="
+       history view/workflowHistory;
+     "
      i18n:domain="plone"
-     tal:define="history view/workflowHistory;">
-    <tal:history tal:condition="history">
-      <dl id="history" class="collapsible inline collapsedOnLoad">
-        <dt class="collapsibleHeader" i18n:translate="label_history">History</dt>
-        <dd class="collapsibleContent">
-
-        <table class="listing nosort" summary="Review History"
-               i18n:attributes="summary summary_review_history;">
+>
+  <tal:history tal:condition="history">
+    <dl class="collapsible inline collapsedOnLoad"
+        id="history"
+    >
+      <dt class="collapsibleHeader"
+          i18n:translate="label_history"
+      >History</dt>
+      <dd class="collapsibleContent">
+
+        <table class="listing nosort"
+               summary="Review History"
+               i18n:attributes="summary summary_review_history;"
+        >
 
           <tr>
             <th i18n:translate="listingheader_action">Action</th>
             <th i18n:translate="listingheader_performed_by">Performed by</th>
             <th i18n:translate="listingheader_date_and_time">Date and Time</th>
             <th i18n:translate="listingheader_comment">Comment</th>
           </tr>
 
           <metal:block tal:repeat="item history">
-            <tr tal:define="odd repeat/item/odd;
-                            rhComments item/comments|nothing;
-                            state item/review_state|nothing"
-                tal:attributes="class python:odd and 'even' or 'odd'"
-                tal:condition="item/action">
-              <td i18n:translate="" tal:content="item/transition_title"
-                  tal:attributes="class string:state-${state}">
+            <tr tal:define="
+                  odd repeat/item/odd;
+                  rhComments item/comments|nothing;
+                  state item/review_state|nothing;
+                "
+                tal:condition="item/action"
+                tal:attributes="
+                  class python:odd and 'even' or 'odd';
+                "
+            >
+              <td tal:content="item/transition_title"
+                  tal:attributes="
+                    class string:state-${state};
+                  "
+                  i18n:translate=""
+              >
                 action
               </td>
 
-              <td tal:define="actorid python:item.get('actorid');
-                              actor python:item.get('actor');
-                              fullname actor/fullname|nothing;
-                              username actor/username|nothing">
+              <td tal:define="
+                    actorid python:item.get('actorid');
+                    actor python:item.get('actor');
+                    fullname actor/fullname|nothing;
+                    username actor/username|nothing;
+                  ">
                 <a href="/Members/runyaga"
                    tal:condition="item/actor_home"
-                   tal:attributes="href item/actor_home"
-                   tal:content="python:fullname or username or actorid">
+                   tal:content="python:fullname or username or actorid"
+                   tal:attributes="
+                     href item/actor_home;
+                   "
+                >
                   runyaga
                 </a>
                 <span tal:condition="not: item/actor_home"
                       tal:replace="python:fullname or username or actorid"
-                />
+                ></span>
               </td>
 
               <td>
-                <span tal:replace="python:context.toLocalizedTime(item['time'],long_format=True)" />
+                <span tal:replace="python:context.toLocalizedTime(item['time'],long_format=True)"></span>
                 <span tal:condition="item/effective_date|nothing">
-                  (<span i18n:translate="label_publishing_effective" tal:omit-tag="">effective</span>:
+                  (<span tal:omit-tag=""
+                        i18n:translate="label_publishing_effective"
+                  >effective</span>:
                   <span tal:replace="python: context.toLocalizedTime(item['effective_date'],long_format=True)"></span>)
                 </span>
               </td>
 
               <td>
                 <span tal:condition="rhComments">
-                  <span tal:replace="rhComments"> some comments </span>
+                  <span tal:replace="rhComments">
+                    some comments
+                  </span>
                 </span>
 
-                <span tal:condition="not: rhComments" i18n:translate="no_comments">
+                <span tal:condition="not: rhComments"
+                      i18n:translate="no_comments"
+                >
                   No comments.
                 </span>
               </td>
             </tr>
           </metal:block>
         </table>
 
-        </dd>
-      </dl>
-    </tal:history>
+      </dd>
+    </dl>
+  </tal:history>
 </div>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/searchbox.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/searchbox.pt`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,61 @@
-<div id="portal-searchbox" class="d-flex flex-column position-relative"
-  i18n:domain="plone"
-  tal:define="navigation_root_url view/navigation_root_url;">
-
-  <form id="searchGadget_form"
-    action="@@search"
-    role="search"
-    class="d-flex ${python: view.livesearch and 'pat-livesearch'} ${python: view.show_images and 'show_images'} "
-    tal:attributes="action string:${navigation_root_url}/@@search;
-                    data-pat-livesearch string:ajaxUrl:${navigation_root_url}/@@ajax-search;">
+<div class="d-flex flex-column position-relative"
+     id="portal-searchbox"
+     tal:define="
+       navigation_root_url view/navigation_root_url;
+     "
+     i18n:domain="plone"
+>
+
+  <form class="d-flex ${python: view.livesearch and 'pat-livesearch'} ${python: view.show_images and 'show_images'}"
+        id="searchGadget_form"
+        action="@@search"
+        role="search"
+        tal:attributes="
+          action string:${navigation_root_url}/@@search;
+          data-pat-livesearch string:ajaxUrl:${navigation_root_url}/@@ajax-search;
+        "
+  >
 
     <label class="hiddenStructure"
-      for="searchGadget"
-      i18n:translate="text_search">Search Site</label>
-
-    <input name="SearchableText"
-      type="text"
-      size="18"
-      value=""
-      id="searchGadget"
-      title="Search Site"
-      placeholder="Search Site"
-      i18n:attributes="title title_search_site;
+           for="searchGadget"
+           i18n:translate="text_search"
+    >Search Site</label>
+
+    <input class="searchField form-control me-2"
+           id="searchGadget"
+           name="SearchableText"
+           placeholder="Search Site"
+           size="18"
+           title="Search Site"
+           type="text"
+           value=""
+           tal:attributes="
+             value request/form/SearchableText|nothing;
+           "
+           i18n:attributes="title title_search_site;
                         placeholder title_search_site"
-      tal:attributes="value request/form/SearchableText|nothing;"
-      class="searchField form-control me-2" />
+    />
 
     <button class="searchButton btn btn-outline-light"
-      type="submit"
-      i18n:translate="label_search">
+            type="submit"
+            i18n:translate="label_search"
+    >
       Search
     </button>
 
-    <div id="portal-advanced-search"
-          class="hiddenStructure">
+    <div class="hiddenStructure"
+         id="portal-advanced-search"
+    >
       <a href="#"
-          tal:attributes="href string:${navigation_root_url}/@@search"
-          i18n:translate="label_advanced_search">
+         tal:attributes="
+           href string:${navigation_root_url}/@@search;
+         "
+         i18n:translate="label_advanced_search"
+      >
           Advanced Search&hellip;
       </a>
     </div>
 
   </form>
 
 </div>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/sections.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/sections.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-<tal:sections xmlns:tal="http://xml.zope.org/namespaces/tal"
-  xmlns:metal="http://xml.zope.org/namespaces/metal"
-  xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-  tal:condition="python:view.navtree" i18n:domain="plone">
+<tal:sections xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+              xmlns:metal="http://xml.zope.org/namespaces/metal"
+              xmlns:tal="http://xml.zope.org/namespaces/tal"
+              tal:condition="python:view.navtree"
+              i18n:domain="plone"
+>
 
-  <ul class="navbar-nav" id="portal-globalnav">
-    <navtree tal:replace="structure python:view.render_globalnav()" />
+  <ul class="navbar-nav"
+      id="portal-globalnav"
+  >
+    <navtree tal:replace="structure python:view.render_globalnav()"></navtree>
   </ul>
 
-  <button class="navbar-toggler" type="button"
-    aria-label="Toggle navigation" i18n:attributes="aria-label label_toggle_navigation">
+  <button class="navbar-toggler"
+          aria-label="Toggle navigation"
+          type="button"
+          i18n:attributes="aria-label label_toggle_navigation"
+  >
     <span class="navbar-toggler-icon"></span>
   </button>
 
 </tal:sections>
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/social.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/social.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from plone.app.layout.viewlets.common import TitleViewlet
+from plone.base.interfaces import ISocialMediaSchema
+from plone.base.interfaces.syndication import IFeedItem
 from plone.memoize.view import memoize
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.browser.syndication.adapters import BaseItem
 from Products.CMFPlone.browser.syndication.adapters import FolderFeed
-from plone.base.interfaces import ISocialMediaSchema
-from plone.base.interfaces.syndication import IFeedItem
 from Products.CMFPlone.utils import getSiteLogo
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
 from zope.component.hooks import getSite
 
 import logging
 
+
 logger = logging.getLogger("plone.app.layout")
 
 
 class SocialTagsViewlet(TitleViewlet):
     social_image_scale = "great"
 
     def head_tag_filter(self, value):
@@ -95,18 +96,18 @@
             ]
         )
 
         found_image = False
         if item.has_enclosure and item.file_length > 0:
             if item.file_type.startswith("image"):
                 image = None
-                scales = self.context.restrictedTraverse('@@images', None)
+                scales = self.context.restrictedTraverse("@@images", None)
                 if scales:
                     try:
-                        image = scales.scale('image', scale=self.social_image_scale)
+                        image = scales.scale("image", scale=self.social_image_scale)
                     except Exception as e:
                         logger.exception(e)
                 if image:
                     tags.extend(
                         [
                             dict(property="og:image", content=image.url),
                             dict(property="og:image:width", content=image.width),
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/base.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 from plone.app.layout.testing import INTEGRATION_TESTING
 from plone.app.layout.testing import TEST_USER_ID
 
 import unittest
 
 
 class ViewletsTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.app = self.layer["app"]
         self.folder = self.portal["Members"][TEST_USER_ID]
 
 
 class ViewletsFunctionalTestCase(unittest.TestCase):
-
     layer = FUNCTIONAL_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.app = self.layer["app"]
         self.folder = self.portal["Members"][TEST_USER_ID]
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/history.txt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/history.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     >>> browser.follow(url='@@historyview')
     >>> from __future__ import print_function
     >>> print(browser.contents)
     <...<span class="historyAction state-private">Create</span>...
 
 
-The history viewlet handles revert actions sucessfully. Let's make a revision.
+The history viewlet handles revert actions successfully. Let's make a revision.
 
     >>> browser.open(urldoc2)
     >>> browser.follow('Edit')
     >>> browser.getControl('Summary').value = "Changed for revision 2"
     >>> browser.getControl('Save').click()
 
 The history viewlet now shows a Revert button.
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_common.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from plone.base.interfaces import INavigationRoot
 from plone.app.layout.viewlets.common import ContentViewsViewlet
 from plone.app.layout.viewlets.common import GlobalSectionsViewlet
 from plone.app.layout.viewlets.common import LogoViewlet
 from plone.app.layout.viewlets.common import TitleViewlet
 from plone.app.layout.viewlets.common import ViewletBase
 from plone.app.layout.viewlets.tests.base import ViewletsFunctionalTestCase
 from plone.app.layout.viewlets.tests.base import ViewletsTestCase
 from plone.app.testing import setRoles
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
+from plone.base.interfaces import INavigationRoot
+from plone.base.interfaces import INonStructuralFolder
+from plone.base.interfaces import ISiteSchema
 from plone.protect import authenticator as auth
 from plone.registry.interfaces import IRegistry
 from plone.testing.zope import Browser
-from plone.base.interfaces import INonStructuralFolder
-from plone.base.interfaces import ISiteSchema
 from zope.component import getUtility
 from zope.component.hooks import setSite
 from zope.interface import alsoProvides
 from zope.interface import directlyProvides
 from zope.interface import noLongerProvides
 
 import json
@@ -169,15 +169,17 @@
 
     def test_logo_viewlet_portal_root_default(self):
         """When no logo is set, and viewlet is opened on a non-navigation root,
         obtain the default one from the portal.
         """
         viewlet = LogoViewlet(self.folder, self.app.REQUEST, None)
         viewlet.update()
-        self.assertEqual(viewlet.img_src, f"{self.portal.absolute_url()}/++resource++plone-logo.svg")
+        self.assertEqual(
+            viewlet.img_src, f"{self.portal.absolute_url()}/++resource++plone-logo.svg"
+        )
 
     def test_logo_viewlet_portal_root_registry(self):
         """When a logo is set, and viewlet is opened on a non-navigation root,
         obtain the registry logo from the portal.
         """
         registry = getUtility(IRegistry)
         settings = registry.forInterface(ISiteSchema, prefix="plone")
@@ -193,15 +195,17 @@
     def test_logo_viewlet_navigation_root_default(self):
         """When no logo is set, and viewlet is opened on a navigation root,
         obtain the default one from the navigation root.
         """
         self._set_site(self.folder)
         viewlet = LogoViewlet(self.folder, self.app.REQUEST, None)
         viewlet.update()
-        self.assertEqual(viewlet.img_src, f"{self.folder.absolute_url()}/++resource++plone-logo.svg")
+        self.assertEqual(
+            viewlet.img_src, f"{self.folder.absolute_url()}/++resource++plone-logo.svg"
+        )
 
     def test_viewlet_navigation_root_registry(self):
         """When a logo is set, and viewlet is opened on a navigation root,
         obtain the registry logo from the navigation root.
         """
         registry = getUtility(IRegistry)
         settings = registry.forInterface(ISiteSchema, prefix="plone")
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_content.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from plone.app.layout.viewlets.content import DocumentBylineViewlet
 from plone.app.layout.viewlets.content import HistoryByLineView
 from plone.app.layout.viewlets.tests.base import ViewletsTestCase
 from plone.app.testing import logout
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_PASSWORD
-from plone.locking.interfaces import ILockable
-from plone.registry.interfaces import IRegistry
 from plone.base.interfaces import ISecuritySchema
 from plone.base.interfaces import ISiteSchema
+from plone.locking.interfaces import ILockable
+from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from z3c.relationfield import RelationValue
 from zope.component import getUtility
 from zope.interface import Interface
 from zope.intid.interfaces import IIntIds
 
 
@@ -80,15 +80,19 @@
         self.assertEqual(viewlet.get_fullname("bogus"), "bogus")
         # If the fullname is not set we return the user id
         self.assertEqual(viewlet.get_fullname("test_user_1_"), "test_user_1_")
 
         # otherwise we will return the fullname property
         portal_membership = getToolByName(self.portal, "portal_membership")
         portal_membership.addMember(
-            "foo/bar", TEST_USER_PASSWORD, ["Member"], "", properties={"fullname": "Foo Bar"}
+            "foo/bar",
+            TEST_USER_PASSWORD,
+            ["Member"],
+            "",
+            properties={"fullname": "Foo Bar"},
         )
         self.assertEqual(viewlet.get_fullname("foo/bar"), "Foo Bar")
 
     def test_pub_date(self):
         # configure our portal to enable publication date on pages globally on
         # the site
         self.site_settings.display_publication_date_in_byline = True
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_functional.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_history.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/tests/test_social.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_social.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from plone.app.layout.viewlets.social import SocialTagsViewlet
 from plone.app.layout.viewlets.tests.base import ViewletsTestCase
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
-from plone.registry.interfaces import IRegistry
 from plone.base.interfaces import ISocialMediaSchema
+from plone.registry.interfaces import IRegistry
 from zope.annotation.interfaces import IAnnotations
 from zope.component import getUtility
 
 
 class TestSocialViewlet(ViewletsTestCase):
     """Test the content views viewlet."""
 
@@ -127,16 +127,22 @@
         )
 
     def testLogo(self):
         viewlet = SocialTagsViewlet(self.news, self.app.REQUEST, None)
         viewlet.update()
         self.assertTrue(
             self.tagFound(
-                viewlet, "property", "og:image", "http://nohost/plone/++resource++plone-logo.svg"
+                viewlet,
+                "property",
+                "og:image",
+                "http://nohost/plone/++resource++plone-logo.svg",
             )
         )
         self.assertFalse(self.tagFound(viewlet, "itemprop"))
         self.assertTrue(
             self.bodyTagFound(
-                viewlet, "itemprop", "image", "http://nohost/plone/++resource++plone-logo.svg"
+                viewlet,
+                "itemprop",
+                "image",
+                "http://nohost/plone/++resource++plone-logo.svg",
             )
         )
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/toolbar.pt` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,156 @@
 00000000: 3c73 6563 7469 6f6e 2069 643d 2265 6469  <section id="edi
-00000010: 742d 6261 7222 2072 6f6c 653d 2274 6f6f  t-bar" role="too
-00000020: 6c62 6172 220a 2020 2020 2020 2020 2074  lbar".         t
-00000030: 616c 3a64 6566 696e 653d 2263 6f6e 7465  al:define="conte
-00000040: 7874 5f73 7461 7465 2076 6965 772f 636f  xt_state view/co
-00000050: 6e74 6578 745f 7374 6174 653b 0a20 2020  ntext_state;.   
-00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000070: 2020 6963 6f6e 7320 7079 7468 6f6e 3a63    icons python:c
-00000080: 6f6e 7465 7874 2e72 6573 7472 6963 7465  ontext.restricte
-00000090: 6454 7261 7665 7273 6528 2740 4069 636f  dTraverse('@@ico
-000000a0: 6e72 6573 6f6c 7665 7227 293b 0a20 2020  nresolver');.   
-000000b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000c0: 2020 7065 7273 6f6e 616c 5f62 6172 2070    personal_bar p
-000000d0: 7974 686f 6e3a 2076 6965 772e 6765 745f  ython: view.get_
-000000e0: 7065 7273 6f6e 616c 5f62 6172 2829 3b0a  personal_bar();.
-000000f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000100: 2020 2020 2074 6f6f 6c62 6172 5f70 6f73       toolbar_pos
-00000110: 2076 6965 772f 746f 6f6c 6261 725f 706f   view/toolbar_po
-00000120: 7369 7469 6f6e 220a 2020 2020 2020 2020  sition".        
-00000130: 2074 616c 3a63 6f6e 6469 7469 6f6e 3d22   tal:condition="
-00000140: 636f 6e74 6578 745f 7374 6174 652f 6973  context_state/is
-00000150: 5f74 6f6f 6c62 6172 5f76 6973 6962 6c65  _toolbar_visible
-00000160: 220a 2020 2020 2020 2020 2069 3138 6e3a  ".         i18n:
-00000170: 646f 6d61 696e 3d22 706c 6f6e 6522 3e0a  domain="plone">.
-00000180: 0a0a 2020 3c64 6976 2069 643d 2265 6469  ..  <div id="edi
-00000190: 742d 7a6f 6e65 2220 726f 6c65 3d22 746f  t-zone" role="to
-000001a0: 6f6c 6261 7222 0a20 2020 2020 2020 636c  olbar".       cl
-000001b0: 6173 733d 2270 6174 2d74 6f6f 6c62 6172  ass="pat-toolbar
-000001c0: 2220 6461 7461 2d62 732d 7363 726f 6c6c  " data-bs-scroll
-000001d0: 3d22 7472 7565 223e 0a0a 2020 2020 3c64  ="true">..    <d
-000001e0: 6976 2063 6c61 7373 3d22 746f 6f6c 6261  iv class="toolba
-000001f0: 722d 6865 6164 6572 206e 6176 223e 0a20  r-header nav">. 
-00000200: 2020 2020 203c 6120 636c 6173 733d 2274       <a class="t
-00000210: 6f6f 6c62 6172 2d63 6f6c 6c61 7073 6522  oolbar-collapse"
-00000220: 2061 7269 612d 6c61 6265 6c3d 2255 6e70   aria-label="Unp
-00000230: 696e 2220 6931 386e 3a61 7474 7269 6275  in" i18n:attribu
-00000240: 7465 733d 2261 7269 612d 6c61 6265 6c22  tes="aria-label"
-00000250: 3e0a 2020 2020 2020 2020 3c74 616c 3a69  >.        <tal:i
-00000260: 636f 6e20 7461 6c3a 7265 706c 6163 653d  con tal:replace=
-00000270: 2273 7472 7563 7475 7265 2070 7974 686f  "structure pytho
-00000280: 6e3a 6963 6f6e 732e 7461 6728 2761 7272  n:icons.tag('arr
-00000290: 6f77 2d62 6172 2d6c 6566 7427 2922 202f  ow-bar-left')" /
-000002a0: 3e0a 2020 2020 2020 3c2f 613e 0a20 2020  >.      </a>.   
-000002b0: 2020 203c 6120 636c 6173 733d 2274 6f6f     <a class="too
-000002c0: 6c62 6172 2d65 7870 616e 6422 2061 7269  lbar-expand" ari
-000002d0: 612d 6c61 6265 6c3d 2250 696e 2220 6931  a-label="Pin" i1
-000002e0: 386e 3a61 7474 7269 6275 7465 733d 2261  8n:attributes="a
-000002f0: 7269 612d 6c61 6265 6c22 3e0a 2020 2020  ria-label">.    
-00000300: 2020 2020 3c74 616c 3a69 636f 6e20 7461      <tal:icon ta
-00000310: 6c3a 7265 706c 6163 653d 2273 7472 7563  l:replace="struc
-00000320: 7475 7265 2070 7974 686f 6e3a 6963 6f6e  ture python:icon
-00000330: 732e 7461 6728 2761 7272 6f77 2d62 6172  s.tag('arrow-bar
-00000340: 2d72 6967 6874 2729 2220 2f3e 0a20 2020  -right')" />.   
-00000350: 2020 203c 2f61 3e0a 2020 2020 3c2f 6469     </a>.    </di
-00000360: 763e 0a0a 2020 2020 3c75 6c20 636c 6173  v>..    <ul clas
-00000370: 733d 226e 6176 2066 6c65 782d 636f 6c75  s="nav flex-colu
-00000380: 6d6e 2070 6c6f 6e65 2d74 6f6f 6c62 6172  mn plone-toolbar
-00000390: 2d6d 6169 6e22 0a20 2020 2020 2020 2074  -main".        t
-000003a0: 616c 3a64 6566 696e 653d 2274 6f6f 6c62  al:define="toolb
-000003b0: 6172 5f6d 6169 6e20 7669 6577 2f62 6173  ar_main view/bas
-000003c0: 655f 7265 6e64 6572 220a 2020 2020 2020  e_render".      
-000003d0: 2020 7461 6c3a 636f 6e64 6974 696f 6e3d    tal:condition=
-000003e0: 2274 6f6f 6c62 6172 5f6d 6169 6e22 3e0a  "toolbar_main">.
-000003f0: 2020 2020 2020 3c6c 6920 7461 6c3a 7265        <li tal:re
-00000400: 706c 6163 653d 2273 7472 7563 7475 7265  place="structure
-00000410: 2074 6f6f 6c62 6172 5f6d 6169 6e22 3e0a   toolbar_main">.
-00000420: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
-00000430: 3c2f 756c 3e0a 0a20 2020 203c 6469 7620  </ul>..    <div 
-00000440: 7461 6c3a 636f 6e64 6974 696f 6e3d 2270  tal:condition="p
-00000450: 6572 736f 6e61 6c5f 6261 722f 7573 6572  ersonal_bar/user
-00000460: 5f61 6374 696f 6e73 2220 636c 6173 733d  _actions" class=
-00000470: 2270 6572 736f 6e61 6c74 6f6f 6c73 2d77  "personaltools-w
-00000480: 7261 7070 6572 206e 6176 2024 7b70 7974  rapper nav ${pyt
-00000490: 686f 6e3a 2764 726f 7065 6e64 2720 6966  hon:'dropend' if
-000004a0: 2074 6f6f 6c62 6172 5f70 6f73 203d 3d20   toolbar_pos == 
-000004b0: 2773 6964 6527 2065 6c73 6520 2727 7d22  'side' else ''}"
-000004c0: 3e0a 0a20 2020 2020 203c 6120 6964 3d22  >..      <a id="
-000004d0: 7065 7273 6f6e 616c 746f 6f6c 732d 6d65  personaltools-me
-000004e0: 6e75 6c69 6e6b 220a 2020 2020 2020 2020  nulink".        
-000004f0: 2063 6c61 7373 3d22 6e61 762d 6c69 6e6b   class="nav-link
-00000500: 2064 726f 7064 6f77 6e2d 746f 6767 6c65   dropdown-toggle
-00000510: 220a 2020 2020 2020 2020 2064 6174 612d  ".         data-
-00000520: 6273 2d74 6f67 676c 653d 2264 726f 7064  bs-toggle="dropd
-00000530: 6f77 6e22 0a20 2020 2020 2020 2020 6461  own".         da
-00000540: 7461 2d62 732d 6f66 6673 6574 3d22 302c  ta-bs-offset="0,
-00000550: 3022 0a20 2020 2020 2020 2020 6172 6961  0".         aria
-00000560: 2d65 7870 616e 6465 643d 2266 616c 7365  -expanded="false
-00000570: 220a 2020 2020 2020 2020 2074 616c 3a61  ".         tal:a
-00000580: 7474 7269 6275 7465 733d 2268 7265 6620  ttributes="href 
-00000590: 7065 7273 6f6e 616c 5f62 6172 2f68 6f6d  personal_bar/hom
-000005a0: 656c 696e 6b5f 7572 6c22 3e0a 2020 2020  elink_url">.    
-000005b0: 2020 2020 3c74 616c 3a69 636f 6e20 7461      <tal:icon ta
-000005c0: 6c3a 7265 706c 6163 653d 2273 7472 7563  l:replace="struc
-000005d0: 7475 7265 2070 7974 686f 6e3a 6963 6f6e  ture python:icon
-000005e0: 732e 7461 6728 2774 6f6f 6c62 6172 2d61  s.tag('toolbar-a
-000005f0: 6374 696f 6e2f 7065 7273 6f6e 616c 746f  ction/personalto
-00000600: 6f6c 7327 2c20 7461 675f 636c 6173 733d  ols', tag_class=
-00000610: 2727 2922 202f 3e0a 2020 2020 2020 2020  '')" />.        
-00000620: 3c73 7061 6e20 636c 6173 733d 2274 6f6f  <span class="too
-00000630: 6c62 6172 2d6c 6162 656c 2220 7461 6c3a  lbar-label" tal:
-00000640: 636f 6e74 656e 743d 2270 6572 736f 6e61  content="persona
-00000650: 6c5f 6261 722f 7573 6572 5f6e 616d 6522  l_bar/user_name"
-00000660: 3e55 7365 723c 2f73 7061 6e3e 0a20 2020  >User</span>.   
-00000670: 2020 203c 2f61 3e0a 0a20 2020 2020 203c     </a>..      <
-00000680: 756c 2069 643d 2263 6f6c 6c61 7073 652d  ul id="collapse-
-00000690: 7065 7273 6f6e 616c 746f 6f6c 7322 0a20  personaltools". 
-000006a0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-000006b0: 6472 6f70 646f 776e 2d6d 656e 7522 0a20  dropdown-menu". 
-000006c0: 2020 2020 2020 2020 2061 7269 612d 6c61           aria-la
-000006d0: 6265 6c6c 6564 6279 3d22 7065 7273 6f6e  belledby="person
-000006e0: 616c 746f 6f6c 732d 6d65 6e75 6c69 6e6b  altools-menulink
-000006f0: 223e 0a20 2020 2020 2020 203c 6c69 3e0a  ">.        <li>.
-00000700: 2020 2020 2020 2020 2020 3c68 3620 636c            <h6 cl
-00000710: 6173 733d 2264 726f 7064 6f77 6e2d 6865  ass="dropdown-he
-00000720: 6164 6572 223e 247b 7065 7273 6f6e 616c  ader">${personal
-00000730: 5f62 6172 2f75 7365 725f 6e61 6d65 7d3c  _bar/user_name}<
-00000740: 2f68 363e 0a20 2020 2020 2020 203c 2f6c  /h6>.        </l
-00000750: 693e 0a20 2020 2020 2020 203c 6c69 2074  i>.        <li t
-00000760: 616c 3a72 6570 6561 743d 2261 6374 696f  al:repeat="actio
-00000770: 6e20 7065 7273 6f6e 616c 5f62 6172 2f75  n personal_bar/u
-00000780: 7365 725f 6163 7469 6f6e 7322 3e0a 2020  ser_actions">.  
-00000790: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-000007a0: 2224 7b61 6374 696f 6e2f 6872 6566 7d22  "${action/href}"
-000007b0: 2063 6c61 7373 3d22 6e61 762d 6c69 6e6b   class="nav-link
-000007c0: 2064 726f 7064 6f77 6e2d 6974 656d 223e   dropdown-item">
-000007d0: 0a20 2020 2020 2020 2020 2020 203c 7461  .            <ta
-000007e0: 6c3a 6963 6f6e 2072 6570 6c61 6365 3d22  l:icon replace="
-000007f0: 7374 7275 6374 7572 6520 7079 7468 6f6e  structure python
-00000800: 3a69 636f 6e73 2e74 6167 2861 6374 696f  :icons.tag(actio
-00000810: 6e2e 6765 7428 2769 636f 6e27 2c20 2764  n.get('icon', 'd
-00000820: 6f74 2729 2c20 7461 675f 636c 6173 733d  ot'), tag_class=
-00000830: 2727 2922 202f 3e0a 2020 2020 2020 2020  '')" />.        
-00000840: 2020 2020 3c74 616c 3a61 6374 696f 6e6e      <tal:actionn
-00000850: 616d 6520 7461 6c3a 636f 6e74 656e 743d  ame tal:content=
-00000860: 2261 6374 696f 6e2f 7469 746c 6522 3e0a  "action/title">.
-00000870: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00000880: 7469 6f6e 2074 6974 6c65 0a20 2020 2020  tion title.     
-00000890: 2020 2020 2020 203c 2f74 616c 3a61 6374         </tal:act
-000008a0: 696f 6e6e 616d 653e 0a20 2020 2020 2020  ionname>.       
-000008b0: 2020 203c 2f61 3e0a 2020 2020 2020 2020     </a>.        
-000008c0: 3c2f 6c69 3e0a 2020 2020 2020 3c2f 756c  </li>.      </ul
-000008d0: 3e0a 0a20 2020 203c 2f64 6976 3e0a 2020  >..    </div>.  
-000008e0: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
-000008f0: 3e0a                                     >.
+00000010: 742d 6261 7222 0a20 2020 2020 2020 2020  t-bar".         
+00000020: 726f 6c65 3d22 746f 6f6c 6261 7222 0a20  role="toolbar". 
+00000030: 2020 2020 2020 2020 7461 6c3a 6465 6669          tal:defi
+00000040: 6e65 3d22 0a20 2020 2020 2020 2020 2020  ne=".           
+00000050: 636f 6e74 6578 745f 7374 6174 6520 7669  context_state vi
+00000060: 6577 2f63 6f6e 7465 7874 5f73 7461 7465  ew/context_state
+00000070: 3b0a 2020 2020 2020 2020 2020 2069 636f  ;.           ico
+00000080: 6e73 2070 7974 686f 6e3a 636f 6e74 6578  ns python:contex
+00000090: 742e 7265 7374 7269 6374 6564 5472 6176  t.restrictedTrav
+000000a0: 6572 7365 2827 4040 6963 6f6e 7265 736f  erse('@@iconreso
+000000b0: 6c76 6572 2729 3b0a 2020 2020 2020 2020  lver');.        
+000000c0: 2020 2070 6572 736f 6e61 6c5f 6261 7220     personal_bar 
+000000d0: 7079 7468 6f6e 3a20 7669 6577 2e67 6574  python: view.get
+000000e0: 5f70 6572 736f 6e61 6c5f 6261 7228 293b  _personal_bar();
+000000f0: 0a20 2020 2020 2020 2020 2020 746f 6f6c  .           tool
+00000100: 6261 725f 706f 7320 7669 6577 2f74 6f6f  bar_pos view/too
+00000110: 6c62 6172 5f70 6f73 6974 696f 6e3b 0a20  lbar_position;. 
+00000120: 2020 2020 2020 2020 220a 2020 2020 2020          ".      
+00000130: 2020 2074 616c 3a63 6f6e 6469 7469 6f6e     tal:condition
+00000140: 3d22 636f 6e74 6578 745f 7374 6174 652f  ="context_state/
+00000150: 6973 5f74 6f6f 6c62 6172 5f76 6973 6962  is_toolbar_visib
+00000160: 6c65 220a 2020 2020 2020 2020 2069 3138  le".         i18
+00000170: 6e3a 646f 6d61 696e 3d22 706c 6f6e 6522  n:domain="plone"
+00000180: 0a3e 0a0a 0a20 203c 6469 7620 636c 6173  .>...  <div clas
+00000190: 733d 2270 6174 2d74 6f6f 6c62 6172 220a  s="pat-toolbar".
+000001a0: 2020 2020 2020 2069 643d 2265 6469 742d         id="edit-
+000001b0: 7a6f 6e65 220a 2020 2020 2020 2072 6f6c  zone".       rol
+000001c0: 653d 2274 6f6f 6c62 6172 220a 2020 2020  e="toolbar".    
+000001d0: 2020 2064 6174 612d 6273 2d73 6372 6f6c     data-bs-scrol
+000001e0: 6c3d 2274 7275 6522 0a20 203e 0a0a 2020  l="true".  >..  
+000001f0: 2020 3c64 6976 2063 6c61 7373 3d22 746f    <div class="to
+00000200: 6f6c 6261 722d 6865 6164 6572 206e 6176  olbar-header nav
+00000210: 223e 0a20 2020 2020 203c 6120 636c 6173  ">.      <a clas
+00000220: 733d 2274 6f6f 6c62 6172 2d63 6f6c 6c61  s="toolbar-colla
+00000230: 7073 6522 0a20 2020 2020 2020 2020 6172  pse".         ar
+00000240: 6961 2d6c 6162 656c 3d22 556e 7069 6e22  ia-label="Unpin"
+00000250: 0a20 2020 2020 2020 2020 6931 386e 3a61  .         i18n:a
+00000260: 7474 7269 6275 7465 733d 2261 7269 612d  ttributes="aria-
+00000270: 6c61 6265 6c22 0a20 2020 2020 203e 0a20  label".      >. 
+00000280: 2020 2020 2020 203c 7461 6c3a 6963 6f6e         <tal:icon
+00000290: 2074 616c 3a72 6570 6c61 6365 3d22 7374   tal:replace="st
+000002a0: 7275 6374 7572 6520 7079 7468 6f6e 3a69  ructure python:i
+000002b0: 636f 6e73 2e74 6167 2827 6172 726f 772d  cons.tag('arrow-
+000002c0: 6261 722d 6c65 6674 2729 2220 2f3e 0a20  bar-left')" />. 
+000002d0: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
+000002e0: 3c61 2063 6c61 7373 3d22 746f 6f6c 6261  <a class="toolba
+000002f0: 722d 6578 7061 6e64 220a 2020 2020 2020  r-expand".      
+00000300: 2020 2061 7269 612d 6c61 6265 6c3d 2250     aria-label="P
+00000310: 696e 220a 2020 2020 2020 2020 2069 3138  in".         i18
+00000320: 6e3a 6174 7472 6962 7574 6573 3d22 6172  n:attributes="ar
+00000330: 6961 2d6c 6162 656c 220a 2020 2020 2020  ia-label".      
+00000340: 3e0a 2020 2020 2020 2020 3c74 616c 3a69  >.        <tal:i
+00000350: 636f 6e20 7461 6c3a 7265 706c 6163 653d  con tal:replace=
+00000360: 2273 7472 7563 7475 7265 2070 7974 686f  "structure pytho
+00000370: 6e3a 6963 6f6e 732e 7461 6728 2761 7272  n:icons.tag('arr
+00000380: 6f77 2d62 6172 2d72 6967 6874 2729 2220  ow-bar-right')" 
+00000390: 2f3e 0a20 2020 2020 203c 2f61 3e0a 2020  />.      </a>.  
+000003a0: 2020 3c2f 6469 763e 0a0a 2020 2020 3c75    </div>..    <u
+000003b0: 6c20 636c 6173 733d 226e 6176 2066 6c65  l class="nav fle
+000003c0: 782d 636f 6c75 6d6e 2070 6c6f 6e65 2d74  x-column plone-t
+000003d0: 6f6f 6c62 6172 2d6d 6169 6e22 0a20 2020  oolbar-main".   
+000003e0: 2020 2020 2074 616c 3a64 6566 696e 653d       tal:define=
+000003f0: 220a 2020 2020 2020 2020 2020 746f 6f6c  ".          tool
+00000400: 6261 725f 6d61 696e 2076 6965 772f 6261  bar_main view/ba
+00000410: 7365 5f72 656e 6465 723b 0a20 2020 2020  se_render;.     
+00000420: 2020 2022 0a20 2020 2020 2020 2074 616c     ".        tal
+00000430: 3a63 6f6e 6469 7469 6f6e 3d22 746f 6f6c  :condition="tool
+00000440: 6261 725f 6d61 696e 220a 2020 2020 3e0a  bar_main".    >.
+00000450: 2020 2020 2020 3c6c 6920 7461 6c3a 7265        <li tal:re
+00000460: 706c 6163 653d 2273 7472 7563 7475 7265  place="structure
+00000470: 2074 6f6f 6c62 6172 5f6d 6169 6e22 3e0a   toolbar_main">.
+00000480: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+00000490: 3c2f 756c 3e0a 0a20 2020 203c 6469 7620  </ul>..    <div 
+000004a0: 636c 6173 733d 2270 6572 736f 6e61 6c74  class="personalt
+000004b0: 6f6f 6c73 2d77 7261 7070 6572 206e 6176  ools-wrapper nav
+000004c0: 2024 7b70 7974 686f 6e3a 2764 726f 7065   ${python:'drope
+000004d0: 6e64 2720 6966 2074 6f6f 6c62 6172 5f70  nd' if toolbar_p
+000004e0: 6f73 203d 3d20 2773 6964 6527 2065 6c73  os == 'side' els
+000004f0: 6520 2727 7d22 0a20 2020 2020 2020 2020  e ''}".         
+00000500: 7461 6c3a 636f 6e64 6974 696f 6e3d 2270  tal:condition="p
+00000510: 6572 736f 6e61 6c5f 6261 722f 7573 6572  ersonal_bar/user
+00000520: 5f61 6374 696f 6e73 220a 2020 2020 3e0a  _actions".    >.
+00000530: 0a20 2020 2020 203c 6120 636c 6173 733d  .      <a class=
+00000540: 226e 6176 2d6c 696e 6b20 6472 6f70 646f  "nav-link dropdo
+00000550: 776e 2d74 6f67 676c 6522 0a20 2020 2020  wn-toggle".     
+00000560: 2020 2020 6964 3d22 7065 7273 6f6e 616c      id="personal
+00000570: 746f 6f6c 732d 6d65 6e75 6c69 6e6b 220a  tools-menulink".
+00000580: 2020 2020 2020 2020 2061 7269 612d 6578           aria-ex
+00000590: 7061 6e64 6564 3d22 6661 6c73 6522 0a20  panded="false". 
+000005a0: 2020 2020 2020 2020 6461 7461 2d62 732d          data-bs-
+000005b0: 6f66 6673 6574 3d22 302c 3022 0a20 2020  offset="0,0".   
+000005c0: 2020 2020 2020 6461 7461 2d62 732d 746f        data-bs-to
+000005d0: 6767 6c65 3d22 6472 6f70 646f 776e 220a  ggle="dropdown".
+000005e0: 2020 2020 2020 2020 2074 616c 3a61 7474           tal:att
+000005f0: 7269 6275 7465 733d 220a 2020 2020 2020  ributes=".      
+00000600: 2020 2020 2068 7265 6620 7065 7273 6f6e       href person
+00000610: 616c 5f62 6172 2f68 6f6d 656c 696e 6b5f  al_bar/homelink_
+00000620: 7572 6c3b 0a20 2020 2020 2020 2020 220a  url;.         ".
+00000630: 2020 2020 2020 3e0a 2020 2020 2020 2020        >.        
+00000640: 3c74 616c 3a69 636f 6e20 7461 6c3a 7265  <tal:icon tal:re
+00000650: 706c 6163 653d 2273 7472 7563 7475 7265  place="structure
+00000660: 2070 7974 686f 6e3a 6963 6f6e 732e 7461   python:icons.ta
+00000670: 6728 2774 6f6f 6c62 6172 2d61 6374 696f  g('toolbar-actio
+00000680: 6e2f 7065 7273 6f6e 616c 746f 6f6c 7327  n/personaltools'
+00000690: 2c20 7461 675f 636c 6173 733d 2727 2922  , tag_class='')"
+000006a0: 202f 3e0a 2020 2020 2020 2020 3c73 7061   />.        <spa
+000006b0: 6e20 636c 6173 733d 2274 6f6f 6c62 6172  n class="toolbar
+000006c0: 2d6c 6162 656c 220a 2020 2020 2020 2020  -label".        
+000006d0: 2020 2020 2020 7461 6c3a 636f 6e74 656e        tal:conten
+000006e0: 743d 2270 6572 736f 6e61 6c5f 6261 722f  t="personal_bar/
+000006f0: 7573 6572 5f6e 616d 6522 0a20 2020 2020  user_name".     
+00000700: 2020 203e 5573 6572 3c2f 7370 616e 3e0a     >User</span>.
+00000710: 2020 2020 2020 3c2f 613e 0a0a 2020 2020        </a>..    
+00000720: 2020 3c75 6c20 636c 6173 733d 2264 726f    <ul class="dro
+00000730: 7064 6f77 6e2d 6d65 6e75 220a 2020 2020  pdown-menu".    
+00000740: 2020 2020 2020 6964 3d22 636f 6c6c 6170        id="collap
+00000750: 7365 2d70 6572 736f 6e61 6c74 6f6f 6c73  se-personaltools
+00000760: 220a 2020 2020 2020 2020 2020 6172 6961  ".          aria
+00000770: 2d6c 6162 656c 6c65 6462 793d 2270 6572  -labelledby="per
+00000780: 736f 6e61 6c74 6f6f 6c73 2d6d 656e 756c  sonaltools-menul
+00000790: 696e 6b22 0a20 2020 2020 203e 0a20 2020  ink".      >.   
+000007a0: 2020 2020 203c 6c69 3e0a 2020 2020 2020       <li>.      
+000007b0: 2020 2020 3c68 3620 636c 6173 733d 2264      <h6 class="d
+000007c0: 726f 7064 6f77 6e2d 6865 6164 6572 223e  ropdown-header">
+000007d0: 247b 7065 7273 6f6e 616c 5f62 6172 2f75  ${personal_bar/u
+000007e0: 7365 725f 6e61 6d65 7d3c 2f68 363e 0a20  ser_name}</h6>. 
+000007f0: 2020 2020 2020 203c 2f6c 693e 0a20 2020         </li>.   
+00000800: 2020 2020 203c 6c69 2074 616c 3a72 6570       <li tal:rep
+00000810: 6561 743d 2261 6374 696f 6e20 7065 7273  eat="action pers
+00000820: 6f6e 616c 5f62 6172 2f75 7365 725f 6163  onal_bar/user_ac
+00000830: 7469 6f6e 7322 3e0a 2020 2020 2020 2020  tions">.        
+00000840: 2020 3c61 2063 6c61 7373 3d22 6e61 762d    <a class="nav-
+00000850: 6c69 6e6b 2064 726f 7064 6f77 6e2d 6974  link dropdown-it
+00000860: 656d 220a 2020 2020 2020 2020 2020 2020  em".            
+00000870: 2068 7265 663d 2224 7b61 6374 696f 6e2f   href="${action/
+00000880: 6872 6566 7d22 0a20 2020 2020 2020 2020  href}".         
+00000890: 203e 0a20 2020 2020 2020 2020 2020 203c   >.            <
+000008a0: 7461 6c3a 6963 6f6e 2072 6570 6c61 6365  tal:icon replace
+000008b0: 3d22 7374 7275 6374 7572 6520 7079 7468  ="structure pyth
+000008c0: 6f6e 3a69 636f 6e73 2e74 6167 2861 6374  on:icons.tag(act
+000008d0: 696f 6e2e 6765 7428 2769 636f 6e27 2c20  ion.get('icon', 
+000008e0: 2764 6f74 2729 2c20 7461 675f 636c 6173  'dot'), tag_clas
+000008f0: 733d 2727 2922 202f 3e0a 2020 2020 2020  s='')" />.      
+00000900: 2020 2020 2020 3c74 616c 3a61 6374 696f        <tal:actio
+00000910: 6e6e 616d 6520 7461 6c3a 636f 6e74 656e  nname tal:conten
+00000920: 743d 2261 6374 696f 6e2f 7469 746c 6522  t="action/title"
+00000930: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000940: 6163 7469 6f6e 2074 6974 6c65 0a20 2020  action title.   
+00000950: 2020 2020 2020 2020 203c 2f74 616c 3a61           </tal:a
+00000960: 6374 696f 6e6e 616d 653e 0a20 2020 2020  ctionname>.     
+00000970: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
+00000980: 2020 3c2f 6c69 3e0a 2020 2020 2020 3c2f    </li>.      </
+00000990: 756c 3e0a 0a20 2020 203c 2f64 6976 3e0a  ul>..    </div>.
+000009a0: 2020 3c2f 6469 763e 0a3c 2f73 6563 7469    </div>.</secti
+000009b0: 6f6e 3e0a                                on>.
```

### Comparing `plone.app.layout-4.0.2/plone/app/layout/viewlets/toolbar.py` & `plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from plone.app.layout.viewlets.common import PersonalBarViewlet
 from plone.app.viewletmanager.manager import OrderedViewletManager
+from plone.base.interfaces.controlpanel import ISiteSchema
 from plone.memoize.instance import memoize
 from plone.registry.interfaces import IRegistry
-from plone.base.interfaces.controlpanel import ISiteSchema
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 
 
 class ToolbarViewletManager(OrderedViewletManager):
     custom_template = ViewPageTemplateFile("toolbar.pt")
```

### Comparing `plone.app.layout-4.0.2/plone.app.layout.egg-info/PKG-INFO` & `plone.app.layout-4.0.3/plone.app.layout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.2
+Version: 4.0.3
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -49,14 +49,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-04-15)
+------------------
+
+Bug fixes:
+
+
+- Remove Archetypes code from TOC viewlet.
+  @jensens (rm-at-code-from-toc)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (11f0db91)
+
+
 4.0.2 (2023-03-14)
 ------------------
 
 Bug fixes:
 
 
 - Move interface plone.app.layout.navigation.interfaces.INavigationRoot to plone.base.interfaces.siteroot and add a deprecated import to plone.app.layout.
@@ -433,15 +450,15 @@
 3.4.1 (2020-03-09)
 ------------------
 
 Bug fixes:
 
 
 - Analytics viewlet: make webstats_js a property, so that it does not rely on an a call to the update method to be correctly evaluated [ale-rt] (#227)
-- Code formating according to Plone standards (black, isort).
+- Code formatting according to Plone standards (black, isort).
   [thet] (#230)
 - Remove selectedTabs and update method from GlobalSectionsViewlet as both are now unused.
   [thet] (#231)
 - Remove deprecation warnings [ale-rt] (#233)
 - Integrate Plone20200121 hotfix: prevent XSS in title.
   Part of https://plone.org/security/hotfix/20200121/xss-in-the-title-field-on-plone-5-0-and-higher
   [maurits] (#3021)
@@ -468,15 +485,15 @@
 
 3.3.0 (2019-10-12)
 ------------------
 
 New features:
 
 
-- Add a sorrounding div to the webstats js. Fixes #157
+- Add a surrounding div to the webstats js. Fixes #157
   [erral] (#157)
 
 
 Bug fixes:
 
 
 - Fix memory leak on getUserInfo [avoinea] (#204) (#210)
@@ -617,15 +634,15 @@
 ------------------
 
 New features:
 
 - Allow addition of extra body classes via multiple IBodyClassAdapter adapter registrations without the need to overload the ILayoutPolicy view.
   [thet, jensens, agitator]
 
-- Make it easier to override seperator in title viewlet
+- Make it easier to override separator in title viewlet
   [tomgross]
 
 Bug fixes:
 
 - Do not use ``rel="tag"`` attribute on the keywords viewlet as the referenced document is not a tag definition but a search result;
   use ``rel="nofollow"`` instead to avoid search crawlers hammering our sites.
   [hvelarde]
@@ -683,15 +700,15 @@
 New features:
 
 - Added membertools viewlet. If user is not anonymous and toolbar is not visible according to ``is_toolbar_visible`` the viewlet will show at the location of anontools.
   [agitator]
 
 Bug fixes:
 
-- show 'in current section only' before seach input field for a11y reasons. https://github.com/plone/Products.CMFPlone/issues/1619 [polyester]
+- show 'in current section only' before search input field for a11y reasons. https://github.com/plone/Products.CMFPlone/issues/1619 [polyester]
 
 
 2.7.1 (2017-07-03)
 ------------------
 
 Bug fixes:
 
@@ -792,15 +809,15 @@
 
 
 2.6.1 (2016-06-07)
 ------------------
 
 Bug fixes:
 
-- Document byline viewlet is now displayed only to anonymous users if permited by the `Allow anyone to view 'about' information` option in the `Security Settings` of `Site Setup` (closes `CMFPlone#1556`_).
+- Document byline viewlet is now displayed only to anonymous users if permitted by the `Allow anyone to view 'about' information` option in the `Security Settings` of `Site Setup` (closes `CMFPlone#1556`_).
   Code used to show the lock status and history view was removed from the document byline as this information was not available to anonymous users anyway.
   [hvelarde]
 
 
 2.6.0 (2016-05-10)
 ------------------
 
@@ -1009,15 +1026,15 @@
 
 - always show site root syndication links if enabled
   [vangheem]
 
 - by default, show site logo in social settings
   [vangheem]
 
-- Add aria hidden role to avoid screenreaders to nonesense stop by at the
+- Add aria hidden role to avoid screenreaders to nonsense stop by at the
   toolbar tiny logo [sneridagh]
 
 - Get rid completely of the plone.skip_links viewlet because it already doesn't
   worked OOTB since always and this does not follow modern a11y methods and we
   are dropping support for outdated ways [sneridagh]
 
 - Remove all references to "accesskeys" attributes on templates [sneridagh]
@@ -1340,15 +1357,15 @@
 
 2.3.4 (2013-03-05)
 ------------------
 
 - handle missing feed type so it doesn't throw an error
   [vangheem]
 
-- handle absense of ACTUAL_URL on request.
+- handle absence of ACTUAL_URL on request.
   Fixes https://dev.plone.org/ticket/13173
   [vangheem]
 
 - Also show history on the folder contents view
   [vangheem]
 
 
@@ -1404,28 +1421,28 @@
 2.3 (2012-08-11)
 ----------------
 
 - Change breadcrumb separator to / (slash character) for accessibility, and added SEO benefits.
   see https://dev.plone.org/ticket/12904
   [polyester]
 
-- Add language atribute to presentation.pt for WCAG 2.0 compliance.
+- Add language attribute to presentation.pt for WCAG 2.0 compliance.
   See https://dev.plone.org/ticket/12902
   [rmatt, polyester]
 
 - Display publication date in author byline:
   https://dev.plone.org/ticket/8699
   [vipod]
 
 - Remove hard dependency on ATContentTypes.
   [davisagli]
 
 - Correctly hand action URLs not ending / [phrearch]
 
-- Removed obsolete 'define-macro' and 'define-slot' from viewlet page tempates.
+- Removed obsolete 'define-macro' and 'define-slot' from viewlet page templates.
   Fixes http://dev.plone.org/ticket/11541.
   [kleist]
 
 - nextprevious/nextprevious.pt: Use "view/site_url" instead of deprecated "view/portal_url".
   Closes http://dev.plone.org/ticket/12720.
   [kleist]
 
@@ -1436,15 +1453,15 @@
 2.2.7 (2012-08-11)
 ------------------
 
 - Change breadcrumb separator to / (slash character) for accessibility, and added SEO benefits.
   see https://dev.plone.org/ticket/12904
   [polyester]
 
-- Add language atribute to presentation.pt for WCAG 2.0 compliance.
+- Add language attribute to presentation.pt for WCAG 2.0 compliance.
   See https://dev.plone.org/ticket/12902
   [rmatt, polyester]
 
 - Remove hard dependency on ATContentTypes.
   [davisagli]
 
 - Add body class for each part of url path. plip12905
@@ -1476,15 +1493,15 @@
 - Added a page as a not-js fallback for the user dropdown menu
   [giacomos]
 
 
 2.2.4 (2011-12-03)
 ------------------
 
-- Add the ability for the navtree strategy to suppliment the query.
+- Add the ability for the navtree strategy to supplement the query.
   Fixes a problem where the listing of default pages in navigation
   trees could no longer be enabled.
   [rossp]
 
 
 2.2.3 (2011-10-17)
 ------------------
```

### Comparing `plone.app.layout-4.0.2/plone.app.layout.egg-info/SOURCES.txt` & `plone.app.layout-4.0.3/plone.app.layout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.2/setup.py` & `plone.app.layout-4.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.2"
+version = "4.0.3"
 
 long_description = open("README.rst").read() + "\n" + open("CHANGES.rst").read()
 
 setup(
     name="plone.app.layout",
     version=version,
     description="Layout mechanisms for Plone",
@@ -33,46 +33,40 @@
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
-        "Acquisition",
-        "DateTime",
+        "BTrees",
         "plone.app.content",
+        "plone.app.multilingual",
+        "plone.app.relationfield",
+        "plone.app.uuid",
         "plone.app.viewletmanager >=1.2",
         "plone.base >=1.0.4",
-        "plone.batching >=2.0.0",
+        "plone.dexterity",
+        "plone.formwidget.namedfile",
         "plone.i18n",
         "plone.memoize",
         "plone.portlets",
-        "plone.registry",
-        "Products.CMFCore",
-        "Products.CMFDynamicViewFTI",
+        "plone.protect",
         "Products.CMFEditions >=1.2.2",
+        "Products.statusmessages",
+        "Products.ZCatalog",
         "setuptools",
-        "zope.component",
-        "zope.deferredimport",
-        "zope.deprecation",
-        "zope.dottedname",
-        "zope.i18n",
-        "zope.interface",
-        "zope.publisher",
-        "zope.schema",
-        "zope.viewlet",
         "Zope",
     ],
     extras_require=dict(
         test=[
-            "plone.app.contenttypes",
-            "plone.app.intid",
+            "plone.app.contenttypes[test]",
             "plone.app.relationfield",
             "plone.app.testing",
             "plone.dexterity",
             "plone.locking",
             "plone.testing",
             "z3c.relationfield",
             "zope.annotation",
+            "zope.intid",
         ]
     ),
 )
```

