# Comparing `tmp/quom-3.0.0.tar.gz` & `tmp/quom-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quom-3.0.0.tar", last modified: Sun Aug 15 11:40:27 2021, max compression
+gzip compressed data, was "quom-4.0.0.tar", last modified: Sat Apr 15 10:54:33 2023, max compression
```

## Comparing `quom-3.0.0.tar` & `quom-4.0.0.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.286942 quom-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.278941 quom-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-08-15 11:40:17.000000 quom-3.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-08-15 11:40:17.000000 quom-3.0.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-08-15 11:40:17.000000 quom-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-08-15 11:40:17.000000 quom-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2021-08-15 11:40:27.286942 quom-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2021-08-15 11:40:17.000000 quom-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/artwork/
--rw-r--r--   0 runner    (1001) docker     (121)   313993 2021-08-15 11:40:17.000000 quom-3.0.0/artwork/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   180297 2021-08-15 11:40:17.000000 quom-3.0.0/artwork/logo_banner.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.278941 quom-3.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/examples/flat_structure/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/foobar_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/examples/flat_structure/libfoobar/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/bar.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/bar.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/base.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/base.hpp
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/foo.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/foo.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/foobar.hpp
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/util.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-08-15 11:40:17.000000 quom-3.0.0/examples/flat_structure/libfoobar/util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/examples/include_directory/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/foobar_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.278941 quom-3.0.0/examples/include_directory/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/examples/include_directory/include/libfoobar/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/bar.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/bar.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/base.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/base.hpp
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/foo.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/foo.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/foobar.hpp
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/util.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-08-15 11:40:17.000000 quom-3.0.0/examples/include_directory/include/libfoobar/util.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-08-15 11:40:27.286942 quom-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      716 2021-08-15 11:40:17.000000 quom-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.278941 quom-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/src/quom/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2753 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8566 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/quom.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/quom_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.286942 quom-3.0.0/src/quom/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/comment_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/number_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5805 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/preprocessor_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/quote_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/remaining_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/tokenize_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2021-08-15 11:40:17.000000 quom-3.0.0/src/quom/tokenizer/whitespace_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.282941 quom-3.0.0/src/quom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-15 11:40:27.000000 quom-3.0.0/src/quom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.286942 quom-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:17.000000 quom-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 11:40:27.286942 quom-3.0.0/tests/test_quom/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/same_file_different_include.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/test_file_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/test_include_directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/test_last_source_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/test_line_breaks_when_stitching.py
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/test_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_quom/test_source_directory.py
--rw-r--r--   0 runner    (1001) docker     (121)    13507 2021-08-15 11:40:17.000000 quom-3.0.0/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-08-15 11:40:17.000000 quom-3.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 10:54:20.000000 quom-4.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-15 10:54:20.000000 quom-4.0.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-15 10:54:20.000000 quom-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 10:54:20.000000 quom-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-15 10:54:33.201320 quom-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-15 10:54:20.000000 quom-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)   313993 2023-04-15 10:54:20.000000 quom-4.0.0/artwork/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   180297 2023-04-15 10:54:20.000000 quom-4.0.0/artwork/logo_banner.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/examples/flat_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/foobar_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/examples/flat_structure/libfoobar/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/bar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/foo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/foo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/foobar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/examples/include_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/foobar_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/examples/include_directory/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/examples/include_directory/include/libfoobar/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/bar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/foo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/foo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/foobar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 10:54:33.205320 quom-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 10:54:20.000000 quom-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/src/quom/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/quom.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/quom_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/src/quom/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/comment_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/number_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/preprocessor_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/quote_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/remaining_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/tokenize_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/whitespace_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/src/quom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:20.000000 quom-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/tests/test_quom/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/same_file_different_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_file_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_file_without_include_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_include_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_last_source_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_line_breaks_when_stitching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_source_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 10:54:20.000000 quom-4.0.0/tox.ini
```

### Comparing `quom-3.0.0/.github/workflows/publish.yml` & `quom-4.0.0/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v2
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel twine
       - name: Build and publish
         env:
           TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
```

### Comparing `quom-3.0.0/.github/workflows/testing.yml` & `quom-4.0.0/.github/workflows/testing.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,40 +7,40 @@
     branches: [ master ]
 
 jobs:
   python-test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.6', '3.7', '3.8', '3.9' ]
