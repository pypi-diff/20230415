# Comparing `tmp/pynytimes-0.9.0.tar.gz` & `tmp/pynytimes-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynytimes-0.9.0.tar", last modified: Tue Jan 10 15:12:37 2023, max compression
+gzip compressed data, was "pynytimes-0.9.2.tar", last modified: Sat Apr 15 13:21:42 2023, max compression
```

## Comparing `pynytimes-0.9.0.tar` & `pynytimes-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 15:12:37.332302 pynytimes-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 15:12:37.328302 pynytimes-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-01-10 15:12:03.000000 pynytimes-0.9.0/.github/poweredby_nytimes.png
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-01-10 15:12:03.000000 pynytimes-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-10 15:12:03.000000 pynytimes-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-01-10 15:12:37.332302 pynytimes-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-01-10 15:12:03.000000 pynytimes-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 15:12:37.328302 pynytimes-0.9.0/pynytimes/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 15:12:37.332302 pynytimes-0.9.0/pynytimes/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/article_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/article_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/best_sellers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/book_reviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/latest_articles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/most_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/most_viewed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/movie_reviews.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-10 15:12:03.000000 pynytimes-0.9.0/pynytimes/helpers/tag_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 15:12:37.332302 pynytimes-0.9.0/pynytimes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-01-10 15:12:37.000000 pynytimes-0.9.0/pynytimes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-10 15:12:37.000000 pynytimes-0.9.0/pynytimes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 15:12:37.000000 pynytimes-0.9.0/pynytimes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-10 15:12:37.000000 pynytimes-0.9.0/pynytimes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-10 15:12:37.000000 pynytimes-0.9.0/pynytimes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 15:12:37.332302 pynytimes-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-10 15:12:03.000000 pynytimes-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:21:42.822831 pynytimes-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:21:42.818831 pynytimes-0.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-15 13:21:33.000000 pynytimes-0.9.2/.github/poweredby_nytimes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-15 13:21:33.000000 pynytimes-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 13:21:33.000000 pynytimes-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-15 13:21:42.822831 pynytimes-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-15 13:21:33.000000 pynytimes-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:21:42.818831 pynytimes-0.9.2/pynytimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24707 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:21:42.822831 pynytimes-0.9.2/pynytimes/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/article_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/article_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/best_sellers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/book_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/latest_articles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/most_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/most_viewed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/movie_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-15 13:21:33.000000 pynytimes-0.9.2/pynytimes/helpers/tag_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:21:42.822831 pynytimes-0.9.2/pynytimes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-15 13:21:42.000000 pynytimes-0.9.2/pynytimes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 13:21:42.000000 pynytimes-0.9.2/pynytimes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:21:42.000000 pynytimes-0.9.2/pynytimes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 13:21:42.000000 pynytimes-0.9.2/pynytimes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 13:21:42.000000 pynytimes-0.9.2/pynytimes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:21:42.822831 pynytimes-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-15 13:21:33.000000 pynytimes-0.9.2/setup.py
```

### Comparing `pynytimes-0.9.0/.github/poweredby_nytimes.png` & `pynytimes-0.9.2/.github/poweredby_nytimes.png`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/LICENSE` & `pynytimes-0.9.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 - 2022 Micha den Heijer
+Copyright (c) 2019 - 2023 Micha den Heijer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pynytimes-0.9.0/PKG-INFO` & `pynytimes-0.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynytimes
-Version: 0.9.0
+Version: 0.9.2
 Summary: A Python wrapper for (most) New York Times APIs
 Home-page: https://pynytimes.michadenheijer.com/
 Author: Micha den Heijer
 Author-email: micha@michadenheijer.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynytimes
 
 [<img src="https://raw.githubusercontent.com/michadenheijer/pynytimes/main/.github/poweredby_nytimes.png" height="20px">](https://developer.nytimes.com/) [![Run full tests](https://github.com/michadenheijer/pynytimes/actions/workflows/python-full-tests.yaml/badge.svg)](https://github.com/michadenheijer/pynytimes/actions/workflows/python-full-tests.yaml)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynytimes)](https://pypi.org/project/pynytimes/) [![PyPI](https://img.shields.io/pypi/v/pynytimes)](https://pypi.org/project/pynytimes/) [![Downloads](https://pepy.tech/badge/pynytimes)](https://pepy.tech/project/pynytimes) [![Maintainability](https://api.codeclimate.com/v1/badges/7a5ad012587ba707271c/maintainability)](https://codeclimate.com/github/michadenheijer/pynytimes/maintainability)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynytimes)](https://pypi.org/project/pynytimes/) [![PyPI](https://img.shields.io/pypi/v/pynytimes)](https://pypi.org/project/pynytimes/) [![Downloads](https://pepy.tech/badge/pynytimes)](https://pepy.tech/project/pynytimes) [![DOI](https://zenodo.org/badge/216087297.svg)](https://zenodo.org/badge/latestdoi/216087297)
 
 Use all (actually most) New York Times APIs, get all the data you need from the Times!
 
 ## Documentation
 
 Extensive documentation is available at: https://pynytimes.michadenheijer.com/.
 
@@ -212,12 +212,29 @@
 data = nyt.archive_metadata(
     date = datetime.datetime(2019, 1, 1)
 )
 ```
 
 [Read more in the documentation](https://pynytimes.michadenheijer.com/metadata/archive-metadata).
 
+## Citing this Repository
+If you use ```pynytimes```, a citation would be very much appriciated. If you're using BibTeX you can use the following citation:
+
+```bib
+@software{Den_Heijer_pynytimes_2023,
+    author = {Den Heijer, Micha},
+    license = {MIT},
+    title = {{pynytimes}},
+    url = {https://github.com/michadenheijer/pynytimes},
+    version = {[CITATION VERSION]},
+    year = {[CITATION YEAR]},
+    doi = {10.5281/zenodo.7821090}
+}
+```
+
+If you're not using BibTeX, you can [retrieve the preferred citation from Zenodo](https://doi.org/10.5281/zenodo.7821090).
+
 ## License
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 
 **Disclaimer**: *This project is not made by anyone from the New York Times, nor is it affiliated with The New York Times Company.*
```

### Comparing `pynytimes-0.9.0/README.md` & `pynytimes-0.9.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pynytimes
 
 [<img src="https://raw.githubusercontent.com/michadenheijer/pynytimes/main/.github/poweredby_nytimes.png" height="20px">](https://developer.nytimes.com/) [![Run full tests](https://github.com/michadenheijer/pynytimes/actions/workflows/python-full-tests.yaml/badge.svg)](https://github.com/michadenheijer/pynytimes/actions/workflows/python-full-tests.yaml)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynytimes)](https://pypi.org/project/pynytimes/) [![PyPI](https://img.shields.io/pypi/v/pynytimes)](https://pypi.org/project/pynytimes/) [![Downloads](https://pepy.tech/badge/pynytimes)](https://pepy.tech/project/pynytimes) [![Maintainability](https://api.codeclimate.com/v1/badges/7a5ad012587ba707271c/maintainability)](https://codeclimate.com/github/michadenheijer/pynytimes/maintainability)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynytimes)](https://pypi.org/project/pynytimes/) [![PyPI](https://img.shields.io/pypi/v/pynytimes)](https://pypi.org/project/pynytimes/) [![Downloads](https://pepy.tech/badge/pynytimes)](https://pepy.tech/project/pynytimes) [![DOI](https://zenodo.org/badge/216087297.svg)](https://zenodo.org/badge/latestdoi/216087297)
 
 Use all (actually most) New York Times APIs, get all the data you need from the Times!
 
 ## Documentation
 
 Extensive documentation is available at: https://pynytimes.michadenheijer.com/.
 
@@ -188,12 +188,29 @@
 data = nyt.archive_metadata(
     date = datetime.datetime(2019, 1, 1)
 )
 ```
 
 [Read more in the documentation](https://pynytimes.michadenheijer.com/metadata/archive-metadata).
 
+## Citing this Repository
+If you use ```pynytimes```, a citation would be very much appriciated. If you're using BibTeX you can use the following citation:
+
+```bib
+@software{Den_Heijer_pynytimes_2023,
+    author = {Den Heijer, Micha},
+    license = {MIT},
+    title = {{pynytimes}},
+    url = {https://github.com/michadenheijer/pynytimes},
+    version = {[CITATION VERSION]},
+    year = {[CITATION YEAR]},
+    doi = {10.5281/zenodo.7821090}
+}
+```
+
+If you're not using BibTeX, you can [retrieve the preferred citation from Zenodo](https://doi.org/10.5281/zenodo.7821090).
+
 ## License
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 
 **Disclaimer**: *This project is not made by anyone from the New York Times, nor is it affiliated with The New York Times Company.*
```

### Comparing `pynytimes-0.9.0/pynytimes/api.py` & `pynytimes-0.9.2/pynytimes/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Define all URLs that are needed
 BASE_URL: Final = "api.nytimes.com/svc/"
 BASE_TOP_STORIES: Final = BASE_URL + "topstories/v2/"
 BASE_MOST_POPULAR: Final = BASE_URL + "mostpopular/v2/"
 BASE_BOOKS: Final = BASE_URL + "books/v3/"
 BASE_MOVIE_REVIEWS: Final = BASE_URL + "movies/v2/reviews/search.json"
 BASE_META_DATA: Final = BASE_URL + "news/v3/content.json"
-BASE_TAGS: Final = BASE_URL + "semantic/v2/concept/suggest"
+BASE_TAGS: Final = BASE_URL + "suggest/v1/timestags"
 BASE_ARCHIVE_METADATA: Final = BASE_URL + "archive/v1/"
 BASE_ARTICLE_SEARCH: Final = BASE_URL + "search/v2/articlesearch.json"
 BASE_LATEST_ARTICLES: Final = BASE_URL + "news/v3/content/"
 BASE_SECTION_LIST: Final = BASE_URL + "news/v3/content/section-list.json"
 BASE_BOOK_REVIEWS: Final = BASE_BOOKS + "reviews.json"
 BASE_BEST_SELLERS_LISTS: Final = BASE_BOOKS + "lists/names.json"
 BASE_BEST_SELLERS_LIST: Final = BASE_BOOKS + "lists/"
```

### Comparing `pynytimes-0.9.0/pynytimes/helpers/__init__.py` & `pynytimes-0.9.2/pynytimes/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/article_metadata.py` & `pynytimes-0.9.2/pynytimes/helpers/article_metadata.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/article_search.py` & `pynytimes-0.9.2/pynytimes/helpers/article_search.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/best_sellers.py` & `pynytimes-0.9.2/pynytimes/helpers/best_sellers.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/book_reviews.py` & `pynytimes-0.9.2/pynytimes/helpers/book_reviews.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/dates.py` & `pynytimes-0.9.2/pynytimes/helpers/dates.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/latest_articles.py` & `pynytimes-0.9.2/pynytimes/helpers/latest_articles.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/load_data.py` & `pynytimes-0.9.2/pynytimes/helpers/load_data.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/most_shared.py` & `pynytimes-0.9.2/pynytimes/helpers/most_shared.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/movie_reviews.py` & `pynytimes-0.9.2/pynytimes/helpers/movie_reviews.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes/helpers/tag_query.py` & `pynytimes-0.9.2/pynytimes/helpers/tag_query.py`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/pynytimes.egg-info/PKG-INFO` & `pynytimes-0.9.2/pynytimes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynytimes
-Version: 0.9.0
+Version: 0.9.2
 Summary: A Python wrapper for (most) New York Times APIs
 Home-page: https://pynytimes.michadenheijer.com/
 Author: Micha den Heijer
 Author-email: micha@michadenheijer.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynytimes
 
 [<img src="https://raw.githubusercontent.com/michadenheijer/pynytimes/main/.github/poweredby_nytimes.png" height="20px">](https://developer.nytimes.com/) [![Run full tests](https://github.com/michadenheijer/pynytimes/actions/workflows/python-full-tests.yaml/badge.svg)](https://github.com/michadenheijer/pynytimes/actions/workflows/python-full-tests.yaml)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynytimes)](https://pypi.org/project/pynytimes/) [![PyPI](https://img.shields.io/pypi/v/pynytimes)](https://pypi.org/project/pynytimes/) [![Downloads](https://pepy.tech/badge/pynytimes)](https://pepy.tech/project/pynytimes) [![Maintainability](https://api.codeclimate.com/v1/badges/7a5ad012587ba707271c/maintainability)](https://codeclimate.com/github/michadenheijer/pynytimes/maintainability)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynytimes)](https://pypi.org/project/pynytimes/) [![PyPI](https://img.shields.io/pypi/v/pynytimes)](https://pypi.org/project/pynytimes/) [![Downloads](https://pepy.tech/badge/pynytimes)](https://pepy.tech/project/pynytimes) [![DOI](https://zenodo.org/badge/216087297.svg)](https://zenodo.org/badge/latestdoi/216087297)
 
 Use all (actually most) New York Times APIs, get all the data you need from the Times!
 
 ## Documentation
 
 Extensive documentation is available at: https://pynytimes.michadenheijer.com/.
 
@@ -212,12 +212,29 @@
 data = nyt.archive_metadata(
     date = datetime.datetime(2019, 1, 1)
 )
 ```
 
 [Read more in the documentation](https://pynytimes.michadenheijer.com/metadata/archive-metadata).
 
+## Citing this Repository
+If you use ```pynytimes```, a citation would be very much appriciated. If you're using BibTeX you can use the following citation:
+
+```bib
+@software{Den_Heijer_pynytimes_2023,
+    author = {Den Heijer, Micha},
+    license = {MIT},
+    title = {{pynytimes}},
+    url = {https://github.com/michadenheijer/pynytimes},
+    version = {[CITATION VERSION]},
+    year = {[CITATION YEAR]},
+    doi = {10.5281/zenodo.7821090}
+}
+```
+
+If you're not using BibTeX, you can [retrieve the preferred citation from Zenodo](https://doi.org/10.5281/zenodo.7821090).
+
 ## License
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 
 **Disclaimer**: *This project is not made by anyone from the New York Times, nor is it affiliated with The New York Times Company.*
```

### Comparing `pynytimes-0.9.0/pynytimes.egg-info/SOURCES.txt` & `pynytimes-0.9.2/pynytimes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynytimes-0.9.0/setup.py` & `pynytimes-0.9.2/setup.py`

 * *Files identical despite different names*

