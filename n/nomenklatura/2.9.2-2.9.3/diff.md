# Comparing `tmp/nomenklatura-2.9.2.tar.gz` & `tmp/nomenklatura-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-2.9.2.tar", last modified: Thu Apr 13 11:43:14 2023, max compression
+gzip compressed data, was "nomenklatura-2.9.3.tar", last modified: Sat Apr 15 16:29:41 2023, max compression
```

## Comparing `nomenklatura-2.9.2.tar` & `nomenklatura-2.9.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.246182 nomenklatura-2.9.2/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.250182 nomenklatura-2.9.2/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/data/match-regression.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.250182 nomenklatura-2.9.2/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.250182 nomenklatura-2.9.2/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.254182 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.254182 nomenklatura-2.9.2/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/judgement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.254182 nomenklatura-2.9.2/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/matching/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.246182 nomenklatura-2.9.2/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:42:37.000000 nomenklatura-2.9.2/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/data/match-regression.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/judgement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/matching/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:29:03.000000 nomenklatura-2.9.3/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/setup.py
```

### Comparing `nomenklatura-2.9.2/LICENSE` & `nomenklatura-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/PKG-INFO` & `nomenklatura-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.2
+Version: 2.9.3
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-2.9.2/README.md` & `nomenklatura-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/cache.py` & `nomenklatura-2.9.3/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/cli.py` & `nomenklatura-2.9.3/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/data/match-regression.pkl` & `nomenklatura-2.9.3/nomenklatura/data/match-regression.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/dataset/catalog.py` & `nomenklatura-2.9.3/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/dataset/coverage.py` & `nomenklatura-2.9.3/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/dataset/dataset.py` & `nomenklatura-2.9.3/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/dataset/publisher.py` & `nomenklatura-2.9.3/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/dataset/resource.py` & `nomenklatura-2.9.3/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/dataset/util.py` & `nomenklatura-2.9.3/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/db.py` & `nomenklatura-2.9.3/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/__init__.py` & `nomenklatura-2.9.3/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/aleph.py` & `nomenklatura-2.9.3/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/common.py` & `nomenklatura-2.9.3/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/nominatim.py` & `nomenklatura-2.9.3/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/opencorporates.py` & `nomenklatura-2.9.3/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/enrich/yente.py` & `nomenklatura-2.9.3/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/entity.py` & `nomenklatura-2.9.3/nomenklatura/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,18 @@
 
     @property
     def _properties(self) -> Dict[str, List[str]]:  # type: ignore
         return {p: [s.value for s in v] for p, v in self._statements.items()}
 
     def _iter_stmt(self) -> Generator[Statement, None, None]:
         for stmts in self._statements.values():
-            yield from stmts
+            for stmt in stmts:
+                if stmt.id is None and stmt.entity_id is not None:
+                    stmt.id = stmt.generate_key()
+                yield stmt
 
     def checksum(self) -> str:
         hash = sha1(self.schema.name.encode("utf-8"))
         for stmt in sorted(self._iter_stmt()):
             if stmt.id is not None:
                 hash.update(stmt.id.encode("utf-8"))
         return hash.hexdigest()
```

### Comparing `nomenklatura-2.9.2/nomenklatura/index/entry.py` & `nomenklatura-2.9.3/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/index/index.py` & `nomenklatura-2.9.3/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/index/tokenizer.py` & `nomenklatura-2.9.3/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/judgement.py` & `nomenklatura-2.9.3/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/loader.py` & `nomenklatura-2.9.3/nomenklatura/loader.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/features/__init__.py` & `nomenklatura-2.9.3/nomenklatura/matching/features/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/features/dates.py` & `nomenklatura-2.9.3/nomenklatura/matching/features/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/features/misc.py` & `nomenklatura-2.9.3/nomenklatura/matching/features/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/features/names.py` & `nomenklatura-2.9.3/nomenklatura/matching/features/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/features/util.py` & `nomenklatura-2.9.3/nomenklatura/matching/features/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/model.py` & `nomenklatura-2.9.3/nomenklatura/matching/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/pairs.py` & `nomenklatura-2.9.3/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/matching/train.py` & `nomenklatura-2.9.3/nomenklatura/matching/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/publish/dates.py` & `nomenklatura-2.9.3/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/publish/edges.py` & `nomenklatura-2.9.3/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/publish/names.py` & `nomenklatura-2.9.3/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/resolver/edge.py` & `nomenklatura-2.9.3/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/resolver/identifier.py` & `nomenklatura-2.9.3/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/resolver/resolver.py` & `nomenklatura-2.9.3/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/senzing.py` & `nomenklatura-2.9.3/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/statement/serialize.py` & `nomenklatura-2.9.3/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/statement/statement.py` & `nomenklatura-2.9.3/nomenklatura/statement/statement.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         self.dataset = dataset
         self.lang = lang
         self.original_value = original_value
         self.first_seen = first_seen
         self.last_seen = last_seen or first_seen
         self.target = target
         self.external = external
-        if id is None and entity_id is not None:
-            id = self.make_key(dataset, entity_id, prop, value, external)
+        if id is None:
+            id = self.generate_key()
         self.id = id
 
     def to_dict(self) -> StatementDict:
         if self.entity_id is None:
             raise ValueError("Statement has no entity ID!")
         return {
             "canonical_id": self.canonical_id or self.entity_id,
@@ -134,30 +134,43 @@
     def __repr__(self) -> str:
         return "<Statement(%r, %r, %r)>" % (self.entity_id, self.prop, self.value)
 
     def __eq__(self, other: Any) -> bool:
         return not self.id != other.id
 
     def __lt__(self, other: Any) -> bool:
-        return (self.prop != self.BASE, self.id) < (other.prop != self.BASE, other.id)
+        self_key = (self.prop != self.BASE, self.id or "")
+        other_key = (other.prop != self.BASE, other.id or "")
+        return self_key < other_key
 
     def clone(self: S) -> S:
         """Make a deep copy of the given statement."""
         return type(self).from_dict(self.to_dict())
 
+    def generate_key(self) -> Optional[str]:
+        return self.make_key(
+            self.dataset,
+            self.entity_id,
+            self.prop,
+            self.value,
+            self.external,
+        )
+
     @classmethod
     def make_key(
         cls,
         dataset: str,
-        entity_id: str,
+        entity_id: Optional[str],
         prop: str,
         value: str,
         external: Optional[bool],
-    ) -> str:
+    ) -> Optional[str]:
         """Hash the key properties of a statement record to make a unique ID."""
+        if entity_id is None:
+            return None
         key = f"{dataset}.{entity_id}.{prop}.{value}"
         if external:
             # We consider the external flag in key composition to avoid race conditions where
             # a certain entity might be emitted as external while it is already linked in to
             # the graph via another route.
             key = f"{key}.ext"
         return hashlib.sha1(key.encode("utf-8")).hexdigest()
```

### Comparing `nomenklatura-2.9.2/nomenklatura/tui/app.py` & `nomenklatura-2.9.3/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/tui/comparison.py` & `nomenklatura-2.9.3/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/tui/util.py` & `nomenklatura-2.9.3/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/util.py` & `nomenklatura-2.9.3/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura/xref.py` & `nomenklatura-2.9.3/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-2.9.3/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.2
+Version: 2.9.3
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-2.9.2/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-2.9.3/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.2/setup.py` & `nomenklatura-2.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="2.9.2",
+    version="2.9.3",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