+        python-version: [ '3.7', '3.8', '3.9', '3.10', '3.11' ]
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install .[testing]
       - name: Run tests with Python ${{ matrix.python-version }}
         run: |
           g++ --version
           python --version
           pytest
       - name: Run flake8
-        if: ${{ matrix.python-version == '3.9' }}
+        if: ${{ matrix.python-version == '3.10' }}
         run: flake8
   publish-python-test:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v2
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel twine
       - name: Build
         run: |
           python setup.py dists
```

### Comparing `quom-3.0.0/.gitignore` & `quom-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/LICENSE` & `quom-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/README.md` & `quom-4.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 # Quom
 Quom is a single file generator for C/C++.
 
 It resolves all included local headers starting with your main C/C++ file. This is also known as amalgamation.
 
-Afterwards, it tries to find the related source files and there headers and places them at the end of the main file
+Afterwards, it tries to find the related source files and their headers and places them at the end of the main file
 or at a specific stitch location if provided.
 
 At the end there will be one single file with all your header and sources joined together.
 
 ## Installation
 
 ```
@@ -127,15 +127,15 @@
 
 *foo.hpp*
 
 ```cpp
 #pragma once
 
 #ifndef FOOBAR_FOO_HPP
-#endif FOOBAR_FOO_HPP
+#define FOOBAR_FOO_HPP
 
 extern int foo; 
 
 #endif
 ```
 
 *foo.cpp*
@@ -148,15 +148,15 @@
 
 *foobar.hpp*
 
 ```cpp
 #pragma once
 
 #ifndef FOOBAR_HPP
-#endif FOOBAR_HPP
+#define FOOBAR_HPP
 
 #include "foo.hpp"
 
 #endif
 
 #ifdef FOO_MAIN
 
@@ -173,15 +173,15 @@
 
 *foobar_gen.hpp*
 
 ```cpp
 #pragma once
 
 #ifndef FOOBAR_HPP
-#endif FOOBAR_HPP
+#define FOOBAR_HPP
 
 extern int foo;
 
 #endif
 
 #ifdef FOO_MAIN
```

### Comparing `quom-3.0.0/artwork/logo.png` & `quom-4.0.0/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/artwork/logo_banner.png` & `quom-4.0.0/artwork/logo_banner.png`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/examples/flat_structure/foobar_gen.hpp` & `quom-4.0.0/examples/flat_structure/foobar_gen.hpp`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/examples/include_directory/foobar_gen.hpp` & `quom-4.0.0/examples/include_directory/foobar_gen.hpp`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/setup.cfg` & `quom-4.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/setup.py` & `quom-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/__init__.py` & `quom-4.0.0/src/quom/__init__.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/__main__.py` & `quom-4.0.0/src/quom/__main__.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/quom.py` & `quom-4.0.0/src/quom/quom.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .quom_error import QuomError
 from .tokenizer import tokenize, Token, CommentToken, PreprocessorToken, PreprocessorIfNotDefinedToken, \
     PreprocessorDefineToken, PreprocessorEndIfToken, PreprocessorIncludeToken, PreprocessorPragmaOnceToken, \
     RemainingToken, LinebreakWhitespaceToken, EmptyToken, StartToken, EndToken, WhitespaceToken
 
 CONTINUOUS_LINE_BREAK_START = 0
 CONTINUOUS_BREAK_REACHED = 3
+SOURCE_FILE_EXTENSIONS = ['.c', '.cpp', '.cxx', '.cc', '.c++', '.cp', '.C']
 
 
 def find_token(tokens: List[Token], token_type: any):
     for i, token in enumerate(tokens):
         if isinstance(token, token_type):
             return i, token
     return None, None
@@ -73,19 +74,22 @@
             else:
                 raise QuomError('Include not found: "{}"'.format(include_path))
 
         # Skip already processed files.
         file_path = file_path.resolve()
         if file_path in self.__processed_files:
             return
-        self.__processed_files.add(file_path)
 
         # Tokenize the file.
         tokens = tokenize(file_path.read_text(encoding=self.__encoding))
 
+        # Add to processed files.
+        if is_main_header or self.__has_guard(tokens):
+            self.__processed_files.add(file_path)
+
         for token in tokens:
             # Find local includes.
             token = self.__scan_for_include(file_path, token, is_source_file)
             if not token or self.__scan_for_source_files_stitch(token):
                 continue
 
             self.__write_token(token, is_main_header)
@@ -106,14 +110,20 @@
         if self.__is_cont_line_break(token):
             return
 
         # Write token and store.
         self.__dst.write(str(token.raw))
         self.__prev_token = token
 
+    def __has_guard(self, tokens: List[Token]):
+        for token in tokens:
+            if self.__is_pragma_once(token) or self.__is_include_guard(token):
+                return True
+        return False
+
     @staticmethod
     def __is_pragma_once(token: Token):
         if isinstance(token, PreprocessorPragmaOnceToken):
             return True
         return False
 
     def __is_include_guard(self, token: Token):
@@ -128,21 +138,22 @@
                 return True
         elif isinstance(token, PreprocessorEndIfToken):
             # Find first comment token matching the include guard format.
             i, comment_token = find_token(token.preprocessor_arguments, CommentToken)
             if comment_token and self.__include_guard_format.match(str(comment_token.content).strip()) and \
                     contains_only_whitespace_and_comment_tokens(token.preprocessor_arguments[i + 1:]):
                 return True
+        return False
 
     def __find_possible_source_file(self, header_file_path: Path) -> Union[Path, None]:
-        if header_file_path.suffix in ['.c', '.cpp', '.cxx', '.cc', '.c++', '.cp', '.C']:
+        if header_file_path.suffix in SOURCE_FILE_EXTENSIONS:
             return
 
         # Checks if a equivalent compilation unit exits.
-        for extension in ['.c', '.cpp', '.cxx', '.cc', '.c++', '.cp', '.C']:
+        for extension in SOURCE_FILE_EXTENSIONS:
             for src_dir in self.__relative_source_directories:
                 file_path = (header_file_path.parent / src_dir / header_file_path.name).with_suffix(extension)
                 if file_path.exists():
                     return file_path
             for src_dir in self.__source_directories:
                 file_path = (src_dir / header_file_path.name).with_suffix(extension).resolve()
                 if file_path.exists():
```

### Comparing `quom-3.0.0/src/quom/tokenizer/__init__.py` & `quom-4.0.0/src/quom/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/comment_tokenizer.py` & `quom-4.0.0/src/quom/tokenizer/comment_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/iterator.py` & `quom-4.0.0/src/quom/tokenizer/iterator.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/number_tokenizer.py` & `quom-4.0.0/src/quom/tokenizer/number_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/preprocessor_tokenizer.py` & `quom-4.0.0/src/quom/tokenizer/preprocessor_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/quote_tokenizer.py` & `quom-4.0.0/src/quom/tokenizer/quote_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/remaining_tokenizer.py` & `quom-4.0.0/src/quom/tokenizer/remaining_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/token.py` & `quom-4.0.0/src/quom/tokenizer/token.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/tokenize.py` & `quom-4.0.0/src/quom/tokenizer/tokenize.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom/tokenizer/whitespace_tokenizer.py` & `quom-4.0.0/src/quom/tokenizer/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/src/quom.egg-info/SOURCES.txt` & `quom-4.0.0/src/quom.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -53,12 +53,13 @@
 src/quom/tokenizer/tokenize_error.py
 src/quom/tokenizer/whitespace_tokenizer.py
 tests/__init__.py
 tests/test_iterator.py
 tests/test_tokenizer.py
 tests/test_quom/same_file_different_include.py
 tests/test_quom/test_file_encoding.py
+tests/test_quom/test_file_without_include_guard.py
 tests/test_quom/test_include_directory.py
 tests/test_quom/test_last_source_file.py
 tests/test_quom/test_line_breaks_when_stitching.py
 tests/test_quom/test_normal.py
 tests/test_quom/test_source_directory.py
```

### Comparing `quom-3.0.0/tests/test_iterator.py` & `quom-4.0.0/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/same_file_different_include.py` & `quom-4.0.0/tests/test_quom/same_file_different_include.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/test_file_encoding.py` & `quom-4.0.0/tests/test_quom/test_file_encoding.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/test_include_directory.py` & `quom-4.0.0/tests/test_quom/test_include_directory.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/test_last_source_file.py` & `quom-4.0.0/tests/test_quom/test_last_source_file.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/test_line_breaks_when_stitching.py` & `quom-4.0.0/tests/test_quom/test_line_breaks_when_stitching.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/test_normal.py` & `quom-4.0.0/tests/test_quom/test_normal.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_quom/test_source_directory.py` & `quom-4.0.0/tests/test_quom/test_source_directory.py`

 * *Files identical despite different names*

### Comparing `quom-3.0.0/tests/test_tokenizer.py` & `quom-4.0.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

